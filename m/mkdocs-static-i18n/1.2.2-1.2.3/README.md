# Comparing `tmp/mkdocs_static_i18n-1.2.2.tar.gz` & `tmp/mkdocs_static_i18n-1.2.3.tar.gz`

## Comparing `mkdocs_static_i18n-1.2.2.tar` & `mkdocs_static_i18n-1.2.3.tar`

### file list

```diff
@@ -1,184 +1,184 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/__init__.py
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/config.py
--rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/folder.py
--rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/plugin.py
--rw-r--r--   0        0        0    34949 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/reconfigure.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/suffix.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/utils.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/custom_i18n_sitemap/sitemap.xml
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/conftest.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/hooks.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/hooks_jinja_on_env.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/mkdocs.yml
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_admonitions.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_config.py
--rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_control.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_hooks.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_language_selector.py
--rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_languages_option.py
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_navigation.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_rtd.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_search.py
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_structure_folder.py
--rw-r--r--   0        0        0    10509 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/test_structure_suffix.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/admonitions/index.fr.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/admonitions/index.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/assets/image_non_localized.png
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/image.fake
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/image.png
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/index.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/english_default/index.md
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/topic2/1.1.filename.html
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/image.fake
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/image.png
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/index.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/french_only/index.md
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/topic2/1.1.filename.html
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/assets/image_non_localized.png
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/image.fake
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/image.png
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/index.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/english_default/index.md
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/topic2/1.1.filename.html
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/image.fake
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/image.png
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/index.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/french_only/index.md
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/topic2/1.1.filename.html
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/topic2/README.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/assets/image_non_localized.png
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/image.fake
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/image.png
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/index.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/english_default/index.md
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/topic2/1.1.filename.html
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/image.fake
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/image.png
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/index.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/french_only/index.md
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/topic2/1.1.filename.html
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/image.en.fake
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/image.en.png
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/image.fr.fake
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/image.fr.png
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/index.fr.md
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/index.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/assets/image_non_localized.png
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/english_default/index.en.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/french_only/index.fr.md
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic1/named_file.en.md
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic1/named_file.fr.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic2/1.1.filename.fr.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic2/1.1.filename.html
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic2/README.fr.md
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/image.en.fake
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/image.en.png
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/image.fr.fake
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/image.fr.png
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/index.fr.md
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/index.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/assets/image_non_localized.png
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/english_default/index.en.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/french_only/index.fr.md
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic1/named_file.en.md
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic1/named_file.fr.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic2/1.1.filename.fr.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic2/1.1.filename.html
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic2/README.fr.md
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/mkdocs.yml
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/image.fake
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/image.png
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/index.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/assets/image_non_localized.png
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/english_default/index.md
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/image.fake
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/image.png
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/index.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/assets/image_non_localized.png
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/english_default/index.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/french_only/index.md
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/topic2/1.1.filename.html
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/topic2/1.1.filename.html
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/mkdocs.yml
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/image.fake
--rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/image.png
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/index.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/assets/image_non_localized.png
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/english_default/index.md
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/topic2/1.1.filename.html
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/mkdocs.yml
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/image.fake
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/image.png
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/index.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/assets/image_non_localized.png
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/french_only/index.md
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/topic2/1.1.filename.html
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/mkdocs.yml
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/image.fake
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/image.png
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/index.md
--rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/assets/image_non_localized.png
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/english_default/index.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/french_only/index.md
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/topic2/1.1.filename.html
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/topic2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/topic2/release_notes_17.1.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/topic2/release_notes_17.2.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/mkdocs.yml
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/image.fake
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/image.png
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/index.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/french_only/index.md
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/topic1/named_file.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/topic2/1.1.filename.html
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/topic2/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/tests/theme_overrides/content.html
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/LICENSE
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/README.md
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/__init__.py
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/config.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/folder.py
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/plugin.py
+-rw-r--r--   0        0        0    34984 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/reconfigure.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/suffix.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/utils.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/custom_i18n_sitemap/sitemap.xml
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/conftest.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/hooks.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/hooks_jinja_on_env.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/mkdocs.yml
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_admonitions.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_config.py
+-rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_control.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_hooks.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_language_selector.py
+-rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_languages_option.py
+-rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_navigation.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_rtd.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_search.py
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_structure_folder.py
+-rw-r--r--   0        0        0    10509 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/test_structure_suffix.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/admonitions/index.fr.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/admonitions/index.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/assets/image_non_localized.png
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/image.fake
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/image.png
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/index.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/english_default/index.md
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/image.fake
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/image.png
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/index.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/french_only/index.md
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/assets/image_non_localized.png
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/image.fake
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/image.png
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/index.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/english_default/index.md
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/image.fake
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/image.png
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/index.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/french_only/index.md
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/topic2/README.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/assets/image_non_localized.png
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/image.fake
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/image.png
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/index.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/english_default/index.md
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/image.fake
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/image.png
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/index.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/french_only/index.md
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/image.en.fake
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/image.en.png
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/image.fr.fake
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/image.fr.png
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/index.fr.md
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/index.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/assets/image_non_localized.png
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/english_default/index.en.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/french_only/index.fr.md
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic1/named_file.en.md
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic1/named_file.fr.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic2/1.1.filename.fr.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic2/README.fr.md
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/image.en.fake
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/image.en.png
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/image.fr.fake
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/image.fr.png
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/index.fr.md
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/index.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/assets/image_non_localized.png
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/english_default/index.en.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/french_only/index.fr.md
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic1/named_file.en.md
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic1/named_file.fr.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic2/1.1.filename.fr.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic2/README.fr.md
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/mkdocs.yml
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/image.fake
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/image.png
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/index.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/assets/image_non_localized.png
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/english_default/index.md
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/image.fake
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/image.png
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/index.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/assets/image_non_localized.png
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/english_default/index.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/french_only/index.md
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/mkdocs.yml
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/image.fake
+-rw-r--r--   0        0        0    16067 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/image.png
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/index.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/assets/image_non_localized.png
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/english_default/index.md
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/mkdocs.yml
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/image.fake
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/image.png
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/index.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/assets/image_non_localized.png
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/french_only/index.md
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/mkdocs.yml
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/image.fake
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/image.png
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/index.md
+-rw-r--r--   0        0        0   108053 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/assets/image_non_localized.png
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/english_default/index.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/french_only/index.md
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/topic2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/topic2/release_notes_17.1.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/topic2/release_notes_17.2.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/mkdocs.yml
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/image.fake
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/image.png
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/index.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/french_only/index.md
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/topic1/named_file.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/topic2/1.1.filename.html
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/topic2/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/tests/theme_overrides/content.html
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/README.md
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 mkdocs_static_i18n-1.2.3/PKG-INFO
```

