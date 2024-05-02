# Comparing `tmp/mau-4.0.0.tar.gz` & `tmp/mau-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mau-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mau-4.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mau-4.0.0.tar` & `mau-4.0.1.tar`

### file list

```diff
@@ -1,151 +1,228 @@
--rw-r--r--   0        0        0      528 2022-10-26 07:17:29.495806 mau-4.0.0/.gitignore
--rw-r--r--   0        0        0     8985 2024-04-28 20:04:41.973523 mau-4.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1084 2023-08-14 07:33:57.840796 mau-4.0.0/LICENSE
--rw-r--r--   0        0        0     1477 2024-04-28 20:06:54.954456 mau-4.0.0/README.md
--rw-r--r--   0        0        0     2203 2024-04-28 20:04:41.973523 mau-4.0.0/mau/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 20:04:41.973523 mau-4.0.0/mau/environment/__init__.py
--rw-r--r--   0        0        0     2721 2024-04-28 20:04:41.973523 mau-4.0.0/mau/environment/environment.py
--rw-r--r--   0        0        0     1190 2024-04-28 20:04:41.973523 mau-4.0.0/mau/errors.py
--rw-r--r--   0        0        0      142 2024-03-29 22:28:59.350920 mau-4.0.0/mau/helpers.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.346920 mau-4.0.0/mau/lexers/__init__.py
--rw-r--r--   0        0        0      914 2024-03-29 22:28:59.346920 mau-4.0.0/mau/lexers/arguments_lexer.py
--rw-r--r--   0        0        0     6172 2024-04-28 20:04:41.973523 mau-4.0.0/mau/lexers/base_lexer.py
--rw-r--r--   0        0        0     8613 2024-04-28 20:04:41.973523 mau-4.0.0/mau/lexers/main_lexer.py
--rw-r--r--   0        0        0      530 2024-03-29 22:28:59.346920 mau-4.0.0/mau/lexers/preprocess_variables_lexer.py
--rw-r--r--   0        0        0      919 2024-04-28 20:04:41.973523 mau-4.0.0/mau/lexers/text_lexer.py
--rw-r--r--   0        0        0     5594 2024-04-28 20:04:41.973523 mau-4.0.0/mau/main.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.346920 mau-4.0.0/mau/nodes/__init__.py
--rw-r--r--   0        0        0      936 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/arguments.py
--rw-r--r--   0        0        0     2468 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/block.py
--rw-r--r--   0        0        0     2047 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/content.py
--rw-r--r--   0        0        0     1731 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/footnotes.py
--rw-r--r--   0        0        0      842 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/header.py
--rw-r--r--   0        0        0      989 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/inline.py
--rw-r--r--   0        0        0     1508 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/lists.py
--rw-r--r--   0        0        0     3770 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/macros.py
--rw-r--r--   0        0        0     2569 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/nodes.py
--rw-r--r--   0        0        0      739 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/page.py
--rw-r--r--   0        0        0      686 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/paragraph.py
--rw-r--r--   0        0        0     3476 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/source.py
--rw-r--r--   0        0        0     1004 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/toc.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/mau/parsers/__init__.py
--rw-r--r--   0        0        0     1287 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/arguments.py
--rw-r--r--   0        0        0     3876 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/arguments_parser.py
--rw-r--r--   0        0        0      855 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/attributes.py
--rw-r--r--   0        0        0    12389 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/base_parser.py
--rw-r--r--   0        0        0     3758 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/footnotes.py
--rw-r--r--   0        0        0      998 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/internal_links.py
--rw-r--r--   0        0        0    38156 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/main_parser.py
--rw-r--r--   0        0        0     2254 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/preprocess_variables_parser.py
--rw-r--r--   0        0        0    14892 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/text_parser.py
--rw-r--r--   0        0        0     3516 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/toc.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/mau/text_buffer/__init__.py
--rw-r--r--   0        0        0     1169 2024-04-23 21:38:42.846385 mau-4.0.0/mau/text_buffer/context.py
--rw-r--r--   0        0        0     5331 2024-03-29 22:28:59.350920 mau-4.0.0/mau/text_buffer/text_buffer.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.346920 mau-4.0.0/mau/tokens/__init__.py
--rw-r--r--   0        0        0     1230 2024-03-29 22:28:59.346920 mau-4.0.0/mau/tokens/tokens.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/mau/visitors/__init__.py
--rw-r--r--   0        0        0    13054 2024-04-28 20:04:41.973523 mau-4.0.0/mau/visitors/base_visitor.py
--rw-r--r--   0        0        0     8564 2024-04-28 20:04:41.977522 mau-4.0.0/mau/visitors/jinja_visitor.py
--rw-r--r--   0        0        0      152 2023-08-14 07:33:57.844796 mau-4.0.0/noxfile.py
--rw-r--r--   0        0        0     2040 2024-04-28 20:04:41.977522 mau-4.0.0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-08-14 07:33:57.844796 mau-4.0.0/requirements.txt
--rw-r--r--   0        0        0       15 2023-08-14 07:33:57.844796 mau-4.0.0/requirements/development.txt
--rw-r--r--   0        0        0        2 2023-08-14 07:33:57.844796 mau-4.0.0/requirements/production.txt
--rw-r--r--   0        0        0       11 2023-08-14 07:33:57.844796 mau-4.0.0/requirements/testing.txt
--rw-r--r--   0        0        0        0 2024-04-17 20:37:15.825771 mau-4.0.0/tests/__init__.py
--rw-r--r--   0        0        0     6907 2024-04-28 20:04:41.977522 mau-4.0.0/tests/environment/test_environment.py
--rw-r--r--   0        0        0     2209 2024-04-28 20:04:41.977522 mau-4.0.0/tests/helpers.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/tests/lexers/__init__.py
--rw-r--r--   0        0        0      483 2023-08-14 07:33:57.844796 mau-4.0.0/tests/lexers/data_file_lexer.txt
--rw-r--r--   0        0        0     5165 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_arguments_lexer.py
--rw-r--r--   0        0        0     6038 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_base_lexer.py
--rw-r--r--   0        0        0    20055 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_main_lexer.py
--rw-r--r--   0        0        0     4905 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_preprocess_variables_lexer.py
--rw-r--r--   0        0        0     7048 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_text_lexer.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/tests/nodes/__init__.py
--rw-r--r--   0        0        0      566 2024-03-29 22:28:59.350920 mau-4.0.0/tests/nodes/test_arguments.py
--rw-r--r--   0        0        0      357 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_block.py
--rw-r--r--   0        0        0     1044 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_content.py
--rw-r--r--   0        0        0     2207 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_footnotes.py
--rw-r--r--   0        0        0      793 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_header.py
--rw-r--r--   0        0        0     1075 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_inline.py
--rw-r--r--   0        0        0     1281 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_lists.py
--rw-r--r--   0        0        0     2224 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_macros.py
--rw-r--r--   0        0        0      937 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_nodes.py
--rw-r--r--   0        0        0     1142 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_page.py
--rw-r--r--   0        0        0      741 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_paragraph.py
--rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_references.py
--rw-r--r--   0        0        0     1511 2024-03-29 22:28:59.350920 mau-4.0.0/tests/nodes/test_source.py
--rw-r--r--   0        0        0     1689 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_toc.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.0/tests/parsers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.0/tests/parsers/main_parser/__init__.py
--rw-r--r--   0        0        0     1763 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_arguments.py
--rw-r--r--   0        0        0    11978 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_attributes.py
--rw-r--r--   0        0        0     4537 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_basic.py
--rw-r--r--   0        0        0     4448 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_engine_group.py
--rw-r--r--   0        0        0     7240 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_engine_mau.py
--rw-r--r--   0        0        0     1063 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_engine_raw.py
--rw-r--r--   0        0        0     2107 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_other.py
--rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_source.py
--rw-r--r--   0        0        0     2625 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_content.py
--rw-r--r--   0        0        0     6304 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_control.py
--rw-r--r--   0        0        0    11881 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_footnotes.py
--rw-r--r--   0        0        0     7903 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_headers.py
--rw-r--r--   0        0        0      795 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_horizontal_rule.py
--rw-r--r--   0        0        0     4214 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_internal_links.py
--rw-r--r--   0        0        0     8408 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_lists.py
--rw-r--r--   0        0        0     3880 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_main_parser.py
--rw-r--r--   0        0        0     2153 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_paragraph.py
--rw-r--r--   0        0        0      778 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_parent.py
--rw-r--r--   0        0        0     7926 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_source.py
--rw-r--r--   0        0        0     2459 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_title.py
--rw-r--r--   0        0        0     7622 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_toc.py
--rw-r--r--   0        0        0     4100 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_variables.py
--rw-r--r--   0        0        0    11168 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/test_arguments_parser.py
--rw-r--r--   0        0        0    12199 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/test_base_parser.py
--rw-r--r--   0        0        0     4287 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/test_create_toc.py
--rw-r--r--   0        0        0     3468 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/test_preprocess_variables_parser.py
--rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/__init__.py
--rw-r--r--   0        0        0     1626 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_arguments.py
--rw-r--r--   0        0        0     1637 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_class.py
--rw-r--r--   0        0        0     5553 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_control.py
--rw-r--r--   0        0        0      575 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_footnote.py
--rw-r--r--   0        0        0     1290 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_generic_macro.py
--rw-r--r--   0        0        0      802 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_header.py
--rw-r--r--   0        0        0      973 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_image.py
--rw-r--r--   0        0        0     1929 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_link.py
--rw-r--r--   0        0        0     1223 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/test_basic_text.py
--rw-r--r--   0        0        0     2443 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/test_escaped.py
--rw-r--r--   0        0        0     2624 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/test_style.py
--rw-r--r--   0        0        0     1246 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/test_verbatim.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.0/tests/text_buffer/__init__.py
--rw-r--r--   0        0        0      386 2024-03-29 22:28:59.354920 mau-4.0.0/tests/text_buffer/test_context.py
--rw-r--r--   0        0        0     4786 2024-03-29 22:28:59.354920 mau-4.0.0/tests/text_buffer/test_text_buffer.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/tests/tokens/__init__.py
--rw-r--r--   0        0        0     2192 2024-03-29 22:28:59.350920 mau-4.0.0/tests/tokens/test_tokens.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.0/tests/visitors/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/tests/visitors/base_visitor/__init__.py
--rw-r--r--   0        0        0     8808 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_block.py
--rw-r--r--   0        0        0     3074 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_content.py
--rw-r--r--   0        0        0     3093 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_footnotes.py
--rw-r--r--   0        0        0     1556 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_header.py
--rw-r--r--   0        0        0    13787 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_inline.py
--rw-r--r--   0        0        0     2547 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_lists.py
--rw-r--r--   0        0        0     2370 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_page.py
--rw-r--r--   0        0        0     1872 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_paragraph.py
--rw-r--r--   0        0        0     4295 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_source.py
--rw-r--r--   0        0        0     5265 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_toc.py
--rw-r--r--   0        0        0     6392 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_block.py
--rw-r--r--   0        0        0     2115 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_content.py
--rw-r--r--   0        0        0     1406 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_footnotes.py
--rw-r--r--   0        0        0     1151 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_header.py
--rw-r--r--   0        0        0     7556 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_inline.py
--rw-r--r--   0        0        0     1638 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_lists.py
--rw-r--r--   0        0        0      857 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_page.py
--rw-r--r--   0        0        0     2069 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_paragraph.py
--rw-r--r--   0        0        0     1283 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_source.py
--rw-r--r--   0        0        0     7366 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_templates.py
--rw-r--r--   0        0        0     1354 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/toc.py
--rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 mau-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0      528 2022-10-26 07:17:29.495806 mau-4.0.1/.gitignore
+-rw-r--r--   0        0        0     9067 2024-04-29 16:28:49.466140 mau-4.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1084 2023-08-14 07:33:57.840796 mau-4.0.1/LICENSE
+-rw-r--r--   0        0        0     1477 2024-04-28 20:06:54.954456 mau-4.0.1/README.md
+-rw-r--r--   0        0        0     2203 2024-04-28 20:04:41.973523 mau-4.0.1/mau/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.973523 mau-4.0.1/mau/environment/__init__.py
+-rw-r--r--   0        0        0     2721 2024-04-28 20:04:41.973523 mau-4.0.1/mau/environment/environment.py
+-rw-r--r--   0        0        0     1190 2024-04-28 20:04:41.973523 mau-4.0.1/mau/errors.py
+-rw-r--r--   0        0        0      142 2024-03-29 22:28:59.350920 mau-4.0.1/mau/helpers.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.346920 mau-4.0.1/mau/lexers/__init__.py
+-rw-r--r--   0        0        0      914 2024-03-29 22:28:59.346920 mau-4.0.1/mau/lexers/arguments_lexer.py
+-rw-r--r--   0        0        0     6172 2024-04-28 20:04:41.973523 mau-4.0.1/mau/lexers/base_lexer.py
+-rw-r--r--   0        0        0     8613 2024-04-28 20:04:41.973523 mau-4.0.1/mau/lexers/main_lexer.py
+-rw-r--r--   0        0        0      530 2024-03-29 22:28:59.346920 mau-4.0.1/mau/lexers/preprocess_variables_lexer.py
+-rw-r--r--   0        0        0      919 2024-04-28 20:04:41.973523 mau-4.0.1/mau/lexers/text_lexer.py
+-rw-r--r--   0        0        0     5594 2024-04-28 20:04:41.973523 mau-4.0.1/mau/main.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.346920 mau-4.0.1/mau/nodes/__init__.py
+-rw-r--r--   0        0        0      936 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/arguments.py
+-rw-r--r--   0        0        0     2468 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/block.py
+-rw-r--r--   0        0        0     2047 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/content.py
+-rw-r--r--   0        0        0     1731 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/footnotes.py
+-rw-r--r--   0        0        0      842 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/header.py
+-rw-r--r--   0        0        0      989 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/inline.py
+-rw-r--r--   0        0        0     1508 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/lists.py
+-rw-r--r--   0        0        0     3770 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/macros.py
+-rw-r--r--   0        0        0     2569 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/nodes.py
+-rw-r--r--   0        0        0      739 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/page.py
+-rw-r--r--   0        0        0      686 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/paragraph.py
+-rw-r--r--   0        0        0     3476 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/source.py
+-rw-r--r--   0        0        0     1004 2024-04-28 20:04:41.973523 mau-4.0.1/mau/nodes/toc.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.1/mau/parsers/__init__.py
+-rw-r--r--   0        0        0     1287 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/arguments.py
+-rw-r--r--   0        0        0     3876 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/arguments_parser.py
+-rw-r--r--   0        0        0      855 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/attributes.py
+-rw-r--r--   0        0        0    12389 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/base_parser.py
+-rw-r--r--   0        0        0     3758 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/footnotes.py
+-rw-r--r--   0        0        0      998 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/internal_links.py
+-rw-r--r--   0        0        0    38156 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/main_parser.py
+-rw-r--r--   0        0        0     2254 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/preprocess_variables_parser.py
+-rw-r--r--   0        0        0    14892 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/text_parser.py
+-rw-r--r--   0        0        0     3516 2024-04-28 20:04:41.973523 mau-4.0.1/mau/parsers/toc.py
+-rw-r--r--   0        0        0     2897 2024-04-29 16:27:03.265556 mau-4.0.1/mau/test_helpers.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.1/mau/text_buffer/__init__.py
+-rw-r--r--   0        0        0     1169 2024-04-23 21:38:42.846385 mau-4.0.1/mau/text_buffer/context.py
+-rw-r--r--   0        0        0     5331 2024-03-29 22:28:59.350920 mau-4.0.1/mau/text_buffer/text_buffer.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.346920 mau-4.0.1/mau/tokens/__init__.py
+-rw-r--r--   0        0        0     1230 2024-03-29 22:28:59.346920 mau-4.0.1/mau/tokens/tokens.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.1/mau/visitors/__init__.py
+-rw-r--r--   0        0        0    13054 2024-04-28 20:04:41.973523 mau-4.0.1/mau/visitors/base_visitor.py
+-rw-r--r--   0        0        0     8564 2024-04-28 20:04:41.977522 mau-4.0.1/mau/visitors/jinja_visitor.py
+-rw-r--r--   0        0        0      152 2023-08-14 07:33:57.844796 mau-4.0.1/noxfile.py
+-rw-r--r--   0        0        0     2040 2024-04-29 16:29:03.930220 mau-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-08-14 07:33:57.844796 mau-4.0.1/requirements.txt
+-rw-r--r--   0        0        0       15 2023-08-14 07:33:57.844796 mau-4.0.1/requirements/development.txt
+-rw-r--r--   0        0        0        2 2023-08-14 07:33:57.844796 mau-4.0.1/requirements/production.txt
+-rw-r--r--   0        0        0       11 2023-08-14 07:33:57.844796 mau-4.0.1/requirements/testing.txt
+-rw-r--r--   0        0        0        0 2024-04-17 20:37:15.825771 mau-4.0.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/__init__.py
+-rw-r--r--   0        0        0     2196 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/block/block_admonition.yaml
+-rw-r--r--   0        0        0      650 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/block/block_conditionals.yaml
+-rw-r--r--   0        0        0     1731 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/block/block_quote.yaml
+-rw-r--r--   0        0        0     2783 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/block/block_simple.yaml
+-rw-r--r--   0        0        0      954 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/block/block_title.yaml
+-rw-r--r--   0        0        0     1836 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/commands/footnotes.yaml
+-rw-r--r--   0        0        0    11353 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/commands/footnotes_advanced.yaml
+-rw-r--r--   0        0        0     3880 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/commands/references.yaml
+-rw-r--r--   0        0        0     1139 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/commands/toc.yaml
+-rw-r--r--   0        0        0     7925 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/commands/toc_advanced.yaml
+-rw-r--r--   0        0        0      883 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/classes.yaml
+-rw-r--r--   0        0        0     1560 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/conditionals.yaml
+-rw-r--r--   0        0        0      796 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/inline_image.yaml
+-rw-r--r--   0        0        0     1788 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/internal_link.yaml
+-rw-r--r--   0        0        0     2709 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/link.yaml
+-rw-r--r--   0        0        0     1223 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/mailto.yaml
+-rw-r--r--   0        0        0      697 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/multiple_paragraphs.yaml
+-rw-r--r--   0        0        0      394 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/single_paragraph.yaml
+-rw-r--r--   0        0        0      475 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/split_paragraph.yaml
+-rw-r--r--   0        0        0     3158 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/styles.yaml
+-rw-r--r--   0        0        0     4208 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/styles_mixed.yaml
+-rw-r--r--   0        0        0      670 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/inline/verbatim.yaml
+-rw-r--r--   0        0        0     1174 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/other/directives.yaml
+-rw-r--r--   0        0        0     1525 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/other/variable_advanced.yaml
+-rw-r--r--   0        0        0     1117 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/other/variable_simple.yaml
+-rw-r--r--   0        0        0       89 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/page/comments.yaml
+-rw-r--r--   0        0        0     1481 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/page/header_multiple.yaml
+-rw-r--r--   0        0        0      551 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/page/header_single.yaml
+-rw-r--r--   0        0        0     2336 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/page/header_with_paragraphs.yaml
+-rw-r--r--   0        0        0      819 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/page/horizontal_line.yaml
+-rw-r--r--   0        0        0     1038 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/page/image.yaml
+-rw-r--r--   0        0        0     2683 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/page/list_ordered.yaml
+-rw-r--r--   0        0        0     5648 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/page/list_start.yaml
+-rw-r--r--   0        0        0     2687 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/page/list_unordered.yaml
+-rw-r--r--   0        0        0     1771 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/source/source_callouts.yaml
+-rw-r--r--   0        0        0     3294 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/source/source_highlight.yaml
+-rw-r--r--   0        0        0     1784 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/expected/source/source_simple.yaml
+-rw-r--r--   0        0        0      248 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/source/block/block_admonition.mau
+-rw-r--r--   0        0        0      131 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/source/block/block_conditionals.mau
+-rw-r--r--   0        0        0      201 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/source/block/block_quote.mau
+-rw-r--r--   0        0        0      237 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/source/block/block_simple.mau
+-rw-r--r--   0        0        0       38 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/source/block/block_title.mau
+-rw-r--r--   0        0        0      108 2024-04-29 16:27:03.265556 mau-4.0.1/tests/e2e/source/commands/footnotes.mau
+-rw-r--r--   0        0        0      682 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/commands/footnotes_advanced.mau
+-rw-r--r--   0        0        0       20 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/commands/toc.mau
+-rw-r--r--   0        0        0      328 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/commands/toc_advanced.mau
+-rw-r--r--   0        0        0       56 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/classes.mau
+-rw-r--r--   0        0        0      131 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/conditionals.mau
+-rw-r--r--   0        0        0      107 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/inline_image.mau
+-rw-r--r--   0        0        0       68 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/internal_link.mau
+-rw-r--r--   0        0        0      228 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/link.mau
+-rw-r--r--   0        0        0      121 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/mailto.mau
+-rw-r--r--   0        0        0       82 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/multiple_paragraphs.mau
+-rw-r--r--   0        0        0       43 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/single_paragraph.mau
+-rw-r--r--   0        0        0      112 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/split_paragraph.mau
+-rw-r--r--   0        0        0      159 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/styles.mau
+-rw-r--r--   0        0        0      366 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/styles_mixed.mau
+-rw-r--r--   0        0        0       41 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/inline/verbatim.mau
+-rw-r--r--   0        0        0      102 2024-04-29 16:38:49.397465 mau-4.0.1/tests/e2e/source/other/directives.mau
+-rw-r--r--   0        0        0       48 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/other/include_text.txt
+-rw-r--r--   0        0        0      257 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/other/variable_advanced.mau
+-rw-r--r--   0        0        0      219 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/other/variable_simple.mau
+-rw-r--r--   0        0        0      129 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/page/comments.mau
+-rw-r--r--   0        0        0       38 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/page/header_multiple.mau
+-rw-r--r--   0        0        0       11 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/page/header_single.mau
+-rw-r--r--   0        0        0      101 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/page/header_with_paragraphs.mau
+-rw-r--r--   0        0        0      104 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/page/horizontal_line.mau
+-rw-r--r--   0        0        0      228 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/page/image.mau
+-rw-r--r--   0        0        0       76 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/page/list_ordered.mau
+-rw-r--r--   0        0        0      287 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/page/list_start.mau
+-rw-r--r--   0        0        0       78 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/page/list_unordered.mau
+-rw-r--r--   0        0        0      241 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/source/source_callouts.mau
+-rw-r--r--   0        0        0      441 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/source/source_highlight.mau
+-rw-r--r--   0        0        0      124 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/source/source/source_simple.mau
+-rw-r--r--   0        0        0     1139 2024-04-29 16:27:03.269556 mau-4.0.1/tests/e2e/test_e2e.py
+-rw-r--r--   0        0        0     6907 2024-04-28 20:04:41.977522 mau-4.0.1/tests/environment/test_environment.py
+-rw-r--r--   0        0        0       31 2024-04-29 16:27:03.265556 mau-4.0.1/tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.1/tests/lexers/__init__.py
+-rw-r--r--   0        0        0      483 2023-08-14 07:33:57.844796 mau-4.0.1/tests/lexers/data_file_lexer.txt
+-rw-r--r--   0        0        0     5165 2024-04-28 20:04:41.977522 mau-4.0.1/tests/lexers/test_arguments_lexer.py
+-rw-r--r--   0        0        0     6038 2024-04-28 20:04:41.977522 mau-4.0.1/tests/lexers/test_base_lexer.py
+-rw-r--r--   0        0        0    20055 2024-04-28 20:04:41.977522 mau-4.0.1/tests/lexers/test_main_lexer.py
+-rw-r--r--   0        0        0     4905 2024-04-28 20:04:41.977522 mau-4.0.1/tests/lexers/test_preprocess_variables_lexer.py
+-rw-r--r--   0        0        0     7048 2024-04-28 20:04:41.977522 mau-4.0.1/tests/lexers/test_text_lexer.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.1/tests/nodes/__init__.py
+-rw-r--r--   0        0        0      566 2024-03-29 22:28:59.350920 mau-4.0.1/tests/nodes/test_arguments.py
+-rw-r--r--   0        0        0      357 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_block.py
+-rw-r--r--   0        0        0     1044 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_content.py
+-rw-r--r--   0        0        0     2207 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_footnotes.py
+-rw-r--r--   0        0        0      793 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_header.py
+-rw-r--r--   0        0        0     1075 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_inline.py
+-rw-r--r--   0        0        0     1281 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_lists.py
+-rw-r--r--   0        0        0     2224 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_macros.py
+-rw-r--r--   0        0        0      937 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_nodes.py
+-rw-r--r--   0        0        0     1142 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_page.py
+-rw-r--r--   0        0        0      741 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_paragraph.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_references.py
+-rw-r--r--   0        0        0     1511 2024-03-29 22:28:59.350920 mau-4.0.1/tests/nodes/test_source.py
+-rw-r--r--   0        0        0     1689 2024-04-28 20:04:41.977522 mau-4.0.1/tests/nodes/test_toc.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.1/tests/parsers/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.1/tests/parsers/main_parser/__init__.py
+-rw-r--r--   0        0        0     1763 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_arguments.py
+-rw-r--r--   0        0        0    12011 2024-04-29 16:27:03.265556 mau-4.0.1/tests/parsers/main_parser/test_block_attributes.py
+-rw-r--r--   0        0        0     4537 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_block_basic.py
+-rw-r--r--   0        0        0     4448 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_block_engine_group.py
+-rw-r--r--   0        0        0     7240 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_block_engine_mau.py
+-rw-r--r--   0        0        0     1063 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_block_engine_raw.py
+-rw-r--r--   0        0        0     2107 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_block_other.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_block_source.py
+-rw-r--r--   0        0        0     2625 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_content.py
+-rw-r--r--   0        0        0     6304 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_control.py
+-rw-r--r--   0        0        0    11881 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_footnotes.py
+-rw-r--r--   0        0        0     7903 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_headers.py
+-rw-r--r--   0        0        0      795 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_horizontal_rule.py
+-rw-r--r--   0        0        0     4214 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_internal_links.py
+-rw-r--r--   0        0        0     8408 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_lists.py
+-rw-r--r--   0        0        0     3880 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_main_parser.py
+-rw-r--r--   0        0        0     2153 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_paragraph.py
+-rw-r--r--   0        0        0      778 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_parent.py
+-rw-r--r--   0        0        0     7926 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_source.py
+-rw-r--r--   0        0        0     2459 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_title.py
+-rw-r--r--   0        0        0     7622 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_toc.py
+-rw-r--r--   0        0        0     4100 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/main_parser/test_variables.py
+-rw-r--r--   0        0        0    11168 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/test_arguments_parser.py
+-rw-r--r--   0        0        0    12199 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/test_base_parser.py
+-rw-r--r--   0        0        0     4287 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/test_create_toc.py
+-rw-r--r--   0        0        0     3468 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/test_preprocess_variables_parser.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/macros/__init__.py
+-rw-r--r--   0        0        0     1626 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/macros/test_arguments.py
+-rw-r--r--   0        0        0     1637 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/macros/test_class.py
+-rw-r--r--   0        0        0     5553 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/macros/test_control.py
+-rw-r--r--   0        0        0      575 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/macros/test_footnote.py
+-rw-r--r--   0        0        0     1290 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/macros/test_generic_macro.py
+-rw-r--r--   0        0        0      802 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/macros/test_header.py
+-rw-r--r--   0        0        0      973 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/macros/test_image.py
+-rw-r--r--   0        0        0     1929 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/macros/test_link.py
+-rw-r--r--   0        0        0     1223 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/test_basic_text.py
+-rw-r--r--   0        0        0     2443 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/test_escaped.py
+-rw-r--r--   0        0        0     2624 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/test_style.py
+-rw-r--r--   0        0        0     1246 2024-04-28 20:04:41.977522 mau-4.0.1/tests/parsers/text_parser/test_verbatim.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.1/tests/text_buffer/__init__.py
+-rw-r--r--   0        0        0      386 2024-03-29 22:28:59.354920 mau-4.0.1/tests/text_buffer/test_context.py
+-rw-r--r--   0        0        0     4786 2024-03-29 22:28:59.354920 mau-4.0.1/tests/text_buffer/test_text_buffer.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.1/tests/tokens/__init__.py
+-rw-r--r--   0        0        0     2192 2024-03-29 22:28:59.350920 mau-4.0.1/tests/tokens/test_tokens.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.1/tests/visitors/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.1/tests/visitors/base_visitor/__init__.py
+-rw-r--r--   0        0        0     8808 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_block.py
+-rw-r--r--   0        0        0     3074 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_content.py
+-rw-r--r--   0        0        0     3093 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_footnotes.py
+-rw-r--r--   0        0        0     1556 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_header.py
+-rw-r--r--   0        0        0    13787 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_inline.py
+-rw-r--r--   0        0        0     2547 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_lists.py
+-rw-r--r--   0        0        0     2370 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_page.py
+-rw-r--r--   0        0        0     1872 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_paragraph.py
+-rw-r--r--   0        0        0     4295 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_source.py
+-rw-r--r--   0        0        0     5265 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/base_visitor/test_toc.py
+-rw-r--r--   0        0        0     6392 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_block.py
+-rw-r--r--   0        0        0     2115 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_content.py
+-rw-r--r--   0        0        0     1406 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_footnotes.py
+-rw-r--r--   0        0        0     1151 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_header.py
+-rw-r--r--   0        0        0     7556 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_inline.py
+-rw-r--r--   0        0        0     1638 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_lists.py
+-rw-r--r--   0        0        0      857 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_page.py
+-rw-r--r--   0        0        0     2069 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_paragraph.py
+-rw-r--r--   0        0        0     1283 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_source.py
+-rw-r--r--   0        0        0     7366 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/test_templates.py
+-rw-r--r--   0        0        0     1354 2024-04-28 20:04:41.977522 mau-4.0.1/tests/visitors/jinja_visitor/toc.py
+-rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 mau-4.0.1/PKG-INFO
```

