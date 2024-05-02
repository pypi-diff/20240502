# Comparing `tmp/hexdoc-1!0.1.0a8.tar.gz` & `tmp/hexdoc-1!0.1.0a9.tar.gz`

## Comparing `hexdoc-1!0.1.0a8.tar` & `hexdoc-1!0.1.0a9.tar`

### file list

```diff
@@ -1,149 +1,182 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/__version__.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/py.typed
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/generated/__init__.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/generated/hexdoc.hexdoc.json
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/generated/assets/hexdoc/textures/gui/crafting_table.png
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/generated/assets/hexdoc/textures/gui/spotlight.png
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/generated/assets/hexdoc/textures/item/missing.png
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/emi/LICENSE
--rw-r--r--   0        0        0    18419 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/emi/lang/en_us.json
--rw-r--r--   0        0        0    24668 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/emi/lang/ru_ru.json
--rw-r--r--   0        0        0    16205 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/emi/lang/zh_cn.json
--rw-r--r--   0        0        0    15814 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/forge/lang/en_us.json
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/hexdoc/lang/en_us.flatten.json5
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/hexdoc/lang/zh_cn.flatten.json5
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/hexdoc/textures/gui/crafting_table.png
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/hexdoc/textures/gui/spotlight.png
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/hexdoc/textures/item/missing.png
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/data/hexdoc/tags/advancements/spoilered.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/data/hexdoc/tags/items/gaslighting.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/book.html.jinja
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/category.html.jinja
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/entry.html.jinja
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/index.css.jinja
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/index.html.jinja
--rw-r--r--   0        0        0    10339 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/index.js.jinja
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/redirect.html.jinja
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/textures.jcss.jinja
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/components/navbar.html.jinja
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/components/opengraph.html.jinja
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/components/table_of_contents.html.jinja
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/components/welcome.html.jinja
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/macros/formatting.html.jinja
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/macros/recipes.html.jinja
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/macros/styles.html.jinja
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/macros/textures.html.jinja
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/pages/patchouli/crafting.html.jinja
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/pages/patchouli/image.html.jinja
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/pages/patchouli/link.html.jinja
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/pages/patchouli/page.html.jinja
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/pages/patchouli/spotlight.html.jinja
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/_templates/pages/patchouli/text.html.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/cli/__init__.py
--rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/cli/app.py
--rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/cli/ci.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/cli/render_block.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/cli/utils/__init__.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/cli/utils/args.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/cli/utils/load.py
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/cli/utils/render.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/cli/utils/sitemap.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/core/__init__.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/core/compat.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/core/loader.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/core/properties.py
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/core/resource.py
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/core/resource_dir.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/data/__init__.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/data/metadata.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/jinja/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/jinja/extensions.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/jinja/filters.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/__init__.py
--rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/i18n.py
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/tags.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/__init__.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/animated.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/constants.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/items.py
--rw-r--r--   0        0        0    10972 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/load_assets.py
--rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/models.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/textures.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/with_texture.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/recipe/__init__.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/recipe/ingredients.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/minecraft/recipe/recipes.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/model/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/model/base.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/model/id.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/model/inline.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/model/strip_hidden.py
--rw-r--r--   0        0        0     9491 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/model/tagged_union.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/model/types.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/patchouli/__init__.py
--rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/patchouli/book.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/patchouli/book_context.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/patchouli/category.py
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/patchouli/entry.py
--rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/patchouli/text.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/patchouli/page/__init__.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/patchouli/page/abstract_pages.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/patchouli/page/pages.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/plugin/__init__.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/plugin/book_plugin.py
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/plugin/manager.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/plugin/mod_plugin.py
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/plugin/specs.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/plugin/types.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/cd.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/classproperties.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/context.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/contextmanagers.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/git.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/iterators.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/logging.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/path.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/singletons.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/types.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/deserialize/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/deserialize/assertions.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/deserialize/json.py
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc/utils/deserialize/toml.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/__init__.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/_hooks.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/book.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/category.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/condition.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/entry.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/_export/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/_export/generated/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/_export/resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/_templates/__init__.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/page/__init__.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/page/abstract_pages.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/page/pages.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/README.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/__init__.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_constants.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_exceptions.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_generate.py
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/py.typed
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_types/__init__.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_types/color.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_types/properties.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/LICENSE
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/README.md
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/__version__.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/py.typed
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/__init__.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/hexdoc.hexdoc.json
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/hexdoc/textures/gui/any_block.png
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/hexdoc/textures/gui/spotlight.png
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/hexdoc/textures/item/missing.png
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/minecraft/textures/gui/hexdoc/blast_furnace.png
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/minecraft/textures/gui/hexdoc/campfire.png
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/minecraft/textures/gui/hexdoc/crafting_table.png
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/minecraft/textures/gui/hexdoc/furnace.png
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/minecraft/textures/gui/hexdoc/smithing_table.png
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/minecraft/textures/gui/hexdoc/smoker.png
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/minecraft/textures/gui/hexdoc/stonecutter.png
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/minecraft/textures/gui/hexdoc/legacy/smithing_table.png
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/emi/LICENSE
+-rw-r--r--   0        0        0    18419 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/emi/lang/en_us.json
+-rw-r--r--   0        0        0    24668 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/emi/lang/ru_ru.json
+-rw-r--r--   0        0        0    16205 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/emi/lang/zh_cn.json
+-rw-r--r--   0        0        0    15814 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/forge/lang/en_us.json
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/hexdoc/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/hexdoc/lang/zh_cn.flatten.json5
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/hexdoc/textures/gui/any_block.png
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/hexdoc/textures/gui/spotlight.png
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/hexdoc/textures/item/missing.png
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/minecraft/textures/gui/hexdoc/blast_furnace.png
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/minecraft/textures/gui/hexdoc/campfire.png
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/minecraft/textures/gui/hexdoc/crafting_table.png
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/minecraft/textures/gui/hexdoc/furnace.png
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/minecraft/textures/gui/hexdoc/smithing_table.png
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/minecraft/textures/gui/hexdoc/smoker.png
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/minecraft/textures/gui/hexdoc/stonecutter.png
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/minecraft/textures/gui/hexdoc/legacy/smithing_table.png
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/data/hexdoc/tags/advancements/spoilered.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/data/hexdoc/tags/items/gaslighting.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/book.html.jinja
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/category.html.jinja
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/entry.html.jinja
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/index.css.jinja
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/index.html.jinja
+-rw-r--r--   0        0        0    10586 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/index.js.jinja
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/redirect.html.jinja
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/textures.jcss.jinja
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/components/navbar.html.jinja
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/components/opengraph.html.jinja
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/components/table_of_contents.html.jinja
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/components/welcome.html.jinja
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/macros/formatting.html.jinja
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/macros/recipes.html.jinja
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/macros/styles.html.jinja
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/macros/textures.html.jinja
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/blasting.html.jinja
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/campfire_cooking.html.jinja
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/crafting.html.jinja
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/image.html.jinja
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/link.html.jinja
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/multiblock.html.jinja
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/page.html.jinja
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/quest.html.jinja
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/recipes.html.jinja
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/smelting.html.jinja
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/smithing.html.jinja
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/smoking.html.jinja
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/spotlight.html.jinja
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/stonecutting.html.jinja
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/text.html.jinja
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/recipes/base.html.jinja
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/recipes/minecraft/blast_furnace.html.jinja
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/recipes/minecraft/campfire.html.jinja
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/recipes/minecraft/crafting_table.html.jinja
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/recipes/minecraft/furnace.html.jinja
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/recipes/minecraft/smithing_table.html.jinja
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/recipes/minecraft/smoker.html.jinja
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/_templates/recipes/minecraft/stonecutter.html.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/cli/__init__.py
+-rw-r--r--   0        0        0    14371 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/cli/app.py
+-rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/cli/ci.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/cli/render_block.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/cli/utils/args.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/cli/utils/load.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/core/__init__.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/core/compat.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/core/loader.py
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/core/properties.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/core/resource.py
+-rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/core/resource_dir.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/data/__init__.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/data/metadata.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/data/sitemap.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/jinja/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/jinja/extensions.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/jinja/filters.py
+-rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/jinja/render.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/__init__.py
+-rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/i18n.py
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/tags.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/__init__.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/animated.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/constants.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/items.py
+-rw-r--r--   0        0        0    11398 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/load_assets.py
+-rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/models.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/textures.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/with_texture.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/recipe/__init__.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/recipe/ingredients.py
+-rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/minecraft/recipe/recipes.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/model/__init__.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/model/base.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/model/id.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/model/inline.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/model/strip_hidden.py
+-rw-r--r--   0        0        0     9491 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/model/tagged_union.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/model/types.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/patchouli/__init__.py
+-rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/patchouli/book.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/patchouli/book_context.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/patchouli/category.py
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/patchouli/entry.py
+-rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/patchouli/text.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/patchouli/page/__init__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/patchouli/page/abstract_pages.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/patchouli/page/pages.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/plugin/__init__.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/plugin/book_plugin.py
+-rw-r--r--   0        0        0     9961 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/plugin/manager.py
+-rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/plugin/mod_plugin.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/plugin/specs.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/plugin/types.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/cd.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/classproperties.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/context.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/contextmanagers.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/git.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/iterators.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/logging.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/path.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/singletons.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/types.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/deserialize/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/deserialize/assertions.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/deserialize/json.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc/utils/deserialize/toml.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/__init__.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/_hooks.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/book.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/category.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/condition.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/entry.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/_export/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/_export/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/_export/generated/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/_export/resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/_templates/__init__.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/page/__init__.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/page/abstract_pages.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/page/pages.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/README.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/__init__.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_constants.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_exceptions.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_generate.py
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/py.typed
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_types/__init__.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_types/color.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_types/properties.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/LICENSE
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/README.md
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0     7991 2020-02-02 00:00:00.000000 hexdoc-1!0.1.0a9/PKG-INFO
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_hooks.py` & `hexdoc-1!0.1.0a9/src/hexdoc/_hooks.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_export/generated/assets/hexdoc/textures/gui/spotlight.png` & `hexdoc-1!0.1.0a9/src/hexdoc/_export/generated/assets/hexdoc/textures/gui/spotlight.png`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/emi/LICENSE` & `hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/emi/LICENSE`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/emi/lang/en_us.json` & `hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/emi/lang/en_us.json`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/emi/lang/ru_ru.json` & `hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/emi/lang/ru_ru.json`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/emi/lang/zh_cn.json` & `hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/emi/lang/zh_cn.json`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/forge/lang/en_us.json` & `hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/forge/lang/en_us.json`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/hexdoc/lang/en_us.flatten.json5` & `hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/hexdoc/lang/en_us.flatten.json5`

 * *Files 13% similar despite different names*