### Comparing `mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/config.py` & `mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/folder.py` & `mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/folder.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/plugin.py` & `mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,22 @@
             "markdown_extensions" not in config or "admonition" not in config["markdown_extensions"]
         ):
             log.warning(
                 "admonition_translations used, but admonitions won't be rendered properly without 'admonition' in mkdocs.yml's markdown_extensions."
             )
 
         # reconfigure the mkdocs config
-        return self.reconfigure_mkdocs_config(config)
+        config = self.reconfigure_mkdocs_config(config)
+
+        # manually trigger with-pdf, to apply language specific overrides
+        with_pdf_plugin = config.plugins.get("with-pdf")
+        if with_pdf_plugin:
+            config = with_pdf_plugin.on_config(config)
+
+        return config
 
     @plugins.event_priority(-100)
     def on_files(self, files: Files, config: MkDocsConfig):
         """
         Construct the lang specific file tree which will be used to
         generate the navigation for the default site and per language.
```

### Comparing `mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/reconfigure.py` & `mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/reconfigure.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,15 +644,15 @@
             else:
                 log.warning(f"Unhandled file case - {file.src_uri}")
 
         # populate the resulting Files and keep track of all the alternates
         # that will be used by the sitemap.xml template
         for file in i18n_src_uris.values():
             if "index" in file.src_uri:
-                log.info(f"Selected {file.locale} {file.localization} {file}")
+                log.debug(f"Selected {file.locale} {file.localization} {file}")
             i18n_files.append(file)
 
         # build the alternates for all the Files
         self.reconfigure_files_alternates(
             i18n_src_uris, i18n_alternate_src_uris, mkdocs_config, create_i18n_file
         )
 
@@ -760,15 +760,16 @@
                 file.alternates = {self.current_language: file}
                 file.dest_uri = i18n_file.dest_uri
                 file.locale = i18n_file.locale
                 file.locale_alternate_of = self.current_language
                 file.norm_src_uri = i18n_file.norm_src_uri
                 file.url = i18n_file._get_url(mkdocs_config.use_directory_urls)
                 #
-                file.page._set_canonical_url(mkdocs_config.get('site_url', None))
+                if file.page:
+                    file.page._set_canonical_url(mkdocs_config.get('site_url', None))
 
         # reconfigure blog files alternates to the best we can
         # since we are past the on_files event and files useless to the current language
         # have been filtered out and new ones got generated by the blog plugin,
         # we can't get the complete view of the alternates
         self.reconfigure_files_alternates(
             i18n_src_uris, i18n_alternate_src_uris, mkdocs_config, create_i18n_file
```

### Comparing `mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/suffix.py` & `mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/suffix.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/utils.py` & `mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/mkdocs_static_i18n/custom_i18n_sitemap/sitemap.xml` & `mkdocs_static_i18n-1.2.3/mkdocs_static_i18n/custom_i18n_sitemap/sitemap.xml`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/conftest.py` & `mkdocs_static_i18n-1.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_admonitions.py` & `mkdocs_static_i18n-1.2.3/tests/test_admonitions.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_config.py` & `mkdocs_static_i18n-1.2.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_control.py` & `mkdocs_static_i18n-1.2.3/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_hooks.py` & `mkdocs_static_i18n-1.2.3/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_language_selector.py` & `mkdocs_static_i18n-1.2.3/tests/test_language_selector.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_languages_option.py` & `mkdocs_static_i18n-1.2.3/tests/test_languages_option.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_navigation.py` & `mkdocs_static_i18n-1.2.3/tests/test_navigation.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_rtd.py` & `mkdocs_static_i18n-1.2.3/tests/test_rtd.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_search.py` & `mkdocs_static_i18n-1.2.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_structure_folder.py` & `mkdocs_static_i18n-1.2.3/tests/test_structure_folder.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/test_structure_suffix.py` & `mkdocs_static_i18n-1.2.3/tests/test_structure_suffix.py`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/image.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/image.png` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/index.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/en/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/en/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/image.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/image.png` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/index.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_one_language/fr/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_one_language/fr/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/image.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/image.png` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/index.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/en/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/en/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/image.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/image.png` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/index.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages/fr/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages/fr/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/image.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/image.png` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/index.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/en/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/en/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/image.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/image.png` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/index.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_folder_structure_two_languages_with_default/fr/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/docs_folder_structure_two_languages_with_default/fr/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/image.en.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/image.en.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/image.en.png` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/image.en.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/image.fr.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/image.fr.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/image.fr.png` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/image.fr.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/index.fr.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/index.fr.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/index.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic1/named_file.en.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic1/named_file.en.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic1/named_file.fr.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic1/named_file.fr.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic2/README.fr.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic2/README.fr.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_one_language/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_one_language/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/image.en.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/image.en.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/image.en.png` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/image.en.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/image.fr.fake` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/image.fr.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/image.fr.png` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/image.fr.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/index.fr.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/index.fr.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/index.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic1/named_file.en.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic1/named_file.en.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic1/named_file.fr.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic1/named_file.fr.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic2/README.fr.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic2/README.fr.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/docs_suffix_structure_two_languages/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/docs_suffix_structure_two_languages/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/image.fake` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/image.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/index.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/image.fake` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/image.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/index.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/fr/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/fr/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_fr/docs/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_fr/docs/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/image.fake` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/image.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/index.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/en_only/docs/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/en_only/docs/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/image.fake` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/image.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/index.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_only/docs/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_only/docs/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/image.fake` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/image.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/index.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/assets/image_non_localized.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/assets/image_non_localized.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_with_default/docs/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_with_default/docs/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/image.fake` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/image.fake`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/image.png` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/index.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/topic1/named_file.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/topic1/named_file.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/tests/structures/control/fr_without_default/docs/topic2/README.md` & `mkdocs_static_i18n-1.2.3/tests/structures/control/fr_without_default/docs/topic2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/LICENSE` & `mkdocs_static_i18n-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/README.md` & `mkdocs_static_i18n-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/pyproject.toml` & `mkdocs_static_i18n-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs_static_i18n-1.2.2/PKG-INFO` & `mkdocs_static_i18n-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mkdocs-static-i18n
-Version: 1.2.2
+Version: 1.2.3
 Summary: MkDocs i18n plugin using static translation markdown files
 Project-URL: Documentation, https://github.com/ultrabug/mkdocs-static-i18n#readme
 Project-URL: Download, https://github.com/ultrabug/mkdocs-static-i18n/tags
 Project-URL: Funding, https://ultrabug.fr/#support-me
 Project-URL: Homepage, https://github.com/ultrabug/mkdocs-static-i18n
 Project-URL: Source, https://github.com/ultrabug/mkdocs-static-i18n
 Project-URL: Tracker, https://github.com/ultrabug/mkdocs-static-i18n/issues
```

