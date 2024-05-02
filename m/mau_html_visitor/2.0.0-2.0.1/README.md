# Comparing `tmp/mau_html_visitor-2.0.0.tar.gz` & `tmp/mau_html_visitor-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mau_html_visitor-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mau_html_visitor-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mau_html_visitor-2.0.0.tar` & `mau_html_visitor-2.0.1.tar`

### file list

```diff
@@ -1,39 +1,114 @@
--rw-r--r--   0        0        0     3077 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/.gitignore
--rw-r--r--   0        0        0      493 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1084 2023-08-14 21:18:34.423988 mau_html_visitor-2.0.0/LICENSE
--rw-r--r--   0        0        0      982 2023-08-14 21:09:11.770701 mau_html_visitor-2.0.0/README.md
--rw-r--r--   0        0        0     3572 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/__init__.py
--rw-r--r--   0        0        0      210 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/block.html
--rw-r--r--   0        0        0      190 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/block/admonition.html
--rw-r--r--   0        0        0       82 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/block/quote.html
--rw-r--r--   0        0        0      143 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/block_group.html
--rw-r--r--   0        0        0       42 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/callout.html
--rw-r--r--   0        0        0       87 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/callouts_entry.html
--rw-r--r--   0        0        0       14 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/container.html
--rw-r--r--   0        0        0      211 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/content_image.html
--rw-r--r--   0        0        0       60 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/document.html
--rw-r--r--   0        0        0       94 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/footnote.html
--rw-r--r--   0        0        0       45 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/footnotes.html
--rw-r--r--   0        0        0      107 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/footnotes_entry.html
--rw-r--r--   0        0        0       59 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/header.html
--rw-r--r--   0        0        0        5 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/horizontal_rule.html
--rw-r--r--   0        0        0      119 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/list.html
--rw-r--r--   0        0        0       23 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/list_item.html
--rw-r--r--   0        0        0       61 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/macro/class.html
--rw-r--r--   0        0        0       49 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/macro/header.html
--rw-r--r--   0        0        0      102 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/macro/image.html
--rw-r--r--   0        0        0       41 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/macro/link.html
--rw-r--r--   0        0        0       21 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/paragraph.html
--rw-r--r--   0        0        0       12 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/raw.html
--rw-r--r--   0        0        0       14 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/sentence.html
--rw-r--r--   0        0        0      467 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/source.html
--rw-r--r--   0        0        0       25 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/style/caret.html
--rw-r--r--   0        0        0       31 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/style/star.html
--rw-r--r--   0        0        0       25 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/style/tilde.html
--rw-r--r--   0        0        0       23 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/style/underscore.html
--rw-r--r--   0        0        0       12 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/text.html
--rw-r--r--   0        0        0       70 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/toc.html
--rw-r--r--   0        0        0      107 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/toc_entry.html
--rw-r--r--   0        0        0       25 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/verbatim.html
--rw-r--r--   0        0        0     1949 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 mau_html_visitor-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3077 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/.gitignore
+-rw-r--r--   0        0        0      575 2024-04-29 16:40:26.490005 mau_html_visitor-2.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1084 2023-08-14 21:18:34.423988 mau_html_visitor-2.0.1/LICENSE
+-rw-r--r--   0        0        0      982 2023-08-14 21:09:11.770701 mau_html_visitor-2.0.1/README.md
+-rw-r--r--   0        0        0     3572 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/__init__.py
+-rw-r--r--   0        0        0      210 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/block.html
+-rw-r--r--   0        0        0      190 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/block/admonition.html
+-rw-r--r--   0        0        0       82 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/block/quote.html
+-rw-r--r--   0        0        0      143 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/block_group.html
+-rw-r--r--   0        0        0       42 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/callout.html
+-rw-r--r--   0        0        0       87 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/callouts_entry.html
+-rw-r--r--   0        0        0       14 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/container.html
+-rw-r--r--   0        0        0      211 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/content_image.html
+-rw-r--r--   0        0        0       60 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/document.html
+-rw-r--r--   0        0        0       94 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/footnote.html
+-rw-r--r--   0        0        0       45 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/footnotes.html
+-rw-r--r--   0        0        0      107 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/footnotes_entry.html
+-rw-r--r--   0        0        0       59 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/header.html
+-rw-r--r--   0        0        0        5 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/horizontal_rule.html
+-rw-r--r--   0        0        0      119 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/list.html
+-rw-r--r--   0        0        0       23 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/list_item.html
+-rw-r--r--   0        0        0       61 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/macro/class.html
+-rw-r--r--   0        0        0       49 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/macro/header.html
+-rw-r--r--   0        0        0      102 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/macro/image.html
+-rw-r--r--   0        0        0       41 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/macro/link.html
+-rw-r--r--   0        0        0       21 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/paragraph.html
+-rw-r--r--   0        0        0       12 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/raw.html
+-rw-r--r--   0        0        0       14 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/sentence.html
+-rw-r--r--   0        0        0      467 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/source.html
+-rw-r--r--   0        0        0       25 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/style/caret.html
+-rw-r--r--   0        0        0       31 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/style/star.html
+-rw-r--r--   0        0        0       25 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/style/tilde.html
+-rw-r--r--   0        0        0       23 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/style/underscore.html
+-rw-r--r--   0        0        0       12 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/text.html
+-rw-r--r--   0        0        0       70 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/toc.html
+-rw-r--r--   0        0        0      107 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/toc_entry.html
+-rw-r--r--   0        0        0       25 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.1/mau_html_visitor/templates/verbatim.html
+-rw-r--r--   0        0        0     1829 2024-04-29 16:40:26.490005 mau_html_visitor-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      578 2024-04-29 16:40:26.490005 mau_html_visitor-2.0.1/tests/e2e/expected/block/block_admonition.html
+-rw-r--r--   0        0        0      176 2024-04-29 16:40:26.490005 mau_html_visitor-2.0.1/tests/e2e/expected/block/block_conditionals.html
+-rw-r--r--   0        0        0      374 2024-04-29 16:40:26.490005 mau_html_visitor-2.0.1/tests/e2e/expected/block/block_quote.html
+-rw-r--r--   0        0        0      583 2024-04-29 16:40:26.490005 mau_html_visitor-2.0.1/tests/e2e/expected/block/block_simple.html
+-rw-r--r--   0        0        0      205 2024-04-29 16:40:26.490005 mau_html_visitor-2.0.1/tests/e2e/expected/block/block_title.html
+-rw-r--r--   0        0        0      408 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/commands/footnotes.html
+-rw-r--r--   0        0        0     2263 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/commands/footnotes_advanced.html
+-rw-r--r--   0        0        0      661 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/commands/references.html
+-rw-r--r--   0        0        0      230 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/commands/toc.html
+-rw-r--r--   0        0        0     1677 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/commands/toc_advanced.html
+-rw-r--r--   0        0        0      148 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/classes.html
+-rw-r--r--   0        0        0      140 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/conditionals.html
+-rw-r--r--   0        0        0      228 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/inline_image.html
+-rw-r--r--   0        0        0      178 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/internal_link.html
+-rw-r--r--   0        0        0      440 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/link.html
+-rw-r--r--   0        0        0      255 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/mailto.html
+-rw-r--r--   0        0        0      167 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/multiple_paragraphs.html
+-rw-r--r--   0        0        0      113 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/single_paragraph.html
+-rw-r--r--   0        0        0      182 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/split_paragraph.html
+-rw-r--r--   0        0        0      366 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/styles.html
+-rw-r--r--   0        0        0      697 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/styles_mixed.html
+-rw-r--r--   0        0        0      135 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/inline/verbatim.html
+-rw-r--r--   0        0        0      224 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/other/directives.html
+-rw-r--r--   0        0        0      306 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/other/variable_advanced.html
+-rw-r--r--   0        0        0      309 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/other/variable_simple.html
+-rw-r--r--   0        0        0       54 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/page/comments.html
+-rw-r--r--   0        0        0      192 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/page/header_multiple.html
+-rw-r--r--   0        0        0      100 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/page/header_single.html
+-rw-r--r--   0        0        0      300 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/page/header_with_paragraphs.html
+-rw-r--r--   0        0        0      193 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/page/horizontal_line.html
+-rw-r--r--   0        0        0      450 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/page/image.html
+-rw-r--r--   0        0        0      325 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/page/list_ordered.html
+-rw-r--r--   0        0        0      698 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/page/list_start.html
+-rw-r--r--   0        0        0      307 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/page/list_unordered.html
+-rw-r--r--   0        0        0     1838 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/source/source_callouts.html
+-rw-r--r--   0        0        0     1784 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/source/source_highlight.html
+-rw-r--r--   0        0        0      339 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/expected/source/source_simple.html
+-rw-r--r--   0        0        0      248 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/block/block_admonition.mau
+-rw-r--r--   0        0        0      131 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/block/block_conditionals.mau
+-rw-r--r--   0        0        0      201 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/block/block_quote.mau
+-rw-r--r--   0        0        0      237 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/block/block_simple.mau
+-rw-r--r--   0        0        0       38 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/block/block_title.mau
+-rw-r--r--   0        0        0      108 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/commands/footnotes.mau
+-rw-r--r--   0        0        0      682 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/commands/footnotes_advanced.mau
+-rw-r--r--   0        0        0       20 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/commands/toc.mau
+-rw-r--r--   0        0        0      327 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/commands/toc_advanced.mau
+-rw-r--r--   0        0        0       56 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/classes.mau
+-rw-r--r--   0        0        0      131 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/conditionals.mau
+-rw-r--r--   0        0        0      107 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/inline_image.mau
+-rw-r--r--   0        0        0       68 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/internal_link.mau
+-rw-r--r--   0        0        0      228 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/link.mau
+-rw-r--r--   0        0        0      121 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/mailto.mau
+-rw-r--r--   0        0        0       82 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/multiple_paragraphs.mau
+-rw-r--r--   0        0        0       43 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/single_paragraph.mau
+-rw-r--r--   0        0        0      112 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/split_paragraph.mau
+-rw-r--r--   0        0        0      159 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/styles.mau
+-rw-r--r--   0        0        0      366 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/styles_mixed.mau
+-rw-r--r--   0        0        0       41 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/inline/verbatim.mau
+-rw-r--r--   0        0        0      102 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/other/directives.mau
+-rw-r--r--   0        0        0       48 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/other/include_text.txt
+-rw-r--r--   0        0        0      257 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/other/variable_advanced.mau
+-rw-r--r--   0        0        0      219 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/other/variable_simple.mau
+-rw-r--r--   0        0        0      129 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/page/comments.mau
+-rw-r--r--   0        0        0       38 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/page/header_multiple.mau
+-rw-r--r--   0        0        0       11 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/page/header_single.mau
+-rw-r--r--   0        0        0      101 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/page/header_with_paragraphs.mau
+-rw-r--r--   0        0        0      104 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/page/horizontal_line.mau
+-rw-r--r--   0        0        0      228 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/page/image.mau
+-rw-r--r--   0        0        0       76 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/page/list_ordered.mau
+-rw-r--r--   0        0        0      287 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/page/list_start.mau
+-rw-r--r--   0        0        0       78 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/page/list_unordered.mau
+-rw-r--r--   0        0        0      241 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/source/source_callouts.mau
+-rw-r--r--   0        0        0      441 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/source/source_highlight.mau
+-rw-r--r--   0        0        0      124 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/source/source/source_simple.mau
+-rw-r--r--   0        0        0     1406 2024-04-29 16:40:26.494005 mau_html_visitor-2.0.1/tests/e2e/test_e2e.py
+-rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 mau_html_visitor-2.0.1/PKG-INFO
```

