# Comparing `tmp/xklb-2.7.8.tar.gz` & `tmp/xklb-2.7.9.tar.gz`

## Comparing `xklb-2.7.8.tar` & `xklb-2.7.9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.7.8/.gitattributes
--rw-r--r--   0        0        0   216289 2020-02-02 00:00:00.000000 xklb-2.7.8/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/examples/art.avif
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/__init__.py
--rw-r--r--   0        0        0    14290 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/lb.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/media_printer.py
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/readme.py
--rw-r--r--   0        0        0   112269 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/__init__.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/av.py
--rw-r--r--   0        0        0    21197 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/fs_add.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/gallery_add.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/gallery_backend.py
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/hn_add.py
--rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/links_add.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/places_import.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/reddit_add.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/row_add.py
--rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/site_add.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/substack.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/subtitle.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/tabs_add.py
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/tildes.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/tube_add.py
--rw-r--r--   0        0        0    20265 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/tube_backend.py
--rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/createdb/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/data/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/__init__.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/dedupe_db.py
--rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/dedupe_media.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/merge_online_local.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/mpv_watchlater.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/pushshift.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/editdb/reddit_selftext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/christen.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/sample_compare.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/sample_hash.py
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/files/similar_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/__init__.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/merge_folders.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/mount_stats.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/move_list.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/rel_mv.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/scatter.py
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/folders/similar_folders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/fsdb/__init__.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/fsdb/big_dirs.py
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/fsdb/disk_usage.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/fsdb/search_db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/__init__.py
--rw-r--r--   0        0        0    11660 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/block.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/db_history.py
--rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/db_media.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/db_playlists.py
--rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/download.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/download_status.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/history.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/history_add.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/optimize_db.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/playlists.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/redownload.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/search.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediadb/stats.py
--rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediafiles/media_check.py
--rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediafiles/process_ffmpeg.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/mediafiles/process_image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/misc/__init__.py
--rw-r--r--   0        0        0    13764 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/misc/dedupe_czkawka.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/misc/export_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/multidb/__init__.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/multidb/copy_play_counts.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/multidb/merge_dbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/__init__.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/links_open.py
--rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/media_player.py
--rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/play_actions.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/playback_control.py
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/post_actions.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/surf.py
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/playback/tabs_open.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/tablefiles/__init__.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/tablefiles/eda.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/tablefiles/incremental_diff.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/tablefiles/mcda.py
--rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/cluster_sort.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/extract_links.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/extract_text.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/markdown_links.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/text/nouns.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/__init__.py
--rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    17658 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/consts.py
--rw-r--r--   0        0        0    11382 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/devices.py
--rw-r--r--   0        0        0    15295 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/nums.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/objects.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/printing.py
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/processes.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/strings.py
--rw-r--r--   0        0        0    22864 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/utils/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/assets/__init__.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.7.8/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.7.8/.gitignore
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 xklb-2.7.8/pyproject.toml
--rw-r--r--   0        0        0   156014 2020-02-02 00:00:00.000000 xklb-2.7.8/.github/README.md
--rw-r--r--   0        0        0   159795 2020-02-02 00:00:00.000000 xklb-2.7.8/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.7.9/.gitattributes
+-rw-r--r--   0        0        0   216289 2020-02-02 00:00:00.000000 xklb-2.7.9/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/examples/art.avif
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/__init__.py
+-rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/lb.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/media_printer.py
+-rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/readme.py
+-rw-r--r--   0        0        0   112269 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/__init__.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/av.py
+-rw-r--r--   0        0        0    21197 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/fs_add.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/gallery_add.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/gallery_backend.py
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/hn_add.py
+-rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/links_add.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/places_import.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/reddit_add.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/row_add.py
+-rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/site_add.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/substack.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/subtitle.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/tabs_add.py
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/tildes.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/tube_add.py
+-rw-r--r--   0        0        0    20265 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/tube_backend.py
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/data/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/__init__.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/dedupe_db.py
+-rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/dedupe_media.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/merge_online_local.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/mpv_watchlater.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/pushshift.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/reddit_selftext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/christen.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/sample_compare.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/sample_hash.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/similar_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/__init__.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/merge_folders.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/mount_stats.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/move_list.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/rel_mv.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/scatter.py
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/similar_folders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/fsdb/__init__.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/fsdb/big_dirs.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/fsdb/disk_usage.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/fsdb/search_db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/__init__.py
+-rw-r--r--   0        0        0    11660 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/block.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/db_history.py
+-rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/db_media.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/db_playlists.py
+-rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/download.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/download_status.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/history.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/history_add.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/optimize_db.py
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/playlists.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/redownload.py
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/search.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/stats.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediafiles/media_check.py
+-rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediafiles/process_ffmpeg.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediafiles/process_image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/misc/__init__.py
+-rw-r--r--   0        0        0    13764 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/misc/dedupe_czkawka.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/misc/export_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/multidb/__init__.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/multidb/copy_play_counts.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/multidb/merge_dbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/__init__.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/links_open.py
+-rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/media_player.py
+-rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/play_actions.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/playback_control.py
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/post_actions.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/surf.py
+-rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/tabs_open.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/tablefiles/__init__.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/tablefiles/eda.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/tablefiles/incremental_diff.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/tablefiles/mcda.py
+-rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/cluster_sort.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/extract_links.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/extract_text.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/markdown_links.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/nouns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    17737 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/consts.py
+-rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/nums.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/processes.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/strings.py
+-rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/assets/__init__.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.7.9/.gitignore
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 xklb-2.7.9/pyproject.toml
+-rw-r--r--   0        0        0   156009 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/README.md
+-rw-r--r--   0        0        0   159790 2020-02-02 00:00:00.000000 xklb-2.7.9/PKG-INFO
```

### Comparing `xklb-2.7.8/pdm.lock` & `xklb-2.7.9/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/.github/LICENSE` & `xklb-2.7.9/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/.github/Windows.md` & `xklb-2.7.9/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/.github/examples/art.avif` & `xklb-2.7.9/.github/examples/art.avif`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/.github/examples/extract.svg` & `xklb-2.7.9/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/.github/examples/tubeadd.svg` & `xklb-2.7.9/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/.github/workflows/push.yaml` & `xklb-2.7.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/lb.py` & `xklb-2.7.9/xklb/lb.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,15 +116,16 @@
             [(key.replace("_", "-"), value) for key, value in category_progs.items()],
             tablefmt="rounded_grid",
             showindex=False,
         )
         subcommands_list.append(textwrap.indent(category_progs_text, "    "))
         subcommands_list.append("\n")
 
-    return f"""xk media library subcommands (v{__version__})
+    subcommands = list(iterables.flatten((v.keys() for k, v in progs.items())))
+    return f"""library (v{__version__}; {len(subcommands)} subcommands)
 {''.join(subcommands_list)}"""
 
 
 def print_help(parser) -> None:
     print(usage())
     print(parser.epilog)
```