```diff
@@ -20,12 +20,23 @@
     },
 
     linkout: "Link: ",
 
     recipe: {
       show: "Click to show recipes",
       hide: "Click to hide recipes",
+      smelting: {
+        cooktime: "{} Seconds",
+        exp: "{} XP"
+      }
+    },
+
+    multiblock: {
+      show: "Click to show multiblock",
+      hide: "Click to hide multiblock",
     },
 
     when_clicked: "When clicked, would execute: {}",
+
+    any_block:  "Any Block",
   },
 }
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/hexdoc/lang/zh_cn.flatten.json5` & `hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/hexdoc/lang/zh_cn.flatten.json5`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_export/resources/assets/hexdoc/textures/gui/spotlight.png` & `hexdoc-1!0.1.0a9/src/hexdoc/_export/resources/assets/hexdoc/textures/gui/spotlight.png`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/book.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/book.html.jinja`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/index.css.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/index.css.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -125,20 +125,19 @@
 
   display: grid;
   grid: repeat(3, 32px) / repeat(3, 32px);
   gap: 4px;
 }
 
 .crafting-table-result {
-  position: absolute;
   top: 50px;
   left: 202px;
 }
 
-.crafting-table-result .badge {
+.item-texture-count {
   position: absolute;
   background-color: #292929;
   bottom: -4px;
   right: -4px;
 }
 
 .item-texture {
@@ -150,14 +149,101 @@
   image-rendering: pixelated;
 }
 
 .multi-textures .texture {
   position: absolute;
 }
 
+.item-slot {
+  position: relative;
+  width: min-content;
+}
+
+.item-slot > .texture {
+  position: absolute;
+  top: 10px;
+  left: 10px;
+}
+
+.extra-info .texture {
+  width: 16px;
+  height: 16px;
+  margin: 2px;
+}
+
+.extra-info {
+  display: grid;
+  grid-auto-flow: column;
+  align-items: center;
+  justify-content: start;
+}
+
+.recipe {
+  position:relative;
+}
+
+.recipe-item-slot {
+  position: absolute;
+}
+
+.smelting-input {
+  top: 50px;
+  left: 54px;
+}
+
+.smelting-result {
+  top: 50px;
+  left: 174px;
+}
+
+.stonecutting-input {
+  top: 50px;
+  left: 54px;
+}
+
+.stonecutting-result {
+  top: 50px;
+  left: 174px;
+}
+
+.smithing-template {
+  top: 64px;
+  left: 34px;
+}
+
+.smithing-base {
+  top: 64px;
+  left: 70px;
+}
+
+.smithing-addition {
+  top: 64px;
+  left: 106px;
+}
+
+.smithing-result {
+  top: 64px;
+  left: 198px;
+}
+
+.multiblock-details {
+  width: max-content;
+}
+
+.multiblock-ingredient {
+  display: grid;
+  grid-auto-flow: column;
+  justify-content: start;
+  align-items: center;
+}
+
+.multiblock-ingredient .item-slot {
+  margin-right: 4px;
+}
+
 .toc-elem > .texture {
   margin-right: 2px;
   display: inline-block;
   vertical-align: middle;
   position: relative;
 }
 
@@ -248,14 +334,15 @@
   top: 0;
   left: 100%;
   margin-top: -6px;
   margin-left: -1px;
   -webkit-border-radius: 0 6px 6px 6px;
   -moz-border-radius: 0 6px 6px;
   border-radius: 0 6px 6px 6px;
+  width: max-content;
 }
 
 .dropdown-submenu:hover > .dropdown-menu {
   display: block;
 }
 
 .dropdown-submenu > a:after {
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/index.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/index.html.jinja`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/index.js.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/index.js.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -176,26 +176,26 @@
   let li = document.createElement("li");
   li.appendChild(a);
   return li;
 }
 
 function versionDropdownItem(sitemap, versionKey) {
   const {defaultPath, langPaths, markers, defaultLang} = sitemap[versionKey];
-  const {version, full_version} = markers[LANG] ?? markers[defaultLang];
+  const {version, full_version, minecraft_version} = markers[LANG] ?? markers[defaultLang];
 
   // link to the current language if available, else link to the default language
   let path;
   if (langPaths.hasOwnProperty(LANG)) {
     path = langPaths[LANG];
   } else {
     path = defaultPath;
   }
 
   const li = dropdownItem(version, BOOK_URL + path);
-  if (full_version === FULL_VERSION) {
+  if (full_version === FULL_VERSION && versionKey == VERSION && minecraft_version == MINECRAFT_VERSION) {
     li.classList.add("disabled");
   }
   return li;
 }
 
 function versionDropdownItems(sitemap, versions) {
   return versions.map((version) => (
@@ -270,30 +270,36 @@
     dropdownItems = [];
 
     for (const minecraftVersion of minecraftVersions) {
       const subSitemap = sitemap[minecraftVersion];
 
       const [branches, versions] = sortSitemapVersions(Object.keys(subSitemap));
 
-      // honestly, i shouldn't be allowed to write javascript
       dropdownItems.push(
         dropdownHeader(minecraftVersion),
         ...versionDropdownItems(subSitemap, versions),
-        ...(branches.length ? [dropdownSubmenu(
-          "latest/...",
-          versionDropdownItems(subSitemap, branches).map(item => {
-            item.firstChild.textContent = item.firstChild.textContent.replace(/^latest\//, "");
-            return item;
-          }),
-        )] : []),
-        dropdownSeparator(),
       );
-    }
 
-    dropdownItems.pop(); // remove trailing separator
+      // honestly, i shouldn't be allowed to write javascript
+      if (branches.length > 1) {
+        dropdownItems.push(
+          dropdownSubmenu(
+            "latest/...", // TODO: this really shouldn't be hardcoded
+            versionDropdownItems(subSitemap, branches).map(item => {
+              item.firstChild.textContent = item.firstChild.textContent.replace(/^latest\//, "");
+              return item;
+            }),
+          ),
+        );
+      } else if (branches.length == 1) {
+        dropdownItems.push(
+          versionDropdownItem(subSitemap, branches[0]),
+        );
+      }
+    }
 
     langNames = sitemap[MINECRAFT_VERSION][VERSION].langNames;
     langPaths = sitemap[MINECRAFT_VERSION][VERSION].langPaths;
 
   } else { // legacy sitemap, not using minecraft versions
     let [branches, versions] = sortSitemapVersions(Object.keys(sitemap));
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/redirect.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/redirect.html.jinja`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/components/navbar.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/components/navbar.html.jinja`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/components/table_of_contents.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/components/table_of_contents.html.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% import "macros/formatting.html.jinja" as fmt -%}
+{% import "macros/formatting.html.jinja" as fmt with context -%}
 
 {# put the link target outside of toc-container so jump to top still works in sidebar mode #}
 <div id="table-of-contents"></div>
 <nav class="toc-container">
   <h2 class="page-header">
     {{ _("hexdoc.toc.title") }}<a
       href="javascript:void(0)"
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-{% import "macros/formatting.html.jinja" as fmt -%} {# put the link target
-outside of toc-container so jump to top still works in sidebar mode #}
+{% import "macros/formatting.html.jinja" as fmt with context -%} {# put the
+link target outside of toc-container so jump to top still works in sidebar mode
+#}
 {{{{ __((""hheexxddoocc..ttoocc..ttiittllee"")) }}}}{{{{ ffmmtt..ppeerrmmaalliinnkk((""ttaabbllee--ooff--ccoonntteennttss"",, ""ttoocc--
 ppeerrmmaalliinnkk"")) }}}}
 {% for category in book.categories.values() if category.entries.values() %} {#
 category #} {{ fmt.maybe_spoilered_link(category) }} {# list of entries in the
 category #}
     * {% for entry in category.entries.values() %}
     * {{ fmt.maybe_spoilered_link(entry) }}
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/components/welcome.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/components/welcome.html.jinja`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/macros/formatting.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/macros/formatting.html.jinja`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% import "macros/styles.html.jinja" as styles with context -%}
+{% import "macros/styles.html.jinja" as html_styles with context -%}
 {% import "macros/textures.html.jinja" as texture_macros with context -%}
 
 {# jump to top icon in section headers #}
 {% macro jump_to_top() -%}
   <a
     href="#table-of-contents"
     class="permalink small"
@@ -42,21 +42,29 @@
     </div>
   {% else %}
     {{ caller() }}
   {% endif %}
 {%- endmacro %}
 
 {# FormatTree handler #}
-{% macro styled(value) -%}
+{% macro styled(value, separator="<br />", styles=html_styles) -%}
   {%- if value is string -%}
     {%- for line in value.splitlines() -%}
       {{- line -}}
-      {%- if not loop.last -%}<br />{%- endif -%}
+      {%- if not loop.last -%}{{ separator|safe }}{%- endif -%}
     {%- endfor -%}
   {%- elif value is not none -%}
     {%- call styles[value.style.macro](value.style) -%}
       {%- for child in value.children -%}
         {{- styled(child) -}}
       {%- endfor -%}
     {%- endcall -%}
   {%- endif -%}
 {%- endmacro %}
+
+{# dropdown(base_key: str) #}
+{% macro dropdown(base_key) -%}
+  <summary class="collapse-details">
+    <span class="collapse-recipe-show">{{ _(base_key~".show") }}</span>
+    <span class="collapse-recipe-hide">{{ _(base_key~".hide") }}</span>
+  </summary>
+{%- endmacro %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% import "macros/styles.html.jinja" as styles with context -%} {% import
+{% import "macros/styles.html.jinja" as html_styles with context -%} {% import
 "macros/textures.html.jinja" as texture_macros with context -%} {# jump to top
 icon in section headers #} {% macro jump_to_top() -%} {%- endmacro %} {# link
 icon in section headers to get a permalink to that section #} {% macro
 permalink(href, class_name="") -%} {%- endmacro %} {# header for categories and
 entries #} {% macro section_header(value, header_tag, class_name) -%} <{
 { header_tag }} class="{{ class_name }} page-header"> {
 { texture_macros.render_icon(value.icon) }} {{- value.name ~ jump_to_top() ~
@@ -10,12 +10,15 @@
 { header_tag }}> {%- endmacro %} {# link to value.id, with spoiler blur if
 value is a spoiler #} {% macro maybe_spoilered_link(value) -%} _{_{_-
 _t_e_x_t_u_r_e___m_a_c_r_o_s_._r_e_n_d_e_r___i_c_o_n_(_v_a_l_u_e_._i_c_o_n_)_ _}_}_ _{_{_ _v_a_l_u_e_._n_a_m_e_ _-_}_}_ {%- endmacro %} {#
 macro block which spoiler blurs its content if value is a spoiler #} {% macro
 maybe_spoilered(value) -%} {% if value.is_spoiler %}
 {{ caller() }}
 {% else %} {{ caller() }} {% endif %} {%- endmacro %} {# FormatTree handler #}
-{% macro styled(value) -%} {%- if value is string -%} {%- for line in
-value.splitlines() -%} {{- line -}} {%- if not loop.last -%}
-{%- endif -%} {%- endfor -%} {%- elif value is not none -%} {%- call styles
+{% macro styled(value, separator="
+", styles=html_styles) -%} {%- if value is string -%} {%- for line in
+value.splitlines() -%} {{- line -}} {%- if not loop.last -%}{{ separator|safe
+}}{%- endif -%} {%- endfor -%} {%- elif value is not none -%} {%- call styles
 [value.style.macro](value.style) -%} {%- for child in value.children -%} {{-
 styled(child) -}} {%- endfor -%} {%- endcall -%} {%- endif -%} {%- endmacro %}
+{# dropdown(base_key: str) #} {% macro dropdown(base_key) -%} {{ _
+(base_key~".show") }} {{ _(base_key~".hide") }} {%- endmacro %}
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/macros/recipes.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/macros/recipes.html.jinja`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% import "macros/textures.html.jinja" as texture_macros with context -%}
+{% import "macros/formatting.html.jinja" as fmt with context -%}
 
 {# show the names of all the recipe results in a list of recipes #}
 {% macro generic(recipes, result_attribute, description, separator) -%}
   <blockquote class="crafting-info">
     {{ description }} {{
       recipes
       |map(attribute="result."~result_attribute)
@@ -20,46 +21,7 @@
       {{ render_ingredients(ingredient.default, true) }}
       {{ render_ingredients(ingredient.if_loaded, true) }}
     {% else %}
       {{ texture_macros.render_item(ingredient.item, is_first=loop.first and not is_recursive) }}
     {% endif %}
   {% endfor %}
 {%- endmacro %}
-
-{# render a crafting table for each recipe #}
-{% macro crafting_table(recipes) -%}
-  <details class="details-collapsible crafting-table-details">
-    <summary class="collapse-details">
-      <span class="collapse-recipe-show">{{ _('hexdoc.recipe.show') }}</span>
-      <span class="collapse-recipe-hide">{{ _('hexdoc.recipe.hide') }}</span>
-    </summary>
-    <div class="crafting-tables">
-      {% for recipe in recipes %}
-        <div>
-          <h5>{{ recipe.result.item.name }}</h5>
-          <div class="crafting-table">
-            <img
-              alt="Crafting table"
-              src="{{ 'hexdoc:textures/gui/crafting_table.png'|hexdoc_texture }}"
-            >
-
-            <div class="crafting-table-grid">
-              {% for cell_ingredients in recipe.ingredients %}
-                {% if cell_ingredients is none %}
-                  <div></div> {#- empty slot / air #}
-                {% else %}
-                  <div class="texture item-texture multi-textures cycle-textures">
-                    {{ render_ingredients(cell_ingredients) }}
-                  </div>
-                {% endif %}
-              {% endfor %}
-            </div>
-
-            <div class="crafting-table-result">
-              {{ texture_macros.render_item(recipe.result.item, count=recipe.result.count) }}
-            </div>
-          </div>
-        </div>
-      {% endfor %}
-    </div>
-  </details>
-{%- endmacro %}
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/macros/styles.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/macros/styles.html.jinja`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/macros/textures.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/macros/textures.html.jinja`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   {% if item_or_texture.texture is defined %}
     {{- render_item(item_or_texture) -}}
   {% else %}
     {{- render_texture(name, item_or_texture) -}}
   {% endif %}
 {%- endmacro %}
 
-{% macro render_texture(name, texture, class_names=[], lazy=true) -%}
+{% macro render_texture(name, texture, class_names=[], lazy=true, title=true) -%}
   {% if texture.meta is defined -%}
     <div
       role="img"
-      title="{{ name }}"
+      {{ ('title="'~name~'"')|safe if title }}
       aria-label="{{ name }} (animated)"
       class="{{
         (class_names + [
           'texture',
           'animated-sync',
           texture.css_class,
           'pixelated' if texture.pixelated,
         ])|join(' ')
       }}"
     ></div>
   {%- else -%}
     <img
-      title="{{ name }}"
+      {{ ('title="'~name~'"')|safe if title }}
       alt="{{ name }}"
       src="{{ texture.url }}"
       {{ 'loading="lazy"'|safe if lazy }}
       class="{{
         (class_names + [
           'texture',
           'pixelated' if texture.pixelated,
@@ -67,10 +67,19 @@
       class_names=[
         "item-texture",
         "multi-texture-active" if is_first is true,
       ],
     ) }}
   {%- endif -%}
   {% if count > 1 -%}
-    <div class="badge">{{ count }}</div>
+    <div class="badge item-texture-count">{{ count }}</div>
   {%- endif %}
 {%- endmacro %}
+
+{% macro render_recipe_gui(recipe, class_names=[]) -%}
+  {{ render_texture(
+    name=recipe.gui_name,
+    texture=recipe.gui_texture,
+    class_names=class_names,
+    lazy=false,
+  ) }}
+{%- endmacro %}
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/_templates/pages/patchouli/text.html.jinja` & `hexdoc-1!0.1.0a9/src/hexdoc/_templates/pages/patchouli/text.html.jinja`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends "pages/patchouli/page.html.jinja" %}
 {% import "macros/formatting.html.jinja" as fmt with context %}
 
 {% block body %}
-  {% if page.title is not none %}
+  {% if page.title is defined and page.title is not none %}
     {# need title_attrs for LookupPatternPage -#}
     <h4{% block title_attrs %}{% endblock %}>
       {{- page.title -}}
       {# conditionally defined in Page #}
       {%- if page_anchor_id is defined %}
         {{- fmt.permalink(page_anchor_id) -}}
       {% endif -%}
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/cli/app.py` & `hexdoc-1!0.1.0a9/src/hexdoc/cli/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,28 +10,31 @@
 from textwrap import dedent
 from typing import Annotated, Any, Optional
 
 from packaging.version import Version
 from typer import Option, Typer
 from yarl import URL
 
-from hexdoc.core import ModResourceLoader
-from hexdoc.core.resource import ResourceLocation
+from hexdoc.core import ModResourceLoader, ResourceLocation
 from hexdoc.data.metadata import HexdocMetadata
+from hexdoc.data.sitemap import (
+    delete_updated_books,
+    dump_sitemap,
+    load_sitemap,
+)
+from hexdoc.jinja.render import create_jinja_env, get_templates, render_book
 from hexdoc.minecraft import I18n
 from hexdoc.minecraft.assets import (
     AnimatedTexture,
     PNGTexture,
+    TextureContext,
 )
-from hexdoc.minecraft.assets.textures import TextureContext
-from hexdoc.patchouli.book_context import BookContext
-from hexdoc.patchouli.text import FormattingContext
-from hexdoc.plugin.mod_plugin import ModPluginWithBook
-from hexdoc.utils import git_root, setup_logging, write_to_path
-from hexdoc.utils.context import ContextSource
+from hexdoc.patchouli import BookContext, FormattingContext
+from hexdoc.plugin import ModPluginWithBook
+from hexdoc.utils import ContextSource, git_root, setup_logging, write_to_path
 from hexdoc.utils.logging import repl_readfunc
 
 from . import ci, render_block
 from .utils.args import (
     DEFAULT_MERGE_DST,
     DEFAULT_MERGE_SRC,
     BranchOption,
@@ -41,20 +44,14 @@
     VerbosityOption,
 )
 from .utils.load import (
     init_context,
     load_common_data,
     render_textures_and_export_metadata,
 )
-from .utils.render import create_jinja_env, render_book
-from .utils.sitemap import (
-    delete_updated_books,
-    dump_sitemap,
-    load_sitemap,
-)
 
 logger = logging.getLogger(__name__)
 
 app = Typer(
     pretty_exceptions_enable=False,
     context_settings={
         "help_option_names": ["--help", "-h"],
@@ -225,34 +222,30 @@
                 f"ModPlugin registered for modid `{props.modid}` (from props.modid)"
                 f" does not inherit from ModPluginWithBook: {plugin}"
             )
 
         logger.info("Setting up Jinja template environment.")
         env = create_jinja_env(pm, props.template.include, props_file)
 
-        if props.template.override_default_render:
-            template_names = props.template.render
-        else:
-            template_names = pm.default_rendered_templates(props.template.include)
-
-        template_names |= props.template.extend_render
-
-        templates = {
-            Path(path): env.get_template(template_name)
-            for path, template_name in template_names.items()
-        }
-        if not templates:
-            raise RuntimeError(
-                "No templates to render, check your props.template configuration "
-                f"(in {props_file.as_posix()})"
-            )
-
         logger.info(f"Rendering book for {len(books)} language(s).")
         for book_info in books:
             try:
+                templates = get_templates(
+                    props=props,
+                    pm=pm,
+                    book=book_info.book,
+                    context=book_info.context,
+                    env=env,
+                )
+                if not templates:
+                    raise RuntimeError(
+                        "No templates to render, check your props.template configuration "
+                        f"(in {props_file.as_posix()})"
+                    )
+
                 book_ctx = BookContext.of(book_info.context)
                 formatting_ctx = FormattingContext.of(book_info.context)
                 texture_ctx = TextureContext.of(book_info.context)
 
                 site_book_path = plugin.site_book_path(
                     book_info.language,
                     versioned=release,
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/cli/ci.py` & `hexdoc-1!0.1.0a9/src/hexdoc/cli/ci.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/cli/render_block.py` & `hexdoc-1!0.1.0a9/src/hexdoc/cli/render_block.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/cli/utils/args.py` & `hexdoc-1!0.1.0a9/src/hexdoc/cli/utils/args.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/cli/utils/load.py` & `hexdoc-1!0.1.0a9/src/hexdoc/cli/utils/load.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/cli/utils/render.py` & `hexdoc-1!0.1.0a9/src/hexdoc/jinja/render.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pyright: reportUnknownMemberType=false, reportUnknownArgumentType=false
 # pyright: reportUnknownLambdaType=false, reportUnknownVariableType=false
 
 import logging
 import shutil
 from pathlib import Path
-from typing import Any, Sequence
+from typing import Any, Mapping, Sequence
 
 from _hexdoc_favicons import Favicons
 from jinja2 import (
     BaseLoader,
     ChoiceLoader,
     Environment,
     PrefixLoader,
@@ -16,26 +16,26 @@
     Template,
     TemplateNotFound,
 )
 from jinja2.sandbox import SandboxedEnvironment
 
 from hexdoc.core import MinecraftVersion, Properties, ResourceLocation
 from hexdoc.core.properties import JINJA_NAMESPACE_ALIASES
-from hexdoc.jinja import (
-    IncludeRawExtension,
+from hexdoc.data.sitemap import MARKER_NAME, LatestSitemapMarker, VersionedSitemapMarker
+from hexdoc.minecraft import I18n
+from hexdoc.plugin import ModPluginWithBook, PluginManager
+from hexdoc.utils import ContextSource, write_to_path
+
+from .extensions import IncludeRawExtension
+from .filters import (
     hexdoc_item,
     hexdoc_localize,
     hexdoc_texture,
     hexdoc_wrap,
 )
-from hexdoc.minecraft import I18n
-from hexdoc.plugin import ModPluginWithBook, PluginManager
-from hexdoc.utils import write_to_path
-
-from .sitemap import MARKER_NAME, LatestSitemapMarker, VersionedSitemapMarker
 
 logger = logging.getLogger(__name__)
 
 
 class HexdocTemplateLoader(BaseLoader):
     def __init__(
         self,
@@ -108,25 +108,52 @@
         "hexdoc_texture": hexdoc_texture,
         "hexdoc_item": hexdoc_item,
     }
 
     return env
 
 
+def get_templates(
+    *,
+    props: Properties,
+    pm: PluginManager,
+    book: Any,
+    context: ContextSource,
+    env: Environment,
+) -> dict[Path, tuple[Template, Mapping[str, Any]]]:
+    assert props.template is not None
+
+    if props.template.override_default_render:
+        template_names = {k: (v, {}) for k, v in props.template.render.items()}
+    else:
+        template_names = pm.default_rendered_templates(
+            modids=props.template.render_from,
+            book=book,
+            context=context,
+        )
+
+    template_names |= {k: (v, {}) for k, v in props.template.extend_render.items()}
+
+    return {
+        Path(path): (env.get_template(template_name), args)
+        for path, (template_name, args) in template_names.items()
+    }
+
+
 def render_book(
     *,
     props: Properties,
     pm: PluginManager,
     plugin: ModPluginWithBook,
     lang: str,
     book_id: ResourceLocation,
     i18n: I18n,
     macros: dict[str, str],
     env: Environment,
-    templates: dict[Path, Template],
+    templates: dict[Path, tuple[Template, Mapping[str, Any]]],
     output_dir: Path,
     site_path: Path,
     version: str,
     versioned: bool,
     template_args: dict[str, Any],
 ):
     if not props.template:
@@ -191,16 +218,16 @@
             macros=macros,
             pm=pm,
         ),
         **props.template.args,
     }
     pm.update_template_args(template_args)
 
-    for filename, template in templates.items():
-        file = template.render(template_args)
+    for filename, (template, extra_args) in templates.items():
+        file = template.render(template_args | dict(extra_args))
         stripped_file = strip_empty_lines(file)
         write_to_path(output_dir / filename, stripped_file)
 
     if props.template.static_dir:
         shutil.copytree(props.template.static_dir, output_dir, dirs_exist_ok=True)
 
     # redirect file for this book
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/cli/utils/sitemap.py` & `hexdoc-1!0.1.0a9/src/hexdoc/data/sitemap.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/core/__init__.py` & `hexdoc-1!0.1.0a9/src/hexdoc/core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = [
     "AssumeTag",
     "BaseProperties",
     "BaseResourceDir",
+    "BaseResourceLocation",
     "BookFolder",
     "Entity",
     "ExportFn",
     "IsVersion",
     "ItemStack",
     "METADATA_SUFFIX",
     "MinecraftVersion",
@@ -17,17 +18,17 @@
     "ResourceDir",
     "ResourceLocation",
     "ResourceType",
     "ValueIfVersion",
     "VersionSource",
     "Versioned",
     "compat",
+    "properties",
 ]
 
-from . import compat
 from .compat import (
     IsVersion,
     MinecraftVersion,
     ValueIfVersion,
     Versioned,
     VersionSource,
 )
@@ -36,14 +37,15 @@
     BookFolder,
     ExportFn,
     ModResourceLoader,
 )
 from .properties import BaseProperties, Properties
 from .resource import (
     AssumeTag,
+    BaseResourceLocation,
     Entity,
     ItemStack,
     ResLoc,
     ResourceLocation,
     ResourceType,
 )
 from .resource_dir import (
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/core/compat.py` & `hexdoc-1!0.1.0a9/src/hexdoc/core/compat.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/core/loader.py` & `hexdoc-1!0.1.0a9/src/hexdoc/core/loader.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/core/properties.py` & `hexdoc-1!0.1.0a9/src/hexdoc/core/properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Self, Sequence
 
-from pydantic import Field, PrivateAttr, field_validator
+from pydantic import Field, PrivateAttr, field_validator, model_validator
 from yarl import URL
 
 from hexdoc.model.base import HexdocSettings
 from hexdoc.model.strip_hidden import StripHiddenModel
 from hexdoc.utils import (
     TRACE,
     PydanticOrderedSet,
@@ -69,46 +69,59 @@
 
 
 class TemplateProps(StripHiddenModel, validate_assignment=True):
     static_dir: RelativePath | None = None
     icon: RelativePath | None = None
     include: PydanticOrderedSet[str]
 
+    render_from: PydanticOrderedSet[str] = Field(None, validate_default=False)
+    """List of modids to include default rendered templates from.
+
+    If not provided, defaults to `self.include`.
+    """
     render: dict[Path, str] = Field(default_factory=dict)
     extend_render: dict[Path, str] = Field(default_factory=dict)
 
     redirect: tuple[Path, str] | None = (Path("index.html"), "redirect.html.jinja")
     """filename, template"""
 
     args: dict[str, Any]
 
     _was_render_set: bool = PrivateAttr(False)
 
     @property
     def override_default_render(self):
         return self._was_render_set
 
-    @field_validator("include", mode="after")
+    @field_validator("include", "render_from", mode="after")
     @classmethod
-    def _resolve_aliases(cls, values: PydanticOrderedSet[str]):
-        for alias, replacement in JINJA_NAMESPACE_ALIASES.items():
-            if alias in values:
-                values.remove(alias)
-                values.add(replacement)
+    def _resolve_aliases(cls, values: PydanticOrderedSet[str] | None):
+        if values:
+            for alias, replacement in JINJA_NAMESPACE_ALIASES.items():
+                if alias in values:
+                    values.remove(alias)
+                    values.add(replacement)
         return values
 
+    @model_validator(mode="after")
+    def _set_default_render_from(self):
+        if self.render_from is None:  # pyright: ignore[reportUnnecessaryComparison]
+            self.render_from = self.include
+        return self
+
 
 # TODO: support item/block override
 class PNGTextureOverride(StripHiddenModel):
     url: PydanticURL
     pixelated: bool
 
 
 class TextureTextureOverride(StripHiddenModel):
     texture: ResourceLocation
+    """The id of an image texture (eg. `minecraft:textures/item/stick.png`)."""
 
 
 class TexturesProps(StripHiddenModel):
     enabled: bool = True
     """Set to False to disable texture rendering."""
     missing: set[ResourceLocation] = Field(default_factory=set)
     override: dict[
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/core/resource.py` & `hexdoc-1!0.1.0a9/src/hexdoc/core/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,17 +158,20 @@
         if isinstance(path, Path):
             path = path.as_posix()
         return self.__class__(self.namespace, path)
 
     def match(self, pattern: Self) -> bool:
         return fnmatch(str(self), str(pattern))
 
+    def template_path(self, type: str, folder: str = "") -> str:
+        return self.file_path_stub(type, folder, assume_json=False).as_posix()
+
     def file_path_stub(
         self,
-        type: ResourceType,
+        type: ResourceType | str,
         folder: str | Path = "",
         assume_json: bool = True,
     ) -> Path:
         """Returns the path to find this resource within a resource directory.
 
         If `assume_json` is True and no file extension is provided, `.json` is assumed.
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/core/resource_dir.py` & `hexdoc-1!0.1.0a9/src/hexdoc/core/resource_dir.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/data/metadata.py` & `hexdoc-1!0.1.0a9/src/hexdoc/data/metadata.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/jinja/extensions.py` & `hexdoc-1!0.1.0a9/src/hexdoc/jinja/extensions.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/jinja/filters.py` & `hexdoc-1!0.1.0a9/src/hexdoc/jinja/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from hexdoc.core import Properties, ResourceLocation
 from hexdoc.core.resource import ItemStack
 from hexdoc.minecraft import I18n
 from hexdoc.minecraft.assets import (
     ItemWithTexture,
     PNGTexture,
+    validate_texture,
 )
 from hexdoc.patchouli import FormatTree
 from hexdoc.plugin import PluginManager
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
@@ -80,16 +81,19 @@
     return formatted
 
 
 # TODO: support the full texture lookup
 @pass_context
 @make_jinja_exceptions_suck_a_bit_less
 def hexdoc_texture(context: Context, id: str | ResourceLocation) -> str:
-    id = ResourceLocation.model_validate(id)
-    texture = PNGTexture.load_id(id, context)
+    texture = validate_texture(
+        id,
+        context=context,
+        model_type=PNGTexture,
+    )
     return str(texture.url)
 
 
 @pass_context
 @make_jinja_exceptions_suck_a_bit_less
 def hexdoc_item(
     context: Context,
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/i18n.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/i18n.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/tags.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/tags.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/__init__.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "PNGTexture",
     "SingleItemTexture",
     "TagWithTexture",
     "Texture",
     "TextureContext",
     "TextureLookup",
     "TextureLookups",
+    "validate_texture",
 ]
 
 from .animated import (
     AnimatedTexture,
     AnimationMeta,
 )
 from .items import (
@@ -28,14 +29,15 @@
     MultiItemTexture,
     SingleItemTexture,
 )
 from .load_assets import (
     HexdocAssetLoader,
     HexdocPythonResourceLoader,
     Texture,
+    validate_texture,
 )
 from .models import ModelItem
 from .textures import (
     PNGTexture,
     TextureContext,
     TextureLookup,
     TextureLookups,
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/animated.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/animated.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/constants.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/constants.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/items.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/items.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/load_assets.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/load_assets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import base64
 import logging
 from collections.abc import Set
 from dataclasses import dataclass
 from functools import cached_property
 from pathlib import Path
-from typing import Iterable, Iterator
+from typing import Any, Iterable, Iterator, TypeVar, cast
 
 from minecraft_render import ResourcePath, js
 from minecraft_render.types.dataset.RenderClass import IRenderClass
 from minecraft_render.types.dataset.types import IResourceLoader
+from pydantic import TypeAdapter
 from yarl import URL
 
 from hexdoc.core import ModResourceLoader, ResourceLocation
 from hexdoc.core.properties import (
     PNGTextureOverride,
     TextureTextureOverride,
 )
 from hexdoc.model import HexdocModel
 from hexdoc.utils import PydanticURL
+from hexdoc.utils.context import ContextSource
 
 from ..tags import Tag
 from .animated import AnimatedTexture, AnimationMeta
 from .items import (
     ImageTexture,
     ItemTexture,
     MultiItemTexture,
@@ -33,14 +35,29 @@
     PNGTexture,
 )
 
 logger = logging.getLogger(__name__)
 
 Texture = ImageTexture | ItemTexture
 
+_T_Texture = TypeVar("_T_Texture", bound=Texture)
+
+
+def validate_texture(
+    value: Any,
+    *,
+    context: ContextSource,
+    model_type: type[_T_Texture] = Texture,
+) -> _T_Texture:
+    ta = TypeAdapter(model_type)
+    return ta.validate_python(
+        value,
+        context=cast(dict[str, Any], context),  # lie
+    )
+
 
 class TextureNotFoundError(FileNotFoundError):
     def __init__(self, id_type: str, id: ResourceLocation):
         self.message = f"No texture found for {id_type} id: {id}"
         super().__init__(self.message)
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/models.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/models.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/textures.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/textures.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/assets/with_texture.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/assets/with_texture.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/recipe/__init__.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/recipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/minecraft/recipe/ingredients.py` & `hexdoc-1!0.1.0a9/src/hexdoc/minecraft/recipe/ingredients.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,40 @@
+from abc import ABC
 from typing import Annotated, Any, Iterator
 
 from pydantic import (
     AfterValidator,
     BeforeValidator,
+    Field,
     ValidationError,
     ValidationInfo,
 )
 
 from hexdoc.core import ResourceLocation
 from hexdoc.core.loader import ModResourceLoader
 from hexdoc.core.resource import AssumeTag
 from hexdoc.model import HexdocModel, NoValue, TypeTaggedUnion
 from hexdoc.utils import listify
 
 from ..assets import ItemWithTexture, TagWithTexture
 from ..tags import Tag
 
 
-class ItemIngredient(TypeTaggedUnion):
-    pass
+class ItemIngredient(TypeTaggedUnion, ABC):
+    @property
+    def item(self) -> ItemWithTexture | TagWithTexture:
+        ...
 
 
 class MinecraftItemIdIngredient(ItemIngredient, type=NoValue):
-    item: ItemWithTexture
+    item_: ItemWithTexture = Field(alias="item")
+
+    @property
+    def item(self):
+        return self.item_
 
 
 class MinecraftItemTagIngredient(ItemIngredient, type=NoValue):
     tag: AssumeTag[TagWithTexture]
 
     @property
     def item(self):
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/model/__init__.py` & `hexdoc-1!0.1.0a9/src/hexdoc/model/__init__.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/model/base.py` & `hexdoc-1!0.1.0a9/src/hexdoc/model/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     """Base class for all Pydantic models in hexdoc.
 
     Sets the default model config, and overrides __init__ to allow using the
     `init_context` context manager to set validation context for constructors.
     """
 
     model_config = DEFAULT_CONFIG
+    """@private"""
 
     __hexdoc_before_validator__: ClassVar[ModelBeforeValidator | None] = None
 
     def __init__(__pydantic_self__, **data: Any) -> None:  # type: ignore
         __tracebackhide__ = True
         __pydantic_self__.__pydantic_validator__.validate_python(
             data,
@@ -74,15 +75,19 @@
         return cls.model_validate(defaults or {})
 
 
 _T = TypeVar("_T")
 
 
 class HexdocTypeAdapter(TypeAdapter[_T]):
-    def __init__(self, type: _T, *, config: ConfigDict | None = None):
-        if config is None and not isinstance(type, BaseModel):
-            config = DEFAULT_CONFIG
+    """Subclass of `pydantic.TypeAdapter` that sets `config` to the default hexdoc
+    model config.
+
+    Do not use this with Pydantic models, as it won't work.
+    """
+
+    def __init__(self, type: _T, *, config: ConfigDict = DEFAULT_CONFIG):
         return super().__init__(type, config=config)
 
 
 class ValidationContextModel(HexdocModel, ValidationContext):
     pass
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/model/id.py` & `hexdoc-1!0.1.0a9/src/hexdoc/model/id.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/model/inline.py` & `hexdoc-1!0.1.0a9/src/hexdoc/model/inline.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/model/strip_hidden.py` & `hexdoc-1!0.1.0a9/src/hexdoc/model/strip_hidden.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/model/tagged_union.py` & `hexdoc-1!0.1.0a9/src/hexdoc/model/tagged_union.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/model/types.py` & `hexdoc-1!0.1.0a9/src/hexdoc/model/types.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/patchouli/book.py` & `hexdoc-1!0.1.0a9/src/hexdoc/patchouli/book.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/patchouli/book_context.py` & `hexdoc-1!0.1.0a9/src/hexdoc/patchouli/book_context.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/patchouli/category.py` & `hexdoc-1!0.1.0a9/src/hexdoc/patchouli/category.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/patchouli/entry.py` & `hexdoc-1!0.1.0a9/src/hexdoc/patchouli/entry.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/patchouli/text.py` & `hexdoc-1!0.1.0a9/src/hexdoc/patchouli/text.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/patchouli/page/__init__.py` & `hexdoc-1!0.1.0a9/src/hexdoc/patchouli/page/__init__.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/patchouli/page/abstract_pages.py` & `hexdoc-1!0.1.0a9/src/hexdoc/patchouli/page/abstract_pages.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,22 +38,30 @@
     def type(cls) -> ResourceLocation | None:
         assert cls._type is not NoValue
         return cls._type
 
     @model_validator(mode="wrap")
     @classmethod
     def _pre_root(cls, value: str | Any, handler: ModelWrapValidatorHandler[Self]):
-        if isinstance(value, str):
-            return handler({"type": "patchouli:text", "text": value})
+        match value:
+            case str(text):
+                # treat a plain string as a text page
+                value = {"type": "patchouli:text", "text": text}
+            case {"type": str(raw_type)} if ":" not in raw_type:
+                # default to the patchouli namespace if not specified
+                # see: https://github.com/VazkiiMods/Patchouli/blob/b87e91a5a08d/Xplat/src/main/java/vazkii/patchouli/client/book/ClientBookRegistry.java#L110
+                value["type"] = f"patchouli:{raw_type}"
+            case _:
+                pass
         return handler(value)
 
     @classproperty
     @classmethod
     def template(cls) -> str:
-        return f"pages/{cls.template_id.namespace}/{cls.template_id.path}"
+        return cls.template_id.template_path("pages")
 
 
 class PageWithText(Page, type=None):
     """Base class for a `Page` with optional text.
 
     If text is required, do not subclass this type.
     """
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/plugin/__init__.py` & `hexdoc-1!0.1.0a9/src/hexdoc/plugin/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __all__ = [
     "BookPlugin",
     "BookPluginImpl",
+    "DefaultRenderedTemplates",
     "HEXDOC_PROJECT_NAME",
     "HookReturn",
     "LoadTaggedUnionsImpl",
     "ModPlugin",
     "ModPluginImpl",
     "ModPluginImplWithProps",
     "ModPluginWithBook",
@@ -21,14 +22,15 @@
 
 from .book_plugin import BookPlugin
 from .manager import (
     PluginManager,
     PluginNotFoundError,
 )
 from .mod_plugin import (
+    DefaultRenderedTemplates,
     ModPlugin,
     ModPluginWithBook,
     VersionedModPlugin,
 )
 from .specs import (
     HEXDOC_PROJECT_NAME,
     BookPluginImpl,
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/plugin/book_plugin.py` & `hexdoc-1!0.1.0a9/src/hexdoc/plugin/book_plugin.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/plugin/manager.py` & `hexdoc-1!0.1.0a9/src/hexdoc/plugin/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,35 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Generic,
     Iterable,
     Iterator,
     Literal,
+    Mapping,
     Never,
     ParamSpec,
     Sequence,
     TypeVar,
     overload,
 )
 
 import pluggy
 from jinja2 import BaseLoader, ChoiceLoader, PackageLoader
 from jinja2.sandbox import SandboxedEnvironment
 
-from hexdoc.utils import ValidationContext
+from hexdoc.utils import ContextSource, ValidationContext
 
 if TYPE_CHECKING:
     from hexdoc.core import Properties, ResourceLocation
     from hexdoc.minecraft import I18n
     from hexdoc.patchouli import FormatTree
 
 from .book_plugin import BookPlugin
-from .mod_plugin import ModPlugin, ModPluginWithBook
+from .mod_plugin import DefaultRenderedTemplates, ModPlugin, ModPluginWithBook
 from .specs import HEXDOC_PROJECT_NAME, PluginSpec
 from .types import HookReturns
 
 _T = TypeVar("_T")
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R", covariant=True)
@@ -256,20 +257,36 @@
                     )
                     for package, package_path in flatten([result])
                 ]
             )
 
         return loaders
 
-    def default_rendered_templates(self, modids: Iterable[str]) -> dict[Path, str]:
-        templates = dict[str | Path, str]()
+    def default_rendered_templates(
+        self,
+        modids: Iterable[str],
+        book: Any,
+        context: ContextSource,
+    ):
+        templates: DefaultRenderedTemplates = {}
         for modid in modids:
             plugin = self.mod_plugin(modid)
             templates |= plugin.default_rendered_templates()
-        return {Path(path): template for path, template in templates.items()}
+            templates |= plugin.default_rendered_templates_v2(book, context)
+
+        result = dict[Path, tuple[str, Mapping[str, Any]]]()
+        for path, value in templates.items():
+            match value:
+                case str(template):
+                    args = dict[str, Any]()
+                case (template, args):
+                    pass
+            result[Path(path)] = (template, args)
+
+        return result
 
     def _import_from_hook(
         self,
         __spec: Callable[_P, HookReturns[Package]],
         *args: _P.args,
         **kwargs: _P.kwargs,
     ) -> Iterator[ModuleType]:
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/plugin/mod_plugin.py` & `hexdoc-1!0.1.0a9/src/hexdoc/plugin/mod_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from importlib.resources import Package
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Mapping
 
 from jinja2.sandbox import SandboxedEnvironment
 from typing_extensions import override
 from yarl import URL
 
+from hexdoc.utils import ContextSource
+
 from .types import HookReturn
 
 if TYPE_CHECKING:
     from hexdoc.core import ModResourceLoader, Properties
     from hexdoc.minecraft.assets import HexdocAssetLoader
 
+DefaultRenderedTemplates = Mapping[
+    str | Path,
+    str | tuple[str, Mapping[str, Any]],
+]
+
 
 @dataclass(kw_only=True)
 class ModPlugin(ABC):
     """Hexdoc plugin hooks that are tied to a specific Minecraft mod.
 
     If you want to render a web book, subclass `ModPluginWithBook` instead.
 
@@ -99,24 +106,37 @@
         """The module that contains the folder with your plugin's Jinja templates, and
         the name of that folder.
 
         For example: `your_plugin, "_templates"`
         """
         return None
 
-    def default_rendered_templates(self) -> dict[str | Path, str]:
+    def default_rendered_templates(self) -> DefaultRenderedTemplates:
         """Extra templates to be rendered by default when your plugin is active.
 
         The key is the output path, and the value is the template to import and render.
+        It may also be a tuple where the first item is the template and the second is
+        a dict to be merged with the arguments for that template.
 
         This hook is not called if `props.template.render` is set, since that option
         overrides all default templates.
         """
         return {}
 
+    def default_rendered_templates_v2(
+        self,
+        book: Any,
+        context: ContextSource,
+    ) -> DefaultRenderedTemplates:
+        """Like `default_rendered_templates`, but gets access to the book and context.
+
+        This is useful for dynamically generating multi-file output structures.
+        """
+        return {}
+
     def update_jinja_env(self, env: SandboxedEnvironment) -> None:
         """Modify the Jinja environment/configuration.
 
         This is called after hexdoc is done setting up the Jinja environment but before
         rendering the book.
         """
```

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/plugin/specs.py` & `hexdoc-1!0.1.0a9/src/hexdoc/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/__init__.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/classproperties.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/classproperties.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/context.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/context.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/iterators.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/logging.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/path.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/path.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/singletons.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/singletons.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/types.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/types.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/deserialize/assertions.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/deserialize/assertions.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/deserialize/json.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/deserialize/json.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc/utils/deserialize/toml.py` & `hexdoc-1!0.1.0a9/src/hexdoc/utils/deserialize/toml.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/_hooks.py` & `hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/_hooks.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/book.py` & `hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/book.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/category.py` & `hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/category.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/entry.py` & `hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/entry.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/src/hexdoc_modonomicon/page/abstract_pages.py` & `hexdoc-1!0.1.0a9/src/hexdoc_modonomicon/page/abstract_pages.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/LICENSE` & `hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/LICENSE`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_constants.py` & `hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_constants.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_exceptions.py` & `hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_exceptions.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_generate.py` & `hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_generate.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_util.py` & `hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_util.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_types/color.py` & `hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_types/color.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/vendor/_hexdoc_favicons/_types/properties.py` & `hexdoc-1!0.1.0a9/vendor/_hexdoc_favicons/_types/properties.py`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/.gitignore` & `hexdoc-1!0.1.0a9/.gitignore`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/LICENSE` & `hexdoc-1!0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `hexdoc-1!0.1.0a8/README.md` & `hexdoc-1!0.1.0a9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 
 # hexdoc
 
 A [Jinja](https://jinja.palletsprojects.com/en/3.1.x/)-based documentation generator for [Patchouli](https://github.com/VazkiiMods/Patchouli) books.
 
 This is the library that powers [Hex Casting](https://github.com/gamma-delta/HexMod)'s web book.
 
+## IMPORTANT: Version incompatibilities
+
+There are issues related to installing hexdoc with the following dependency versions:
+* Python 3.12+ on Windows: https://github.com/aio-libs/multidict/issues/887
+* Node.js 20+: https://github.com/stackgl/headless-gl/issues/268
+
+hexdoc is known to work with Python 3.11 and Node.js 18.
+
 ## Plugins
 
 See [hexdoc-hexcasting-template](https://github.com/hexdoc-dev/hexdoc-hexcasting-template) for instructions to set up a hexdoc plugin for a pre-existing Hex Casting addon.
 
 ## Contributing
 
 ### Setup
```

#### html2text {}

```diff
@@ -1,37 +1,42 @@
                                  [hexdoc logo]
 
    _[_D_o_c_s_ _-_ _h_e_x_d_o_c_._h_e_x_x_y_._m_e_d_i_a_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_][PyPI - Python Version]_[_G_i_t_H_u_b
                      _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]_[_h_e_x_d_o_c_]
 # hexdoc A [Jinja](https://jinja.palletsprojects.com/en/3.1.x/)-based
 documentation generator for [Patchouli](https://github.com/VazkiiMods/
 Patchouli) books. This is the library that powers [Hex Casting](https://
-github.com/gamma-delta/HexMod)'s web book. ## Plugins See [hexdoc-hexcasting-
-template](https://github.com/hexdoc-dev/hexdoc-hexcasting-template) for
-instructions to set up a hexdoc plugin for a pre-existing Hex Casting addon. ##
-Contributing ### Setup ```sh git submodule update --init python3.11 -m venv
-venv .\venv\Scripts\activate # Windows . venv/bin/activate.fish # fish source
-venv/bin/activate # everything else pip install -e .[dev] pre-commit install
-``` ### Usage For local testing, create a file called `.env` in the repo root
-following this template: ```sh GITHUB_SHA=main GITHUB_REPOSITORY=hexdoc-dev/
-hexdoc GITHUB_PAGES_URL=https://hexdoc.hexxy.media ``` Useful commands: ```sh #
-show help hexdoc -h # serve hexdoc resources locally # this is useful if
-serving other books locally that depend on hexdoc resources nodemon --exec
-"hexdoc serve --port 8001 --no-merge" # render and serve the Hex Casting web
-book in watch mode nodemon # start the Python interpreter with some extra local
-variables hexdoc repl # run tests pytest # fast, skips Cookiecutter nox # slow,
-full test suite in an isolated venv nox --no-install # after the first Nox run,
-use this to skip reinstalling everything # update test snapshots (only running
-sessions with the tag "test") nox -t test -- --snapshot-update # run hexdoc
-commands in an isolated environment to ensure it works on its own nox -s hexdoc
--- build nox -s hexdoc -- repl # set up a dummy book for local testing nox -
-s dummy_setup nox -s dummy_serve nox -s dummy_hexdoc -- build nox -
-s dummy_clean ``` ## Badges _[_h_e_x_d_o_c_]_[_p_o_w_e_r_e_d_ _b_y_ _h_e_x_d_o_c_]### Markdown ```md [!
-[hexdoc](https://img.shields.io/endpoint?url=https://hexxy.media/api/v0/badge/
-hexdoc)](https://github.com/hexdoc-dev/hexdoc) [![powered by hexdoc](https://
-img.shields.io/endpoint?url=https://hexxy.media/api/v0/badge/hexdoc?label=1)]
-(https://github.com/hexdoc-dev/hexdoc) ``` ### HTML ```html _[_h_e_x_d_o_c_]_[_p_o_w_e_r_e_d_ _b_y
-_h_e_x_d_o_c_]``` ### reStructuredText ```rst .. image:: https://img.shields.io/
-endpoint?url=https://hexxy.media/api/v0/badge/hexdoc :target: https://
-github.com/hexdoc-dev/hexdoc :alt: hexdoc .. image:: https://img.shields.io/
-endpoint?url=https://hexxy.media/api/v0/badge/hexdoc?label=1 :target: https://
-github.com/hexdoc-dev/hexdoc :alt: powered by hexdoc ```
+github.com/gamma-delta/HexMod)'s web book. ## IMPORTANT: Version
+incompatibilities There are issues related to installing hexdoc with the
+following dependency versions: * Python 3.12+ on Windows: https://github.com/
+aio-libs/multidict/issues/887 * Node.js 20+: https://github.com/stackgl/
+headless-gl/issues/268 hexdoc is known to work with Python 3.11 and Node.js 18.
+## Plugins See [hexdoc-hexcasting-template](https://github.com/hexdoc-dev/
+hexdoc-hexcasting-template) for instructions to set up a hexdoc plugin for a
+pre-existing Hex Casting addon. ## Contributing ### Setup ```sh git submodule
+update --init python3.11 -m venv venv .\venv\Scripts\activate # Windows . venv/
+bin/activate.fish # fish source venv/bin/activate # everything else pip install
+-e .[dev] pre-commit install ``` ### Usage For local testing, create a file
+called `.env` in the repo root following this template: ```sh GITHUB_SHA=main
+GITHUB_REPOSITORY=hexdoc-dev/hexdoc GITHUB_PAGES_URL=https://hexdoc.hexxy.media
+``` Useful commands: ```sh # show help hexdoc -h # serve hexdoc resources
+locally # this is useful if serving other books locally that depend on hexdoc
+resources nodemon --exec "hexdoc serve --port 8001 --no-merge" # render and
+serve the Hex Casting web book in watch mode nodemon # start the Python
+interpreter with some extra local variables hexdoc repl # run tests pytest #
+fast, skips Cookiecutter nox # slow, full test suite in an isolated venv nox --
+no-install # after the first Nox run, use this to skip reinstalling everything
+# update test snapshots (only running sessions with the tag "test") nox -t test
+-- --snapshot-update # run hexdoc commands in an isolated environment to ensure
+it works on its own nox -s hexdoc -- build nox -s hexdoc -- repl # set up a
+dummy book for local testing nox -s dummy_setup nox -s dummy_serve nox -
+s dummy_hexdoc -- build nox -s dummy_clean ``` ## Badges _[_h_e_x_d_o_c_]_[_p_o_w_e_r_e_d_ _b_y
+_h_e_x_d_o_c_]### Markdown ```md [![hexdoc](https://img.shields.io/endpoint?url=https:
+//hexxy.media/api/v0/badge/hexdoc)](https://github.com/hexdoc-dev/hexdoc) [!
+[powered by hexdoc](https://img.shields.io/endpoint?url=https://hexxy.media/
+api/v0/badge/hexdoc?label=1)](https://github.com/hexdoc-dev/hexdoc) ``` ###
+HTML ```html _[_h_e_x_d_o_c_]_[_p_o_w_e_r_e_d_ _b_y_ _h_e_x_d_o_c_]``` ### reStructuredText ```rst ..
+image:: https://img.shields.io/endpoint?url=https://hexxy.media/api/v0/badge/
+hexdoc :target: https://github.com/hexdoc-dev/hexdoc :alt: hexdoc .. image::
+https://img.shields.io/endpoint?url=https://hexxy.media/api/v0/badge/
+hexdoc?label=1 :target: https://github.com/hexdoc-dev/hexdoc :alt: powered by
+hexdoc ```
```

### Comparing `hexdoc-1!0.1.0a8/pyproject.toml` & `hexdoc-1!0.1.0a9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 ]
 
 [project.optional-dependencies]
 pdoc = [
     "pdoc~=14.1",
 ]
 test = [
-    "pyright~=1.1.338",
+    "pyright~=1.1.343,!=1.1.344",
     "pytest~=7.4",
     "pytest-dependency~=0.5",
     "syrupy~=4.6",
     "copier_template_tester",
 ]
 dev = [
     "hexdoc[pdoc,test]",
```

### Comparing `hexdoc-1!0.1.0a8/PKG-INFO` & `hexdoc-1!0.1.0a9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexdoc
-Version: 1!0.1.0a8
+Version: 1!0.1.0a9
 Summary: Python web book docgen for Patchouli and Hex Casting.
 Project-URL: Homepage, https://book.hexxy.media
 Project-URL: Documentation, https://hexdoc.hexxy.media
 Project-URL: Source, https://github.com/hexdoc-dev/hexdoc
 Author: object-Object, Alwinfy
 License: MIT License
         
@@ -69,15 +69,15 @@
 Requires-Dist: nox; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: ruff==0.1.4; extra == 'dev'
 Provides-Extra: pdoc
 Requires-Dist: pdoc~=14.1; extra == 'pdoc'
 Provides-Extra: test
 Requires-Dist: copier-template-tester; extra == 'test'
-Requires-Dist: pyright~=1.1.338; extra == 'test'
+Requires-Dist: pyright!=1.1.344,~=1.1.343; extra == 'test'
 Requires-Dist: pytest-dependency~=0.5; extra == 'test'
 Requires-Dist: pytest~=7.4; extra == 'test'
 Requires-Dist: syrupy~=4.6; extra == 'test'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img alt="hexdoc logo" src="https://github.com/hexdoc-dev/hexdoc/raw/main/media/hexdoc.svg" height="200" />
@@ -91,14 +91,22 @@
 
 # hexdoc
 
 A [Jinja](https://jinja.palletsprojects.com/en/3.1.x/)-based documentation generator for [Patchouli](https://github.com/VazkiiMods/Patchouli) books.
 
 This is the library that powers [Hex Casting](https://github.com/gamma-delta/HexMod)'s web book.
 
+## IMPORTANT: Version incompatibilities
+
+There are issues related to installing hexdoc with the following dependency versions:
+* Python 3.12+ on Windows: https://github.com/aio-libs/multidict/issues/887
+* Node.js 20+: https://github.com/stackgl/headless-gl/issues/268
+
+hexdoc is known to work with Python 3.11 and Node.js 18.
+
 ## Plugins
 
 See [hexdoc-hexcasting-template](https://github.com/hexdoc-dev/hexdoc-hexcasting-template) for instructions to set up a hexdoc plugin for a pre-existing Hex Casting addon.
 
 ## Contributing
 
 ### Setup
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hexdoc Version: 1!0.1.0a8 Summary: Python web book
+Metadata-Version: 2.1 Name: hexdoc Version: 1!0.1.0a9 Summary: Python web book
 docgen for Patchouli and Hex Casting. Project-URL: Homepage, https://
 book.hexxy.media Project-URL: Documentation, https://hexdoc.hexxy.media
 Project-URL: Source, https://github.com/hexdoc-dev/hexdoc Author: object-
 Object, Alwinfy License: MIT License Copyright (c) 2023 object-Object
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -35,47 +35,53 @@
 Requires-Dist: requests~=2.31 Requires-Dist: rich~=13.3.4 Requires-Dist:
 svglib~=1.5.1 Requires-Dist: typer[all]~=0.9 Requires-Dist: typing-
 extensions~=4.6 Requires-Dist: yarl~=1.9 Provides-Extra: dev Requires-Dist:
 hexdoc[pdoc,test]; extra == 'dev' Requires-Dist: nox; extra == 'dev' Requires-
 Dist: pre-commit; extra == 'dev' Requires-Dist: ruff==0.1.4; extra == 'dev'
 Provides-Extra: pdoc Requires-Dist: pdoc~=14.1; extra == 'pdoc' Provides-Extra:
 test Requires-Dist: copier-template-tester; extra == 'test' Requires-Dist:
-pyright~=1.1.338; extra == 'test' Requires-Dist: pytest-dependency~=0.5; extra
-== 'test' Requires-Dist: pytest~=7.4; extra == 'test' Requires-Dist:
-syrupy~=4.6; extra == 'test' Description-Content-Type: text/markdown
+pyright!=1.1.344,~=1.1.343; extra == 'test' Requires-Dist: pytest-
+dependency~=0.5; extra == 'test' Requires-Dist: pytest~=7.4; extra == 'test'
+Requires-Dist: syrupy~=4.6; extra == 'test' Description-Content-Type: text/
+markdown
                                  [hexdoc logo]
 
    _[_D_o_c_s_ _-_ _h_e_x_d_o_c_._h_e_x_x_y_._m_e_d_i_a_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_][PyPI - Python Version]_[_G_i_t_H_u_b
                      _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]_[_h_e_x_d_o_c_]
 # hexdoc A [Jinja](https://jinja.palletsprojects.com/en/3.1.x/)-based
 documentation generator for [Patchouli](https://github.com/VazkiiMods/
 Patchouli) books. This is the library that powers [Hex Casting](https://
-github.com/gamma-delta/HexMod)'s web book. ## Plugins See [hexdoc-hexcasting-
-template](https://github.com/hexdoc-dev/hexdoc-hexcasting-template) for
-instructions to set up a hexdoc plugin for a pre-existing Hex Casting addon. ##
-Contributing ### Setup ```sh git submodule update --init python3.11 -m venv
-venv .\venv\Scripts\activate # Windows . venv/bin/activate.fish # fish source
-venv/bin/activate # everything else pip install -e .[dev] pre-commit install
-``` ### Usage For local testing, create a file called `.env` in the repo root
-following this template: ```sh GITHUB_SHA=main GITHUB_REPOSITORY=hexdoc-dev/
-hexdoc GITHUB_PAGES_URL=https://hexdoc.hexxy.media ``` Useful commands: ```sh #
-show help hexdoc -h # serve hexdoc resources locally # this is useful if
-serving other books locally that depend on hexdoc resources nodemon --exec
-"hexdoc serve --port 8001 --no-merge" # render and serve the Hex Casting web
-book in watch mode nodemon # start the Python interpreter with some extra local
-variables hexdoc repl # run tests pytest # fast, skips Cookiecutter nox # slow,
-full test suite in an isolated venv nox --no-install # after the first Nox run,
-use this to skip reinstalling everything # update test snapshots (only running
-sessions with the tag "test") nox -t test -- --snapshot-update # run hexdoc
-commands in an isolated environment to ensure it works on its own nox -s hexdoc
--- build nox -s hexdoc -- repl # set up a dummy book for local testing nox -
-s dummy_setup nox -s dummy_serve nox -s dummy_hexdoc -- build nox -
-s dummy_clean ``` ## Badges _[_h_e_x_d_o_c_]_[_p_o_w_e_r_e_d_ _b_y_ _h_e_x_d_o_c_]### Markdown ```md [!
-[hexdoc](https://img.shields.io/endpoint?url=https://hexxy.media/api/v0/badge/
-hexdoc)](https://github.com/hexdoc-dev/hexdoc) [![powered by hexdoc](https://
-img.shields.io/endpoint?url=https://hexxy.media/api/v0/badge/hexdoc?label=1)]
-(https://github.com/hexdoc-dev/hexdoc) ``` ### HTML ```html _[_h_e_x_d_o_c_]_[_p_o_w_e_r_e_d_ _b_y
-_h_e_x_d_o_c_]``` ### reStructuredText ```rst .. image:: https://img.shields.io/
-endpoint?url=https://hexxy.media/api/v0/badge/hexdoc :target: https://
-github.com/hexdoc-dev/hexdoc :alt: hexdoc .. image:: https://img.shields.io/
-endpoint?url=https://hexxy.media/api/v0/badge/hexdoc?label=1 :target: https://
-github.com/hexdoc-dev/hexdoc :alt: powered by hexdoc ```
+github.com/gamma-delta/HexMod)'s web book. ## IMPORTANT: Version
+incompatibilities There are issues related to installing hexdoc with the
+following dependency versions: * Python 3.12+ on Windows: https://github.com/
+aio-libs/multidict/issues/887 * Node.js 20+: https://github.com/stackgl/
+headless-gl/issues/268 hexdoc is known to work with Python 3.11 and Node.js 18.
+## Plugins See [hexdoc-hexcasting-template](https://github.com/hexdoc-dev/
+hexdoc-hexcasting-template) for instructions to set up a hexdoc plugin for a
+pre-existing Hex Casting addon. ## Contributing ### Setup ```sh git submodule
+update --init python3.11 -m venv venv .\venv\Scripts\activate # Windows . venv/
+bin/activate.fish # fish source venv/bin/activate # everything else pip install
+-e .[dev] pre-commit install ``` ### Usage For local testing, create a file
+called `.env` in the repo root following this template: ```sh GITHUB_SHA=main
+GITHUB_REPOSITORY=hexdoc-dev/hexdoc GITHUB_PAGES_URL=https://hexdoc.hexxy.media
+``` Useful commands: ```sh # show help hexdoc -h # serve hexdoc resources
+locally # this is useful if serving other books locally that depend on hexdoc
+resources nodemon --exec "hexdoc serve --port 8001 --no-merge" # render and
+serve the Hex Casting web book in watch mode nodemon # start the Python
+interpreter with some extra local variables hexdoc repl # run tests pytest #
+fast, skips Cookiecutter nox # slow, full test suite in an isolated venv nox --
+no-install # after the first Nox run, use this to skip reinstalling everything
+# update test snapshots (only running sessions with the tag "test") nox -t test
+-- --snapshot-update # run hexdoc commands in an isolated environment to ensure
+it works on its own nox -s hexdoc -- build nox -s hexdoc -- repl # set up a
+dummy book for local testing nox -s dummy_setup nox -s dummy_serve nox -
+s dummy_hexdoc -- build nox -s dummy_clean ``` ## Badges _[_h_e_x_d_o_c_]_[_p_o_w_e_r_e_d_ _b_y
+_h_e_x_d_o_c_]### Markdown ```md [![hexdoc](https://img.shields.io/endpoint?url=https:
+//hexxy.media/api/v0/badge/hexdoc)](https://github.com/hexdoc-dev/hexdoc) [!
+[powered by hexdoc](https://img.shields.io/endpoint?url=https://hexxy.media/
+api/v0/badge/hexdoc?label=1)](https://github.com/hexdoc-dev/hexdoc) ``` ###
+HTML ```html _[_h_e_x_d_o_c_]_[_p_o_w_e_r_e_d_ _b_y_ _h_e_x_d_o_c_]``` ### reStructuredText ```rst ..
+image:: https://img.shields.io/endpoint?url=https://hexxy.media/api/v0/badge/
+hexdoc :target: https://github.com/hexdoc-dev/hexdoc :alt: hexdoc .. image::
+https://img.shields.io/endpoint?url=https://hexxy.media/api/v0/badge/
+hexdoc?label=1 :target: https://github.com/hexdoc-dev/hexdoc :alt: powered by
+hexdoc ```
```