### Comparing `mau-4.0.0/.gitignore` & `mau-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/CHANGELOG.rst` & `mau-4.0.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 4.0.1
+=============
+
+- [internal] Added end-to-end tests for BaseVisitor
+
 Version 4.0.0
 =============
 
 Please be aware that this major release contains breaking changes from Mau 3. All changes marked `syntax` are breaking and thus require manual modification of the Mau source.
 
 - [enhancement] Block aliases can be defined through the environment.
 - [enhancement] Header anchor can be forced through the attribute `anchor`.
```

### Comparing `mau-4.0.0/LICENSE` & `mau-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/README.md` & `mau-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/__init__.py` & `mau-4.0.1/mau/__init__.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/environment/environment.py` & `mau-4.0.1/mau/environment/environment.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/errors.py` & `mau-4.0.1/mau/errors.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/lexers/arguments_lexer.py` & `mau-4.0.1/mau/lexers/arguments_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/lexers/base_lexer.py` & `mau-4.0.1/mau/lexers/base_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/lexers/main_lexer.py` & `mau-4.0.1/mau/lexers/main_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/lexers/preprocess_variables_lexer.py` & `mau-4.0.1/mau/lexers/preprocess_variables_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/lexers/text_lexer.py` & `mau-4.0.1/mau/lexers/text_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/main.py` & `mau-4.0.1/mau/main.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/arguments.py` & `mau-4.0.1/mau/nodes/arguments.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/block.py` & `mau-4.0.1/mau/nodes/block.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/content.py` & `mau-4.0.1/mau/nodes/content.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/footnotes.py` & `mau-4.0.1/mau/nodes/footnotes.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/header.py` & `mau-4.0.1/mau/nodes/header.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/inline.py` & `mau-4.0.1/mau/nodes/inline.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/lists.py` & `mau-4.0.1/mau/nodes/lists.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/macros.py` & `mau-4.0.1/mau/nodes/macros.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/nodes.py` & `mau-4.0.1/mau/nodes/nodes.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/page.py` & `mau-4.0.1/mau/nodes/page.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/paragraph.py` & `mau-4.0.1/mau/nodes/paragraph.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/source.py` & `mau-4.0.1/mau/nodes/source.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/nodes/toc.py` & `mau-4.0.1/mau/nodes/toc.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/arguments.py` & `mau-4.0.1/mau/parsers/arguments.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/arguments_parser.py` & `mau-4.0.1/mau/parsers/arguments_parser.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/attributes.py` & `mau-4.0.1/mau/parsers/attributes.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/base_parser.py` & `mau-4.0.1/mau/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/footnotes.py` & `mau-4.0.1/mau/parsers/footnotes.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/internal_links.py` & `mau-4.0.1/mau/parsers/internal_links.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/main_parser.py` & `mau-4.0.1/mau/parsers/main_parser.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/preprocess_variables_parser.py` & `mau-4.0.1/mau/parsers/preprocess_variables_parser.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/text_parser.py` & `mau-4.0.1/mau/parsers/text_parser.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/parsers/toc.py` & `mau-4.0.1/mau/parsers/toc.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/text_buffer/context.py` & `mau-4.0.1/mau/text_buffer/context.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/text_buffer/text_buffer.py` & `mau-4.0.1/mau/text_buffer/text_buffer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/tokens/tokens.py` & `mau-4.0.1/mau/tokens/tokens.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/visitors/base_visitor.py` & `mau-4.0.1/mau/visitors/base_visitor.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/mau/visitors/jinja_visitor.py` & `mau-4.0.1/mau/visitors/jinja_visitor.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/pyproject.toml` & `mau-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mau"
-version = "4.0.0"
+version = "4.0.1"
 description = "A lightweight template-driven markup language"
 authors = [{name = "Leonardo Giordani", email = "giordani.leonardo@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
 "Development Status :: 5 - Production/Stable",
 "License :: OSI Approved :: MIT License",
 "Intended Audience :: Developers",
```

### Comparing `mau-4.0.0/tests/environment/test_environment.py` & `mau-4.0.1/tests/environment/test_environment.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/helpers.py` & `mau-4.0.1/mau/test_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import pytest
+import pathlib
+
+
 import textwrap
 
 from mau.environment.environment import Environment
 from mau.text_buffer.context import Context
 from mau.text_buffer.text_buffer import TextBuffer
 
 
@@ -83,7 +87,30 @@
         parser = init_parser(textwrap.dedent(source), environment, *args, **kwds)
         parser.parse(parser.tokens)
         parser.finalise()
 
         return parser
 
     return _run
+
+
+def load_files(source_dir, source_ext, expected_dir, expected_ext):
+    source_files = pathlib.Path(source_dir).rglob(f"*.{source_ext}")
+
+    files = [
+        (i, expected_dir / i.with_suffix(f".{expected_ext}").relative_to(source_dir))
+        for i in source_files
+    ]
+
+    return files
+
+
+def collect_test_files(
+    tests_dir, source_dir_name, source_ext, expected_dir_name, expected_ext
+):
+    source_dir = tests_dir / source_dir_name
+    expected_dir = tests_dir / expected_dir_name
+
+    return [
+        pytest.param(i, j, id=str(i.relative_to(tests_dir)))
+        for i, j in load_files(source_dir, source_ext, expected_dir, expected_ext)
+    ]
```

### Comparing `mau-4.0.0/tests/lexers/test_arguments_lexer.py` & `mau-4.0.1/tests/lexers/test_arguments_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/lexers/test_base_lexer.py` & `mau-4.0.1/tests/lexers/test_base_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/lexers/test_main_lexer.py` & `mau-4.0.1/tests/lexers/test_main_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/lexers/test_preprocess_variables_lexer.py` & `mau-4.0.1/tests/lexers/test_preprocess_variables_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/lexers/test_text_lexer.py` & `mau-4.0.1/tests/lexers/test_text_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_arguments.py` & `mau-4.0.1/tests/nodes/test_arguments.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_content.py` & `mau-4.0.1/tests/nodes/test_content.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_footnotes.py` & `mau-4.0.1/tests/nodes/test_footnotes.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_header.py` & `mau-4.0.1/tests/nodes/test_header.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_inline.py` & `mau-4.0.1/tests/nodes/test_inline.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_lists.py` & `mau-4.0.1/tests/nodes/test_lists.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_macros.py` & `mau-4.0.1/tests/nodes/test_macros.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_nodes.py` & `mau-4.0.1/tests/nodes/test_nodes.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_page.py` & `mau-4.0.1/tests/nodes/test_page.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_paragraph.py` & `mau-4.0.1/tests/nodes/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_source.py` & `mau-4.0.1/tests/nodes/test_source.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/nodes/test_toc.py` & `mau-4.0.1/tests/nodes/test_toc.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_arguments.py` & `mau-4.0.1/tests/parsers/main_parser/test_arguments.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_block_attributes.py` & `mau-4.0.1/tests/parsers/main_parser/test_block_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from unittest.mock import patch
+
 import pytest
 from mau.environment.environment import Environment
 from mau.errors import MauErrorException
 from mau.lexers.main_lexer import MainLexer
 from mau.nodes.block import BlockNode
 from mau.nodes.header import HeaderNode
 from mau.nodes.inline import SentenceNode, TextNode
```

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_block_basic.py` & `mau-4.0.1/tests/parsers/main_parser/test_block_basic.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_block_engine_group.py` & `mau-4.0.1/tests/parsers/main_parser/test_block_engine_group.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_block_engine_mau.py` & `mau-4.0.1/tests/parsers/main_parser/test_block_engine_mau.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_block_engine_raw.py` & `mau-4.0.1/tests/parsers/main_parser/test_block_engine_raw.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_block_other.py` & `mau-4.0.1/tests/parsers/main_parser/test_block_other.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_content.py` & `mau-4.0.1/tests/parsers/main_parser/test_content.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_control.py` & `mau-4.0.1/tests/parsers/main_parser/test_control.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_footnotes.py` & `mau-4.0.1/tests/parsers/main_parser/test_footnotes.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_headers.py` & `mau-4.0.1/tests/parsers/main_parser/test_headers.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_horizontal_rule.py` & `mau-4.0.1/tests/parsers/main_parser/test_horizontal_rule.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_internal_links.py` & `mau-4.0.1/tests/parsers/main_parser/test_internal_links.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_lists.py` & `mau-4.0.1/tests/parsers/main_parser/test_lists.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_main_parser.py` & `mau-4.0.1/tests/parsers/main_parser/test_main_parser.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_paragraph.py` & `mau-4.0.1/tests/parsers/main_parser/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_parent.py` & `mau-4.0.1/tests/parsers/main_parser/test_parent.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_source.py` & `mau-4.0.1/tests/parsers/main_parser/test_source.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_title.py` & `mau-4.0.1/tests/parsers/main_parser/test_title.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_toc.py` & `mau-4.0.1/tests/parsers/main_parser/test_toc.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/main_parser/test_variables.py` & `mau-4.0.1/tests/parsers/main_parser/test_variables.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/test_arguments_parser.py` & `mau-4.0.1/tests/parsers/test_arguments_parser.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/test_base_parser.py` & `mau-4.0.1/tests/parsers/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/test_create_toc.py` & `mau-4.0.1/tests/parsers/test_create_toc.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/test_preprocess_variables_parser.py` & `mau-4.0.1/tests/parsers/test_preprocess_variables_parser.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/macros/test_arguments.py` & `mau-4.0.1/tests/parsers/text_parser/macros/test_arguments.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/macros/test_class.py` & `mau-4.0.1/tests/parsers/text_parser/macros/test_class.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/macros/test_control.py` & `mau-4.0.1/tests/parsers/text_parser/macros/test_control.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/macros/test_footnote.py` & `mau-4.0.1/tests/parsers/text_parser/macros/test_footnote.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/macros/test_generic_macro.py` & `mau-4.0.1/tests/parsers/text_parser/macros/test_generic_macro.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/macros/test_header.py` & `mau-4.0.1/tests/parsers/text_parser/macros/test_header.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/macros/test_image.py` & `mau-4.0.1/tests/parsers/text_parser/macros/test_image.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/macros/test_link.py` & `mau-4.0.1/tests/parsers/text_parser/macros/test_link.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/test_basic_text.py` & `mau-4.0.1/tests/parsers/text_parser/test_basic_text.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/test_escaped.py` & `mau-4.0.1/tests/parsers/text_parser/test_escaped.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/test_style.py` & `mau-4.0.1/tests/parsers/text_parser/test_style.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/parsers/text_parser/test_verbatim.py` & `mau-4.0.1/tests/parsers/text_parser/test_verbatim.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/text_buffer/test_text_buffer.py` & `mau-4.0.1/tests/text_buffer/test_text_buffer.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/tokens/test_tokens.py` & `mau-4.0.1/tests/tokens/test_tokens.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_block.py` & `mau-4.0.1/tests/visitors/base_visitor/test_block.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_content.py` & `mau-4.0.1/tests/visitors/base_visitor/test_content.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_footnotes.py` & `mau-4.0.1/tests/visitors/base_visitor/test_footnotes.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_header.py` & `mau-4.0.1/tests/visitors/base_visitor/test_header.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_inline.py` & `mau-4.0.1/tests/visitors/base_visitor/test_inline.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_lists.py` & `mau-4.0.1/tests/visitors/base_visitor/test_lists.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_page.py` & `mau-4.0.1/tests/visitors/base_visitor/test_page.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_paragraph.py` & `mau-4.0.1/tests/visitors/base_visitor/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_source.py` & `mau-4.0.1/tests/visitors/base_visitor/test_source.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/base_visitor/test_toc.py` & `mau-4.0.1/tests/visitors/base_visitor/test_toc.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_block.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_block.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_content.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_content.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_footnotes.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_footnotes.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_header.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_header.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_inline.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_inline.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_lists.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_lists.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_page.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_page.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_paragraph.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_source.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_source.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/test_templates.py` & `mau-4.0.1/tests/visitors/jinja_visitor/test_templates.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/tests/visitors/jinja_visitor/toc.py` & `mau-4.0.1/tests/visitors/jinja_visitor/toc.py`

 * *Files identical despite different names*

### Comparing `mau-4.0.0/PKG-INFO` & `mau-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mau
-Version: 4.0.0
+Version: 4.0.1
 Summary: A lightweight template-driven markup language
 Author-email: Leonardo Giordani <giordani.leonardo@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