### Comparing `xklb-2.7.8/xklb/media_printer.py` & `xklb-2.7.9/xklb/media_printer.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/readme.py` & `xklb-2.7.9/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/usage.py` & `xklb-2.7.9/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/av.py` & `xklb-2.7.9/xklb/createdb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/fs_add.py` & `xklb-2.7.9/xklb/createdb/fs_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/gallery_add.py` & `xklb-2.7.9/xklb/createdb/gallery_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/gallery_backend.py` & `xklb-2.7.9/xklb/createdb/gallery_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/hn_add.py` & `xklb-2.7.9/xklb/createdb/hn_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/links_add.py` & `xklb-2.7.9/xklb/createdb/links_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/places_import.py` & `xklb-2.7.9/xklb/createdb/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/reddit_add.py` & `xklb-2.7.9/xklb/createdb/reddit_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/row_add.py` & `xklb-2.7.9/xklb/createdb/row_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/site_add.py` & `xklb-2.7.9/xklb/createdb/site_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/substack.py` & `xklb-2.7.9/xklb/createdb/substack.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/subtitle.py` & `xklb-2.7.9/xklb/createdb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/tabs_add.py` & `xklb-2.7.9/xklb/createdb/tabs_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/tildes.py` & `xklb-2.7.9/xklb/createdb/tildes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/tube_add.py` & `xklb-2.7.9/xklb/createdb/tube_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/tube_backend.py` & `xklb-2.7.9/xklb/createdb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/createdb/web_add.py` & `xklb-2.7.9/xklb/createdb/web_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/data/imagemagick_errors.py` & `xklb-2.7.9/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/data/wordbank.py` & `xklb-2.7.9/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/data/yt_dlp_errors.py` & `xklb-2.7.9/xklb/data/yt_dlp_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/editdb/dedupe_db.py` & `xklb-2.7.9/xklb/editdb/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/editdb/dedupe_media.py` & `xklb-2.7.9/xklb/editdb/dedupe_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/editdb/merge_online_local.py` & `xklb-2.7.9/xklb/editdb/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/editdb/mpv_watchlater.py` & `xklb-2.7.9/xklb/editdb/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/editdb/pushshift.py` & `xklb-2.7.9/xklb/editdb/pushshift.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     args = parse_args("pushshift", usage=usage.pushshift)
 
     args.db.enable_wal()
 
     count = 0
     reddit_posts = []
     media = []