### Comparing `mau_html_visitor-2.0.0/.gitignore` & `mau_html_visitor-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mau_html_visitor-2.0.0/LICENSE` & `mau_html_visitor-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mau_html_visitor-2.0.0/README.md` & `mau_html_visitor-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mau_html_visitor-2.0.0/mau_html_visitor/__init__.py` & `mau_html_visitor-2.0.1/mau_html_visitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mau_html_visitor-2.0.0/pyproject.toml` & `mau_html_visitor-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mau_html_visitor"
-version = "2.0.0"
+version = "2.0.1"
 description = "A visitor for Mau that converts the AST into HTML"
 authors = [{name = "Leonardo Giordani", email = "giordani.leonardo@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
 "Development Status :: 5 - Production/Stable",
 "License :: OSI Approved :: MIT License",
 "Intended Audience :: Developers",
@@ -72,16 +72,7 @@
 "too-many-return-statements",
 "use-implicit-booleaness-not-comparison"
 ]
 
 [tool.isort]
 profile = "black"
 src_paths = ["src", "tests"]
-
-[tool.pytest.ini_options]
-addopts = """\
---cov mau \
---cov tests \
---cov-report term-missing \
---no-cov-on-fail \
-"""
-
```

### Comparing `mau_html_visitor-2.0.0/PKG-INFO` & `mau_html_visitor-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mau_html_visitor
-Version: 2.0.0
+Version: 2.0.1
 Summary: A visitor for Mau that converts the AST into HTML
 Author-email: Leonardo Giordani <giordani.leonardo@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

