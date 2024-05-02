# Comparing `tmp/robotcode_language_server-0.79.0.tar.gz` & `tmp/robotcode_language_server-0.80.0.tar.gz`

## Comparing `robotcode_language_server-0.79.0.tar` & `robotcode_language_server-0.80.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    29749 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0     9382 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18904 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0     9948 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0     8457 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_action_helper_mixin.py
--rw-r--r--   0        0        0    30803 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_action_quick_fixes.py
--rw-r--r--   0        0        0    25436 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_action_refactor.py
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_lens.py
--rw-r--r--   0        0        0    99859 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    18825 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/http_server.py
--rw-r--r--   0        0        0    13356 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/keywords_treeview.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24938 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     7332 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    47991 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/README.md
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/pyproject.toml
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 robotcode_language_server-0.79.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    29749 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0     9382 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    18904 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0     9948 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0     8457 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_action_helper_mixin.py
+-rw-r--r--   0        0        0    30803 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_action_quick_fixes.py
+-rw-r--r--   0        0        0    25436 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_action_refactor.py
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_lens.py
+-rw-r--r--   0        0        0    99859 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    18825 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/http_server.py
+-rw-r--r--   0        0        0    13356 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/keywords_treeview.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24938 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     7332 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    47991 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/LICENSE.txt
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/README.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/pyproject.toml
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 robotcode_language_server-0.80.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/protocol_part.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/protocol_part.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_action_helper_mixin.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_action_helper_mixin.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_action_quick_fixes.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_action_quick_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_action_refactor.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_action_refactor.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/code_lens.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/http_server.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/http_server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/keywords_treeview.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/keywords_treeview.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.80.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/.gitignore` & `robotcode_language_server-0.80.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/LICENSE.txt` & `robotcode_language_server-0.80.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.79.0/README.md` & `robotcode_language_server-0.80.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
-[![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
+[![License](https://img.shields.io/github/license/robotcodedev/robotcode?style=flat&logo=apache)](https://github.com/robotcodedev/robotcode/blob/master/LICENSE.txt)
 
 -----
 
 ## Introduction
 
 The Language Server for [RobotCode](https://robotcode.io).
```

### Comparing `robotcode_language_server-0.79.0/pyproject.toml` & `robotcode_language_server-0.80.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -23,30 +23,30 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.79.0",
-  "robotcode-robot==0.79.0",
-  "robotcode==0.79.0",
+  "robotcode-jsonrpc2==0.80.0",
+  "robotcode-robot==0.80.0",
+  "robotcode==0.80.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
-Documentation = "https://github.com/d-biehl/robotcode#readme"
-Changelog = "https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md"
-Issues = "https://github.com/d-biehl/robotcode/issues"
-Source = "https://github.com/d-biehl/robotcode"
+Documentation = "https://github.com/robotcodedev/robotcode#readme"
+Changelog = "https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md"
+Issues = "https://github.com/robotcodedev/robotcode/issues"
+Source = "https://github.com/robotcodedev/robotcode"
 
 [tool.hatch.version]
 path = "src/robotcode/language_server/__version__.py"
 
 [tool.hatch.build]
 dev-mode-dirs = ["src"]
```