-    print("Reading from stdin...", file=sys.stderr)
+    print("library pushshift: Reading from stdin...", file=sys.stderr)
     for line in sys.stdin:
         line = line.rstrip("\n")
         if line in ["", '""', "\n"]:
             continue
 
         try:
             post_dict = orjson.loads(line)
```

### Comparing `xklb-2.7.8/xklb/editdb/reddit_selftext.py` & `xklb-2.7.9/xklb/editdb/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/files/christen.py` & `xklb-2.7.9/xklb/files/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/files/sample_compare.py` & `xklb-2.7.9/xklb/files/sample_compare.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/files/sample_hash.py` & `xklb-2.7.9/xklb/files/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/files/similar_files.py` & `xklb-2.7.9/xklb/files/similar_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,7 +146,10 @@
                     headers="keys",
                     showindex=False,
                 )
             )
 
         if not args.only_originals and not args.only_duplicates:
             print()
+
+    if not args.only_originals and not args.only_duplicates:
+        print(len(groups), "groups found")
```

### Comparing `xklb-2.7.8/xklb/folders/merge_folders.py` & `xklb-2.7.9/xklb/folders/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/folders/mount_stats.py` & `xklb-2.7.9/xklb/folders/mount_stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/folders/move_list.py` & `xklb-2.7.9/xklb/folders/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/folders/rel_mv.py` & `xklb-2.7.9/xklb/folders/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/folders/scatter.py` & `xklb-2.7.9/xklb/folders/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/folders/similar_folders.py` & `xklb-2.7.9/xklb/folders/similar_folders.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import humanize
 from tabulate import tabulate
 
 from xklb import usage
 from xklb.fsdb import big_dirs
 from xklb.text import cluster_sort
-from xklb.utils import arg_utils, arggroups, consts, nums, objects, path_utils, printing, strings
+from xklb.utils import arg_utils, arggroups, consts, nums, objects, path_utils, printing, sql_utils, strings
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser(usage=usage.similar_folders)
     arggroups.operation_group_folders(parser)
     arggroups.operation_cluster(parser)
@@ -136,14 +136,17 @@
     return groups
 
 
 def similar_folders():
     args = parse_args()
     media = list(arg_utils.gen_d(args))
     media = big_dirs.group_files_by_parent(args, media)
+    if args.folder_size:
+        args.folder_size = sql_utils.parse_human_to_lambda(nums.human_to_bytes, args.folder_size)
+        media = [d for d in media if args.folder_size(d["size"])]
 
     if args.filter_sizes or args.filter_counts:
         clusters = cluster_by_size(args, media)
         groups = map_and_name(media, clusters)
         log.info("Folder size/count clustering sorted %s folders into %s groups", len(media), len(groups))
         single_folder_groups = [d for d in groups if len(d["grouped_paths"]) == 1]
         groups = [d for d in groups if len(d["grouped_paths"]) > 1]
@@ -194,7 +197,10 @@
                     headers="keys",
                     showindex=False,
                 )
             )
 
         if not args.only_originals and not args.only_duplicates:
             print()
+
+    if not args.only_originals and not args.only_duplicates:
+        print(len(groups), "groups found")
```

### Comparing `xklb-2.7.8/xklb/fsdb/big_dirs.py` & `xklb-2.7.9/xklb/fsdb/big_dirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/fsdb/disk_usage.py` & `xklb-2.7.9/xklb/fsdb/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/fsdb/search_db.py` & `xklb-2.7.9/xklb/fsdb/search_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/block.py` & `xklb-2.7.9/xklb/mediadb/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/db_history.py` & `xklb-2.7.9/xklb/mediadb/db_history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/db_media.py` & `xklb-2.7.9/xklb/mediadb/db_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/db_playlists.py` & `xklb-2.7.9/xklb/mediadb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/download.py` & `xklb-2.7.9/xklb/mediadb/download.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/download_status.py` & `xklb-2.7.9/xklb/mediadb/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/history.py` & `xklb-2.7.9/xklb/mediadb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/history_add.py` & `xklb-2.7.9/xklb/mediadb/history_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/optimize_db.py` & `xklb-2.7.9/xklb/mediadb/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/playlists.py` & `xklb-2.7.9/xklb/mediadb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/redownload.py` & `xklb-2.7.9/xklb/mediadb/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/search.py` & `xklb-2.7.9/xklb/mediadb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediadb/stats.py` & `xklb-2.7.9/xklb/mediadb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediafiles/media_check.py` & `xklb-2.7.9/xklb/mediafiles/media_check.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediafiles/process_ffmpeg.py` & `xklb-2.7.9/xklb/mediafiles/process_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/mediafiles/process_image.py` & `xklb-2.7.9/xklb/mediafiles/process_image.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/misc/dedupe_czkawka.py` & `xklb-2.7.9/xklb/misc/dedupe_czkawka.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/misc/export_text.py` & `xklb-2.7.9/xklb/misc/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/multidb/copy_play_counts.py` & `xklb-2.7.9/xklb/multidb/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/multidb/merge_dbs.py` & `xklb-2.7.9/xklb/multidb/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/playback/links_open.py` & `xklb-2.7.9/xklb/playback/links_open.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/playback/media_player.py` & `xklb-2.7.9/xklb/playback/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/playback/play_actions.py` & `xklb-2.7.9/xklb/playback/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/playback/playback_control.py` & `xklb-2.7.9/xklb/playback/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/playback/post_actions.py` & `xklb-2.7.9/xklb/playback/post_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/playback/surf.py` & `xklb-2.7.9/xklb/playback/surf.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/playback/tabs_open.py` & `xklb-2.7.9/xklb/playback/tabs_open.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/scratch/javguru.py` & `xklb-2.7.9/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/scratch/javtiful.py` & `xklb-2.7.9/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/scratch/mam_search.py` & `xklb-2.7.9/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/scratch/mam_slots.py` & `xklb-2.7.9/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/tablefiles/eda.py` & `xklb-2.7.9/xklb/tablefiles/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/tablefiles/incremental_diff.py` & `xklb-2.7.9/xklb/tablefiles/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/tablefiles/mcda.py` & `xklb-2.7.9/xklb/tablefiles/mcda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/text/cluster_sort.py` & `xklb-2.7.9/xklb/text/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/text/extract_links.py` & `xklb-2.7.9/xklb/text/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/text/extract_text.py` & `xklb-2.7.9/xklb/text/extract_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/text/markdown_links.py` & `xklb-2.7.9/xklb/text/markdown_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/text/nouns.py` & `xklb-2.7.9/xklb/text/nouns.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,10 +60,10 @@
 
 
 def nouns() -> None:
     parser = argparse.ArgumentParser(usage.nouns)
     arggroups.debug(parser)
     args = parser.parse_args()
 
-    print("Reading from stdin...", file=sys.stderr)
+    print("library nouns: Reading from stdin...", file=sys.stderr)
     for line in sys.stdin:
         line_processor(line)
```

### Comparing `xklb-2.7.8/xklb/utils/arg_utils.py` & `xklb-2.7.9/xklb/utils/arg_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,25 @@
                 for line in f:
                     line = line.rstrip("\n")
                     if line.strip():
                         yield line
     elif args.paths_from_dbs or args.titles_from_dbs:
         for path in args.paths:
             if is_sqlite(path):
-                s_db = db_utils.connect(args, conn=sqlite3.connect(args.database))
+                s_db = db_utils.connect(args, conn=sqlite3.connect(path))
                 m_columns = s_db["media"].columns_dict
                 yield from (
                     d["path"]
                     for d in s_db.query(
                         f"""
                     SELECT
                         {'title AS path' if args.titles_from_dbs else 'path'}
                     FROM media
                     WHERE 1=1
-                    {'and COALESCE(m.time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
+                    {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
                     """
                     )
                 )
             else:
                 print("Skipping non-SQLite file:", path)
     else:
         is_large = len(args.paths) > 1000
@@ -72,25 +72,25 @@
                     if line.strip():
                         d = d_from_path(line)
                         if d:
                             yield d
     elif args.paths_from_dbs or args.titles_from_dbs:
         for path in args.paths:
             if is_sqlite(path):
-                s_db = db_utils.connect(args, conn=sqlite3.connect(args.database))
+                s_db = db_utils.connect(args, conn=sqlite3.connect(path))
                 m_columns = s_db["media"].columns_dict
                 yield from s_db.query(
                     f"""
                     SELECT
                         path
                         {', size' if 'size' in m_columns else ''}
                         {', title' if 'title' in m_columns else ''}
                     FROM media
                     WHERE 1=1
-                    {'and COALESCE(m.time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
+                    {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
                     """
                 )
             else:
                 print("Skipping non-SQLite file:", path)
     else:
         for path in args.paths:
             if path.strip():
```

### Comparing `xklb-2.7.8/xklb/utils/arggroups.py` & `xklb-2.7.9/xklb/utils/arggroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,15 @@
     )
 
 
 def requests(parser):
     parser.add_argument("--cookies", help="path to a Netscape formatted cookies file")
     parser.add_argument("--cookies-from-browser", metavar="BROWSER[+KEYRING][:PROFILE][::CONTAINER]")
     parser.add_argument("--allow-insecure", "--allow-untrusted", "--disable-tls", action="store_true")
+    parser.add_argument("--http-max-retries", "--https-max-retries", type=int)
 
 
 def selenium(parser):
     parser.add_argument("--selenium", "--js", action="store_true")
     parser.add_argument("--firefox", action="store_true")
     parser.add_argument("--chrome", action="store_true")
     parser.add_argument("--scroll", action="store_true", help="Scroll down the page; infinite scroll")
```

### Comparing `xklb-2.7.8/xklb/utils/argparse_utils.py` & `xklb-2.7.9/xklb/utils/argparse_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,16 @@
             raise argparse.ArgumentError(self, msg) from ex
         setattr(args, self.dest, d)
 
 
 class ArgparseArgsOrStdin(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         if values == STDIN_DASH:
-            print("Reading from stdin...", file=sys.stderr)
+            prog = " ".join((parser.usage or "").split(" ", maxsplit=3)[0:2])
+            print(f"{prog}: Reading from stdin...", file=sys.stderr)
             lines = sys.stdin.readlines()
             if not lines or (len(lines) == 1 and lines[0].strip() == ""):
                 lines = None
             else:
                 lines = [s.strip() for s in lines]
         else:
             lines = values
```

### Comparing `xklb-2.7.8/xklb/utils/consts.py` & `xklb-2.7.9/xklb/utils/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/db_utils.py` & `xklb-2.7.9/xklb/utils/db_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         db = DB(tracer=tracer if args.verbose >= consts.LOG_DEBUG_SQL else None, **kwargs)  # type: ignore
         return db
 
     db_override = getattr(args, "db", None)
     if db_override and isinstance(db_override, str):
         args.database = db_override
 
-    if not Path(args.database).exists() and ":memory:" not in args.database:
+    if conn is None and not Path(args.database).exists() and ":memory:" not in args.database:
         log.error(f"Database file '{args.database}' does not exist. Create one with lb fsadd, tubeadd, or tabsadd.")
         raise SystemExit(1)
 
     db = DB(conn or args.database, tracer=tracer if args.verbose >= consts.LOG_DEBUG_SQL else None, **kwargs)  # type: ignore
     with db.conn:  # type: ignore
         db.conn.execute("PRAGMA main.cache_size = 8000")  # type: ignore
```

### Comparing `xklb-2.7.8/xklb/utils/devices.py` & `xklb-2.7.9/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/file_utils.py` & `xklb-2.7.9/xklb/utils/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         except (FileNotFoundError, PermissionError):
             pass
         else:
             for entry in scanned_dir:
                 if entry.is_dir(follow_symlinks=False):
                     folders.add(entry.path)
                     stack.append(entry.path)
+                elif entry.is_symlink():
+                    pass
                 else:
                     if extensions is None:
                         files.add(entry.path)
                     else:
                         extension = entry.path.rsplit(".", 1)[-1].lower()
                         if extension in extensions:
                             files.add(entry.path)
```

### Comparing `xklb-2.7.8/xklb/utils/gui.py` & `xklb-2.7.9/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/iterables.py` & `xklb-2.7.9/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/log_utils.py` & `xklb-2.7.9/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/mpv_utils.py` & `xklb-2.7.9/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/nums.py` & `xklb-2.7.9/xklb/utils/nums.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/objects.py` & `xklb-2.7.9/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/path_utils.py` & `xklb-2.7.9/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/pd_utils.py` & `xklb-2.7.9/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/printing.py` & `xklb-2.7.9/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/processes.py` & `xklb-2.7.9/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/sql_utils.py` & `xklb-2.7.9/xklb/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/strings.py` & `xklb-2.7.9/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/xklb/utils/web.py` & `xklb-2.7.9/xklb/utils/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,34 +11,38 @@
 from xklb.utils.log_utils import clamp_index, log
 
 headers = {"User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:121.0) Gecko/20100101 Firefox/121.0"}
 session = None
 
 
 def _get_retry_adapter(max_retries):
-    import requests.adapters, urllib3.util.retry
+    import requests.adapters
 
-    retries = urllib3.util.retry.Retry(
+    retry = requests.adapters.Retry(
         total=max_retries,
         connect=max_retries,
         read=max_retries,
-        status=2,
-        redirect=False,  # don't fail on redirect
-        backoff_factor=5,
+        status=max_retries // 2,
+        other=1,
+        redirect=4,
+        raise_on_redirect=False,
+        backoff_factor=3,
         status_forcelist=[
+            104,
             413,
             429,
             500,
             502,
             503,
             504,
+            522,
         ],
     )
 
-    return requests.adapters.HTTPAdapter(max_retries=retries)
+    return requests.adapters.HTTPAdapter(max_retries=retry)
 
 
 def parse_cookies_from_browser(input_str):
     from yt_dlp.cookies import SUPPORTED_BROWSERS, SUPPORTED_KEYRINGS
 
     # lifted from yt_dlp to have a compatible interface
     container = None
@@ -72,21 +76,22 @@
 
 def requests_session(args=argparse.Namespace()):
     global session  # TODO: maybe run_once similar to log_utils.log
 
     if session is None:
         import requests
 
-        http_max_retries = getattr(args, "http_max_retries", None) or 5
+        http_max_retries = getattr(args, "http_max_retries", None) or 8
         cookie_file = getattr(args, "cookies", None)
         cookies_from_browser = getattr(args, "cookies_from_browser", None)
 
         session = requests.Session()
-        session.mount("http", _get_retry_adapter(http_max_retries))  # also includes https
-        session.request = functools.partial(session.request, headers=headers, timeout=(4, 45))  # type: ignore
+        session.mount("http://", _get_retry_adapter(http_max_retries))
+        session.mount("https://", _get_retry_adapter(http_max_retries))
+        session.request = functools.partial(session.request, headers=headers, timeout=(5, 45))  # type: ignore
 
         if getattr(args, "allow_insecure", False):
             from urllib3.exceptions import InsecureRequestWarning
 
             requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)  # type: ignore
             session.verify = False
```

### Comparing `xklb-2.7.8/xklb/assets/kotobago.png` & `xklb-2.7.9/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/.gitignore` & `xklb-2.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/pyproject.toml` & `xklb-2.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.7.8/.github/README.md` & `xklb-2.7.9/.github/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.7.008)
+    library (v2.7.009; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
```

### Comparing `xklb-2.7.8/PKG-INFO` & `xklb-2.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.7.8
+Version: 2.7.9
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -182,15 +182,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.7.008)
+    library (v2.7.009; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
```

