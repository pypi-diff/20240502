# Comparing `tmp/pygpt_net-2.2.7.tar.gz` & `tmp/pygpt_net-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt_net-2.2.7.tar", max compression
+gzip compressed data, was "pygpt_net-2.2.8.tar", max compression
```

## Comparing `pygpt_net-2.2.7.tar` & `pygpt_net-2.2.8.tar`

### file list

```diff
@@ -1,855 +1,869 @@
--rwxr-xr-x   0        0        0    59167 2024-05-01 18:08:40.466948 pygpt_net-2.2.7/CHANGELOG.md
--rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.7/LICENSE
--rwxr-xr-x   0        0        0   136279 2024-05-01 18:08:40.466948 pygpt_net-2.2.7/README.md
--rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.7/icon.png
--rw-r--r--   0        0        0     2979 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/pyproject.toml
--rwxr-xr-x   0        0        0    58137 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/CHANGELOG.txt
--rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.7/src/pygpt_net/LICENSE
--rwxr-xr-x   0        0        0     1024 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/__init__.py
--rwxr-xr-x   0        0        0    14447 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/app.py
--rwxr-xr-x   0        0        0    15485 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/config.py
--rwxr-xr-x   0        0        0     3683 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/container.py
--rwxr-xr-x   0        0        0     5164 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/__init__.py
--rw-r--r--   0        0        0     4730 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/agent/__init__.py
--rw-r--r--   0        0        0     1408 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/agent/experts.py
--rw-r--r--   0        0        0     6829 2024-03-17 13:18:45.622350 pygpt_net-2.2.7/src/pygpt_net/controller/agent/flow.py
--rw-r--r--   0        0        0     9877 2024-04-29 15:13:32.571516 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/__init__.py
--rw-r--r--   0        0        0    20310 2024-04-30 16:41:29.971889 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/batch.py
--rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/editor.py
--rw-r--r--   0        0        0    14434 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/files.py
--rwxr-xr-x   0        0        0    15545 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/store.py
--rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/threads.py
--rwxr-xr-x   0        0        0    15524 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/attachment.py
--rw-r--r--   0        0        0     5972 2024-03-20 16:01:43.275339 pygpt_net-2.2.7/src/pygpt_net/controller/audio/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/calendar/__init__.py
--rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/controller/calendar/note.py
--rwxr-xr-x   0        0        0    12681 2024-04-30 16:41:29.971889 pygpt_net-2.2.7/src/pygpt_net/controller/camera.py
--rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/chat/__init__.py
--rwxr-xr-x   0        0        0    11581 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/common.py
--rw-r--r--   0        0        0     2156 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/chat/files.py
--rwxr-xr-x   0        0        0     6533 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/image.py
--rwxr-xr-x   0        0        0    10399 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/input.py
--rwxr-xr-x   0        0        0    11382 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/output.py
--rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.7/src/pygpt_net/controller/chat/render.py
--rw-r--r--   0        0        0    12683 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/text.py
--rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.7/src/pygpt_net/controller/chat/vision.py
--rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.7/src/pygpt_net/controller/command.py
--rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.7/src/pygpt_net/controller/config/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/__init__.py
--rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/checkbox.py
--rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/cmd.py
--rw-r--r--   0        0        0     3237 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/combo.py
--rw-r--r--   0        0        0     6657 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/dictionary.py
--rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/input.py
--rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/slider.py
--rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/textarea.py
--rw-r--r--   0        0        0     7255 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/config/placeholder.py
--rw-r--r--   0        0        0    29541 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/ctx/__init__.py
--rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.7/src/pygpt_net/controller/ctx/common.py
--rwxr-xr-x   0        0        0     7477 2024-04-29 04:57:38.321533 pygpt_net-2.2.7/src/pygpt_net/controller/ctx/extra.py
--rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.7/src/pygpt_net/controller/ctx/summarizer.py
--rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/debug/__init__.py
--rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/__init__.py
--rwxr-xr-x   0        0        0    13546 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/confirm.py
--rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/debug.py
--rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/info.py
--rwxr-xr-x   0        0        0    15699 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/files.py
--rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.7/src/pygpt_net/controller/finder.py
--rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/idx/__init__.py
--rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.7/src/pygpt_net/controller/idx/common.py
--rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.7/src/pygpt_net/controller/idx/indexer.py
--rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.7/src/pygpt_net/controller/idx/settings.py
--rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/lang/__init__.py
--rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/controller/lang/custom.py
--rw-r--r--   0        0        0    20222 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/controller/lang/mapping.py
--rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.7/src/pygpt_net/controller/lang/plugins.py
--rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.7/src/pygpt_net/controller/lang/settings.py
--rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.7/src/pygpt_net/controller/launcher.py
--rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/layout.py
--rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/mode.py
--rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.7/src/pygpt_net/controller/model/__init__.py
--rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.7/src/pygpt_net/controller/model/editor.py
--rwxr-xr-x   0        0        0    11795 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/notepad.py
--rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/painter/__init__.py
--rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.7/src/pygpt_net/controller/painter/capture.py
--rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.7/src/pygpt_net/controller/painter/common.py
--rw-r--r--   0        0        0    14232 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/plugins/__init__.py
--rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.7/src/pygpt_net/controller/plugins/presets.py
--rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.7/src/pygpt_net/controller/plugins/settings.py
--rwxr-xr-x   0        0        0    17127 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/presets/__init__.py
--rwxr-xr-x   0        0        0    16058 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/presets/editor.py
--rw-r--r--   0        0        0     4937 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/presets/experts.py
--rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/settings/__init__.py
--rwxr-xr-x   0        0        0    14833 2024-04-24 02:39:32.054775 pygpt_net-2.2.7/src/pygpt_net/controller/settings/editor.py
--rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/settings/profile.py
--rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.7/src/pygpt_net/controller/settings/workdir.py
--rwxr-xr-x   0        0        0     6308 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/theme/__init__.py
--rwxr-xr-x   0        0        0     5437 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/controller/theme/common.py
--rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/controller/theme/markdown.py
--rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.7/src/pygpt_net/controller/theme/menu.py
--rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/controller/theme/nodes.py
--rw-r--r--   0        0        0     6093 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/controller/ui/__init__.py
--rw-r--r--   0        0        0     6663 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/ui/mode.py
--rw-r--r--   0        0        0     2378 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/controller/ui/vision.py
--rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.7/src/pygpt_net/core/__init__.py
--rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.7/src/pygpt_net/core/assistants/__init__.py
--rw-r--r--   0        0        0     9796 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/core/assistants/files.py
--rw-r--r--   0        0        0     7990 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/core/assistants/store.py
--rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.7/src/pygpt_net/core/attachments.py
--rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.7/src/pygpt_net/core/audio.py
--rw-r--r--   0        0        0     7490 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/core/bridge.py
--rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/core/calendar/__init__.py
--rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.7/src/pygpt_net/core/camera.py
--rw-r--r--   0        0        0     3330 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/core/chain/__init__.py
--rw-r--r--   0        0        0     4988 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/core/chain/chat.py
--rw-r--r--   0        0        0     5413 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/core/chain/completion.py
--rwxr-xr-x   0        0        0    10217 2024-03-17 14:26:02.923314 pygpt_net-2.2.7/src/pygpt_net/core/command.py
--rwxr-xr-x   0        0        0    34627 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/ctx/__init__.py
--rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.7/src/pygpt_net/core/ctx/idx.py
--rw-r--r--   0        0        0    15975 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/db/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.7/src/pygpt_net/core/db/viewer.py
--rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.7/src/pygpt_net/core/debug/__init__.py
--rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.7/src/pygpt_net/core/debug/agent.py
--rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.7/src/pygpt_net/core/debug/assistants.py
--rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/attachments.py
--rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.7/src/pygpt_net/core/debug/config.py
--rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.7/src/pygpt_net/core/debug/context.py
--rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.7/src/pygpt_net/core/debug/db.py
--rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/core/debug/indexes.py
--rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/models.py
--rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/plugins.py
--rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/presets.py
--rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/ui.py
--rwxr-xr-x   0        0        0     9307 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/dispatcher.py
--rw-r--r--   0        0        0     9117 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/experts/__init__.py
--rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/__init__.py
--rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/actions.py
--rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/editor.py
--rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/types.py
--rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/url.py
--rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/core/history.py
--rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.7/src/pygpt_net/core/idx/__init__.py
--rwxr-xr-x   0        0        0    13030 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/idx/chat.py
--rw-r--r--   0        0        0     2443 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/idx/context.py
--rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.7/src/pygpt_net/core/idx/indexing.py
--rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.7/src/pygpt_net/core/idx/llm.py
--rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.7/src/pygpt_net/core/idx/metadata.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.7/src/pygpt_net/core/idx/types/__init__.py
--rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.7/src/pygpt_net/core/idx/types/ctx.py
--rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.7/src/pygpt_net/core/idx/types/external.py
--rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/core/idx/types/files.py
--rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.7/src/pygpt_net/core/idx/worker.py
--rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.7/src/pygpt_net/core/image.py
--rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.7/src/pygpt_net/core/info.py
--rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.7/src/pygpt_net/core/installer.py
--rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.7/src/pygpt_net/core/llm/__init__.py
--rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.7/src/pygpt_net/core/locale.py
--rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/core/models.py
--rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/core/modes.py
--rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.7/src/pygpt_net/core/notepad.py
--rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/core/platforms.py
--rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.7/src/pygpt_net/core/plugins.py
--rw-r--r--   0        0        0    12366 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/presets.py
--rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.7/src/pygpt_net/core/profile.py
--rw-r--r--   0        0        0     4529 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/prompt/__init__.py
--rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.7/src/pygpt_net/core/prompt/template.py
--rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.7/src/pygpt_net/core/render/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/core/render/base.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/__init__.py
--rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/parser.py
--rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/renderer.py
--rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.7/src/pygpt_net/core/render/plain/__init__.py
--rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/render/plain/renderer.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.7/src/pygpt_net/core/render/web/__init__.py
--rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.7/src/pygpt_net/core/render/web/parser.py
--rwxr-xr-x   0        0        0    43236 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/render/web/renderer.py
--rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/text/__init__.py
--rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/text/finder.py
--rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/core/text/utils.py
--rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/text/web_finder.py
--rwxr-xr-x   0        0        0    14472 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/tokens.py
--rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.7/src/pygpt_net/core/updater/__init__.py
--rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.7/src/pygpt_net/core/web.py
--rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.7/src/pygpt_net/core/worker.py
--rwxr-xr-x   0        0        0    14457 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/config.json
--rwxr-xr-x   0        0        0    20573 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/models.json
--rw-r--r--   0        0        0     1595 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/modes.json
--rwxr-xr-x   0        0        0      528 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/batman_and_joker.json
--rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.agent.json
--rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.assistant.json
--rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.chat.json
--rwxr-xr-x   0        0        0      436 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.completion.json
--rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.expert.json
--rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.img.json
--rwxr-xr-x   0        0        0      433 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.langchain.json
--rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.llama_index.json
--rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.vision.json
--rwxr-xr-x   0        0        0      552 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/dalle_white_cat.json
--rw-r--r--   0        0        0      474 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/joke_agent.json
--rw-r--r--   0        0        0      683 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/joke_expert.json
--rwxr-xr-x   0        0        0    33579 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/settings.json
--rw-r--r--   0        0        0      804 2024-03-17 13:18:45.634349 pygpt_net-2.2.7/src/pygpt_net/data/config/settings_section.json
--rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/fix_windows.css
--rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.css
--rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.dark.css
--rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.light.css
--rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/style.css
--rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/data/css/style.dark.css
--rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/style.light.css
--rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/data/css/web.css
--rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.7/src/pygpt_net/data/css/web.dark.css
--rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.7/src/pygpt_net/data/css/web.light.css
--rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
--rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
--rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
--rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
--rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
--rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
--rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
--rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
--rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
--rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
--rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/OFL.txt
--rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
--rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
--rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
--rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
--rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
--rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
--rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
--rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
--rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
--rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
--rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
--rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
--rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
--rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
--rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
--rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
--rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
--rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
--rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
--rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
--rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
--rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
--rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
--rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
--rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
--rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.7/src/pygpt_net/data/icon.ico
--rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.7/src/pygpt_net/data/icon.png
--rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_busy.ico
--rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_error.ico
--rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_idle.ico
--rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/abc.svg
--rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/add.svg
--rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/add_circle.svg
--rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/add_folder.svg
--rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/add_library.svg
--rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/alarm.svg
--rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/apps.svg
--rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/asterisk.svg
--rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/attachment.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/attachments.svg
--rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/back.svg
--rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/backspace.svg
--rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/block.svg
--rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/bookmark.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/brush.svg
--rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/build.svg
--rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/calendar.svg
--rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/camera.svg
--rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/audio.png
--rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/copy.png
--rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/delete.png
--rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/edit.png
--rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/join.png
--rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/reload.png
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/check.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/check_circle.svg
--rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/checklist.svg
--rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/circle.svg
--rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/clear.svg
--rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/clock.svg
--rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/close.svg
--rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/close_circle.svg
--rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/code.svg
--rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/computer.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/copy.svg
--rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/crop.svg
--rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/cut.svg
--rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/db.svg
--rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/delete.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/done.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/download.svg
--rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/draft.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/drag.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/edit.svg
--rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/emergency.svg
--rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/equalizer.svg
--rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/error.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/event_available.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/expand.svg
--rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/fast_forward.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/fast_rewind.svg
--rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/favorite.svg
--rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/folder.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/folder_filled.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/forward.svg
--rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/full.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/fullscreen.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/grid.svg
--rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/hearing.svg
--rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/help.svg
--rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/history.svg
--rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/home.svg
--rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/home_filled.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/image.svg
--rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/info.svg
--rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/input.svg
--rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/key.svg
--rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/keyboard.svg
--rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/language.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/list.svg
--rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/lock.svg
--rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/logout.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/map.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/memory.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/menu.svg
--rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/mic.svg
--rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/mic_off.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/more_horizontal.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/mute.svg
--rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/open_tab.svg
--rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/palette.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/paste.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/pause.svg
--rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/pause_circle.svg
--rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/photos.svg
--rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/pin.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/play.svg
--rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/play_pause.svg
--rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/playlist_add.svg
--rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/power.svg
--rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/print.svg
--rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/public_filled.svg
--rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.7/src/pygpt_net/data/icons/redo.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/reload.svg
--rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/repeat.svg
--rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/replay.svg
--rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/resize.svg
--rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/robot.svg
--rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/router.svg
--rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/save.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/schedule.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/screenshot.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/search.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/security.svg
--rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/sensors.svg
--rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/settings.svg
--rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/settings_filled.svg
--rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/share.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/shedule.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/sort.svg
--rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/stack.svg
--rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/stacks.svg
--rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/star.svg
--rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/stop.svg
--rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/stop_circle.svg
--rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/sync.svg
--rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/tag.svg
--rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/task.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/terminal.svg
--rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/text.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/textfile.svg
--rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/timer.svg
--rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/today.svg
--rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/tune.svg
--rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/undo.svg
--rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/update.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/updater.svg
--rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/upload.svg
--rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/video.svg
--rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/view.svg
--rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/voice.svg
--rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/volume.svg
--rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/warning.svg
--rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/webcam.svg
--rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.7/src/pygpt_net/data/icons/webcam_off.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/width.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/window.svg
--rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/work.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/zoom_in.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/zoom_out.svg
--rwxr-xr-x   0        0        0    47611 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.de.ini
--rwxr-xr-x   0        0        0    55722 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.en.ini
--rwxr-xr-x   0        0        0    47738 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.es.ini
--rwxr-xr-x   0        0        0    49440 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.fr.ini
--rwxr-xr-x   0        0        0    46777 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.it.ini
--rwxr-xr-x   0        0        0    46707 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.pl.ini
--rwxr-xr-x   0        0        0    65739 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.uk.ini
--rwxr-xr-x   0        0        0    50133 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.zh.ini
--rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.agent.en.ini
--rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.agent.pl.ini
--rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_input.en.ini
--rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
--rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_output.en.ini
--rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
--rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
--rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
--rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
--rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
--rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
--rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
--rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
--rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
--rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
--rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
--rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
--rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
--rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
--rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
--rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.crontab.en.ini
--rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.crontab.pl.ini
--rw-r--r--   0        0        0       99 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.experts.en.ini
--rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
--rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
--rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
--rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
--rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
--rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
--rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
--rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
--rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.real_time.en.ini
--rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.real_time.pl.ini
--rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.7/src/pygpt_net/data/logo.png
--rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.7/src/pygpt_net/data/prompts.csv
--rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.7/src/pygpt_net/data/win32/README.rtf
--rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.7/src/pygpt_net/data/win32/USER-LICENSE.rtf
--rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.7/src/pygpt_net/data/win32/pygpt.aip
--rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.7/src/pygpt_net/data/win32/qt.conf
--rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.2.7/src/pygpt_net/icons.qrc
--rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.2.7/src/pygpt_net/icons_rc.py
--rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.7/src/pygpt_net/item/__init__.py
--rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/item/assistant.py
--rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/item/attachment.py
--rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/item/calendar_note.py
--rw-r--r--   0        0        0    12376 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/item/ctx.py
--rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/item/index.py
--rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.7/src/pygpt_net/item/mode.py
--rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/item/model.py
--rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/item/notepad.py
--rw-r--r--   0        0        0     4680 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/item/preset.py
--rwxr-xr-x   0        0        0     7995 2024-04-21 18:06:27.128064 pygpt_net-2.2.7/src/pygpt_net/launcher.py
--rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231227152900.py
--rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231230095000.py
--rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231231230000.py
--rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240106060000.py
--rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240107060000.py
--rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240222160000.py
--rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240223050000.py
--rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240303190000.py
--rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240408180000.py
--rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240426050000.py
--rw-r--r--   0        0        0     1052 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240501030000.py
--rw-r--r--   0        0        0     1974 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/migrations/__init__.py
--rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.7/src/pygpt_net/migrations/base.py
--rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.7/src/pygpt_net/plugin/__init__.py
--rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/plugin/agent/__init__.py
--rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/__init__.py
--rw-r--r--   0        0        0     4669 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/simple.py
--rwxr-xr-x   0        0        0    10466 2024-03-19 09:04:41.054930 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/worker.py
--rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_output/__init__.py
--rw-r--r--   0        0        0     1806 2024-03-10 10:31:05.897000 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_output/worker.py
--rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.7/src/pygpt_net/plugin/base.py
--rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_api/__init__.py
--rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_api/worker.py
--rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
--rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
--rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
--rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_custom/__init__.py
--rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_custom/worker.py
--rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_files/__init__.py
--rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_files/worker.py
--rwxr-xr-x   0        0        0    20404 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_history/__init__.py
--rw-r--r--   0        0        0     6768 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_history/worker.py
--rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_serial/__init__.py
--rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_serial/worker.py
--rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/__init__.py
--rwxr-xr-x   0        0        0    12772 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/websearch.py
--rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/worker.py
--rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.7/src/pygpt_net/plugin/crontab/__init__.py
--rwxr-xr-x   0        0        0     2455 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/plugin/experts/__init__.py
--rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.7/src/pygpt_net/plugin/extra_prompt/__init__.py
--rwxr-xr-x   0        0        0    14776 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/plugin/idx_llama_index/__init__.py
--rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.7/src/pygpt_net/plugin/idx_llama_index/worker.py
--rwxr-xr-x   0        0        0     6579 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/plugin/openai_dalle/__init__.py
--rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.7/src/pygpt_net/plugin/openai_vision/__init__.py
--rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.7/src/pygpt_net/plugin/real_time/__init__.py
--rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.7/src/pygpt_net/provider/__init__.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/__init__.py
--rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/base.py
--rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
--rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
--rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/google_speech_recognition.py
--rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/openai_whisper.py
--rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/openai_whisper_local.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/__init__.py
--rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/base.py
--rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/eleven_labs.py
--rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/google_tts.py
--rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/ms_azure_tts.py
--rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/openai_tts.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/__init__.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/__init__.py
--rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/base.py
--rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/json_file.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/base.py
--rw-r--r--   0        0        0     5363 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
--rw-r--r--   0        0        0    10845 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
--rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/base.py
--rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
--rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
--rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
--rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/base.py
--rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/__init__.py
--rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/base.py
--rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
--rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/config/__init__.py
--rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/config/base.py
--rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.7/src/pygpt_net/provider/core/config/json_file.py
--rwxr-xr-x   0        0        0    76707 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/config/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/__init__.py
--rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/base.py
--rw-r--r--   0        0        0     9648 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
--rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
--rw-r--r--   0        0        0    33381 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
--rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
--rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/history/__init__.py
--rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/history/base.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/history/patch.py
--rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/history/txt_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/__init__.py
--rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/base.py
--rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/patch.py
--rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/storage.py
--rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/utils.py
--rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/__init__.py
--rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/base.py
--rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/model/__init__.py
--rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/model/base.py
--rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/model/json_file.py
--rw-r--r--   0        0        0    10462 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/model/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/__init__.py
--rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/base.py
--rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
--rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
--rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/json_file.py
--rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/__init__.py
--rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/base.py
--rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/json_file.py
--rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/patch.py
--rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/__init__.py
--rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/base.py
--rwxr-xr-x   0        0        0     8307 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/json_file.py
--rw-r--r--   0        0        0     4651 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/patch.py
--rw-r--r--   0        0        0     7297 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/__init__.py
--rw-r--r--   0        0        0    13637 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/assistants.py
--rw-r--r--   0        0        0     7034 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/chat.py
--rw-r--r--   0        0        0     5876 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/completion.py
--rw-r--r--   0        0        0     8255 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/image.py
--rw-r--r--   0        0        0    16810 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/store.py
--rw-r--r--   0        0        0     2072 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/summarizer.py
--rw-r--r--   0        0        0     8266 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/vision.py
--rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/__init__.py
--rw-r--r--   0        0        0    20403 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/assistants.py
--rw-r--r--   0        0        0    15467 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/importer.py
--rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/__init__.py
--rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/anthropic.py
--rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.7/src/pygpt_net/provider/llms/azure_openai.py
--rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.7/src/pygpt_net/provider/llms/base.py
--rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/hugging_face.py
--rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/llama.py
--rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/ollama.py
--rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.7/src/pygpt_net/provider/llms/openai.py
--rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/base.py
--rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_csv.py
--rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_docx.py
--rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_epub.py
--rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_excel.py
--rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_html.py
--rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_image_vision.py
--rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_ipynb.py
--rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_json.py
--rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_markdown.py
--rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_pdf.py
--rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_video_audio.py
--rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_xml.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
--rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
--rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/database/__init__.py
--rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/database/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/issues.py
--rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/__init__.py
--rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/calendar.py
--rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/docs.py
--rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/gmail.py
--rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/keep.py
--rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/sheets.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
--rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/image_vision/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/json/__init__.py
--rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/json/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
--rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
--rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
--rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/video_audio/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
--rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/web_page/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/__init__.py
--rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/base.py
--rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/utils.py
--rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_bitbucket.py
--rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_database.py
--rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_github_issues.py
--rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_github_repo.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_calendar.py
--rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_docs.py
--rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_drive.py
--rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_gmail.py
--rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_keep.py
--rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_sheets.py
--rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
--rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_page.py
--rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_rss.py
--rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_sitemap.py
--rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_twitter.py
--rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_yt.py
--rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/__init__.py
--rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/base.py
--rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/chroma.py
--rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/elasticsearch.py
--rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/pinecode.py
--rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/redis.py
--rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/simple.py
--rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/temp.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.7/src/pygpt_net/provider/web/__init__.py
--rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/web/base.py
--rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.7/src/pygpt_net/provider/web/google_custom_search.py
--rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.7/src/pygpt_net/provider/web/microsoft_bing.py
--rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/tools/__init__.py
--rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
--rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/tools/base.py
--rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/__init__.py
--rw-r--r--   0        0        0     6622 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
--rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/widgets.py
--rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/ui/__init__.py
--rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/ui/dialogs.py
--rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/__init__.py
--rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/browse.py
--rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/ctx.py
--rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/dialogs.py
--rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/files.py
--rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/web.py
--rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/widgets.py
--rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/media_player/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/__init__.py
--rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/dialogs.py
--rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/widgets.py
--rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/__init__.py
--rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/dialogs.py
--rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/widgets.py
--rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.7/src/pygpt_net/ui/base/__init__.py
--rw-r--r--   0        0        0     9209 2024-03-11 07:32:25.337990 pygpt_net-2.2.7/src/pygpt_net/ui/base/config_dialog.py
--rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/base/context_menu.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/__init__.py
--rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/about.py
--rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/applog.py
--rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/assistant.py
--rw-r--r--   0        0        0    22532 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/assistant_store.py
--rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/changelog.py
--rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/create.py
--rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/db.py
--rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/debug.py
--rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/dictionary.py
--rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/editor.py
--rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/find.py
--rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/image.py
--rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/license.py
--rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/logger.py
--rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/models.py
--rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/plugins.py
--rwxr-xr-x   0        0        0     7391 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/preset.py
--rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/preset_plugins.py
--rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/profile.py
--rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/rename.py
--rwxr-xr-x   0        0        0    15113 2024-03-10 12:05:00.639613 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/settings.py
--rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/snap.py
--rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/start.py
--rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/update.py
--rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/workdir.py
--rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/dialogs.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/layout/__init__.py
--rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/__init__.py
--rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/attachments.py
--rwxr-xr-x   0        0        0     5280 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
--rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/calendar.py
--rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/input.py
--rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/markdown.py
--rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/output.py
--rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/painter.py
--rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/__init__.py
--rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/ctx_list.py
--rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/search_input.py
--rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/video.py
--rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.7/src/pygpt_net/ui/layout/status.py
--rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/__init__.py
--rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/agent.py
--rwxr-xr-x   0        0        0     4436 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/assistants.py
--rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/footer.py
--rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/image.py
--rw-r--r--   0        0        0     7007 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/indexes.py
--rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/mode.py
--rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/model.py
--rwxr-xr-x   0        0        0     5109 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/presets.py
--rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/prompt.py
--rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/vision.py
--rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.7/src/pygpt_net/ui/main.py
--rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/menu/__init__.py
--rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/ui/menu/about.py
--rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.7/src/pygpt_net/ui/menu/audio.py
--rw-r--r--   0        0        0     7870 2024-04-21 01:33:54.247764 pygpt_net-2.2.7/src/pygpt_net/ui/menu/config.py
--rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/menu/debug.py
--rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.7/src/pygpt_net/ui/menu/file.py
--rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/ui/menu/lang.py
--rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/menu/plugins.py
--rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.7/src/pygpt_net/ui/menu/theme.py
--rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/menu/tools.py
--rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.7/src/pygpt_net/ui/menu/video.py
--rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.7/src/pygpt_net/ui/tray.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.7/src/pygpt_net/ui/widget/__init__.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/__init__.py
--rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/input.py
--rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/input_button.py
--rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/output.py
--rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.7/src/pygpt_net/ui/widget/calendar/__init__.py
--rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.7/src/pygpt_net/ui/widget/calendar/select.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/__init__.py
--rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/alert.py
--rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/applog.py
--rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/assistant_store.py
--rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/audio.py
--rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/base.py
--rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/confirm.py
--rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/create.py
--rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/db.py
--rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/debug.py
--rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/editor.py
--rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/editor_file.py
--rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/find.py
--rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/image.py
--rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/info.py
--rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/license.py
--rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/logger.py
--rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/model.py
--rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/preset_plugins.py
--rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/profile.py
--rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/rename.py
--rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/settings.py
--rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/settings_plugin.py
--rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/snap.py
--rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/update.py
--rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/workdir.py
--rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.7/src/pygpt_net/ui/widget/draw/__init__.py
--rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.7/src/pygpt_net/ui/widget/draw/painter.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/__init__.py
--rw-r--r--   0        0        0     4173 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/button.py
--rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/checkbox.py
--rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/group.py
--rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/labels.py
--rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/filesystem/__init__.py
--rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/filesystem/explorer.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/image/__init__.py
--rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/widget/image/display.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/__init__.py
--rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/assistant.py
--rw-r--r--   0        0        0     3715 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/assistant_store.py
--rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/attachment.py
--rwxr-xr-x   0        0        0     2435 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/base.py
--rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/context.py
--rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/db.py
--rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/debug.py
--rw-r--r--   0        0        0     5739 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/experts.py
--rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/index.py
--rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/index_combo.py
--rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/mode.py
--rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/model.py
--rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/model_editor.py
--rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/plugin.py
--rwxr-xr-x   0        0        0     5655 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/preset.py
--rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/preset_plugins.py
--rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/profile.py
--rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/settings.py
--rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/uploaded.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/__init__.py
--rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/checkbox.py
--rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/cmd.py
--rw-r--r--   0        0        0     3592 2024-04-27 10:44:46.049374 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/combo.py
--rwxr-xr-x   0        0        0    12672 2024-03-11 03:15:21.879593 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/dictionary.py
--rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/input.py
--rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/prompt.py
--rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/slider.py
--rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/textarea.py
--rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/Input.py
--rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/__init__.py
--rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/output.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/__init__.py
--rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/calendar_note.py
--rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/create.py
--rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/editor.py
--rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/find.py
--rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/input.py
--rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/name.py
--rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/notepad.py
--rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/output.py
--rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/rename.py
--rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/search_input.py
--rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/web.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/vision/__init__.py
--rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/vision/camera.py
--rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/utils.py
--rw-r--r--   0        0        0   139995 1970-01-01 00:00:00.000000 pygpt_net-2.2.7/PKG-INFO
+-rwxr-xr-x   0        0        0    59583 2024-05-02 17:16:19.056982 pygpt_net-2.2.8/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.8/LICENSE
+-rwxr-xr-x   0        0        0   139884 2024-05-02 17:15:54.645157 pygpt_net-2.2.8/README.md
+-rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.8/icon.png
+-rw-r--r--   0        0        0     2979 2024-05-02 17:16:47.776781 pygpt_net-2.2.8/pyproject.toml
+-rwxr-xr-x   0        0        0    58551 2024-05-02 17:16:17.700991 pygpt_net-2.2.8/src/pygpt_net/CHANGELOG.txt
+-rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.8/src/pygpt_net/LICENSE
+-rwxr-xr-x   0        0        0     1024 2024-05-02 17:18:08.492251 pygpt_net-2.2.8/src/pygpt_net/__init__.py
+-rwxr-xr-x   0        0        0    14447 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/app.py
+-rwxr-xr-x   0        0        0    15485 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/config.py
+-rwxr-xr-x   0        0        0     3839 2024-05-02 17:09:01.677147 pygpt_net-2.2.8/src/pygpt_net/container.py
+-rwxr-xr-x   0        0        0     5333 2024-05-02 17:09:01.681147 pygpt_net-2.2.8/src/pygpt_net/controller/__init__.py
+-rwxr-xr-x   0        0        0     2209 2024-05-02 18:21:41.000000 pygpt_net-2.2.8/src/pygpt_net/controller/access/__init__.py
+-rwxr-xr-x   0        0        0     9179 2024-05-02 17:49:27.000000 pygpt_net-2.2.8/src/pygpt_net/controller/access/control.py
+-rwxr-xr-x   0        0        0    11692 2024-05-02 18:21:41.000000 pygpt_net-2.2.8/src/pygpt_net/controller/access/voice.py
+-rw-r--r--   0        0        0     3823 2024-05-02 17:09:01.877145 pygpt_net-2.2.8/src/pygpt_net/controller/agent/__init__.py
+-rw-r--r--   0        0        0     1748 2024-05-02 17:09:01.797146 pygpt_net-2.2.8/src/pygpt_net/controller/agent/common.py
+-rw-r--r--   0        0        0     1407 2024-05-02 17:09:01.761146 pygpt_net-2.2.8/src/pygpt_net/controller/agent/experts.py
+-rw-r--r--   0        0        0     6904 2024-05-02 17:09:01.801146 pygpt_net-2.2.8/src/pygpt_net/controller/agent/flow.py
+-rw-r--r--   0        0        0     9877 2024-04-29 15:13:32.571516 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/__init__.py
+-rw-r--r--   0        0        0    20310 2024-04-30 16:41:29.971889 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/batch.py
+-rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/editor.py
+-rw-r--r--   0        0        0    14434 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/files.py
+-rwxr-xr-x   0        0        0    15545 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/store.py
+-rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/threads.py
+-rwxr-xr-x   0        0        0    15661 2024-05-02 17:49:27.617904 pygpt_net-2.2.8/src/pygpt_net/controller/attachment.py
+-rw-r--r--   0        0        0     6560 2024-05-02 17:09:01.665147 pygpt_net-2.2.8/src/pygpt_net/controller/audio/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.8/src/pygpt_net/controller/calendar/__init__.py
+-rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/controller/calendar/note.py
+-rwxr-xr-x   0        0        0    13013 2024-05-02 17:09:01.793146 pygpt_net-2.2.8/src/pygpt_net/controller/camera.py
+-rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.8/src/pygpt_net/controller/chat/__init__.py
+-rwxr-xr-x   0        0        0    11749 2024-05-02 17:09:01.809146 pygpt_net-2.2.8/src/pygpt_net/controller/chat/common.py
+-rw-r--r--   0        0        0     2156 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/chat/files.py
+-rwxr-xr-x   0        0        0     6533 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/chat/image.py
+-rwxr-xr-x   0        0        0    10650 2024-05-02 17:09:01.713147 pygpt_net-2.2.8/src/pygpt_net/controller/chat/input.py
+-rwxr-xr-x   0        0        0    11366 2024-05-02 17:09:01.693147 pygpt_net-2.2.8/src/pygpt_net/controller/chat/output.py
+-rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.8/src/pygpt_net/controller/chat/render.py
+-rw-r--r--   0        0        0    13022 2024-05-02 17:09:01.757146 pygpt_net-2.2.8/src/pygpt_net/controller/chat/text.py
+-rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.8/src/pygpt_net/controller/chat/vision.py
+-rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.8/src/pygpt_net/controller/command.py
+-rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.8/src/pygpt_net/controller/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/__init__.py
+-rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/checkbox.py
+-rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/cmd.py
+-rw-r--r--   0        0        0     3237 2024-05-02 10:44:22.869251 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/combo.py
+-rw-r--r--   0        0        0     6657 2024-05-02 14:53:21.198368 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/dictionary.py
+-rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/input.py
+-rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/slider.py
+-rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/textarea.py
+-rw-r--r--   0        0        0     8222 2024-05-02 17:09:01.869145 pygpt_net-2.2.8/src/pygpt_net/controller/config/placeholder.py
+-rw-r--r--   0        0        0    30255 2024-05-02 17:09:01.845145 pygpt_net-2.2.8/src/pygpt_net/controller/ctx/__init__.py
+-rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.8/src/pygpt_net/controller/ctx/common.py
+-rwxr-xr-x   0        0        0     7529 2024-05-02 17:54:44.930189 pygpt_net-2.2.8/src/pygpt_net/controller/ctx/extra.py
+-rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.8/src/pygpt_net/controller/ctx/summarizer.py
+-rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/debug/__init__.py
+-rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/__init__.py
+-rwxr-xr-x   0        0        0    13546 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/confirm.py
+-rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/debug.py
+-rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/info.py
+-rwxr-xr-x   0        0        0    15699 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/files.py
+-rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.8/src/pygpt_net/controller/finder.py
+-rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/idx/__init__.py
+-rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.8/src/pygpt_net/controller/idx/common.py
+-rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.8/src/pygpt_net/controller/idx/indexer.py
+-rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.8/src/pygpt_net/controller/idx/settings.py
+-rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/lang/__init__.py
+-rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/controller/lang/custom.py
+-rw-r--r--   0        0        0    20280 2024-05-02 17:09:01.729147 pygpt_net-2.2.8/src/pygpt_net/controller/lang/mapping.py
+-rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.8/src/pygpt_net/controller/lang/plugins.py
+-rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.8/src/pygpt_net/controller/lang/settings.py
+-rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.8/src/pygpt_net/controller/launcher.py
+-rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/layout.py
+-rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/mode.py
+-rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.8/src/pygpt_net/controller/model/__init__.py
+-rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.8/src/pygpt_net/controller/model/editor.py
+-rwxr-xr-x   0        0        0    13052 2024-05-02 17:09:01.821145 pygpt_net-2.2.8/src/pygpt_net/controller/notepad.py
+-rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/painter/__init__.py
+-rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.8/src/pygpt_net/controller/painter/capture.py
+-rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.8/src/pygpt_net/controller/painter/common.py
+-rw-r--r--   0        0        0    13977 2024-05-02 17:09:01.753146 pygpt_net-2.2.8/src/pygpt_net/controller/plugins/__init__.py
+-rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.8/src/pygpt_net/controller/plugins/presets.py
+-rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.8/src/pygpt_net/controller/plugins/settings.py
+-rwxr-xr-x   0        0        0    17127 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/presets/__init__.py
+-rwxr-xr-x   0        0        0    16058 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/presets/editor.py
+-rw-r--r--   0        0        0     4937 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/presets/experts.py
+-rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/settings/__init__.py
+-rwxr-xr-x   0        0        0    15241 2024-05-02 17:09:01.841145 pygpt_net-2.2.8/src/pygpt_net/controller/settings/editor.py
+-rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/settings/profile.py
+-rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.8/src/pygpt_net/controller/settings/workdir.py
+-rwxr-xr-x   0        0        0     6308 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/theme/__init__.py
+-rwxr-xr-x   0        0        0     5437 2024-04-30 16:41:29.975888 pygpt_net-2.2.8/src/pygpt_net/controller/theme/common.py
+-rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/controller/theme/markdown.py
+-rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.8/src/pygpt_net/controller/theme/menu.py
+-rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/controller/theme/nodes.py
+-rw-r--r--   0        0        0     6934 2024-05-02 17:09:01.849145 pygpt_net-2.2.8/src/pygpt_net/controller/ui/__init__.py
+-rw-r--r--   0        0        0     6663 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/ui/mode.py
+-rw-r--r--   0        0        0     2378 2024-04-30 16:41:29.975888 pygpt_net-2.2.8/src/pygpt_net/controller/ui/vision.py
+-rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.8/src/pygpt_net/core/__init__.py
+-rw-r--r--   0        0        0      874 2024-05-02 17:09:01.865145 pygpt_net-2.2.8/src/pygpt_net/core/access/__init__.py
+-rw-r--r--   0        0        0     2351 2024-05-02 17:09:01.709147 pygpt_net-2.2.8/src/pygpt_net/core/access/actions.py
+-rwxr-xr-x   0        0        0     2902 2024-05-02 18:17:27.000000 pygpt_net-2.2.8/src/pygpt_net/core/access/events.py
+-rw-r--r--   0        0        0     3397 2024-05-02 17:09:01.749146 pygpt_net-2.2.8/src/pygpt_net/core/access/shortcuts.py
+-rw-r--r--   0        0        0    10590 2024-05-02 17:43:40.444809 pygpt_net-2.2.8/src/pygpt_net/core/access/voice.py
+-rw-r--r--   0        0        0     1382 2024-05-02 17:09:01.653148 pygpt_net-2.2.8/src/pygpt_net/core/agents/__init__.py
+-rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.8/src/pygpt_net/core/assistants/__init__.py
+-rw-r--r--   0        0        0     9796 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/core/assistants/files.py
+-rw-r--r--   0        0        0     7990 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/core/assistants/store.py
+-rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.8/src/pygpt_net/core/attachments.py
+-rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.8/src/pygpt_net/core/audio.py
+-rw-r--r--   0        0        0     7483 2024-05-02 17:09:01.725147 pygpt_net-2.2.8/src/pygpt_net/core/bridge.py
+-rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/core/calendar/__init__.py
+-rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.8/src/pygpt_net/core/camera.py
+-rw-r--r--   0        0        0     3330 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/core/chain/__init__.py
+-rw-r--r--   0        0        0     4988 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/core/chain/chat.py
+-rw-r--r--   0        0        0     5413 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/core/chain/completion.py
+-rwxr-xr-x   0        0        0    10538 2024-05-02 17:09:01.861145 pygpt_net-2.2.8/src/pygpt_net/core/command.py
+-rwxr-xr-x   0        0        0    35701 2024-05-02 17:09:01.661147 pygpt_net-2.2.8/src/pygpt_net/core/ctx/__init__.py
+-rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.8/src/pygpt_net/core/ctx/idx.py
+-rw-r--r--   0        0        0    15975 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/db/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.8/src/pygpt_net/core/db/viewer.py
+-rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.8/src/pygpt_net/core/debug/__init__.py
+-rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.8/src/pygpt_net/core/debug/agent.py
+-rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.8/src/pygpt_net/core/debug/assistants.py
+-rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/attachments.py
+-rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.8/src/pygpt_net/core/debug/config.py
+-rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.8/src/pygpt_net/core/debug/context.py
+-rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.8/src/pygpt_net/core/debug/db.py
+-rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/core/debug/indexes.py
+-rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/models.py
+-rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/plugins.py
+-rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/presets.py
+-rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/ui.py
+-rwxr-xr-x   0        0        0    10010 2024-05-02 17:09:01.741146 pygpt_net-2.2.8/src/pygpt_net/core/dispatcher.py
+-rw-r--r--   0        0        0    10014 2024-05-02 17:09:01.669147 pygpt_net-2.2.8/src/pygpt_net/core/experts/__init__.py
+-rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/__init__.py
+-rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/actions.py
+-rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/editor.py
+-rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/types.py
+-rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/url.py
+-rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/core/history.py
+-rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.8/src/pygpt_net/core/idx/__init__.py
+-rwxr-xr-x   0        0        0    13030 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/idx/chat.py
+-rw-r--r--   0        0        0     2443 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/idx/context.py
+-rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.8/src/pygpt_net/core/idx/indexing.py
+-rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.8/src/pygpt_net/core/idx/llm.py
+-rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.8/src/pygpt_net/core/idx/metadata.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.8/src/pygpt_net/core/idx/types/__init__.py
+-rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.8/src/pygpt_net/core/idx/types/ctx.py
+-rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.8/src/pygpt_net/core/idx/types/external.py
+-rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/core/idx/types/files.py
+-rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.8/src/pygpt_net/core/idx/worker.py
+-rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.8/src/pygpt_net/core/image.py
+-rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.8/src/pygpt_net/core/info.py
+-rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.8/src/pygpt_net/core/installer.py
+-rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.8/src/pygpt_net/core/llm/__init__.py
+-rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.8/src/pygpt_net/core/locale.py
+-rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/core/models.py
+-rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/core/modes.py
+-rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.8/src/pygpt_net/core/notepad.py
+-rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/core/platforms.py
+-rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.8/src/pygpt_net/core/plugins.py
+-rw-r--r--   0        0        0    12366 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/presets.py
+-rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.8/src/pygpt_net/core/profile.py
+-rw-r--r--   0        0        0     4529 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/prompt/__init__.py
+-rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.8/src/pygpt_net/core/prompt/template.py
+-rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.8/src/pygpt_net/core/render/__init__.py
+-rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/core/render/base.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/__init__.py
+-rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/parser.py
+-rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/renderer.py
+-rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.8/src/pygpt_net/core/render/plain/__init__.py
+-rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/render/plain/renderer.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.8/src/pygpt_net/core/render/web/__init__.py
+-rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.8/src/pygpt_net/core/render/web/parser.py
+-rwxr-xr-x   0        0        0    43236 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/render/web/renderer.py
+-rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/text/__init__.py
+-rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/text/finder.py
+-rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/core/text/utils.py
+-rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/text/web_finder.py
+-rwxr-xr-x   0        0        0    14472 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/tokens.py
+-rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.8/src/pygpt_net/core/updater/__init__.py
+-rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.8/src/pygpt_net/core/web.py
+-rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.8/src/pygpt_net/core/worker.py
+-rw-r--r--   0        0        0    65201 2024-05-02 09:05:10.390389 pygpt_net-2.2.8/src/pygpt_net/data/audio/click_off.mp3
+-rw-r--r--   0        0        0    65201 2024-05-02 09:04:45.466493 pygpt_net-2.2.8/src/pygpt_net/data/audio/click_on.mp3
+-rw-r--r--   0        0        0    32256 2024-05-02 12:19:15.320423 pygpt_net-2.2.8/src/pygpt_net/data/audio/ok.mp3
+-rwxr-xr-x   0        0        0    15381 2024-05-02 17:23:01.538643 pygpt_net-2.2.8/src/pygpt_net/data/config/config.json
+-rwxr-xr-x   0        0        0    20573 2024-05-02 17:17:50.696364 pygpt_net-2.2.8/src/pygpt_net/data/config/models.json
+-rw-r--r--   0        0        0     1595 2024-05-02 17:17:45.868395 pygpt_net-2.2.8/src/pygpt_net/data/config/modes.json
+-rwxr-xr-x   0        0        0      528 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.agent.json
+-rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.assistant.json
+-rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.chat.json
+-rwxr-xr-x   0        0        0      436 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.completion.json
+-rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.expert.json
+-rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.img.json
+-rwxr-xr-x   0        0        0      433 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.langchain.json
+-rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.llama_index.json
+-rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.vision.json
+-rwxr-xr-x   0        0        0      552 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/dalle_white_cat.json
+-rw-r--r--   0        0        0      474 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/joke_agent.json
+-rw-r--r--   0        0        0      683 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/joke_expert.json
+-rwxr-xr-x   0        0        0    36092 2024-05-02 16:55:04.321108 pygpt_net-2.2.8/src/pygpt_net/data/config/settings.json
+-rw-r--r--   0        0        0      870 2024-05-02 06:04:41.700908 pygpt_net-2.2.8/src/pygpt_net/data/config/settings_section.json
+-rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/fix_windows.css
+-rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.css
+-rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.dark.css
+-rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.light.css
+-rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/style.css
+-rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/data/css/style.dark.css
+-rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/style.light.css
+-rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/data/css/web.css
+-rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.8/src/pygpt_net/data/css/web.dark.css
+-rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.8/src/pygpt_net/data/css/web.light.css
+-rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
+-rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
+-rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
+-rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
+-rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
+-rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
+-rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
+-rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
+-rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
+-rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
+-rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/OFL.txt
+-rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
+-rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
+-rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
+-rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
+-rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
+-rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
+-rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
+-rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
+-rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
+-rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
+-rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
+-rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
+-rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
+-rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
+-rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
+-rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
+-rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
+-rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
+-rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
+-rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
+-rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
+-rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
+-rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
+-rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
+-rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
+-rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.8/src/pygpt_net/data/icon.ico
+-rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.8/src/pygpt_net/data/icon.png
+-rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_busy.ico
+-rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_error.ico
+-rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_idle.ico
+-rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/abc.svg
+-rw-r--r--   0        0        0      360 2024-05-02 14:44:36.720121 pygpt_net-2.2.8/src/pygpt_net/data/icons/accessibility.svg
+-rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/add.svg
+-rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/add_circle.svg
+-rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/add_folder.svg
+-rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/add_library.svg
+-rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/alarm.svg
+-rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/apps.svg
+-rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/asterisk.svg
+-rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/attachment.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/attachments.svg
+-rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/back.svg
+-rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/backspace.svg
+-rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/block.svg
+-rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/bookmark.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/brush.svg
+-rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/build.svg
+-rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/calendar.svg
+-rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/camera.svg
+-rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/audio.png
+-rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/copy.png
+-rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/delete.png
+-rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/edit.png
+-rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/join.png
+-rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/reload.png
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/check.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/check_circle.svg
+-rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/checklist.svg
+-rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/circle.svg
+-rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/clear.svg
+-rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/clock.svg
+-rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/close.svg
+-rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/close_circle.svg
+-rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/code.svg
+-rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/computer.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/copy.svg
+-rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/crop.svg
+-rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/cut.svg
+-rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/db.svg
+-rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/delete.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/done.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/download.svg
+-rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/draft.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/drag.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/edit.svg
+-rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/emergency.svg
+-rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/equalizer.svg
+-rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/error.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/event_available.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/expand.svg
+-rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/fast_forward.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/fast_rewind.svg
+-rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/favorite.svg
+-rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/folder.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/folder_filled.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/forward.svg
+-rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/full.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/fullscreen.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/grid.svg
+-rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/hearing.svg
+-rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/help.svg
+-rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/history.svg
+-rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/home.svg
+-rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/home_filled.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/image.svg
+-rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/info.svg
+-rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/input.svg
+-rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/key.svg
+-rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/keyboard.svg
+-rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/language.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/list.svg
+-rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/lock.svg
+-rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/logout.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/map.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/memory.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/menu.svg
+-rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/mic.svg
+-rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/mic_off.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/more_horizontal.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/mute.svg
+-rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/open_tab.svg
+-rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/palette.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/paste.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/pause.svg
+-rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/pause_circle.svg
+-rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/photos.svg
+-rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/pin.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/play.svg
+-rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/play_pause.svg
+-rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/playlist_add.svg
+-rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/power.svg
+-rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/print.svg
+-rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/public_filled.svg
+-rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.8/src/pygpt_net/data/icons/redo.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/reload.svg
+-rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/repeat.svg
+-rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/replay.svg
+-rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/resize.svg
+-rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/robot.svg
+-rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/router.svg
+-rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/save.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/schedule.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/screenshot.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/search.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/security.svg
+-rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/sensors.svg
+-rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/settings.svg
+-rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/settings_filled.svg
+-rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/share.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/shedule.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/sort.svg
+-rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/stack.svg
+-rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/stacks.svg
+-rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/star.svg
+-rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/stop.svg
+-rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/stop_circle.svg
+-rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/sync.svg
+-rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/tag.svg
+-rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/task.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/terminal.svg
+-rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/text.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/textfile.svg
+-rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/timer.svg
+-rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/today.svg
+-rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/tune.svg
+-rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/undo.svg
+-rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/update.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/updater.svg
+-rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/upload.svg
+-rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/video.svg
+-rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/view.svg
+-rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/voice.svg
+-rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/volume.svg
+-rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/warning.svg
+-rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/webcam.svg
+-rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.8/src/pygpt_net/data/icons/webcam_off.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/width.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/window.svg
+-rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/work.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/zoom_in.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/zoom_out.svg
+-rwxr-xr-x   0        0        0    52116 2024-05-02 17:53:00.806146 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.de.ini
+-rwxr-xr-x   0        0        0    59899 2024-05-02 17:51:12.166053 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.en.ini
+-rwxr-xr-x   0        0        0    52304 2024-05-02 17:53:33.870164 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.es.ini
+-rwxr-xr-x   0        0        0    54105 2024-05-02 17:53:10.970152 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.fr.ini
+-rwxr-xr-x   0        0        0    51291 2024-05-02 17:53:22.782159 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.it.ini
+-rwxr-xr-x   0        0        0    51375 2024-05-02 17:52:46.058137 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.pl.ini
+-rwxr-xr-x   0        0        0    71739 2024-05-02 17:39:36.711163 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.uk.ini
+-rwxr-xr-x   0        0        0    54448 2024-05-02 17:53:45.590170 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.zh.ini
+-rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.agent.en.ini
+-rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.agent.pl.ini
+-rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_input.en.ini
+-rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
+-rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_output.en.ini
+-rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
+-rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
+-rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
+-rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
+-rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
+-rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
+-rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
+-rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
+-rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
+-rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
+-rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
+-rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
+-rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
+-rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
+-rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
+-rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.crontab.en.ini
+-rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.crontab.pl.ini
+-rw-r--r--   0        0        0       99 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.experts.en.ini
+-rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
+-rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
+-rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
+-rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
+-rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
+-rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
+-rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
+-rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
+-rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.real_time.en.ini
+-rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.real_time.pl.ini
+-rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.8/src/pygpt_net/data/logo.png
+-rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.8/src/pygpt_net/data/prompts.csv
+-rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.8/src/pygpt_net/data/win32/README.rtf
+-rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.8/src/pygpt_net/data/win32/USER-LICENSE.rtf
+-rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.8/src/pygpt_net/data/win32/pygpt.aip
+-rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.8/src/pygpt_net/data/win32/qt.conf
+-rw-r--r--   0        0        0    21910 2024-05-02 14:46:17.971808 pygpt_net-2.2.8/src/pygpt_net/icons.qrc
+-rw-r--r--   0        0        0    91076 2024-05-02 14:46:18.099807 pygpt_net-2.2.8/src/pygpt_net/icons_rc.py
+-rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.8/src/pygpt_net/item/__init__.py
+-rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/item/assistant.py
+-rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/item/attachment.py
+-rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/item/calendar_note.py
+-rw-r--r--   0        0        0    12376 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/item/ctx.py
+-rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/item/index.py
+-rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.8/src/pygpt_net/item/mode.py
+-rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/item/model.py
+-rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/item/notepad.py
+-rw-r--r--   0        0        0     4680 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/item/preset.py
+-rwxr-xr-x   0        0        0     8362 2024-05-02 17:09:01.717147 pygpt_net-2.2.8/src/pygpt_net/launcher.py
+-rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231227152900.py
+-rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231230095000.py
+-rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231231230000.py
+-rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240106060000.py
+-rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240107060000.py
+-rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240222160000.py
+-rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240223050000.py
+-rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240303190000.py
+-rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240408180000.py
+-rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240426050000.py
+-rw-r--r--   0        0        0     1052 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240501030000.py
+-rw-r--r--   0        0        0     1974 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/migrations/__init__.py
+-rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.8/src/pygpt_net/migrations/base.py
+-rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.8/src/pygpt_net/plugin/__init__.py
+-rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/plugin/agent/__init__.py
+-rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/__init__.py
+-rw-r--r--   0        0        0     4929 2024-05-02 17:09:01.813145 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/simple.py
+-rwxr-xr-x   0        0        0    11433 2024-05-02 17:09:01.781146 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/worker.py
+-rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_output/__init__.py
+-rw-r--r--   0        0        0     2340 2024-05-02 17:09:01.785146 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_output/worker.py
+-rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.8/src/pygpt_net/plugin/base.py
+-rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_api/__init__.py
+-rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_api/worker.py
+-rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
+-rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
+-rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_custom/__init__.py
+-rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_custom/worker.py
+-rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_files/__init__.py
+-rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_files/worker.py
+-rwxr-xr-x   0        0        0    20404 2024-04-30 16:41:29.975888 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_history/__init__.py
+-rw-r--r--   0        0        0     6768 2024-04-30 16:41:29.975888 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_history/worker.py
+-rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_serial/__init__.py
+-rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_serial/worker.py
+-rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/__init__.py
+-rwxr-xr-x   0        0        0    12772 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/websearch.py
+-rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/worker.py
+-rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.8/src/pygpt_net/plugin/crontab/__init__.py
+-rwxr-xr-x   0        0        0     2475 2024-05-02 17:09:01.789146 pygpt_net-2.2.8/src/pygpt_net/plugin/experts/__init__.py
+-rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.8/src/pygpt_net/plugin/extra_prompt/__init__.py
+-rwxr-xr-x   0        0        0    14776 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/plugin/idx_llama_index/__init__.py
+-rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.8/src/pygpt_net/plugin/idx_llama_index/worker.py
+-rwxr-xr-x   0        0        0     6579 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/plugin/openai_dalle/__init__.py
+-rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.8/src/pygpt_net/plugin/openai_vision/__init__.py
+-rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.8/src/pygpt_net/plugin/real_time/__init__.py
+-rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.8/src/pygpt_net/provider/__init__.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/__init__.py
+-rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/base.py
+-rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
+-rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
+-rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/google_speech_recognition.py
+-rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/openai_whisper.py
+-rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/openai_whisper_local.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/__init__.py
+-rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/base.py
+-rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/eleven_labs.py
+-rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/google_tts.py
+-rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/ms_azure_tts.py
+-rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/openai_tts.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/__init__.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/__init__.py
+-rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/base.py
+-rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/json_file.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/base.py
+-rw-r--r--   0        0        0     5363 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
+-rw-r--r--   0        0        0    10845 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
+-rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/base.py
+-rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
+-rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
+-rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/__init__.py
+-rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/base.py
+-rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/__init__.py
+-rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/base.py
+-rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
+-rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/config/__init__.py
+-rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/config/base.py
+-rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.8/src/pygpt_net/provider/core/config/json_file.py
+-rwxr-xr-x   0        0        0    78799 2024-05-02 17:22:33.110782 pygpt_net-2.2.8/src/pygpt_net/provider/core/config/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/__init__.py
+-rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/base.py
+-rw-r--r--   0        0        0     9815 2024-05-02 17:09:01.689147 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
+-rw-r--r--   0        0        0    33830 2024-05-02 17:09:01.873145 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
+-rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/history/__init__.py
+-rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/history/base.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/history/patch.py
+-rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/history/txt_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/__init__.py
+-rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/base.py
+-rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/patch.py
+-rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/storage.py
+-rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/utils.py
+-rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/__init__.py
+-rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/base.py
+-rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/model/__init__.py
+-rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/model/base.py
+-rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/model/json_file.py
+-rw-r--r--   0        0        0    10462 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/core/model/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/__init__.py
+-rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/base.py
+-rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/json_file.py
+-rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/__init__.py
+-rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/base.py
+-rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/json_file.py
+-rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/patch.py
+-rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/__init__.py
+-rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/base.py
+-rwxr-xr-x   0        0        0     8307 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/json_file.py
+-rw-r--r--   0        0        0     4651 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/patch.py
+-rw-r--r--   0        0        0     7410 2024-05-02 17:43:40.452809 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/__init__.py
+-rw-r--r--   0        0        0    13637 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/assistants.py
+-rw-r--r--   0        0        0     7034 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/chat.py
+-rw-r--r--   0        0        0     5876 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/completion.py
+-rw-r--r--   0        0        0     8255 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/image.py
+-rw-r--r--   0        0        0    16810 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/store.py
+-rw-r--r--   0        0        0     2072 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/summarizer.py
+-rw-r--r--   0        0        0     8266 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/vision.py
+-rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/__init__.py
+-rw-r--r--   0        0        0    20403 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/assistants.py
+-rw-r--r--   0        0        0    15467 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/importer.py
+-rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/__init__.py
+-rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/anthropic.py
+-rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.8/src/pygpt_net/provider/llms/azure_openai.py
+-rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.8/src/pygpt_net/provider/llms/base.py
+-rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/hugging_face.py
+-rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/llama.py
+-rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/ollama.py
+-rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.8/src/pygpt_net/provider/llms/openai.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/base.py
+-rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_csv.py
+-rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_docx.py
+-rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_epub.py
+-rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_excel.py
+-rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_html.py
+-rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_image_vision.py
+-rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_ipynb.py
+-rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_json.py
+-rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_markdown.py
+-rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_pdf.py
+-rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_video_audio.py
+-rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_xml.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
+-rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
+-rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/database/__init__.py
+-rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/database/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/__init__.py
+-rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/issues.py
+-rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/__init__.py
+-rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/calendar.py
+-rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/docs.py
+-rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/gmail.py
+-rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/keep.py
+-rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/sheets.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
+-rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/image_vision/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/json/__init__.py
+-rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/json/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
+-rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/video_audio/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
+-rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/web_page/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/__init__.py
+-rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/base.py
+-rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/utils.py
+-rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_bitbucket.py
+-rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_database.py
+-rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_github_issues.py
+-rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_github_repo.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_calendar.py
+-rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_docs.py
+-rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_drive.py
+-rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_gmail.py
+-rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_keep.py
+-rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_sheets.py
+-rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
+-rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_page.py
+-rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_rss.py
+-rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_sitemap.py
+-rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_twitter.py
+-rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_yt.py
+-rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/__init__.py
+-rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/base.py
+-rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/chroma.py
+-rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/elasticsearch.py
+-rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/pinecode.py
+-rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/redis.py
+-rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/simple.py
+-rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/temp.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.8/src/pygpt_net/provider/web/__init__.py
+-rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/web/base.py
+-rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.8/src/pygpt_net/provider/web/google_custom_search.py
+-rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.8/src/pygpt_net/provider/web/microsoft_bing.py
+-rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/tools/__init__.py
+-rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
+-rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
+-rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/tools/base.py
+-rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/__init__.py
+-rw-r--r--   0        0        0     6622 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
+-rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/widgets.py
+-rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/ui/__init__.py
+-rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/ui/dialogs.py
+-rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/__init__.py
+-rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/browse.py
+-rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/ctx.py
+-rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/dialogs.py
+-rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/files.py
+-rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/web.py
+-rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/widgets.py
+-rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/media_player/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/__init__.py
+-rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/dialogs.py
+-rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/widgets.py
+-rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/__init__.py
+-rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/dialogs.py
+-rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/widgets.py
+-rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.8/src/pygpt_net/ui/base/__init__.py
+-rw-r--r--   0        0        0     9255 2024-05-02 17:09:01.777146 pygpt_net-2.2.8/src/pygpt_net/ui/base/config_dialog.py
+-rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/base/context_menu.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/__init__.py
+-rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/about.py
+-rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/applog.py
+-rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/assistant.py
+-rw-r--r--   0        0        0    22532 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/assistant_store.py
+-rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/changelog.py
+-rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/create.py
+-rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/db.py
+-rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/debug.py
+-rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/dictionary.py
+-rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/editor.py
+-rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/find.py
+-rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/image.py
+-rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/license.py
+-rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/logger.py
+-rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/models.py
+-rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/plugins.py
+-rwxr-xr-x   0        0        0     7391 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/preset.py
+-rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/profile.py
+-rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/rename.py
+-rwxr-xr-x   0        0        0    15114 2024-05-02 17:09:01.773146 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/settings.py
+-rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/snap.py
+-rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/start.py
+-rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/update.py
+-rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/workdir.py
+-rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/dialogs.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/layout/__init__.py
+-rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/__init__.py
+-rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/attachments.py
+-rwxr-xr-x   0        0        0     5280 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
+-rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/calendar.py
+-rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/input.py
+-rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/markdown.py
+-rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/output.py
+-rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/painter.py
+-rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/__init__.py
+-rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/ctx_list.py
+-rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/search_input.py
+-rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/video.py
+-rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.8/src/pygpt_net/ui/layout/status.py
+-rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/__init__.py
+-rw-r--r--   0        0        0     2385 2024-05-02 17:09:01.701147 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/agent.py
+-rwxr-xr-x   0        0        0     4436 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/assistants.py
+-rwxr-xr-x   0        0        0     4555 2024-05-02 17:09:01.697147 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/footer.py
+-rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/image.py
+-rw-r--r--   0        0        0     7007 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/indexes.py
+-rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/mode.py
+-rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/model.py
+-rwxr-xr-x   0        0        0     5109 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/presets.py
+-rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/prompt.py
+-rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/vision.py
+-rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.8/src/pygpt_net/ui/main.py
+-rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/menu/__init__.py
+-rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/ui/menu/about.py
+-rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.8/src/pygpt_net/ui/menu/audio.py
+-rw-r--r--   0        0        0     8291 2024-05-02 17:09:01.769146 pygpt_net-2.2.8/src/pygpt_net/ui/menu/config.py
+-rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/menu/debug.py
+-rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.8/src/pygpt_net/ui/menu/file.py
+-rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/ui/menu/lang.py
+-rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/menu/plugins.py
+-rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.8/src/pygpt_net/ui/menu/theme.py
+-rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/menu/tools.py
+-rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.8/src/pygpt_net/ui/menu/video.py
+-rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.8/src/pygpt_net/ui/tray.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.8/src/pygpt_net/ui/widget/__init__.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/__init__.py
+-rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/input.py
+-rw-r--r--   0        0        0     3771 2024-05-02 17:09:01.685147 pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/input_button.py
+-rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/output.py
+-rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.8/src/pygpt_net/ui/widget/calendar/__init__.py
+-rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.8/src/pygpt_net/ui/widget/calendar/select.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/__init__.py
+-rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/alert.py
+-rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/applog.py
+-rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/assistant_store.py
+-rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/audio.py
+-rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/base.py
+-rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/confirm.py
+-rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/create.py
+-rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/db.py
+-rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/debug.py
+-rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/editor.py
+-rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/editor_file.py
+-rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/find.py
+-rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/image.py
+-rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/info.py
+-rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/license.py
+-rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/logger.py
+-rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/profile.py
+-rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/rename.py
+-rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/settings.py
+-rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/settings_plugin.py
+-rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/snap.py
+-rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/update.py
+-rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/workdir.py
+-rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.8/src/pygpt_net/ui/widget/draw/__init__.py
+-rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.8/src/pygpt_net/ui/widget/draw/painter.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/__init__.py
+-rw-r--r--   0        0        0     4173 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/button.py
+-rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/checkbox.py
+-rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/group.py
+-rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/labels.py
+-rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/filesystem/__init__.py
+-rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/filesystem/explorer.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/image/__init__.py
+-rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/widget/image/display.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/__init__.py
+-rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/assistant.py
+-rw-r--r--   0        0        0     3715 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/assistant_store.py
+-rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/attachment.py
+-rwxr-xr-x   0        0        0     2435 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/base.py
+-rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/context.py
+-rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/db.py
+-rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/debug.py
+-rw-r--r--   0        0        0     5739 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/experts.py
+-rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/index.py
+-rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/index_combo.py
+-rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/mode.py
+-rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/model.py
+-rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/model_editor.py
+-rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/plugin.py
+-rwxr-xr-x   0        0        0     5655 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/preset.py
+-rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/preset_plugins.py
+-rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/profile.py
+-rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/settings.py
+-rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/uploaded.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/__init__.py
+-rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/checkbox.py
+-rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/cmd.py
+-rw-r--r--   0        0        0     3594 2024-05-02 17:09:01.737146 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/combo.py
+-rwxr-xr-x   0        0        0    13004 2024-05-02 17:09:01.649148 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/dictionary.py
+-rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/input.py
+-rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/prompt.py
+-rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/slider.py
+-rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/textarea.py
+-rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/Input.py
+-rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/__init__.py
+-rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/output.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/calendar_note.py
+-rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/create.py
+-rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/editor.py
+-rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/find.py
+-rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/input.py
+-rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/name.py
+-rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/notepad.py
+-rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/output.py
+-rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/rename.py
+-rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/search_input.py
+-rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/web.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/vision/__init__.py
+-rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/vision/camera.py
+-rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/utils.py
+-rw-r--r--   0        0        0   143600 1970-01-01 00:00:00.000000 pygpt_net-2.2.8/PKG-INFO
```

### Comparing `pygpt_net-2.2.7/CHANGELOG.md` & `pygpt_net-2.2.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+# 2.2.8 (2024-05-02)
+
+- Added support for disabled people, including voice control and screen event translation with audio synthesis.
+- A new section in Settings called 'Accessibility' has been added with options for assistance: voice control, keyboard shortcut definitions for actions, and screen event translation using audio synthesis.
+- A new section called 'Accessibility' has been added to the Documentation.
+
 # 2.2.7 (2024-05-01)
 
 - A new experimental work mode has been added: 'Experts', which allows the creation of separate background instances with their own instructions that can be consulted for help. See the documentation: 'Work Modes / Experts'.
 - Added a new plugin: 'Experts (inline)`.
 - Improved the Agent mode by adding the ability to configure and invoke defined Experts.
 - Improved the prompts that control the autonomous mode.
 - The main prompt controlling the agents has been moved from presets to the application's settings window.
```

### Comparing `pygpt_net-2.2.7/LICENSE` & `pygpt_net-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/README.md` & `pygpt_net-2.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.7** | build: **2024.05.01** | Python: **>=3.10, <3.12**
+Release: **2.2.8** | build: **2024.05.02** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -34,14 +34,15 @@
 
 ## Features
 
 - Desktop AI Assistant for `Linux`, `Windows` and `Mac`, written in Python.
 - Works similarly to `ChatGPT`, but locally (on a desktop computer).
 - 9 modes of operation: Chat, Vision, Completion, Assistant, Image generation, Langchain, Chat with files, Experts and Agent (autonomous).
 - Supports multiple models: `GPT-4`, `GPT-3.5`, and any model accessible through `Langchain`.
+- Included support for disabled people: voice control and translates actions on the screen using audio synthesis.
 - Handles and stores the full context of conversations (short-term memory).
 - Real-time video camera capture in Vision mode.
 - Internet access via `Google` and `Microsoft Bing`.
 - Speech synthesis via `Microsoft Azure`, `Google`, `Eleven Labs` and `OpenAI` Text-To-Speech services.
 - Speech recognition via `OpenAI Whisper`, `Google`, `Google Cloud` and `Microsoft Bing`.
 - Image analysis via `GPT-4 Vision`.
 - Crontab / Task scheduler included.
@@ -858,14 +859,112 @@
 
 You can also ask for a list of active experts at any time:
 
 ```bash
 Give me a list of active experts.
 ```
 
+# Accessibility
+
+Since version `2.2.8`, PyGPT has added beta support for disabled people and voice control. This may be very useful for blind people.
+
+
+In the `Config / Accessibility` menu, you can turn on accessibility features such as:
+
+
+- activating voice control
+
+- translating actions and events on the screen with audio speech
+
+- setting up keyboard shortcuts for actions.
+
+
+**To enable voice control:**
+
+
+Turn on the voice control option in `Config / Accessibility`:
+
+
+```bash
+Enable voice control (using microphone)
+```
+
+Once you enable this option, an `Audio Control` button will appear at the bottom right corner of the window. When you click on this button, the microphone will start listening; clicking it again stops listening and starts recognizing the voice command you said. You can cancel voice recording at any time with the `ESC` key. You can also set a keyboard shortcut to turn voice recording on/off.
+
+
+Voice command recognition works based on a model, so you don't have to worry about saying things perfectly.
+
+
+**Here's a list of commands you can ask for by voice:**
+
+- Get the current application status
+- Exit the application
+- Enable audio output
+- Disable audio output
+- Enable audio input
+- Disable audio input
+- Enable the camera
+- Disable the camera
+- Capture the camera
+- Create a new context
+- Go to the previous context
+- Go to the next context
+- Go to the last context
+- Focus on the input
+- Send the input
+- Clear the input
+- Get current conversation info
+- Stop executing current action
+- Clear the attachments
+- Read the last conversation entry
+- Read the whole conversation
+- Send the message to input
+- Append message to current input without sending it
+- Switch to chat mode
+- Switch to Chat with files (llama-index) mode
+- Add note to notepad
+- Read current notepad contents
+- Switch to the chat tab
+- Switch to the calendar tab
+- Switch to the draw (painter) tab
+- Switch to the files tab
+- Switch to the notepad tab
+- Switch to the next tab
+- Switch to the previous tab
+- Start listening for voice input
+- Stop listening for voice input
+- Toggle listening for voice input
+
+More commands coming soon.
+
+Just ask for an action that matches one of the descriptions above. These descriptions are also known to the model, and relevant commands are assigned to them. When you voice a command that fits one of those patterns, the model will trigger the appropriate action.
+
+
+For convenience, you can enable a short sound to play when voice recording starts and stops. To do this, turn on the option:
+
+
+```bash
+Audio notify microphone listening start/stop
+```
+
+To enable a sound notification when a voice command is recognized and command execution begins, turn on the option:
+
+
+```bash
+Audio notify voice command execution
+```
+
+For voice translation of on-screen events and information about completed commands via speech synthesis, you can turn on the option:
+
+```bash
+Use voice synthesis to describe events on the screen.
+```
+
+![v2_access](https://github.com/szczyglis-dev/py-gpt/assets/61396542/02dd161b-6fb1-48f9-9217-40c658888833)
+
 
 # Files and attachments
 
 ## Input attachments (upload)
 
 **PyGPT** makes it simple for users to upload files to the server and send them to the model for tasks like analysis, similar to attaching files in `ChatGPT`. There's a separate `Files` tab next to the text input area specifically for managing file uploads. Users can opt to have files automatically deleted after each upload or keep them on the list for repeated use.
 
@@ -3095,14 +3194,20 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.8 (2024-05-02)**
+
+- Added support for disabled people, including voice control and screen event translation with audio synthesis.
+- A new section in Settings called 'Accessibility' has been added with options for assistance: voice control, keyboard shortcut definitions for actions, and screen event translation using audio synthesis.
+- A new section called 'Accessibility' has been added to the Documentation.
+
 **2.2.7 (2024-05-01)**
 
 - A new experimental work mode has been added: 'Experts', which allows the creation of separate background instances with their own instructions that can be consulted for help. See the documentation: 'Work Modes / Experts'.
 - Added a new plugin: 'Experts (inline)`.
 - Improved the Agent mode by adding the ability to configure and invoke defined Experts.
 - Improved the prompts that control the autonomous mode.
 - The main prompt controlling the agents has been moved from presets to the application's settings window.
```

### Comparing `pygpt_net-2.2.7/icon.png` & `pygpt_net-2.2.8/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/pyproject.toml` & `pygpt_net-2.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygpt-net"
-version = "2.2.7"
+version = "2.2.8"
 description = "Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more"
 authors = ["Marcin Szczyglinski <info@pygpt.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/szczyglis-dev/py-gpt"
 repository = "https://github.com/szczyglis-dev/py-gpt"
 documentation = "https://pygpt.readthedocs.io/"
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/CHANGELOG.txt` & `pygpt_net-2.2.8/src/pygpt_net/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2.2.8 (2024-05-02)
+
+- Added support for disabled people, including voice control and screen event translation with audio synthesis.
+- A new section in Settings called 'Accessibility' has been added with options for assistance: voice control, keyboard shortcut definitions for actions, and screen event translation using audio synthesis.
+- A new section called 'Accessibility' has been added to the Documentation.
+
 2.2.7 (2024-05-01)
 
 - A new experimental work mode has been added: 'Experts', which allows the creation of separate background instances with their own instructions that can be consulted for help. See the documentation: 'Work Modes / Experts'.
 - Added a new plugin: 'Experts (inline)`.
 - Improved the Agent mode by adding the ability to configure and invoke defined Experts.
 - Improved the prompts that control the autonomous mode.
 - The main prompt controlling the agents has been moved from presets to the application's settings window.
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/LICENSE` & `pygpt_net-2.2.8/src/pygpt_net/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 18:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2024, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "2.2.7"
-__build__ = "2024.05.01"
+__version__ = "2.2.8"
+__build__ = "2024.05.02"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __pypi__ = "https://pypi.org/project/pygpt-net"
 __snap__ = "https://snapcraft.io/pygpt"
 __donate__ = "https://pygpt.net/#donate"
 __documentation__ = "https://pygpt.readthedocs.io"
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/app.py` & `pygpt_net-2.2.8/src/pygpt_net/app.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/config.py` & `pygpt_net-2.2.8/src/pygpt_net/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/container.py` & `pygpt_net-2.2.8/src/pygpt_net/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from pygpt_net.config import Config
+from pygpt_net.core.access import Access
+from pygpt_net.core.agents import Agents
 from pygpt_net.core.assistants import Assistants
 from pygpt_net.core.attachments import Attachments
 from pygpt_net.core.audio import Audio
 from pygpt_net.core.bridge import Bridge
 from pygpt_net.core.calendar import Calendar
 from pygpt_net.core.camera import Camera
 from pygpt_net.core.chain import Chain
@@ -49,14 +51,16 @@
         Service container
 
         :param window: Window instance
         """
         self.window = window
 
         # core
+        self.access = Access(window)
+        self.agents = Agents(window)
         self.assistants = Assistants(window)
         self.attachments = Attachments(window)
         self.audio = Audio(window)
         self.bridge = Bridge(window)
         self.calendar = Calendar(window)
         self.camera = Camera(window)
         self.chain = Chain(window)
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
+from pygpt_net.controller.access import Access
 from pygpt_net.controller.agent import Agent
 from pygpt_net.controller.assistant import Assistant
 from pygpt_net.controller.attachment import Attachment
 from pygpt_net.controller.audio import Audio
 from pygpt_net.controller.calendar import Calendar
 from pygpt_net.controller.camera import Camera
 from pygpt_net.controller.chat import Chat
@@ -41,14 +42,15 @@
     def __init__(self, window=None):
         """
         Main controller
 
         :param window: Window instance
         """
         self.window = window
+        self.access = Access(window)
         self.agent = Agent(window)
         self.assistant = Assistant(window)
         self.attachment = Attachment(window)
         self.audio = Audio(window)
         self.calendar = Calendar(window)
         self.camera = Camera(window)
         self.chat = Chat(window)
@@ -92,14 +94,15 @@
         self.idx.setup()
         self.ui.update_tokens()
         self.dialogs.setup()
         self.audio.setup()
         self.attachment.setup()
         self.notepad.setup()
         self.camera.setup_ui()
+        self.access.setup()
 
     def post_setup(self):
         """Post-setup, after plugins are loaded"""
         self.settings.setup()
         self.plugins.settings.setup()
         self.model.editor.setup()
         self.launcher.post_setup()
@@ -133,21 +136,23 @@
         self.window.core.reload()  # db, config, patch, etc.
         self.ctx.reload()
         self.settings.reload()
         self.assistant.reload()
         self.attachment.reload()
         self.presets.reload()
         self.idx.reload()
+        self.agent.reload()
         self.calendar.reload()
         self.plugins.reload()
         self.painter.reload()
         self.notepad.reload()
         self.files.reload()
         self.lang.reload()
         self.theme.reload_all()
         self.debug.reload()
         self.chat.reload()
         self.window.tools.on_reload()
+        self.access.reload()
         # self.layout.reload()
 
         # post-reload
         self.ctx.reload_after()
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/agent/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/agent/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
+from .common import Common
 from .experts import Experts
 from .flow import Flow
 
 
 class Agent:
     def __init__(self, window=None):
         """
         Agent controller
 
         :param window: Window instance
         """
         self.window = window
+        self.common = Common(window)
         self.experts = Experts(window)
         self.flow = Flow(window)
         self.options = {
             "agent.iterations": {
                 "type": "int",
                 "slider": True,
                 "label": "agent.iterations",
@@ -34,24 +36,49 @@
                 "value": 3,
                 "multiplier": 1,
             },
         }
 
     def setup(self):
         """Setup agent controller"""
-        # restore options
+        # register hooks
+        self.window.ui.add_hook("update.global.agent.iterations", self.hook_update)
+
+        # restore config
+        self.reload()
+
+    def update(self):
+        """Update agent status"""
+        iterations = "-"
+        mode = self.window.core.config.get('mode')
+
+        # get iterations from plugin or from agent mode
+        if mode == "agent":
+            iterations = int(self.window.core.config.get("agent.iterations"))
+        elif self.is_inline():
+            if self.window.controller.plugins.is_enabled("agent"):
+                iterations = int(self.window.core.plugins.get_option("agent", "iterations"))
+        if iterations == 0:
+            iterations_str = "∞"  # infinity loop
+        else:
+            iterations_str = str(iterations)
+
+        status = str(self.flow.iteration) + " / " + iterations_str
+        self.window.ui.nodes['status.agent'].setText(status)
+        self.common.toggle_status()
+
+    def reload(self):
+        """Reload agent controller"""
+        # auto-stop
         if self.window.core.config.get('agent.auto_stop'):
             self.window.ui.config['global']['agent.auto_stop'].setChecked(True)
         else:
             self.window.ui.config['global']['agent.auto_stop'].setChecked(False)
 
-        # register hooks
-        self.window.ui.add_hook("update.global.agent.iterations", self.hook_update)
-
-        # load config
+        # iterations
         self.window.controller.config.apply_value(
             parent_id="global",
             key="agent.iterations",
             option=self.options["agent.iterations"],
             value=self.window.core.config.get('agent.iterations'),
         )
 
@@ -69,84 +96,26 @@
             return
 
         if key == 'agent.iterations':
             self.window.core.config.set(key, int(value))  # cast to int, if from text input
             self.window.core.config.save()
             self.update()
 
-    def is_agent_inline(self) -> bool:
+    def is_inline(self) -> bool:
         """
         Is agent inline (plugin) enabled
 
         :return: True if enabled
         """
         return self.window.controller.plugins.is_type_enabled("agent")
 
-    def toggle_status(self):
-        """Toggle agent status"""
-        mode = self.window.core.config.get('mode')
-        if mode == 'agent' or self.is_agent_inline():
-            self.show_status()
-        else:
-            self.hide_status()
-
-    def enable_auto_stop(self):
-        """Enable auto stop"""
-        self.window.core.config.set('agent.auto_stop', True)
-        self.window.core.config.save()
-
-    def disable_auto_stop(self):
-        """Disable auto stop"""
-        self.window.core.config.set('agent.auto_stop', False)
-        self.window.core.config.save()
-
     def enabled(self) -> bool:
         """
         Is agent enabled
 
         :return: True if enabled
         """
-        return self.window.core.config.get('mode') == 'agent' or self.is_agent_inline()
+        return self.window.core.config.get('mode') == 'agent' or self.is_inline()
 
     def add_run(self):
         """Increment agent iteration"""
         self.flow.iteration += 1
-
-    def update(self):
-        """Update agent status"""
-        iterations = "-"
-        mode = self.window.core.config.get('mode')
-
-        # get iterations from plugin or from mode
-        if mode == "agent":
-            iterations = int(self.window.core.config.get("agent.iterations"))
-        elif self.is_agent_inline():
-            if self.window.controller.plugins.is_enabled("agent"):
-                iterations = int(self.window.core.plugins.get_option("agent", "iterations"))
-
-        if iterations == 0:
-            iterations_str = "∞"  # infinity loop
-        else:
-            iterations_str = str(iterations)
-
-        status = str(self.flow.iteration) + " / " + iterations_str
-        self.window.ui.nodes['status.agent'].setText(status)
-        self.toggle_status()
-
-    def show_status(self):
-        """Show agent status"""
-        self.window.ui.nodes['status.agent'].setVisible(True)
-
-    def hide_status(self):
-        """Hide agent status"""
-        self.window.ui.nodes['status.agent'].setVisible(False)
-
-    def toggle_auto_stop(self, state: bool):
-        """
-        Toggle auto stop
-
-        :param state: state of checkbox
-        """
-        if not state:
-            self.disable_auto_stop()
-        else:
-            self.enable_auto_stop()
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/agent/experts.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/agent/experts.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 
 class Experts:
     def __init__(self, window=None):
         """
         Experts controller
@@ -44,10 +44,10 @@
         """
         Check if experts are enabled
 
         :return: True if experts are enabled
         """
         modes = ["agent", "expert"]
         mode = self.window.core.config.get('mode')
-        if mode in modes or self.window.controller.plugins.is_type_enabled("experts"):
+        if mode in modes or self.window.controller.plugins.is_type_enabled("expert"):
             return True
         return False
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/agent/flow.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/agent/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.17 13:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.utils import trans
 
 
 class Flow:
@@ -25,14 +25,15 @@
         self.prev_output = None
         self.is_user = True
         self.stop = False
         self.finished = False
         self.allowed_cmds = [
             "goal_update",
         ]
+        self.pause_status = ["pause", "failed", "wait"]
 
     def on_system_prompt(
             self,
             prompt: str,
             append_prompt: str = "",
             auto_stop: bool = True,
     ) -> str:
@@ -58,15 +59,15 @@
 
         :param prompt: prompt
         :return: updated prompt
         """
         if not self.is_user:
             return prompt
 
-        return "user: " + prompt
+        return "user: " + prompt  # add user prefix
 
     def on_user_send(self, text: str):
         """
         Event: On user send text
 
         :param text: text
         """
@@ -180,29 +181,27 @@
             if item["cmd"] in self.allowed_cmds:
                 my_commands.append(item)
                 is_cmd = True
 
         if not is_cmd:
             return
 
-        pause_status = ["pause", "failed", "wait"]
-
         for item in my_commands:
             try:
                 if item["cmd"] == "goal_update":
                     if item["params"]["status"] == "finished":
                         self.on_stop(auto=True)
                         self.window.ui.status(trans('status.finished'))  # show info
                         self.finished = True
                         if self.window.core.config.get("agent.goal.notify"):
                             self.window.ui.tray.show_msg(
                                 trans("notify.agent.goal.title"),
                                 trans("notify.agent.goal.content"),
                             )
-                    elif item["params"]["status"] in pause_status:
+                    elif item["params"]["status"] in self.pause_status:
                         self.on_stop(auto=True)
                         self.window.ui.status(trans('status.finished'))  # show info
                         self.finished = True
             except Exception as e:
                 self.window.core.debug.error(e)
                 return
 
@@ -216,8 +215,11 @@
         self.iteration = 0
         self.prev_output = None
         self.stop = True
         self.finished = False  # reset finished flag
 
         # update index if auto-index enabled
         if auto:
-            self.window.controller.idx.on_ctx_end(ctx=None, mode="agent")
+            self.window.controller.idx.on_ctx_end(
+                ctx=None,
+                mode="agent",
+            )
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/batch.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/batch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/editor.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/files.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/store.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/threads.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/threads.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/attachment.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import os
 from datetime import datetime
 
 from PySide6.QtGui import QImage
 from PySide6.QtWidgets import QFileDialog, QApplication
 
+from pygpt_net.core.access.events import AppEvent
 from pygpt_net.item.assistant import AssistantItem
 from pygpt_net.item.attachment import AttachmentItem
 from pygpt_net.utils import trans
 
 
 class Attachment:
     def __init__(self, window=None):
@@ -215,14 +216,15 @@
         self.window.core.attachments.delete_all(
             mode=mode,
             remove_local=remove_local,
         )
 
         self.window.controller.chat.vision.unavailable()  # set no content to provide
         self.update()
+        self.window.core.dispatcher.dispatch(AppEvent(AppEvent.CTX_ATTACHMENTS_CLEAR))
 
     def open_add(self):
         """Open add attachment file dialog"""
         last_dir = self.window.core.config.get_last_used_dir()
         mode = self.window.core.config.get('mode')
         dialog = QFileDialog(self.window)
         dialog.setDirectory(last_dir)
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/audio/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/audio/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.20 06:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
+import os
 
 from pygpt_net.core.dispatcher import Event
+from pygpt_net.plugin.audio_output.worker import PlayWorker
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.utils import trans
 
 
 class Audio:
     def __init__(self, window=None):
         """
@@ -136,14 +138,35 @@
         ctx = CtxItem()
         ctx.output = text
         all = True  # to all plugins (even if disabled)
         event = Event(Event.AUDIO_READ_TEXT)
         event.ctx = ctx
         self.window.core.dispatcher.dispatch(event, all=all)
 
+    def play_audio(self, path: str):
+        """
+        Play audio file
+
+        :param path: audio file path
+        """
+        worker = PlayWorker()
+        worker.window = self.window
+        worker.path = path
+        self.window.threadpool.start(worker)
+
+    def play_sound(self, filename: str):
+        """
+        Play sound
+
+        :param filename
+        """
+        path = os.path.join(self.window.core.config.get_app_path(), "data", "audio", filename)
+        if path:
+            self.play_audio(path)
+
     def toggle_output_icon(self, state: bool):
         """
         Toggle input icon
 
         :param state: True to enable, False to disable
         """
         if state:
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/calendar/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/calendar/note.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/calendar/note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/camera.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/camera.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 16:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import datetime
 import os
 import cv2
 from PySide6.QtCore import Slot
 
 from PySide6.QtGui import QImage, QPixmap, Qt
+
+from pygpt_net.core.access.events import AppEvent
 from pygpt_net.core.camera import CaptureWorker
 from pygpt_net.utils import trans
 
 
 class Camera:
     def __init__(self, window=None):
         """
@@ -84,21 +86,23 @@
         worker.signals.unfinished.connect(self.handle_unfinished)
         worker.signals.stopped.connect(self.handle_stop)
         worker.signals.error.connect(self.handle_error)
 
         # start
         self.window.threadpool.start(worker)
         self.thread_started = True
+        self.window.core.dispatcher.dispatch(AppEvent(AppEvent.CAMERA_ENABLED))  # app event
 
     def stop_capture(self):
         """Stop camera capture thread"""
         if not self.thread_started:
             return
 
         self.stop = True
+        self.window.core.dispatcher.dispatch(AppEvent(AppEvent.CAMERA_DISABLED))  # app event
 
     @Slot(object)
     def handle_error(self, err):
         """
         Handle thread error signal
 
         :param err: error message
@@ -168,14 +172,15 @@
         if not self.is_auto() or force:
             if not self.capture_frame(True):
                 self.window.statusChanged.emit(
                     trans("vision.capture.manual.captured.error")
                 )
         else:
             self.window.statusChanged.emit(trans('vision.capture.auto.click'))
+        self.window.core.dispatcher.dispatch(AppEvent(AppEvent.CAMERA_CAPTURED))  # app event
 
     def get_current_frame(self, flip_colors: bool = True):
         """Get current frame"""
         if self.frame is None:
             return None
         if flip_colors:
             return cv2.cvtColor(self.frame, cv2.COLOR_BGR2RGB)
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/chat/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/chat/common.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/chat/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtGui import QTextCursor
 from PySide6.QtWidgets import QFileDialog
 
+from pygpt_net.core.access.events import AppEvent
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.utils import trans
 
 
 class Common:
     def __init__(self, window=None):
         """
@@ -215,14 +216,17 @@
         # remotely stop assistant
         if mode == "assistant" and not exit:
             try:
                 self.window.controller.assistant.run_stop()
             except Exception as e:
                 self.window.core.debug.log(e)
 
+        if not exit:
+            self.window.core.dispatcher.dispatch(AppEvent(AppEvent.INPUT_STOPPED))  # app event
+
     def check_api_key(self) -> bool:
         """
         Check if API KEY is set
 
         :return: True if API KEY is set, False otherwise
         """
         result = True
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/chat/files.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/chat/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/chat/image.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/chat/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/chat/input.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/chat/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtWidgets import QApplication
 
+from pygpt_net.core.access.events import AppEvent
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.utils import trans
 
 
 class Input:
     def __init__(self, window=None):
@@ -43,14 +44,16 @@
     def send_input(self, force: bool = False):
         """
         Send text from user input (called from UI)
 
         :param force: force send
         """
         self.window.controller.agent.experts.unlock()  # unlock experts
+        if not force:
+            self.window.core.dispatcher.dispatch(AppEvent(AppEvent.INPUT_SENT))  # app event
 
         # check if not in edit mode
         if not force and self.window.controller.ctx.extra.is_editing():
             self.window.controller.ctx.extra.edit_submit()
             return
 
         # get text from input
@@ -272,14 +275,15 @@
         self.generating = False  # unlock
 
         if mode not in self.no_ctx_idx_modes and not self.window.controller.agent.enabled():
             self.window.controller.idx.on_ctx_end(ctx, mode=mode)  # update ctx DB index
             # disabled in agent mode here to prevent loops, handled in agent flow internally if agent mode
 
         self.log("End.")
+        self.window.core.dispatcher.dispatch(AppEvent(AppEvent.CTX_END))  # app event
 
         # restore state to idle if no errors
         if self.window.state != self.window.STATE_ERROR:
             self.window.stateChanged.emit(self.window.STATE_IDLE)
 
     def log(self, data: any):
         """
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/chat/output.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/chat/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtWidgets import QApplication
 
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.utils import trans
@@ -93,15 +93,15 @@
                     sub_mode = 'completion'
 
         # chunks: stream begin
         self.window.controller.chat.render.stream_begin()
 
         response_mode = mode
         if mode == "agent":
-            tmp_mode = self.window.core.config.get("agent.mode")
+            tmp_mode = self.window.core.agents.get_mode()
             if tmp_mode is not None and tmp_mode != "_":
                 response_mode = tmp_mode
 
         # read stream
         try:
             if ctx.stream is not None:
                 self.log("Reading stream...")  # log
@@ -248,15 +248,15 @@
             # re-send to master
             if ctx.sub_reply:
                 self.window.core.ctx.update_item(ctx)
                 self.window.core.experts.reply(ctx)
             else:
                 # call experts
                 if not ctx.reply:
-                    mentions = self.window.core.experts.extract_mentions(ctx)
+                    mentions = self.window.core.experts.extract_calls(ctx)
                     if mentions:
                         self.log("Calling experts...")
                         self.window.controller.chat.render.end(stream=stream_mode)  # close previous render
                         for expert_id in mentions:
                             self.log("Calling: " + expert_id)
                             ctx.sub_calls += 1
                             self.window.core.experts.call(
@@ -269,15 +269,15 @@
         # extract commands
         cmds = self.window.core.command.extract_cmds(ctx.output)
         if len(cmds) > 0:
             ctx.cmds = cmds  # append commands to ctx
 
             # agent mode
             if mode == 'agent':
-                commands = self.window.controller.plugins.from_commands(cmds)  # pack to execution list
+                commands = self.window.core.command.from_commands(cmds)  # pack to execution list
                 self.window.controller.agent.flow.on_cmd(
                     ctx,
                     commands,
                 )
                 # check if agent flow is not finished
                 if self.window.controller.agent.flow.finished:
                     return
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/chat/render.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/chat/render.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/chat/text.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/chat/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtWidgets import QApplication
 
+from pygpt_net.core.access.events import AppEvent
 from pygpt_net.core.bridge import BridgeContext
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.utils import trans
 
 
 class Text:
@@ -206,19 +207,20 @@
 
         try:
             # make API call
             try:
                 self.window.controller.chat.common.lock_input()  # lock input
                 max_tokens = self.window.core.config.get('max_output_tokens')  # max output tokens
                 files = self.window.core.attachments.get_all(mode)  # get attachments
-                file_ids = self.window.controller.files.uploaded_ids  # uploaded files IDs
-                history = self.window.core.ctx.all(meta_id=parent_id)  # get all history
                 num_files = len(files)
                 if num_files > 0:
                     self.log("Attachments ({}): {}".format(mode, num_files))
+                file_ids = self.window.controller.files.uploaded_ids  # uploaded files IDs
+                history = self.window.core.ctx.all(meta_id=parent_id)  # get all history
+                self.window.core.dispatcher.dispatch(AppEvent(AppEvent.INPUT_CALL))  # app event
 
                 # make call
                 bridge_context = BridgeContext(
                     ctx=ctx,
                     history=history,
                     mode=mode,
                     parent_mode=base_mode,
@@ -255,16 +257,17 @@
                     self.window.ui.status(trans('status.error'))
 
             except Exception as e:
                 self.log("GPT output error: {}".format(e))  # log
                 self.window.core.debug.log(e)
                 self.window.ui.dialogs.alert(e)
                 self.window.ui.status(trans('status.error'))
-                print("Error when calling API: " + str(e))
                 self.window.controller.chat.common.unlock_input()
+                self.window.core.dispatcher.dispatch(AppEvent(AppEvent.INPUT_ERROR))  # app event
+                print("Error when calling API: " + str(e))
             self.window.stateChanged.emit(self.window.STATE_ERROR)
 
             # handle response (if no assistant mode)
             # assistant response is handled in assistant thread
             if mode != "assistant":
                 ctx.from_previous()  # append previous result if exists
                 self.window.controller.chat.output.handle(
@@ -274,17 +277,18 @@
                 )
 
         except Exception as e:
             self.log("Output ERROR: {}".format(e))  # log
             self.window.core.debug.log(e)
             self.window.ui.dialogs.alert(e)
             self.window.ui.status(trans('status.error'))
-            print("Error in sending text: " + str(e))
             self.window.controller.chat.common.unlock_input()
             self.window.stateChanged.emit(self.window.STATE_ERROR)
+            self.window.core.dispatcher.dispatch(AppEvent(AppEvent.INPUT_ERROR))  # app event
+            print("Error in sending text: " + str(e))
 
         # if commands enabled: post-execute commands (if no assistant mode)
         if mode != "assistant":
             ctx.clear_reply()  # reset results
             self.window.controller.chat.output.handle_cmd(ctx)
             ctx.from_previous()  # append previous result again before save
             self.window.core.ctx.update_item(ctx)  # update ctx in DB
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/chat/vision.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/chat/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/command.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/config/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/checkbox.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/cmd.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/combo.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/dictionary.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/input.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/slider.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/textarea.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/config/placeholder.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/config/placeholder.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from pygments.styles import get_all_styles
 
+from pygpt_net.utils import trans
+
+
 class Placeholder:
     def __init__(self, window=None):
         """
         Configuration placeholder options controller
 
         :param window: Window instance
         """
@@ -74,14 +77,20 @@
             return self.get_var_types()
         elif id == "agent_modes":
             return self.get_agent_modes()
         elif id == "syntax_styles":
             return self.get_syntax_styles()
         elif id == "idx":
             return self.get_idx()
+        elif id == "keys":
+            return self.get_keys()
+        elif id == "keys_modifiers":
+            return self.get_modifiers()
+        elif id == "access_actions":
+            return self.get_access_actions()
         else:
             return []
 
     def get_langchain_providers(self) -> list:
         """
         Get langchain placeholders list
 
@@ -185,26 +194,25 @@
         """
         Get models placeholders list
 
         :return: Models placeholders list
         """
         models = self.window.core.models.get_all()
         data = []
-        data.append({'_': '---'})
         for id in models:
             data.append({id: id})  # TODO: name
         return data
 
     def get_agent_modes(self) -> list:
         """
-        Get modes placeholders list
+        Get agent/expert modes placeholders list
 
         :return: Models placeholders list
         """
-        modes = ["chat", "completion", "vision", "langchain", "llama_index", "expert"]
+        modes = self.window.core.agents.get_allowed_modes()
         data = []
         for id in modes:
             data.append({id: id})  # TODO: name
         return data
 
     def get_idx(self) -> list:
         """
@@ -227,7 +235,38 @@
         """
         styles = list(get_all_styles())
         styles.sort()
         data = []
         for id in styles:
             data.append({id: id})
         return data
+
+    def get_keys(self) -> list:
+        """
+        Get keys
+
+        :return: keys
+        """
+        return self.window.core.access.shortcuts.get_keys_choices()
+
+    def get_modifiers(self) -> list:
+        """
+        Get modifiers
+
+        :return: keys
+        """
+        return self.window.core.access.shortcuts.get_modifiers_choices()
+
+    def get_access_actions(self) -> list:
+        """
+        Get access actions list
+
+        :return: app actions list
+        """
+        choices = self.window.core.access.actions.get_access_choices()
+        translated_choices = []
+        for choice in choices:
+            for key, value in choice.items():
+                translated_choices.append({key: trans(value)})
+        return translated_choices
+
+
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/ctx/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/ctx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import QModelIndex
 
 from pygpt_net.core.dispatcher import Event
+from pygpt_net.core.access.events import AppEvent
 from pygpt_net.item.ctx import CtxItem
 
 from .common import Common
 from .summarizer import Summarizer
 from .extra import Extra
 
 from pygpt_net.utils import trans
@@ -113,14 +114,15 @@
 
         :param id: context id
         """
         prev_id = self.window.core.ctx.current
         self.window.core.ctx.current = id
         if prev_id != id:
             self.load(id)
+            self.window.core.dispatcher.dispatch(AppEvent(AppEvent.CTX_SELECTED))  # app event
         else:
             # only update current group if defined
             meta = self.window.core.ctx.get_meta_by_id(id)
             if meta is not None:
                 self.set_group(meta.group_id)
         self.common.focus_chat()
 
@@ -225,23 +227,44 @@
         if mode == 'assistant':
             assistant_id = self.window.core.config.get('assistant')
             self.window.controller.assistant.files.update()  # always update assistant files
 
         self.common.update_label(mode, assistant_id)
         self.common.focus_chat()
 
+        # app event
+        self.window.core.dispatcher.dispatch(AppEvent(AppEvent.CTX_CREATED))
+
     def add(self, ctx: CtxItem):
         """
         Add ctx item (CtxItem object)
 
         :param ctx: CtxItem
         """
         self.window.core.ctx.add(ctx)
         self.update()
 
+    def prev(self):
+        """Select previous ctx"""
+        id = self.window.core.ctx.get_prev()
+        if id is not None:
+            self.select(id)
+
+    def next(self):
+        """Select next ctx"""
+        id = self.window.core.ctx.get_next()
+        if id is not None:
+            self.select(id)
+
+    def last(self):
+        """Select last (newest) ctx"""
+        id = self.window.core.ctx.get_last_meta()
+        if id is not None:
+            self.select(id)
+
     def update_list(self, reload: bool = False):
         """
         Reload current ctx list
 
         :param reload: reload ctx list items
         """
         self.window.ui.contexts.ctx_list.update(
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/ctx/common.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/ctx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/ctx/extra.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/ctx/extra.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,40 +35,40 @@
     def copy_item(self, item_id: int):
         """
         Copy ctx item to clipboard
 
         :param item_id: Item id
         """
         item = self.window.core.ctx.get_item_by_id(item_id)
-        if item is not None:
-            QApplication.clipboard().setText(item.output)
+        if item is not None and item.output is not None:
+            QApplication.clipboard().setText(item.output.strip())
             self.window.ui.status(trans("clipboard.copied"))
 
     def copy_code_block(self, id: int):
         """
         Copy code block to clipboard
 
         :param id: block id
         """
         blocks = self.window.controller.chat.render.get_renderer().parser.get_code_blocks()
         if id not in blocks:
             print("Code block not found: ", id)
             return
         value = blocks.get(id)
-        QApplication.clipboard().setText(value)
-        suffix = value[:20] + "..." if len(value) > 20 else value
+        QApplication.clipboard().setText(value.strip())
+        suffix = value[:30] + "..." if len(value) > 20 else value
         self.window.ui.status(trans("clipboard.copied_to") + " " + suffix)
 
     def copy_code_text(self, value: str):
         """
         Copy code block to clipboard
 
         :param value: block text
         """
-        QApplication.clipboard().setText(value)
+        QApplication.clipboard().setText(value.strip())
         suffix = value[:20] + "..." if len(value) > 20 else value
         self.window.ui.status(trans("clipboard.copied_to") + " " + suffix)
 
     def edit_item(self, item_id: int):
         """
         Edit ctx item
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/ctx/summarizer.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/ctx/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/debug/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/confirm.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/debug.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/info.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/files.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/finder.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/idx/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/idx/common.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/idx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/idx/indexer.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/idx/indexer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/idx/settings.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/idx/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/lang/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/lang/custom.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/lang/custom.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/lang/mapping.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/lang/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from pygpt_net.utils import trans
 
 
 class Mapping:
     def __init__(self, window=None):
@@ -310,14 +310,15 @@
         menu_text['app.ctx.group.new'] = 'menu.file.group.new'
         menu_text['app.ctx.current'] = 'menu.file.current'
         menu_text['app.clear_history'] = 'menu.file_clear_history'
         menu_text['app.clear_history_groups'] = 'menu.file_clear_history_groups'
         menu_text['app.exit'] = 'menu.file.exit'
         menu_text['config.settings'] = 'menu.config.settings'
         menu_text['config.models'] = 'menu.config.models'
+        menu_text['config.access'] = 'menu.config.access'
         menu_text['config.open_dir'] = 'menu.config.open_dir'
         menu_text['config.change_dir'] = 'menu.config.change_dir'
         menu_text['config.edit.css.restore'] = 'menu.config.edit.css.restore'
         menu_text['config.profile.edit'] = 'menu.config.profile.edit'
         menu_text['config.profile.new'] = 'menu.config.profile.new'
         menu_text['config.save'] = 'menu.config.save'
         menu_text['theme.tooltips'] = 'menu.theme.tooltips'
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/lang/plugins.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/lang/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/lang/settings.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/lang/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/launcher.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/layout.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/layout.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/mode.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/model/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/model/editor.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/model/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/notepad.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/notepad.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QIcon, QTextCursor
 
 from pygpt_net.item.notepad import NotepadItem
 from pygpt_net.ui.widget.textarea.notepad import NotepadWidget
 from pygpt_net.utils import trans
@@ -326,7 +326,51 @@
 
     def reload(self):
         """Reload notepads"""
         self.window.core.notepad.locked = True
         self.window.core.notepad.reset()
         self.update_tabs()
         self.window.core.notepad.locked = False
+
+    def switch_to_tab(self, idx: int = None):
+        """
+        Switch to notepad tab
+
+        :param idx: notepad idx
+        """
+        if idx is None:
+            idx = 1  # get first notepad idx
+        tab = idx + (self.start_tab_idx - 1)
+        if tab < self.window.ui.tabs['output'].count():
+            self.window.ui.tabs['output'].setCurrentIndex(tab)
+        else:
+            self.window.ui.tabs['output'].setCurrentIndex(self.window.ui.tabs['output'].count() - 1)
+
+    def get_first_notepad_tab_idx(self) -> int:
+        """
+        Get first notepad tab index
+
+        :return: first notepad tab index
+        """
+        return self.start_tab_idx
+
+    def get_current_notepad_text(self) -> str:
+        """
+        Get current notepad text
+
+        :return: current notepad text
+        """
+        idx = self.get_current_active()
+        if idx in self.window.ui.notepad:
+            return self.window.ui.notepad[idx].toPlainText()
+        return ""
+
+    def get_notepad_text(self, idx: int) -> str:
+        """
+        Get notepad text
+
+        :param idx: notepad index
+        :return: notepad text
+        """
+        if idx in self.window.ui.notepad:
+            return self.window.ui.notepad[idx].toPlainText()
+        return ""
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/painter/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/painter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/painter/capture.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/painter/capture.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/painter/common.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/painter/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/plugins/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QAction
 
 from pygpt_net.controller.plugins.presets import Presets
 from pygpt_net.controller.plugins.settings import Settings
 from pygpt_net.core.dispatcher import Event
@@ -361,36 +361,22 @@
                     c += 1
 
         if c > 0:
             count_str = "+ " + str(c) + " " + trans('chatbox.plugins')
         self.window.ui.nodes['chat.plugins'].setText(count_str)
         self.window.ui.nodes['chat.plugins'].setToolTip(tooltip)
 
-    def from_commands(self, cmds: list):
-        """
-        Pack commands
-
-        :param cmds: commands list
-        :return parsed commands
-        """
-        commands = []
-        for cmd in cmds:
-            if 'cmd' in cmd:
-                commands.append(cmd)
-        return commands
-
     def apply_cmds(self, ctx: CtxItem, cmds: list):
         """
         Apply commands
 
         :param ctx: CtxItem
         :param cmds: commands list
         """
-        commands = self.from_commands(cmds)
-
+        commands = self.window.core.command.from_commands(cmds)
         if len(commands) == 0:
             return
 
         # dispatch command execute event
         event = Event(Event.CMD_EXECUTE, {
             'commands': commands,
         })
@@ -401,16 +387,15 @@
     def apply_cmds_inline(self, ctx: CtxItem, cmds: list):
         """
         Apply inline commands
 
         :param ctx: CtxItem
         :param cmds: commands list
         """
-        commands = self.from_commands(cmds)
-
+        commands = self.window.core.command.from_commands(cmds)
         if len(commands) == 0:
             return
 
         # dispatch inline command event
         event = Event(Event.CMD_INLINE, {
             'commands': commands,
         })
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/plugins/presets.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/plugins/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/plugins/settings.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/presets/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/presets/editor.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/presets/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/presets/experts.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/presets/experts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/settings/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/settings/editor.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/settings/editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.24 02:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import copy
 
 from pygpt_net.utils import trans
 
 
@@ -52,14 +52,15 @@
         self.window.ui.add_hook("update.config.vision.capture.enabled", self.hook_update)
         self.window.ui.add_hook("update.config.vision.capture.auto", self.hook_update)
         self.window.ui.add_hook("update.config.ctx.records.limit", self.hook_update)
         self.window.ui.add_hook("update.config.ctx.convert_lists", self.hook_update)
         self.window.ui.add_hook("update.config.layout.density", self.hook_update)
         self.window.ui.add_hook("update.config.layout.tooltips", self.hook_update)
         self.window.ui.add_hook("update.config.img_dialog_open", self.hook_update)
+        self.window.ui.add_hook("update.config.access.voice_control", self.hook_update)
         self.window.ui.add_hook("update.config.debug", self.hook_update)
         self.window.ui.add_hook("update.config.notepad.num", self.hook_update)
         self.window.ui.add_hook("update.config.render.code_syntax", self.hook_update)
         # self.window.ui.add_hook("llama.idx.storage", self.hook_update)  # vector store update
         # self.window.ui.add_hook("update.config.llama.idx.list", self.hook_update)
 
         if id == 'settings':
@@ -155,14 +156,18 @@
             value = self.window.core.config.get('render.code_syntax')
             self.window.controller.theme.toggle_syntax(value, update_menu=True)
 
         # convert lists
         if self.config_changed('ctx.convert_lists'):
             self.window.controller.ctx.refresh()
 
+        # access: voice control
+        if self.config_changed('access.voice_control'):
+            self.window.controller.access.update()
+
         # reload loaders
         if self.config_changed('llama.hub.loaders.args') or self.config_changed('llama.hub.loaders.use_local'):
             self.window.core.idx.indexing.reload_loaders()
             self.window.tools.get("indexer").refresh()
 
         # update idx list
         if self.config_changed('llama.idx.list'):
@@ -240,14 +245,19 @@
             self.window.controller.ctx.refresh()
 
         # update layout tooltips
         elif key == "layout.tooltips":
             self.window.core.config.set(key, value)
             self.window.controller.theme.common.toggle_tooltips()
 
+        # access: voice control
+        elif key == "access.voice_control":
+            self.window.core.config.set(key, value)
+            self.window.controller.access.update()
+
         # update raw output
         elif key == "render.plain":
             self.window.core.config.set(key, value)
             if not value:
                 self.window.ui.nodes['output.raw'].setChecked(False)
             else:
                 self.window.ui.nodes['output.raw'].setChecked(True)
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/settings/profile.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/settings/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/settings/workdir.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/settings/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/theme/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/theme/common.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/theme/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/theme/markdown.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/theme/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/theme/menu.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/theme/menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/theme/nodes.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/theme/nodes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/ui/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/ui/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.10 23:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QColor
 
 from pygpt_net.utils import trans
 from .mode import Mode
 from .vision import Vision
@@ -166,14 +166,33 @@
         self.vision.update()
 
         if idx == self.tab_idx['calendar']:
             self.window.controller.notepad.opened_once = True
         elif idx == self.tab_idx['draw']:
             if self.window.core.config.get('vision.capture.enabled'):
                 self.window.controller.camera.enable_capture()
+        self.window.controller.access.voice.read_tab_name()
+
+    def next_tab(self):
+        """Switch to next tab"""
+        current = self.window.ui.tabs['output'].currentIndex()
+        all = len(self.window.ui.tabs['output'].children())
+        next = current + 1
+        if next >= all:
+            next = 0
+        self.switch_tab_by_idx(next)
+
+    def prev_tab(self):
+        """Switch to previous tab"""
+        current = self.window.ui.tabs['output'].currentIndex()
+        all = len(self.window.ui.tabs['output'].children())
+        prev = current - 1
+        if prev < 0:
+            prev = all - 1
+        self.switch_tab_by_idx(prev)
 
     def switch_tab(self, tab: str):
         """
         Switch tab
 
         :param tab: tab name
         """
@@ -185,7 +204,15 @@
         """
         Switch tab by index
 
         :param idx: tab index
         """
         self.window.ui.tabs['output'].setCurrentIndex(idx)
         self.output_tab_changed(idx)
+
+    def get_current_tab_name(self) -> str:
+        """
+        Get current tab name
+
+        :return: tab name
+        """
+        return self.window.ui.tabs['output'].tabText(self.current_tab)
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/ui/mode.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/ui/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/controller/ui/vision.py` & `pygpt_net-2.2.8/src/pygpt_net/controller/ui/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/assistants/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/assistants/files.py` & `pygpt_net-2.2.8/src/pygpt_net/core/assistants/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/assistants/store.py` & `pygpt_net-2.2.8/src/pygpt_net/core/assistants/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/attachments.py` & `pygpt_net-2.2.8/src/pygpt_net/core/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/audio.py` & `pygpt_net-2.2.8/src/pygpt_net/core/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/bridge.py` & `pygpt_net-2.2.8/src/pygpt_net/core/bridge.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 03:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import time
 from datetime import datetime, timedelta
 
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.item.model import ModelItem
@@ -108,23 +108,23 @@
 
         # get data
         ctx = context.ctx
         prompt = context.prompt
         mode = context.mode
         model = context.model  # model instance
 
-        # get mode from config
+        # get agent internal sub-mode
         if mode == "agent":
-            mode = "chat"  # inline switch to chat mode, because agent is a virtual mode only
-            tmp_mode = self.window.core.config.get("agent.mode")
-            if tmp_mode is not None and tmp_mode != "_":
-                mode = tmp_mode
+            mode = "chat"  # inline switch to sub-mode, because agent is a virtual mode only
+            sub_mode = self.window.core.agents.get_mode()
+            if sub_mode is not None and sub_mode != "_":
+                mode = sub_mode
             if mode == "llama_index":
                 context.idx_raw = False
-                idx = self.window.core.config.get("agent.idx")
+                idx = self.window.core.agents.get_mode()
                 if idx is not None and idx != "_":
                     context.idx = idx
 
         # inline: internal mode switch if needed
         context.parent_mode = mode  # store REAL mode
         mode = self.window.controller.mode.switch_inline(mode, ctx, prompt)
         context.mode = mode
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/calendar/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/camera.py` & `pygpt_net-2.2.8/src/pygpt_net/core/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/chain/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/chain/chat.py` & `pygpt_net-2.2.8/src/pygpt_net/core/chain/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/chain/completion.py` & `pygpt_net-2.2.8/src/pygpt_net/core/chain/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/command.py` & `pygpt_net-2.2.8/src/pygpt_net/core/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.17 13:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import copy
 import json
 
 from pygpt_net.item.ctx import CtxItem
 
@@ -144,14 +144,27 @@
                                     "params": cmd[key]
                                 }
             except json.JSONDecodeError as e:
                 # do nothing
                 pass
         return cmd
 
+    def from_commands(self, cmds: list) -> list:
+        """
+        Unpack commands to execution list
+
+        :param cmds: commands list
+        :return parsed commands
+        """
+        commands = []
+        for cmd in cmds:
+            if 'cmd' in cmd:
+                commands.append(cmd)
+        return commands
+
     def unpack_tool_calls(self, tool_calls: list) -> list:
         """
         Unpack tool calls from OpenAI response
 
         :param tool_calls: tool calls list
         :return: parsed tool calls list
         """
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/ctx/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/ctx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import copy
 import datetime
 import uuid
 
 from packaging.version import Version
@@ -360,14 +360,23 @@
         :param reload: True if reload from provider
         :return: ctx metas dict
         """
         if reload:
             self.load_meta()
         return self.meta
 
+    def get_current_meta(self) -> CtxMeta or None:
+        """
+        Get current meta
+
+        :return: current meta
+        """
+        if self.current is not None:
+            return self.get_meta_by_id(self.current)
+
     def get_id_by_idx(self, idx: int) -> int:
         """
         Get ctx id (id) by index
 
         :param idx: index
         :return: ctx id
         """
@@ -594,14 +603,48 @@
         slave.root_id = master_ctx.meta_id
         slave.parent_id = master_ctx.meta_id
         slave.preset = preset_id
         id = self.provider.create(slave)
         slave.id = id
         return slave
 
+    def get_prev(self) -> int or None:
+        """
+        Get previous context
+
+        :return: previous context
+        """
+        if self.current is None:
+            return None
+        idx = self.get_idx_by_id(self.current)
+        if idx is not None:
+            if idx > 0:
+                return self.get_id_by_idx(idx - 1)
+
+    def get_next(self) -> int or None:
+        """
+        Get next context
+
+        :return: next context
+        """
+        if self.current is None:
+            return None
+        idx = self.get_idx_by_id(self.current)
+        if idx is not None:
+            if idx < self.count_meta() - 1:
+                return self.get_id_by_idx(idx + 1)
+
+    def get_last_meta(self) -> int or None:
+        """
+        Get last context
+
+        :return: last meta
+        """
+        return self.provider.get_last_meta_id()
+
     def count_history(
             self,
             history_items: list,
             model: str,
             mode: str,
             used_tokens: int = 100,
             max_tokens: int = 1000
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/ctx/idx.py` & `pygpt_net-2.2.8/src/pygpt_net/core/ctx/idx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/db/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/db/viewer.py` & `pygpt_net-2.2.8/src/pygpt_net/core/db/viewer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/agent.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/assistants.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/attachments.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/config.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/context.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/db.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/indexes.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/models.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/plugins.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/presets.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/debug/ui.py` & `pygpt_net-2.2.8/src/pygpt_net/core/debug/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/dispatcher.py` & `pygpt_net-2.2.8/src/pygpt_net/core/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,46 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import json
 
 from PySide6.QtWidgets import QApplication
 
 from pygpt_net.item.ctx import CtxItem
 
 
-class Event:
+class BaseEvent:
+    def __init__(
+            self,
+            name: str = None,
+            data: dict = None,
+            ctx: CtxItem = None
+    ):
+        """
+        Base Event object class
+
+        :param name: event name
+        :param data: event data
+        :param ctx: context instance
+        """
+        self.name = name
+        self.data = data
+        self.ctx = ctx  # CtxItem
+        self.stop = False  # True to stop propagation
+        self.internal = False
+
+
+class Event(BaseEvent):
 
     # Events
     AI_NAME = "ai.name"
     AUDIO_INPUT_RECORD_START = "audio.input.record.start"  # start audio input recording
     AUDIO_INPUT_RECORD_STOP = "audio.input.record.stop"  # stop audio input recording
     AUDIO_INPUT_RECORD_TOGGLE = "audio.input.record.toggle"  # toggle audio input recording
     AUDIO_INPUT_TRANSCRIBE = "audio.input.transcribe"  # transcribe audio file
@@ -65,14 +86,15 @@
         """
         Event object class
 
         :param name: event name
         :param data: event data
         :param ctx: context instance
         """
+        super(Event, self).__init__(name, data, ctx)
         self.name = name
         self.data = data
         self.ctx = ctx  # CtxItem
         self.stop = False  # True to stop propagation
         self.internal = False
         # internal event, not called from user
         # internal event is handled synchronously, ctx item has internal flag
@@ -111,15 +133,15 @@
         :param window: Window instance
         """
         self.window = window
         self.nolog_events = ["system.prompt"]
         self.reply_stack = []
         self.reply_ctx = None
 
-    def is_log(self, event: Event) -> bool:
+    def is_log(self, event: BaseEvent) -> bool:
         """
         Check if event can be logged
 
         :param event: event object
         :return: true if can be logged
         """
         if event.name in self.nolog_events:
@@ -159,29 +181,33 @@
             return False
         if len(ctx.cmds) > 1:  # if multiple commands then run synchronously
             return False
         return True
 
     def dispatch(
             self,
-            event: Event,
+            event: BaseEvent,
             all: bool = False
-    ) -> (list, Event):
+    ) -> (list, BaseEvent):
         """
         Dispatch event to plugins
 
         :param event: event to dispatch
         :param all: true if dispatch to all plugins (enabled or not)
         :return: list of affected plugins ids and event object
         """
         if self.is_log(event):
             self.window.core.debug.info("Dispatch event begin: " + event.name)
             if self.window.core.debug.enabled():
                 self.window.core.debug.debug("EVENT BEFORE: " + str(event))
 
+        # dispatch event to accessibility controller
+        self.window.controller.access.handle(event)
+
+        # dispatch event to plugins
         affected = []
         for id in self.window.core.plugins.plugins:
             if self.window.controller.plugins.is_enabled(id) or all:
                 if event.stop:
                     break
                 if self.window.core.debug.enabled() and self.is_log(event):
                     self.window.core.debug.debug("Apply [{}] to plugin: ".format(event.name) + id)
@@ -194,15 +220,15 @@
                 self.window.core.debug.debug("EVENT AFTER: " + str(event))
 
         return affected, event
 
     def apply(
             self,
             id: str,
-            event: Event
+            event: BaseEvent
     ):
         """
         Handle event in plugin with provided id
 
         :param id: plugin id
         :param event: event object
         """
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/experts/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/experts/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from pygpt_net.core.bridge import BridgeContext
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.item.preset import PresetItem
 
@@ -19,124 +19,153 @@
     def __init__(self, window=None):
         """
         Experts core
 
         :param window: Window instance
         """
         self.window = window
+        self.allowed_modes = ["chat", "completion", "vision", "langchain", "llama_index"]
+        self.allowed_cmds = ["expert_call"]
+
+    def get_mode(self) -> str:
+        """
+        Get sub-mode to use internally
+
+        :return: sub-mode
+        """
+        mode = "chat"
+        current = self.window.core.config.get("experts.mode")
+        if current is not None and current in self.allowed_modes:
+            mode = current
+        return mode
+
+    def stopped(self) -> bool:
+        """
+        Check if experts are stopped
+
+        :return: True if stopped
+        """
+        return self.window.controller.agent.experts.stopped()
+
+    def agent_enabled(self) -> bool:
+        """
+        Check if agent is enabled
+
+        :return: True if enabled
+        """
+        return self.window.controller.agent.enabled()
 
     def get_expert(self, id: str) -> PresetItem:
         """
         Get expert by id
 
         :param id: expert id
-        :return: expert item or None
+        :return: expert item (preset)
         """
         return self.window.core.presets.get_by_id("expert", id)
 
     def get_experts(self) -> dict:
         """
-        Get experts
+        Get experts names with keys
 
         :return: experts dict
         """
         experts = {}
         presets = self.window.core.presets.get_by_mode("expert")
 
         # mode: agent
-        if self.window.controller.agent.enabled():
+        if self.agent_enabled():
             agents = self.window.core.presets.get_by_mode("agent")
             agent = self.window.core.config.get('preset')
             if agent is not None:
                 if agent in agents:
                     for uuid in agents[agent].experts:
                         expert = self.window.core.presets.get_by_uuid(uuid)
                         if expert is not None:
                             id = expert.filename
                             experts[id] = expert.name
         # mode: expert
         else:
             for k in presets:
-                if k.startswith("current."):
+                if k.startswith("current."):  # skip current
                     continue
-                if not presets[k].enabled:
+                if not presets[k].enabled:  # skip disabled experts
                     continue
                 experts[k] = presets[k].name
         return experts
 
     def get_prompt(self) -> str:
         """
-        Get prompt from expert
+        Get prompt for handle experts
 
-        :return: prompt string with experts list
+        :return: prompt with list of experts appended
         """
         prompt = self.window.core.config.get('prompt.expert')
         experts = self.get_experts()
         experts_list = []
         for k in experts:
             if k.startswith("current."): # skip current presets
                 continue
             experts_list.append(" - " + str(k) + ": " + str(experts[k]))
         prompt = prompt.replace("{presets}", "\n".join(experts_list))
         return prompt
 
-    def extract_mentions(self, ctx: CtxItem) -> dict:
+    def extract_calls(self, ctx: CtxItem) -> dict:
         """
-        Extract mentions from context
+        Extract expert calls from context output
 
         :param ctx: context item
-        :return: dict with mentions
+        :return: dict with calls
         """
         ids = self.get_experts().keys()
-        if not ids:
+        if not ids:  # abort if no experts
             return {}
         cmds = self.window.core.command.extract_cmds(ctx.output)
         if len(cmds) > 0:
             ctx.cmds = cmds  # append commands to ctx
-        else:
+        else:  # abort if no cmds
             return {}
-        commands = self.window.controller.plugins.from_commands(cmds)  # pack to execution list
-        allowed_cmds = ["expert_call"]
+        commands = self.window.core.command.from_commands(cmds)  # pack to execution list
         is_cmd = False
         my_commands = []
-        mentions = {}
+        calls = {}
         for item in commands:
-            if item["cmd"] in allowed_cmds:
+            if item["cmd"] in self.allowed_cmds:
                 my_commands.append(item)
                 is_cmd = True
-        if not is_cmd:
+        if not is_cmd:  # abort if no expert calls
             return {}
         for item in my_commands:
             try:
                 if item["cmd"] == "expert_call":
                     if "params" not in item:
                         continue
                     if "id" not in item["params"] or "query" not in item["params"]:
                         continue
                     id = item["params"]["id"]
                     if id not in ids:
                         continue
                     query = item["params"]["query"]
-                    mentions[id] = query
+                    calls[id] = query
             except Exception as e:
                 self.window.core.debug.error(e)
                 return {}
-        return mentions
+        return calls
 
     def reply(self, ctx: CtxItem):
         """
-        Resend response to master expert
+        Re-send response from commands to master expert
 
         :param ctx: context item
-        :return: response text
         """
-        if self.window.controller.agent.experts.stopped():
+        if self.stopped():
             return
+
         internal = False
-        if self.window.controller.agent.enabled():  # hide in agent mode
+        if self.agent_enabled():  # hide in agent mode
             internal = True
         if ctx.output.strip() != "":
             response = ctx.output
         else:
             response = ctx.input
         self.window.controller.chat.input.send(
             "Result from expert:\n\n" + str(response),
@@ -146,59 +175,63 @@
             prev_ctx=ctx,
         )
 
     def call(
             self,
             master_ctx: CtxItem,
             expert_id: str,
-            text: str
+            query: str
     ):
         """
-        Call expert
+        Call the expert
 
         :param master_ctx: master context
         :param expert_id: expert id (preset ID)
-        :param text: input text (master prompt)
+        :param query: input text (master prompt)
         """
-        if self.window.controller.agent.experts.stopped():
+        if self.stopped():
             return
+
         # get or create children meta
         slave = self.window.core.ctx.get_or_create_slave_meta(master_ctx, expert_id)
         expert = self.get_expert(expert_id)
         reply = True
+        hidden = False
+        internal = False
 
-        mode = self.window.core.config.get("experts.mode")
+        if self.agent_enabled():  # hide in agent mode
+            internal = False
+            hidden = True
+
+        mode = self.get_mode()
         base_mode = mode
         model = expert.model
         user_name = expert.name
         ai_name = expert.name
         sys_prompt = expert.prompt
         model_data = self.window.core.models.get(model)
+
         files = []
         file_ids = []
         functions = []
         tools_outputs = []
+
+        # from current config
         max_tokens = self.window.core.config.get('max_output_tokens')
         stream_mode = self.window.core.config.get('stream')
 
-        hidden = False
-        internal = False
-        if self.window.controller.agent.enabled():  # hide in agent mode
-            internal = False
-            hidden = True
-
         # create slave item
         ctx = CtxItem()
         ctx.meta_id = slave.id
         ctx.internal = internal
         ctx.hidden = hidden
         ctx.current = True  # mark as current context item
         ctx.mode = mode  # store current selected mode (not inline changed)
         ctx.model = model  # store model list key, not real model id
-        ctx.set_input(text, user_name)
+        ctx.set_input(query, user_name)
         ctx.set_output(None, str(ai_name))
         ctx.sub_call = True  # mark as sub-call
 
         # render: begin
         self.window.controller.chat.render.begin(stream=stream_mode)
         self.window.core.ctx.provider.append_item(slave, ctx)  # to slave meta
 
@@ -215,39 +248,41 @@
             sys_prompt,
             ctx,
             reply,
             internal,
         )
 
         # call bridge
-        history = self.window.core.ctx.all(meta_id=slave.id)  # get all history for slave ctx
+        history = self.window.core.ctx.all(
+            meta_id=slave.id
+        )  # get history for slave ctx
         bridge_context = BridgeContext(
             ctx=ctx,
             history=history,
             mode=mode,
             parent_mode=base_mode,
             model=model_data,
             system_prompt=sys_prompt,
             system_prompt_raw=sys_prompt_raw,
-            prompt=text,
+            prompt=query,
             stream=stream_mode,
             attachments=files,
             file_ids=file_ids,
             assistant_id=self.window.core.config.get('assistant'),
             idx=self.window.controller.idx.current_idx,
             idx_raw=self.window.core.config.get('llama.idx.raw'),
             external_functions=functions,
             tools_outputs=tools_outputs,
             max_tokens=max_tokens,
         )
         self.window.controller.chat.common.lock_input()  # lock input
         result = self.window.core.bridge.call(
             context=bridge_context,
         )
-        if not result:
+        if not result:  # abort if bridge call failed
             return
 
         # handle output
         ctx.current = False  # reset current state
         self.window.core.ctx.update_item(ctx)
         ctx.from_previous()  # append previous result if exists
         self.window.controller.chat.output.handle(
@@ -256,15 +291,15 @@
             stream_mode,
         )
         ctx.clear_reply()  # reset results
         self.window.controller.chat.output.handle_cmd(ctx)  # handle cmds
         ctx.from_previous()  # append previous result again before save
         self.window.core.ctx.update_item(ctx)  # update ctx in DB
 
-        # if commands reply here, then stop
+        # if commands reply after bridge call, then stop (already handled in dispatcher)
         if ctx.reply:
             return
 
         # send slave expert response to master expert
         self.window.controller.chat.input.send(
             "@"+expert_id+" says:\n\n" + str(ctx.output),
             force=True,
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/actions.py` & `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/actions.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/editor.py` & `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/types.py` & `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/types.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/url.py` & `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/url.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/history.py` & `pygpt_net-2.2.8/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/chat.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/context.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/indexing.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/indexing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/llm.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/llm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/metadata.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/metadata.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/types/ctx.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/types/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/types/external.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/types/external.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/types/files.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/types/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/idx/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/core/idx/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/image.py` & `pygpt_net-2.2.8/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/info.py` & `pygpt_net-2.2.8/src/pygpt_net/core/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/installer.py` & `pygpt_net-2.2.8/src/pygpt_net/core/installer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/llm/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/locale.py` & `pygpt_net-2.2.8/src/pygpt_net/core/locale.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/models.py` & `pygpt_net-2.2.8/src/pygpt_net/core/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/modes.py` & `pygpt_net-2.2.8/src/pygpt_net/core/modes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/notepad.py` & `pygpt_net-2.2.8/src/pygpt_net/core/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/platforms.py` & `pygpt_net-2.2.8/src/pygpt_net/core/platforms.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/plugins.py` & `pygpt_net-2.2.8/src/pygpt_net/core/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/presets.py` & `pygpt_net-2.2.8/src/pygpt_net/core/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/profile.py` & `pygpt_net-2.2.8/src/pygpt_net/core/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/prompt/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/prompt/template.py` & `pygpt_net-2.2.8/src/pygpt_net/core/prompt/template.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/render/base.py` & `pygpt_net-2.2.8/src/pygpt_net/core/render/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/parser.py` & `pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/renderer.py` & `pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/render/plain/renderer.py` & `pygpt_net-2.2.8/src/pygpt_net/core/render/plain/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/render/web/parser.py` & `pygpt_net-2.2.8/src/pygpt_net/core/render/web/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/render/web/renderer.py` & `pygpt_net-2.2.8/src/pygpt_net/core/render/web/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/settings.py` & `pygpt_net-2.2.8/src/pygpt_net/core/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/text/finder.py` & `pygpt_net-2.2.8/src/pygpt_net/core/text/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/text/utils.py` & `pygpt_net-2.2.8/src/pygpt_net/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/text/web_finder.py` & `pygpt_net-2.2.8/src/pygpt_net/core/text/web_finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/tokens.py` & `pygpt_net-2.2.8/src/pygpt_net/core/tokens.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/updater/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/core/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/web.py` & `pygpt_net-2.2.8/src/pygpt_net/core/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/core/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/core/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/config/config.json` & `pygpt_net-2.2.8/src/pygpt_net/data/config/config.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9623493975903614%*

 * *Differences: {"'__meta__'": "{'version': '2.2.8', 'app.version': '2.2.8', 'updated_at': '2024-05-02T00:00:00'}",*

 * * "'access.audio.event.speech'": 'False',*

 * * "'access.audio.notify.execute'": 'True',*

 * * "'access.microphone.notify'": 'True',*

 * * "'access.shortcuts'": "[OrderedDict([('action', 'voice_cmd.toggle'), ('key', 'Space'), "*

 * *                       "('key_modifier', 'Control'), ('voice_command', '')]), "*

 * *                       "OrderedDict([('action', 'tab.chat'), ('key', '1'), ('key_modifier', "*

 * *                       "'C […]*

```diff
@@ -1,13 +1,51 @@
 {
     "__meta__": {
-        "app.version": "2.2.7",
-        "updated_at": "2024-05-01T00:00:00",
-        "version": "2.2.7"
+        "app.version": "2.2.8",
+        "updated_at": "2024-05-02T00:00:00",
+        "version": "2.2.8"
     },
+    "access.audio.event.speech": false,
+    "access.audio.notify.execute": true,
+    "access.microphone.notify": true,
+    "access.shortcuts": [
+        {
+            "action": "voice_cmd.toggle",
+            "key": "Space",
+            "key_modifier": "Control",
+            "voice_command": ""
+        },
+        {
+            "action": "tab.chat",
+            "key": "1",
+            "key_modifier": "Control"
+        },
+        {
+            "action": "tab.files",
+            "key": "2",
+            "key_modifier": "Control"
+        },
+        {
+            "action": "tab.calendar",
+            "key": "3",
+            "key_modifier": "Control"
+        },
+        {
+            "action": "tab.draw",
+            "key": "4",
+            "key_modifier": "Control"
+        },
+        {
+            "action": "tab.notepad",
+            "key": "5",
+            "key_modifier": "Control"
+        }
+    ],
+    "access.voice_control": false,
+    "access.voice_control.model": "gpt-3.5-turbo",
     "agent.auto_stop": true,
     "agent.goal.notify": true,
     "agent.idx": "base",
     "agent.iterations": 3,
     "agent.mode": "chat",
     "ai_name": "",
     "api_endpoint": "https://api.openai.com/v1",
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/config/models.json` & `pygpt_net-2.2.8/src/pygpt_net/data/config/models.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'__meta__'": "{'version': '2.2.8', 'app.version': '2.2.8', 'updated_at': '2024-05-02T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.7",
-        "updated_at": "2024-05-01T00:00:00",
-        "version": "2.2.7"
+        "app.version": "2.2.8",
+        "updated_at": "2024-05-02T00:00:00",
+        "version": "2.2.8"
     },
     "items": {
         "dall-e-2": {
             "ctx": 0,
             "default": false,
             "id": "dall-e-2",
             "langchain": {
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/config/modes.json` & `pygpt_net-2.2.8/src/pygpt_net/data/config/modes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'__meta__'": "{'version': '2.2.8', 'app.version': '2.2.8', 'updated_at': '2024-05-02T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.7",
-        "updated_at": "2024-05-01T00:00:00",
-        "version": "2.2.7"
+        "app.version": "2.2.8",
+        "updated_at": "2024-05-02T00:00:00",
+        "version": "2.2.8"
     },
     "items": {
         "agent": {
             "default": false,
             "id": "agent",
             "label": "mode.agent",
             "name": "Agent (autonomous)"
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/config/presets/batman_and_joker.json` & `pygpt_net-2.2.8/src/pygpt_net/data/config/presets/batman_and_joker.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/config/presets/dalle_white_cat.json` & `pygpt_net-2.2.8/src/pygpt_net/data/config/presets/dalle_white_cat.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/config/presets/joke_expert.json` & `pygpt_net-2.2.8/src/pygpt_net/data/config/presets/joke_expert.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/config/settings.json` & `pygpt_net-2.2.8/src/pygpt_net/data/config/settings.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9405940594059405%*

 * *Differences: {"'access.audio.event.speech'": "OrderedDict([('section', 'access'), ('type', 'bool'), ('slider', "*

 * *                                "False), ('label', 'settings.access.audio.event.speech'), "*

 * *                                "('value', False), ('min', None), ('max', None), ('multiplier', "*

 * *                                "None), ('step', None), ('advanced', False)])",*

 * * "'access.audio.notify.execute'": "OrderedDict([('section', 'access'), ('type', 'bool'), "*

 * *                                  "('slider', False […]*

```diff
@@ -1,8 +1,100 @@
 {
+    "access.audio.event.speech": {
+        "advanced": false,
+        "label": "settings.access.audio.event.speech",
+        "max": null,
+        "min": null,
+        "multiplier": null,
+        "section": "access",
+        "slider": false,
+        "step": null,
+        "type": "bool",
+        "value": false
+    },
+    "access.audio.notify.execute": {
+        "advanced": false,
+        "label": "settings.access.audio.notify.execute",
+        "max": null,
+        "min": null,
+        "multiplier": null,
+        "section": "access",
+        "slider": false,
+        "step": null,
+        "type": "bool",
+        "value": false
+    },
+    "access.microphone.notify": {
+        "advanced": false,
+        "label": "settings.access.microphone.notify",
+        "max": null,
+        "min": null,
+        "multiplier": null,
+        "section": "access",
+        "slider": false,
+        "step": null,
+        "type": "bool",
+        "value": false
+    },
+    "access.shortcuts": {
+        "advanced": false,
+        "description": "settings.access.shortcuts.desc",
+        "keys": {
+            "action": {
+                "type": "combo",
+                "use": "access_actions"
+            },
+            "key": {
+                "type": "combo",
+                "use": "keys"
+            },
+            "key_modifier": {
+                "type": "combo",
+                "use": "keys_modifiers"
+            }
+        },
+        "label": "settings.access.shortcuts",
+        "max": null,
+        "min": null,
+        "multiplier": null,
+        "section": "access",
+        "slider": false,
+        "step": null,
+        "type": "dict",
+        "value": []
+    },
+    "access.voice_control": {
+        "advanced": false,
+        "label": "settings.access.voice_control",
+        "max": null,
+        "min": null,
+        "multiplier": null,
+        "section": "access",
+        "slider": false,
+        "step": null,
+        "type": "bool",
+        "urls": {
+            "List of commands": "https://pygpt.readthedocs.io/en/latest/accessibility.html"
+        },
+        "value": false
+    },
+    "access.voice_control.model": {
+        "advanced": false,
+        "description": "settings.access.voice_control.model.desc",
+        "label": "settings.access.voice_control.model",
+        "max": null,
+        "min": null,
+        "multiplier": null,
+        "section": "access",
+        "slider": false,
+        "step": null,
+        "type": "combo",
+        "use": "models",
+        "value": "gpt-3.5-turbo"
+    },
     "agent.goal.notify": {
         "advanced": false,
         "label": "settings.agent.goal.notify",
         "max": 0,
         "min": 0,
         "multiplier": 1,
         "section": "agent",
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/config/settings_section.json` & `pygpt_net-2.2.8/src/pygpt_net/data/config/settings_section.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9230769230769231%*

 * *Differences: {"'access'": "OrderedDict([('label', 'settings.section.access')])"}*

```diff
@@ -1,8 +1,11 @@
 {
+    "access": {
+        "label": "settings.section.access"
+    },
     "agent": {
         "label": "settings.section.agent"
     },
     "ctx": {
         "label": "settings.section.ctx"
     },
     "developer": {
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/css/fix_windows.css` & `pygpt_net-2.2.8/src/pygpt_net/data/css/fix_windows.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.css` & `pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.dark.css` & `pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.light.css` & `pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/css/style.dark.css` & `pygpt_net-2.2.8/src/pygpt_net/data/css/style.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/css/style.light.css` & `pygpt_net-2.2.8/src/pygpt_net/data/css/style.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/css/web.css` & `pygpt_net-2.2.8/src/pygpt_net/data/css/web.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/css/web.dark.css` & `pygpt_net-2.2.8/src/pygpt_net/data/css/web.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/css/web.light.css` & `pygpt_net-2.2.8/src/pygpt_net/data/css/web.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/OFL.txt` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/OFL.txt` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf` & `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icon.ico` & `pygpt_net-2.2.8/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icon.png` & `pygpt_net-2.2.8/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_busy.ico` & `pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_busy.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_error.ico` & `pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_error.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_idle.ico` & `pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_idle.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/abc.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/abc.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/alarm.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/apps.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/apps.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/build.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/build.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/calendar.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/calendar.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/audio.png` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/audio.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/copy.png` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/copy.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/delete.png` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/delete.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/edit.png` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/edit.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/join.png` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/join.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/reload.png` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/reload.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/cut.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/cut.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/db.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/db.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/error.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/error.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/hearing.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/hearing.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/help.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/info.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/key.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/key.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/keyboard.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/keyboard.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/language.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/language.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/palette.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/palette.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/public_filled.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/public_filled.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/robot.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/router.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/router.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/sensors.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/sensors.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/settings.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/share.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/share.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/view.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/view.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/icons/voice.svg` & `pygpt_net-2.2.8/src/pygpt_net/data/icons/voice.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.de.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.de.ini`

 * *Files 5% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 attachments_uploaded.btn.sync = Synchronisieren
 attachments_uploaded.btn.sync.current = Nur aktuell
 attachments_uploaded.btn.sync.all = Alle Speicher
 attachments_uploaded.clear.confirm = WARNUNG: Sind Sie sicher, dass Sie alle diese Dateien vom Remote-Server löschen möchten?
 attachments_uploaded.delete.confirm = WARNUNG: Sind Sie sicher, dass Sie die Datei vom Remote-Server löschen möchten?
 attachments_uploaded.sync.tip = Tipp: Klicken Sie auf 'Synchronisieren', um die Dateiliste von OpenAI abzurufen
 attachments_uploaded.tab = Hochgeladene Dateien
+audio.control.btn = Sprachsteuerung
 audio.magic_word.detected = Zauberwort erkannt!
 audio.magic_word.invalid = Kein Zauberwort :(
 audio.magic_word.please = Bitte das Zauberwort...
 audio.speak.btn = Mikrofon
 audio.speak.btn.stop = Stopp
 audio.speak.btn.tooltip = Klicken, um das Mikrofonhören zu starten
 audio.speak.btn.stop.tooltip = Klicken, um das Mikrofonhören zu beenden
@@ -320,20 +321,88 @@
 dialog.workdir.title = Arbeitsverzeichnis ändern
 dialog.workdir.result.no_free_space = Zu wenig Speicherplatz auf der Festplatte! Erforderlich: {required}, Freier Speicherplatz: {free}.
 dialog.workdir.result.same_directory = Nichts zu verschieben.
 dialog.workdir.result.success = [OK] Das Arbeitsverzeichnis ist derzeit gesetzt auf: {path}
 dialog.workdir.result.failed = Ein Fehler ist aufgetreten beim Verschieben des Arbeitsverzeichnisses.
 dialog.workdir.result.wait = Bitte warten... das aktuelle Arbeitsverzeichnis wird verschoben... Dies kann eine Weile dauern...
 dialog.workdir.result.directory_not_exists = Zielverzeichnis existiert nicht!
+dictionary.config.access.shortcuts.action = Auszulösende Aktion
+dictionary.config.access.shortcuts.key = Tastaturtaste
+dictionary.config.access.shortcuts.key_modifier = Tastaturmodifikator
 dt.days_ago = vor Tagen
 dt.month = vor einem Monat
 dt.today = heute
 dt.week = vor einer Woche
 dt.weeks = vor Wochen
 dt.yesterday = gestern
+event.audio.app.started = Willkommen!
+event.audio.app.status = Aktueller Modus: {mode}.\nAktuelles Gespräch: {ctx}, zuletzt aktualisiert {last}.\nGesamtzahl der Gespräche: {total}.
+event.audio.ctx.created = Neuer Kontext wurde erstellt.
+event.audio.ctx.current = Aktuelles Gespräch: {ctx}, zuletzt aktualisiert: {last}.
+event.audio.ctx.last = Ihre Eingabe: {input}. KI-Antwort: {output}.
+event.audio.ctx.end = Beendet.
+event.audio.ctx.selected = Ausgewählter Kontext: {ctx}.
+event.audio.ctx.attachments.clear = Anhangsliste leer.
+event.audio.camera.enabled = Kamera aktiviert.
+event.audio.camera.disabled = Kamera deaktiviert.
+event.audio.camera.captured = Bild wurde von der Kamera aufgenommen.
+event.audio.output.enable = Audioausgabe aktiviert.
+event.audio.output.disable = Audioausgabe deaktiviert.
+event.audio.input.append = Text zur Eingabe hinzugefügt.
+event.audio.input.call = Eingabe aufrufen.
+event.audio.input.enable = Audioeingabe aktiviert.
+event.audio.input.disable = Audioeingabe aktiviert.
+event.audio.input.error = Fehler beim Senden der Eingabe aufgetreten.
+event.audio.input.sent = Eingabe gesendet.
+event.audio.input.stopped = Eingabe gestoppt.
+event.audio.input.voice.listen.started = Abhören. Bitte sprechen Sie jetzt.
+event.audio.input.voice.listen.stopped = Zuhören wurde gestoppt.
+event.audio.note.add = Notiz zum Notizblock hinzugefügt.
+event.audio.tab.switch = Ausgewählter Tab ist: {tab}.
+event.audio.voice.control.toggle = Sprachsteuerung wurde umgeschaltet.
+event.audio.voice.control.started = Sprachsteuerung aktiviert.
+event.audio.voice.control.stopped = Sprachsteuerung deaktiviert.
+event.audio.voice.control.sent = OK.
+event.audio.voice.control.unrecognized = Befehl nicht erkannt.
+event.control.app.status = App: Status
+event.control.app.exit = App: Beenden
+event.control.audio.output.enable = Audioausgang: Aktivieren
+event.control.audio.output.disable = Audioausgang: Deaktivieren
+event.control.audio.input.enable = Audioeingang: Aktivieren
+event.control.audio.input.disable = Audioeingang: Deaktivieren
+event.control.camera.enable = Kamera: Aktivieren
+event.control.camera.disable = Kamera: Deaktivieren
+event.control.camera.capture = Kamera: Aufnehmen
+event.control.ctx.new = Kontext: Neu
+event.control.ctx.prev = Kontext: Zurück
+event.control.ctx.next = Kontext: Weiter
+event.control.ctx.last = Kontext: Letzter
+event.control.ctx.input.focus = Eingabe: Fokus
+event.control.ctx.input.send = Eingabe: Senden
+event.control.ctx.input.clear = Eingabe: Löschen
+event.control.ctx.stop = Eingabe: Stoppen
+event.control.ctx.attachments.clear = Anhänge: Löschen
+event.control.input.sent = Eingabe gesendet.
+event.control.input.stopped = Eingabe gestoppt.
+event.control.mode.chat = Modus: Chat
+event.control.mode.llama_index = Modus: Chat mit Dateien
+event.control.note.add = Notiz zum Notizblock hinzugefügt.
+event.control.tab.chat = Tab: Chat
+event.control.tab.calendar = Tab: Kalender
+event.control.tab.draw = Tab: Zeichnen
+event.control.tab.files = Tab: Dateien
+event.control.tab.notepad = Tab: Notizblock
+event.control.tab.next = Tab: Nächster
+event.control.tab.prev = Tab: Vorheriger
+event.control.voice_msg.start = Spracheingabe: Start
+event.control.voice_msg.stop = Spracheingabe: Stopp
+event.control.voice_msg.toggle = Spracheingabe: Umschalten
+event.control.voice_cmd.start = Sprachsteuerung: Start
+event.control.voice_cmd.stop = Sprachsteuerung: Stopp
+event.control.voice_cmd.toggle = Sprachsteuerung: Umschalten
 error.assistant_not_selected = Bitte erstellen, importieren oder wählen Sie zuerst einen Assistenten aus!
 files.local.upload = Dateien hochladen
 files.local.dir.prefix = Verzeichnis
 files.delete.confirm = Datei/Verzeichnis löschen?
 files.delete.recursive.confirm = Verzeichnis ist nicht leer! Sind Sie sicher, dass Sie das Verzeichnis und alle Dateien darin löschen möchten?
 files.explorer.header.name = Name
 files.explorer.header.size = Größe
@@ -405,14 +474,15 @@
 interpreter.edit_label.output = Ausgabe
 interpreter.edit = Bearbeitungsmodus
 interpreter.input.placeholder = Auszuführender Python-Code...
 menu.audio = Audio / Stimme
 menu.audio.input = Eingabe: Spracherkennung
 menu.audio.output = Ausgabe: Sprachsynthese
 menu.config = Konfiguration
+menu.config.access = Barrierefreiheit
 menu.config.edit.config = config.json bearbeiten...
 menu.config.edit.models = models.json bearbeiten...
 menu.config.edit.css = CSS-Stylesheets bearbeiten...
 menu.config.edit.css.restore = Standard-CSS wiederherstellen...
 menu.config.open_dir = Arbeitsverzeichnis öffnen...
 menu.config.change_dir = Arbeitsverzeichnis ändern...
 menu.config.profile = Profil
@@ -543,14 +613,22 @@
 preset.temperature = Temperatur
 preset.untitled = (unbetitelt)
 preset.use = Verwenden
 preset.user_name = Benutzername
 preset.vision = Vision
 profile.current.suffix = (aktuell)
 screenshot.capture.name.prefix = Screenshot von
+settings.access.voice_control = Sprachsteuerung aktivieren (mittels Mikrofon)
+settings.access.voice_control.model = Modell
+settings.access.voice_control.model.desc = Modell zur Befehlserkennung in der Sprachsteuerung verwenden
+settings.access.audio.event.speech = Sprachsynthese zur Beschreibung von Ereignissen auf dem Bildschirm verwenden.
+settings.access.audio.notify.execute = Audio-Benachrichtigung bei Ausführung von Sprachbefehlen
+settings.access.microphone.notify = Audio-Benachrichtigung bei Start/Stop der Mikrofonaufzeichnung
+settings.access.shortcuts = Steuerungstastenkürzel
+settings.access.shortcuts.desc = Tastenkürzel und Sprachbefehle einrichten, um die Anwendung mittels Sprache und Mikrofon zu steuern.
 settings.advanced.collapse = Erweiterte Optionen ein-/ausblenden
 settings.agent.mode = Interner Modus
 settings.agent.mode.desc = Interner Modus für die Verwendung im Agentenmodus (Chat, Vervollständigung, Langchain, Llama_Index usw.)
 settings.agent.goal.notify = Zeige eine Benachrichtigung im Infobereich an, wenn das Ziel erreicht ist.
 settings.agent.idx = Index
 settings.agent.idx.desc = Nur wenn der interne Modus Llama_Index ist (Chat mit Dateien), wählen Sie den Index für die Verwendung im Agentenmodus
 settings.api_endpoint = API-Endpunkt
@@ -645,15 +723,16 @@
 settings.prompt.expert = Experte: Masteraufforderung
 settings.prompt.expert.desc = Anweisung (Systemaufforderung) für den Master-Experten, wie man Sklavenexperten handhabt. Anweisungen für Sklavenexperten werden aus ihren Voreinstellungen gegeben.
 settings.prompt.img = DALL-E: Bildgenerierung
 settings.prompt.img.desc = Aufforderung zur Erzeugung von Anweisungen für DALL-E (falls Rohmodus deaktiviert ist). Nur im Bildmodus.
 settings.render.code_syntax = Stil der Syntaxhervorhebung für Code
 settings.render.plain = Markdown-Formatierung in der Ausgabe deaktivieren (RAW-Textmodus)
 settings.restart.required = Ein Neustart der Anwendung ist notwendig, damit die Änderungen für diese Option übernommen werden.
-settings.section.agent = Agent (autonom)
+settings.section.access = Barrierefreiheit
+settings.section.agent = Agenten und Experten
 settings.section.files = Dateien und Anhänge
 settings.section.general = Allgemein
 settings.section.layout = Layout
 settings.section.ctx = Kontext
 settings.section.model = Modelle
 settings.section.images = Bilder
 settings.section.updates = Aktualisierungen
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.en.ini`

 * *Files 6% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 attachments_uploaded.btn.sync = Sync
 attachments_uploaded.btn.sync.current = Current only
 attachments_uploaded.btn.sync.all = All stores
 attachments_uploaded.clear.confirm = WARNING: are you sure to delete all this files from remote server?
 attachments_uploaded.delete.confirm = WARNING: are you sure to delete file from remote server?
 attachments_uploaded.sync.tip = Tip: click on 'Sync' to retrieve files list from OpenAI
 attachments_uploaded.tab = Uploaded files
+audio.control.btn = Voice control
 audio.magic_word.detected = Magic word detected!
 audio.magic_word.invalid = Not a magic word :(
 audio.magic_word.please = Magic word please...
 audio.speak.btn = Microphone
 audio.speak.btn.stop = Stop
 audio.speak.btn.tooltip = Click to start microphone listening
 audio.speak.btn.stop.tooltip = Click to stop microphone listening
@@ -350,14 +351,17 @@
 dictionary.assistant.tool.function.name = Function name
 dictionary.assistant.tool.function.params = Function params (JSON object)
 dictionary.assistant.tool.function.desc = Description (optional)
 dictionary.cmd.param.name = Param name
 dictionary.cmd.param.type = Param type
 dictionary.cmd.param.description = Description (optional)
 dictionary.cmd.param.required = Required (optional)
+dictionary.config.access.shortcuts.action = Action to trigger
+dictionary.config.access.shortcuts.key = Keyboard key
+dictionary.config.access.shortcuts.key_modifier = Keyboard modifier
 dictionary.config.llama.idx.custom_meta.extensions = File extension(s), separated by comma. Use * (asterisk) as extension if you want to apply field to all files
 dictionary.config.llama.idx.custom_meta.key = Metadata key (field name)
 dictionary.config.llama.idx.custom_meta.value = Metadata value. Allowed placeholders: {path}, {relative_path} {filename}, {dirname}, {relative_dir} {ext}, {size}, {mtime}, {date}, {date_time}, {time}, {timestamp}. Set empty value to remove field with specified key from metadata.
 dictionary.config.llama.idx.custom_meta.web.loader = Data type (loader)
 dictionary.config.llama.idx.custom_meta.web.key = Metadata key (field name)
 dictionary.config.llama.idx.custom_meta.web.value = Metadata value. Allowed placeholders: {mtime}, {date}, {date_time}, {time}, {timestamp} + {data loader args}
 dictionary.config.llama.idx.embeddings.env.name = ENV name (to set with os.environ)
@@ -430,14 +434,79 @@
 dt.days_ago = days ago
 dt.month = month ago
 dt.today = today
 dt.week = week ago
 dt.weeks = weeks ago
 dt.yesterday = yesterday
 error.assistant_not_selected = Please create, import or select assistant at first!
+event.audio.app.started = Welcome!
+event.audio.app.status = Current mode: {mode}.\nCurrent conversation: {ctx}, last updated {last}.\nTotal conversations: {total}.
+event.audio.ctx.created = New context has been created.
+event.audio.ctx.current = Current conversation: {ctx}, last updated: {last}.
+event.audio.ctx.last = Your input: {input}. AI response: {output}.
+event.audio.ctx.end = Finished.
+event.audio.ctx.selected = Selected context: {ctx}.
+event.audio.ctx.attachments.clear = Attachments list empty.
+event.audio.camera.enabled = Camera enabled.
+event.audio.camera.disabled = Camera disabled.
+event.audio.camera.captured = Image has been captured from camera.
+event.audio.output.enable = Audio output enabled.
+event.audio.output.disable = Audio output disabled.
+event.audio.input.append = Text appended to input.
+event.audio.input.call = Input call.
+event.audio.input.enable = Audio input enabled.
+event.audio.input.disable = Audio input enabled.
+event.audio.input.error = Error occurred during sending input.
+event.audio.input.sent = Input sent.
+event.audio.input.stopped = Input stopped.
+event.audio.input.voice.listen.started = Listening. Please speak now.
+event.audio.input.voice.listen.stopped = Listening has been stopped.
+event.audio.note.add = Note added to notepad.
+event.audio.tab.switch = Selected Tab is: {tab}.
+event.audio.voice.control.toggle = Voice control has been toggled.
+event.audio.voice.control.started = Voice control activated.
+event.audio.voice.control.stopped = Voice control deactivated.
+event.audio.voice.control.sent = OK.
+event.audio.voice.control.unrecognized = Unrecognized command.
+event.control.app.status = App: Status
+event.control.app.exit = App: Exit
+event.control.audio.output.enable = Audio output: Enable
+event.control.audio.output.disable = Audio output: Disable
+event.control.audio.input.enable = Audio input: Enable
+event.control.audio.input.disable = Audio input: Disable
+event.control.camera.enable = Camera: Enable
+event.control.camera.disable = Camera: Disable
+event.control.camera.capture = Camera: Capture
+event.control.ctx.new = Context: New
+event.control.ctx.prev = Context: Prev
+event.control.ctx.next = Context: Next
+event.control.ctx.last = Context: Last
+event.control.ctx.input.focus = Input: Focus
+event.control.ctx.input.send = Input: Send
+event.control.ctx.input.clear = Input: Clear
+event.control.ctx.stop = Input: Stop
+event.control.ctx.attachments.clear = Attachments: Clear
+event.control.input.sent = Input sent.
+event.control.input.stopped = Input stopped.
+event.control.mode.chat = Mode: Chat
+event.control.mode.llama_index = Mode: Chat with files
+event.control.note.add = Note added to notepad.
+event.control.tab.chat = Tab: Chat
+event.control.tab.calendar = Tab: Calendar
+event.control.tab.draw = Tab: Draw
+event.control.tab.files = Tab: Files
+event.control.tab.notepad = Tab: Notepad
+event.control.tab.next = Tab: Next
+event.control.tab.prev = Tab: Prev
+event.control.voice_msg.start = Voice input: Start
+event.control.voice_msg.stop = Voice input: Stop
+event.control.voice_msg.toggle = Voice input: Toggle
+event.control.voice_cmd.start = Voice control: Start
+event.control.voice_cmd.stop = Voice control: Stop
+event.control.voice_cmd.toggle = Voice control: Toggle
 files.local.upload = Upload files
 files.local.dir.prefix = Path
 files.delete.confirm = Delete file/directory?
 files.delete.recursive.confirm = Directory is not empty! Are you sure you want to delete the directory and all the files in it?
 files.explorer.header.name = Name
 files.explorer.header.size = Size
 files.explorer.header.type = Type
@@ -510,14 +579,15 @@
 interpreter.edit_label.output = Output
 interpreter.edit = Edit mode
 interpreter.input.placeholder = Python code to execute...
 menu.audio = Audio / Voice
 menu.audio.input = Input: speech recognition
 menu.audio.output = Output: speech synthesis
 menu.config = Config
+menu.config.access = Accessibility
 menu.config.edit.config = Edit config.json...
 menu.config.edit.models = Edit models.json...
 menu.config.edit.css = Edit CSS stylesheets...
 menu.config.edit.css.restore = Restore default CSS...
 menu.config.edit.json = Edit JSON configs...
 menu.config.models = Models...
 menu.config.open_dir = Open working directory...
@@ -678,14 +748,22 @@
 preset.untitled = (untitled)
 preset.use = Use
 preset.user_name = User name
 preset.vision = Vision
 profile.current.suffix = (current)
 screenshot.capture.name.prefix = Screenshot from
 settings.advanced.collapse = Show/hide advanced options
+settings.access.voice_control = Enable voice control (using microphone)
+settings.access.voice_control.model = Model
+settings.access.voice_control.model.desc = Model to use for command recognition in voice control
+settings.access.audio.event.speech = Use voice synthesis to describe events on the screen.
+settings.access.audio.notify.execute = Audio notify voice command execution
+settings.access.microphone.notify = Audio notify microphone listening start/stop
+settings.access.shortcuts = Control shortcut keys
+settings.access.shortcuts.desc = Setup keyboard shortcuts and voice commands to control the application using voice and microphone.
 settings.agent.mode = Sub-mode to use
 settings.agent.mode.desc = Sub-mode to use in Agent mode (chat, completion, langchain, llama_index, etc.)
 settings.agent.goal.notify = Display a tray notification when the goal is achieved.
 settings.agent.idx = Index to use
 settings.agent.idx.desc = Only if sub-mode is llama_index (Chat with files), choose the index to use in Agent mode
 settings.api_endpoint = API Endpoint
 settings.api_endpoint.desc = OpenAI API endpoint URL, default: https://api.openai.com/v1
@@ -812,15 +890,16 @@
 settings.prompt.img.desc = Prompt for generating prompts for DALL-E (if raw-mode is disabled). Image mode only.
 settings.render.engine = Rendering engine
 settings.render.open_gl = OpenGL hardware acceleration
 settings.render.web.only.desc = WebEngine / Chromium rendering engine only
 settings.render.code_syntax = Code syntax highlight
 settings.render.plain = Disable markdown formatting in output (RAW plain text mode)
 settings.restart.required = Restart of the application is required for this option to take effect.
-settings.section.agent = Agent (autonomous)
+settings.section.access = Accessibility
+settings.section.agent = Agents and experts
 settings.section.files = Files and attachments
 settings.section.general = General
 settings.section.layout = Layout
 settings.section.llama_index = Indexes (llama-index)
 settings.section.ctx = Context
 settings.section.developer = Developer
 settings.section.model = Models
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.es.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.es.ini`

 * *Files 9% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 attachments_uploaded.btn.sync = Sincronizar
 attachments_uploaded.btn.sync.current = Solo actual
 attachments_uploaded.btn.sync.all = Todas las bases
 attachments_uploaded.clear.confirm = ADVERTENCIA: ¿Está seguro de querer eliminar todos estos archivos del servidor remoto?
 attachments_uploaded.delete.confirm = ADVERTENCIA: ¿Está seguro de querer eliminar archivo del servidor remoto?
 attachments_uploaded.sync.tip = Consejo: clic en 'Sincronizar' para obtener la lista de archivos de OpenAI
 attachments_uploaded.tab = Archivos subidos
+audio.control.btn = Control de voz
 audio.magic_word.detected = ¡Palabra mágica detectada!
 audio.magic_word.invalid = No es una palabra mágica :(
 audio.magic_word.please = Por favor, una palabra mágica...
 audio.speak.btn = Micrófono
 audio.speak.btn.stop = Detener
 audio.speak.btn.tooltip = Haz clic para empezar a escuchar a través del micrófono
 audio.speak.btn.stop.tooltip = Haz clic para dejar de escuchar a través del micrófono
@@ -326,14 +327,82 @@
 dialog.workdir.result.directory_not_exists = ¡El directorio de destino no existe!
 dt.days_ago = hace días
 dt.month = hace un mes
 dt.today = hoy
 dt.week = hace una semana
 dt.weeks = hace semanas
 dt.yesterday = ayer
+dictionary.config.access.shortcuts.action = Acción a desencadenar
+dictionary.config.access.shortcuts.key = Tecla del teclado
+dictionary.config.access.shortcuts.key_modifier = Modificador del teclado
+event.audio.app.started = ¡Bienvenido!
+event.audio.app.status = Modo actual: {mode}.\nConversación actual: {ctx}, última actualización {last}.\nTotal de conversaciones: {total}.
+event.audio.ctx.created = Se ha creado un nuevo contexto.
+event.audio.ctx.current = Conversación actual: {ctx}, última actualización: {last}.
+event.audio.ctx.last = Tu entrada: {input}. Respuesta de la IA: {output}.
+event.audio.ctx.end = Finalizado.
+event.audio.ctx.selected = Contexto seleccionado: {ctx}.
+event.audio.ctx.attachments.clear = Lista de adjuntos vacía.
+event.audio.camera.enabled = Cámara activada.
+event.audio.camera.disabled = Cámara desactivada.
+event.audio.camera.captured = Se ha capturado una imagen de la cámara.
+event.audio.output.enable = Salida de audio habilitada.
+event.audio.output.disable = salida de audio deshabilitada.
+event.audio.input.append = Texto anexado a la entrada.
+event.audio.input.call = Llamada de entrada.
+event.audio.input.enable = Entrada de audio habilitada.
+event.audio.input.disable = Entrada de audio deshabilitada.
+event.audio.input.error = Error ocurrido durante el envío de la entrada.
+event.audio.input.sent = Entrada enviada.
+event.audio.input.stopped = Entrada detenida.
+event.audio.input.voice.listen.started = Escuchando. Por favor habla ahora.
+event.audio.input.voice.listen.stopped = La escucha ha sido detenida.
+event.audio.note.add = Nota añad
+event.audio.tab.switch = Pestaña seleccionada: {tab}.
+event.audio.voice.control.toggle = Control de voz conmutado.
+event.audio.voice.control.started = Control de voz activado.
+event.audio.voice.control.stopped = Control de voz desactivado.
+event.audio.voice.control.sent = OK.
+event.audio.voice.control.unrecognized = Comando no reconocido.
+event.control.app.status = Aplicación: Estado
+event.control.app.exit = Aplicación: Salir
+event.control.audio.output.enable = Salida de audio: Habilitar
+event.control.audio.output.disable = Salida de audio: Deshabilitar
+event.control.audio.input.enable = Entrada de audio: Habilitar
+event.control.audio.input.disable = Entrada de audio: Deshabilitar
+event.control.camera.enable = Cámara: Habilitar
+event.control.camera.disable = Cámara: Deshabilitar
+event.control.camera.capture = Cámara: Capturar
+event.control.ctx.new = Contexto: Nuevo
+event.control.ctx.prev = Contexto: Anterior
+event.control.ctx.next = Contexto: Siguiente
+event.control.ctx.last = Contexto: Último
+event.control.ctx.input.focus = Entrada: Enfocar
+event.control.ctx.input.send = Entrada: Enviar
+event.control.ctx.input.clear = Entrada: Limpiar
+event.control.ctx.stop = Entrada: Detener
+event.control.ctx.attachments.clear = Adjuntos: Limpiar
+event.control.input.sent = Entrada enviada.
+event.control.input.stopped = Entrada detenida.
+event.control.mode.chat = Modo: Chat
+event.control.mode.llama_index = Modo: Chat con archivos
+event.control.note.add = Nota añad
+event.control.tab.chat = Pestaña: Chat
+event.control.tab.calendar = Pestaña: Calendario
+event.control.tab.draw = Pestaña: Dibujo
+event.control.tab.files = Pestaña: Archivos
+event.control.tab.notepad = Pestaña: Bloc de notas
+event.control.tab.next = Pestaña: Siguiente
+event.control.tab.prev = Pestaña: Anterior
+event.control.voice_msg.start = Entrada de voz: Iniciar
+event.control.voice_msg.stop = Entrada de voz: Detener
+event.control.voice_msg.toggle = Entrada de voz: Conmutar
+event.control.voice_cmd.start = Control de voz: Iniciar
+event.control.voice_cmd.stop = Control de voz: Detener
+event.control.voice_cmd.toggle = Control de voz: Conmutar
 error.assistant_not_selected = Por favor, cree, importe o seleccione primero un asistente.
 files.local.upload = Dateien hochladen
 files.local.dir.prefix = Directorio
 files.delete.confirm = ¿Eliminar archivo/directorio?
 files.delete.recursive.confirm = ¡El directorio no está vacío! ¿Estás seguro de que quieres eliminar el directorio y todos los archivos en él?
 files.explorer.header.name = Nombre
 files.explorer.header.size = Tamaño
@@ -404,14 +473,15 @@
 interpreter.edit_label.output = Salida
 interpreter.edit = Modo de edición
 interpreter.input.placeholder = Código Python a ejecutar...
 menu.audio = Audio / Voz
 menu.audio.input = Entrada: reconocimiento de voz
 menu.audio.output = Salida: síntesis de voz
 menu.config = Configuración
+menu.config.access = Accesibilidad
 menu.config.edit.config = Editar config.json...
 menu.config.edit.models = Editar models.json...
 menu.config.edit.css = Editar hojas de estilo CSS...
 menu.config.edit.css.restore = Restaurar CSS por defecto...
 menu.config.open_dir = Abrir directorio de trabajo...
 menu.config.change_dir = Cambiar directorio de trabajo...
 menu.config.profile = Perfil
@@ -543,14 +613,22 @@
 preset.untitled = (sin título)
 preset.use = Usar
 preset.user_name = Nombre del usuario
 preset.vision = Visión
 profile.current.suffix = (actual)
 screenshot.capture.name.prefix = Captura de pantalla de
 settings.advanced.collapse = Mostrar/ocultar opciones avanzadas
+settings.access.voice_control = Habilitar control de voz (usando micrófono)
+settings.access.voice_control.model = Modelo
+settings.access.voice_control.model.desc = Modelo a usar para reconocimiento de comandos en control de voz
+settings.access.audio.event.speech = Usar síntesis de voz para describir eventos en pantalla.
+settings.access.audio.notify.execute = Notificación de audio al ejecutar comandos de voz
+settings.access.microphone.notify = Notificación de audio al iniciar/detener escucha del micrófono
+settings.access.shortcuts = Teclas de acceso directo de control
+settings.access.shortcuts.desc = Configurar teclas de acceso directo y comandos de voz para controlar la aplicación usando voz y micrófono.
 settings.agent.mode = Modo interno
 settings.agent.mode.desc = Modo interno para usar en modo Agente (chat, completado, langchain, llama_index, etc.)
 settings.agent.goal.notify = Mostrar una notificación en la bandeja del sistema cuando se logre el objetivo.
 settings.agent.idx = Índice
 settings.agent.idx.desc = Solo si el modo interno es llama_index (Chat con archivos), elige el índice a usar en modo Agente
 settings.api_endpoint = Punto final de la API
 settings.api_endpoint.desc = URL del punto final de la API de OpenAI, por defecto: https://api.openai.com/v1
@@ -645,15 +723,16 @@
 settings.prompt.expert = Experto: Master prompt
 settings.prompt.expert.desc = Instrucción (prompt del sistema) para el experto Master cómo manejar a los expertos subordinados. Las instrucciones para los expertos subordinados se dan desde sus presets.
 settings.prompt.img = DALL-E: generación de imagen
 settings.prompt.img.desc = Mensaje para generar comandos para DALL-E (si el modo crudo está desactivado). Solo modo de imagen.
 settings.render.code_syntax = Estilo de resaltado de sintaxis de código
 settings.render.plain = Desactivar el formato markdown en la salida (modo de texto plano RAW)
 settings.restart.required = Es necesario reiniciar la aplicación para que los cambios en esta opción se apliquen.
-settings.section.agent = Agente (autónomo)
+settings.section.access = Accesibilidad
+settings.section.agent = Agentes y expertos
 settings.section.files = Archivos y adjuntos
 settings.section.general = General
 settings.section.layout = Diseño
 settings.section.ctx = Contexto
 settings.section.model = Modelos
 settings.section.images = Imágenes
 settings.section.updates = Actualizaciones
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.fr.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.fr.ini`

 * *Files 7% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 attachments_uploaded.btn.sync = Synchroniser
 attachments_uploaded.btn.sync.current = Uniquement le courant
 attachments_uploaded.btn.sync.all = Toutes les bases
 attachments_uploaded.clear.confirm = ATTENTION : êtes-vous sûr de vouloir supprimer tous ces fichiers du serveur distant ?
 attachments_uploaded.delete.confirm = ATTENTION : êtes-vous sûr de vouloir supprimer le fichier du serveur distant ?
 attachments_uploaded.sync.tip = Astuce : cliquez sur 'Synchroniser' pour récupérer la liste des fichiers depuis OpenAI
 attachments_uploaded.tab = Fichiers téléchargés
+audio.control.btn = Contrôle vocal
 audio.magic_word.detected = Mot magique détecté !
 audio.magic_word.invalid = Pas un mot magique :(
 audio.magic_word.please = S'il vous plaît, le mot magique...
 audio.speak.btn = Microphone
 audio.speak.btn.stop = Arrêt
 audio.speak.btn.tooltip = Cliquez pour commencer l'écoute par le microphone
 audio.speak.btn.stop.tooltip = Cliquez pour arrêter l'écoute par le microphone
@@ -326,14 +327,82 @@
 dialog.workdir.result.directory_not_exists = Le répertoire de destination n'existe pas !
 dt.days_ago = il y a des jours
 dt.month = il y a un mois
 dt.today = aujourd'hui
 dt.week = il y a une semaine
 dt.weeks = il y a des semaines
 dt.yesterday = hier
+dictionary.config.access.shortcuts.action = Action à déclencher
+dictionary.config.access.shortcuts.key = Touche du clavier
+dictionary.config.access.shortcuts.key_modifier = Modificateur du clavier
+event.audio.app.started = Bienvenue !
+event.audio.app.status = Mode actuel : {mode}.\nConversation actuelle: {ctx}, dernière mise à jour {last}.\nNombre total de conversations : {total}.
+event.audio.ctx.created = Nouveau contexte créé.
+event.audio.ctx.current = Conversation actuelle : {ctx}, dernière mise à jour : {last}.
+event.audio.ctx.last = Votre entrée : {input}. Réponse de l'IA : {output}.
+event.audio.ctx.end = Terminé.
+event.audio.ctx.selected = Contexte sélectionné : {ctx}.
+event.audio.ctx.attachments.clear = La liste des pièces jointes est vide.
+event.audio.camera.enabled = Caméra activée.
+event.audio.camera.disabled = Caméra désactivée.
+event.audio.camera.captured = Image capturée de la caméra.
+event.audio.output.enable = Sortie audio activée.
+event.audio.output.disable = Sortie audio désactivée.
+event.audio.input.append = Texte ajouté à l'entrée.
+event.audio.input.call = Appel d'entrée.
+event.audio.input.enable = Entrée audio activée.
+event.audio.input.disable = Entrée audio activée.
+event.audio.input.error = Erreur survenue lors de l'envoi de l'entrée.
+event.audio.input.sent = Entrée envoyée.
+event.audio.input.stopped = Entrée arrêtée.
+event.audio.input.voice.listen.started = Écoute. Veuillez parler maintenant.
+event.audio.input.voice.listen.stopped = Écoute arrêtée.
+event.audio.note.add = Note ajoutée au bloc-notes.
+event.audio.tab.switch = Onglet sélectionné : {tab}.
+event.audio.voice.control.toggle = Contrôle vocal basculé.
+event.audio.voice.control.started = Contrôle vocal activé.
+event.audio.voice.control.stopped = Contrôle vocal désactivé.
+event.audio.voice.control.sent = OK.
+event.audio.voice.control.unrecognized = Commande non reconnue.
+event.control.app.status = Appli : Statut
+event.control.app.exit = Appli : Quitter
+event.control.audio.output.enable = Sortie audio : Activer
+event.control.audio.output.disable = Sortie audio : Désactiver
+event.control.audio.input.enable = Entrée audio : Activer
+event.control.audio.input.disable = Entrée audio : Désactiver
+event.control.camera.enable = Caméra : Activer
+event.control.camera.disable = Caméra : Désactiver
+event.control.camera.capture = Caméra : Capturer
+event.control.ctx.new = Contexte : Nouveau
+event.control.ctx.prev = Contexte : Précédent
+event.control.ctx.next = Contexte : Suivant
+event.control.ctx.last = Contexte : Dernier
+event.control.ctx.input.focus = Entrée : Focus
+event.control.ctx.input.send = Entrée : Envoyer
+event.control.ctx.input.clear = Entrée : Effacer
+event.control.ctx.stop = Entrée : Arrêter
+event.control.ctx.attachments.clear = Pièces jointes : Effacer
+event.control.input.sent = Entrée envoyée.
+event.control.input.stopped = Entrée arrêtée.
+event.control.mode.chat = Mode : Chat
+event.control.mode.llama_index = Mode : Chat avec fichiers
+event.control.note.add = Note ajoutée au bloc-notes.
+event.control.tab.chat = Onglet : Chat
+event.control.tab.calendar = Onglet : Calendrier
+event.control.tab.draw = Onglet : Dessin
+event.control.tab.files = Onglet : Fichiers
+event.control.tab.notepad = Onglet : Bloc-notes
+event.control.tab.next = Onglet : Suivant
+event.control.tab.prev = Onglet : Précédent
+event.control.voice_msg.start = Entrée vocale : Commencer
+event.control.voice_msg.stop = Entrée vocale : Arrêter
+event.control.voice_msg.toggle = Entrée vocale : Basculer
+event.control.voice_cmd.start = Commande vocale : Commencer
+event.control.voice_cmd.stop = Commande vocale : Arrêter
+event.control.voice_cmd.toggle = Commande vocale : Basculer
 error.assistant_not_selected = Veuillez créer, importer ou sélectionner un assistant d'abord !
 files.local.upload = Téléverser des fichiers
 files.local.dir.prefix = Répertoire
 files.delete.confirm = Supprimer le fichier/répertoire ?
 files.delete.recursive.confirm = Le répertoire n'est pas vide ! Êtes-vous sûr de vouloir supprimer le répertoire et tous les fichiers qu'il contient ?
 files.explorer.header.name = Nom
 files.explorer.header.size = Taille
@@ -405,14 +474,15 @@
 interpreter.edit_label.output = Sortie
 interpreter.edit = Mode édition
 interpreter.input.placeholder = Code Python à exécuter...
 menu.audio = Audio / Voix
 menu.audio.input = Entrée : reconnaissance vocale
 menu.audio.output = Sortie : synthèse vocale
 menu.config = Config
+menu.config.access = Accessibilité
 menu.config.edit.config = Modifier config.json...
 menu.config.edit.models = Modifier models.json...
 menu.config.edit.css = Modifier les feuilles de style CSS...
 menu.config.edit.css.restore = Restaurer le CSS par défaut...
 menu.config.open_dir = Ouvrir le répertoire de travail...
 menu.config.change_dir = Changer le répertoire de travail...
 menu.config.profile = Profil
@@ -543,14 +613,22 @@
 preset.untitled = (sans titre)
 preset.use = Utiliser
 preset.user_name = Nom de l'utilisateur
 preset.vision = Vision
 profile.current.suffix = (actuel)
 screenshot.capture.name.prefix = Capture d'écran de
 settings.advanced.collapse = Afficher/masquer les options avancées
+settings.access.voice_control = Activer le contrôle vocal (utilisant le microphone)
+settings.access.voice_control.model = Modèle
+settings.access.voice_control.model.desc = Modèle à utiliser pour la reconnaissance des commandes en contrôle vocal
+settings.access.audio.event.speech = Utiliser la synthèse vocale pour décrire les événements à l'écran.
+settings.access.audio.notify.execute = Notification audio lors de l’exécution d’une commande vocale
+settings.access.microphone.notify = Notification audio pour le démarrage/arrêt de l’écoute du microphone
+settings.access.shortcuts = Raccourcis clavier de contrôle
+settings.access.shortcuts.desc = Configurer les raccourcis clavier et les commandes vocales pour contrôler l'application en utilisant la voix et le microphone.
 settings.agent.mode = Mode interne
 settings.agent.mode.desc = Mode interne à utiliser en mode Agent (chat, complétion, langchain, llama_index, etc.)
 settings.agent.goal.notify = Afficher une notification dans la barre des tâches lorsque l'objectif est atteint.
 settings.agent.idx = Index
 settings.agent.idx.desc = Seulement si le mode interne est llama_index (Chat avec fichiers), choisissez l'index à utiliser en mode Agent
 settings.api_endpoint = Point de terminaison API
 settings.api_endpoint.desc = URL du point de terminaison de l'API OpenAI, par défaut : https://api.openai.com/v1
@@ -645,15 +723,16 @@
 settings.prompt.expert = Expert : Master prompt
 settings.prompt.expert.desc = Instruction (prompt système) pour l'expert Master sur comment gérer les experts esclaves. Les instructions pour les experts esclaves sont données à partir de leurs presets.
 settings.prompt.img = DALL-E: génération d'image
 settings.prompt.img.desc = Prompt pour générer des commandes pour DALL-E (si le mode brut est désactivé). Mode image uniquement.
 settings.render.code_syntax = Style de mise en évidence de la syntaxe du code
 settings.render.plain = Désactiver le formatage markdown dans la sortie (mode texte brut RAW)
 settings.restart.required = Un redémarrage de l'application est requis pour que les modifications de cette option soient appliquées.
-settings.section.agent = Agent (autonome)
+settings.section.access = Accessibilité
+settings.section.agent = Agents et experts
 settings.section.files = Fichiers et pièces jointes
 settings.section.general = Général
 settings.section.layout = Mise en page
 settings.section.ctx = Contexte
 settings.section.model = Modèles
 settings.section.images = Images
 settings.section.updates = Mises à jour
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.it.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.it.ini`

 * *Files 6% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 attachments_uploaded.btn.sync = Sincronizza
 attachments_uploaded.btn.sync.current = Solo corrente
 attachments_uploaded.btn.sync.all = Tutte le basi
 attachments_uploaded.clear.confirm = ATTENZIONE: sei sicuro di voler eliminare tutti questi file dal server remoto?
 attachments_uploaded.delete.confirm = ATTENZIONE: sei sicuro di voler eliminare il file dal server remoto?
 attachments_uploaded.sync.tip = Suggerimento: clicca su 'Sincronizza' per recuperare l'elenco dei file da OpenAI
 attachments_uploaded.tab = File caricati
+audio.control.btn = Controllo vocale
 audio.magic_word.detected = Parola magica rilevata!
 audio.magic_word.invalid = Non è una parola magica :(
 audio.magic_word.please = Per favore, parola magica...
 audio.speak.btn = Microfono
 audio.speak.btn.stop = Stop
 audio.speak.btn.tooltip = Clicca per iniziare l'ascolto tramite microfono
 audio.speak.btn.stop.tooltip = Clicca per terminare l'ascolto tramite microfono
@@ -326,14 +327,82 @@
 dialog.workdir.result.directory_not_exists = La directory di destinazione non esiste!
 dt.days_ago = giorni fa
 dt.month = mese fa
 dt.today = oggi
 dt.week = settimana fa
 dt.weeks = settimane fa
 dt.yesterday = ieri
+dictionary.config.access.shortcuts.action = Azione da attivare
+dictionary.config.access.shortcuts.key = Tasto della tastiera
+dictionary.config.access.shortcuts.key_modifier = Modificatore della tastiera
+event.audio.app.started = Benvenuto!
+event.audio.app.status = Modalità corrente: {mode}.\nConversazione attuale: {ctx}, ultimo aggiornamento {last}.\nConversazioni totali: {total}.
+event.audio.ctx.created = È stato creato un nuovo contesto.
+event.audio.ctx.current = Conversazione attuale: {ctx}, ultimo aggiornamento: {last}.
+event.audio.ctx.last = Il tuo input: {input}. Risposta dell'IA: {output}.
+event.audio.ctx.end = Finito.
+event.audio.ctx.selected = Contesto selezionato: {ctx}.
+event.audio.ctx.attachments.clear = Elenco degli allegati vuoto.
+event.audio.camera.enabled = Fotocamera attivata.
+event.audio.camera.disabled = Fotocamera disattivata.
+event.audio.camera.captured = Immagine catturata dalla fotocamera.
+event.audio.output.enable = Uscita audio attivata.
+event.audio.output.disable = Uscita audio disattivata.
+event.audio.input.append = Testo aggiunto all'input.
+event.audio.input.call = Chiamata input.
+event.audio.input.enable = Ingresso audio attivato.
+event.audio.input.disable = Ingresso audio disattivato.
+event.audio.input.error = Errore durante l'invio dell'input.
+event.audio.input.sent = Input inviato.
+event.audio.input.stopped = Input interrotto.
+event.audio.input.voice.listen.started = Ascoltando. Si prega di parlare ora.
+event.audio.input.voice.listen.stopped = Ascolto interrotto.
+event.audio.note.add = Nota aggiunta al blocco note.
+event.audio.tab.switch = Scheda selezionata: {tab}.
+event.audio.voice.control.toggle = Controllo vocale commutato.
+event.audio.voice.control.started = Controllo vocale attivato.
+event.audio.voice.control.stopped = Controllo vocale disattivato.
+event.audio.voice.control.sent = OK.
+event.audio.voice.control.unrecognized = Comando non riconosciuto.
+event.control.app.status = App: Stato
+event.control.app.exit = App: Uscita
+event.control.audio.output.enable = Uscita audio: Attiva
+event.control.audio.output.disable = Uscita audio: Disattiva
+event.control.audio.input.enable = Ingresso audio: Attiva
+event.control.audio.input.disable = Ingresso audio: Disattiva
+event.control.camera.enable = Fotocamera: Attiva
+event.control.camera.disable = Fotocamera: Disattiva
+event.control.camera.capture = Fotocamera: Cattura
+event.control.ctx.new = Contesto: Nuovo
+event.control.ctx.prev = Contesto: Precedente
+event.control.ctx.next = Contesto: Successivo
+event.control.ctx.last = Contesto: Ultimo
+event.control.ctx.input.focus = Input: Focalizza
+event.control.ctx.input.send = Input: Invia
+event.control.ctx.input.clear = Input: Pulisci
+event.control.ctx.stop = Input: Arresta
+event.control.ctx.attachments.clear = Allegati: Pulisci
+event.control.input.sent = Input inviato.
+event.control.input.stopped = Input interrotto.
+event.control.mode.chat = Modalità: Chat
+event.control.mode.llama_index = Modalità: Chat con file
+event.control.note.add = Nota aggiunta al blocco note.
+event.control.tab.chat = Scheda: Chat
+event.control.tab.calendar = Scheda: Calendario
+event.control.tab.draw = Scheda: Disegno
+event.control.tab.files = Scheda: File
+event.control.tab.notepad = Scheda: Blocco note
+event.control.tab.next = Scheda: Successiva
+event.control.tab.prev = Scheda: Precedente
+event.control.voice_msg.start = Input vocale: Avvia
+event.control.voice_msg.stop = Input vocale: Arresta
+event.control.voice_msg.toggle = Input vocale: Commuta
+event.control.voice_cmd.start = Comando vocale: Avvia
+event.control.voice_cmd.stop = Comando vocale: Arresta
+event.control.voice_cmd.toggle = Comando vocale: Commuta
 error.assistant_not_selected = Per favore, crea, importa o seleziona un assistente prima!
 files.local.upload = Caricare file
 files.local.dir.prefix = Directory
 files.delete.confirm = Eliminare il file/la cartella?
 files.delete.recursive.confirm = La directory non è vuota! Sei sicuro di voler eliminare la directory e tutti i file in essa?
 files.explorer.header.name = Nome
 files.explorer.header.size = Dimensione
@@ -405,14 +474,15 @@
 interpreter.edit_label.output = Risultato
 interpreter.edit = Modalità modifica
 interpreter.input.placeholder = Codice Python da eseguire...
 menu.audio = Audio / Voce
 menu.audio.input = Input: riconoscimento vocale
 menu.audio.output = Output: sintesi vocale
 menu.config = Config
+menu.config.access = Accessibilità
 menu.config.edit.config = Modifica config.json...
 menu.config.edit.models = Modifica models.json...
 menu.config.edit.css = Modifica fogli di stile CSS...
 menu.config.edit.css.restore = Ripristina CSS predefinito...
 menu.config.open_dir = Apri directory di lavoro...
 menu.config.change_dir = Cambia directory di lavoro...
 menu.config.profile = Profilo
@@ -543,14 +613,22 @@
 preset.temperature = Temperatura
 preset.untitled = (senza titolo)
 preset.use = Usa
 preset.user_name = Nome dell'utente
 preset.vision = Visione
 profile.current.suffix = (corrente)
 screenshot.capture.name.prefix = Screenshot da
+settings.access.voice_control = Abilita controllo vocale (utilizzando il microfono)
+settings.access.voice_control.model = Modello
+settings.access.voice_control.model.desc = Modello da usare per il riconoscimento dei comandi nel controllo vocale
+settings.access.audio.event.speech = Usa la sintesi vocale per descrivere gli eventi sullo schermo.
+settings.access.audio.notify.execute = Notifica audio esecuzione comando vocale
+settings.access.microphone.notify = Notifica audio inizio/fine ascolto microfono
+settings.access.shortcuts = Tasti di scelta rapida di controllo
+settings.access.shortcuts.desc = Configurare le scorciatoie da tastiera e i comandi vocali per controllare l'applicazione utilizzando la voce e il microfono.
 settings.advanced.collapse = Mostra/nascondi opzioni avanzate
 settings.agent.mode = Modalità interna
 settings.agent.mode.desc = Modalità interna da utilizzare in modalità Agente (chat, completamento, langchain, llama_index, ecc.)
 settings.agent.goal.notify = Visualizza una notifica nella barra delle applicazioni quando l'obiettivo è raggiunto.
 settings.agent.idx = Indice
 settings.agent.idx.desc = Solo se la modalità interna è llama_index (Chat con file), scegli l'indice da utilizzare in modalità Agente
 settings.api_endpoint = Endpoint API
@@ -645,15 +723,16 @@
 settings.prompt.ctx.auto_summary.user.desc = Placeholder: {input}, {output}
 settings.prompt.expert = Esperto: Master prompt
 settings.prompt.expert.desc = Istruzione (prompt del sistema) per l'esperto Master su come gestire gli esperti subalterni. Le istruzioni per gli esperti subalterni sono date dalle loro preimpostazioni.
 settings.prompt.img = DALL-E: generazione immagine
 settings.prompt.img.desc = Prompt per generare comandi per DALL-E (se la modalità grezza è disabilitata). Solo modalità immagine.
 settings.render.code_syntax = Stile di evidenziazione della sintassi del codice
 settings.restart.required = È necessario riavviare l'applicazione affinché le modifiche a questa opzione siano applicate.
-settings.section.agent = Agente (autonomo)
+settings.section.access = Accessibilità
+settings.section.agent = Agenti ed esperti
 settings.section.files = File e allegati
 settings.section.general = Generale
 settings.section.layout = Layout
 settings.section.ctx = Contesto
 settings.section.model = Modelli
 settings.section.images = Immagini
 settings.section.updates = Aggiornamenti
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files 12% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 audio.transcribe.tip = Wskazówka: kliknij "Otwórz...", aby rozpocząć transkrypcję audio z pliku. Zostanie użyty dostawca wejścia audio z ustawień wtyczki.
 audio.transcribe.open = Otwórz plik audio/wideo i przepisz...
 audio.transcribe.confirm = Czy na pewno chcesz przetransportować ten plik audio/wideo?
 audio.transcribe.clear.confirm = Czy wyczyścić obecną transkrypcję?
 audio.transcribe.auto_convert = Zawsze konwertuj wideo do mp3 przed transkrypcją (wymagany ffmpeg)
 audio.transcribe.result.finished = Zakończono: {path}
 audio.transcribe.result.selected = Wybrany plik: {path}
+audio.control.btn = Kontrola głosowa
 calendar.day.search = Pokaż rozmowy
 calendar.day.label = Ustaw kolor etykiety...
 calendar.day.label.color.default = Domyślny
 calendar.day.label.color.red = Czerwony
 calendar.day.label.color.orange = Pomarańczony
 calendar.day.label.color.yellow = Źółty
 calendar.day.label.color.green = Zielony
@@ -320,20 +321,88 @@
 dialog.workdir.title = Zmiana katalogu roboczego
 dialog.workdir.result.no_free_space = Za mało miejsca na dysku! Wymagane: {required}, Wolne miejsce: {free}.
 dialog.workdir.result.same_directory = Nic do przeniesienia.
 dialog.workdir.result.success = [OK] Bieżący katalog roboczy to teraz: {path}
 dialog.workdir.result.failed = Wystąpił błąd podczas przenoszenia katalogu roboczego.
 dialog.workdir.result.wait = Proszę czekać... przenoszenie bieżącego katalogu roboczego... To może chwilę potrwać...
 dialog.workdir.result.directory_not_exists = Katalog docelowy nie istnieje!
+dictionary.config.access.shortcuts.action = Akcja do wywołania
+dictionary.config.access.shortcuts.key = Klawisz klawiatury
+dictionary.config.access.shortcuts.key_modifier = Modyfikator klawiatury
 dt.days_ago = dni temu
 dt.month = miesiąc temu
 dt.today = dziś
 dt.week = tydzień temu
 dt.weeks = tygodnie temu
 dt.yesterday = wczoraj
+vent.audio.app.started = Witamy!
+event.audio.app.status = Aktualny tryb: {mode}.\nAktualna rozmowa: {ctx}, ostatnia aktualizacja {last}.\nŁączna liczba rozmów: {total}.
+event.audio.ctx.created = Utworzono nowy kontekst.
+event.audio.ctx.current = Aktualna rozmowa: {ctx}, ostatnio zaktualizowana: {last}.
+event.audio.ctx.last = Twoje wejście: {input}. Odpowiedź AI: {output}.
+event.audio.ctx.end = Zakończone.
+event.audio.ctx.selected = Wybrany kontekst: {ctx}.
+event.audio.ctx.attachments.clear = Lista załączników jest pusta.
+event.audio.camera.enabled = Kamera włączona.
+event.audio.camera.disabled = Kamera wyłączona.
+event.audio.camera.captured = Zrobiono zdjęcie z kamery.
+event.audio.output.enable = Włączono wyjście audio.
+event.audio.output.disable = Wyłączono wyjście audio.
+event.audio.input.append = Dodano tekst do wejścia.
+event.audio.input.call = Wejście rozmowy.
+event.audio.input.enable = Włączono wejście audio.
+event.audio.input.disable = Włączono wejście audio.
+event.audio.input.error = Wystąpił błąd podczas wysyłania wejścia.
+event.audio.input.sent = Wejście wysłane.
+event.audio.input.stopped = Wejście zatrzymane.
+event.audio.input.voice.listen.started = Nasłuchiwanie. Proszę mówić.
+event.audio.input.voice.listen.stopped = Nasłuchiwanie zatrzymane.
+event.audio.note.add = Notatka dodana do notatnika.
+event.audio.tab.switch = Wybrana zakładka to: {tab}.
+event.audio.voice.control.toggle = Kontrola głosowa została przełączona.
+event.audio.voice.control.started = Kontrola głosowa aktywowana.
+event.audio.voice.control.stopped = Kontrola głosowa dezaktywowana.
+event.audio.voice.control.sent = OK.
+event.audio.voice.control.unrecognized = Nierozpoznane polecenie.
+event.control.app.status = Aplikacja: Status
+event.control.app.exit = Aplikacja: Wyjście
+event.control.audio.output.enable = Wyjście audio: Włącz
+event.control.audio.output.disable = Wyjście audio: Wyłącz
+event.control.audio.input.enable = Wejście audio: Włącz
+event.control.audio.input.disable = Wejście audio: Wyłącz
+event.control.camera.enable = Kamera: Włącz
+event.control.camera.disable = Kamera: Wyłącz
+event.control.camera.capture = Kamera: Złap obraz
+event.control.ctx.new = Kontekst: Nowy
+event.control.ctx.prev = Kontekst: Poprzedni
+event.control.ctx.next = Kontekst: Następny
+event.control.ctx.last = Kontekst: Ostatni
+event.control.ctx.input.focus = Wejście: Skupienie
+event.control.ctx.input.send = Wejście: Wyślij
+event.control.ctx.input.clear = Wejście: Wyczyść
+event.control.ctx.stop = Wejście: Zatrzymaj
+event.control.ctx.attachments.clear = Załączniki: Wyczyść
+event.control.input.sent = Wejście wysłane.
+event.control.input.stopped = Wejście zatrzymane.
+event.control.mode.chat = Tryb: Czat
+event.control.mode.llama_index = Tryb: Czat z plikami
+event.control.note.add = Notatka dodana do notatnika.
+event.control.tab.chat = Zakładka: Czat
+event.control.tab.calendar = Zakładka: Kalendarz
+event.control.tab.draw = Zakładka: Rysowanie
+event.control.tab.files = Zakładka: Pliki
+event.control.tab.notepad = Zakładka: Notatnik
+event.control.tab.next = Zakładka: Następna
+event.control.tab.prev = Zakładka: Poprzednia
+event.control.voice_msg.start = Wejście głosowe: Rozpocznij
+event.control.voice_msg.stop = Wejście głosowe: Zatrzymaj
+event.control.voice_msg.toggle = Wejście głosowe: Przełącz
+event.control.voice_cmd.start = Kontrola głosowa: Rozpocznij
+event.control.voice_cmd.stop = Kontrola głosowa: Zatrzymaj
+event.control.voice_cmd.toggle = Kontrola głosowa: Przełącz
 error.assistant_not_selected = Musisz najpierw utworzyć, zaimportować lub wybrać asystenta!
 files.local.upload = Wgraj pliki
 files.local.dir.prefix = Katalog
 files.delete.confirm = Usunąć plik/katalog?
 files.delete.recursive.confirm = Katalog nie jest pusty! Czy na pewno chcesz usunąć katalog i wszystkie pliki w nim?
 files.explorer.header.name = Nazwa
 files.explorer.header.size = Rozmiar
@@ -405,14 +474,15 @@
 interpreter.edit_label.output = Wynik
 interpreter.edit = Tryb edycji
 interpreter.input.placeholder = Kod Pythona do wykonania...
 menu.audio = Audio / Mowa
 menu.audio.input = Wejście: rozpoznawanie mowy
 menu.audio.output = Wyjście: synteza mowy
 menu.config = Opcje
+menu.config.access = Dostępność
 menu.config.edit.config = Edytuj config.json...
 menu.config.edit.models = Edytuj models.json...
 menu.config.edit.css = Edytuj style CSS...
 menu.config.edit.css.restore = Przywróć domyślny CSS...
 menu.config.open_dir = Otwórz katalog roboczy...
 menu.config.change_dir = Zmień katalog roboczy...
 menu.config.profile = Profil
@@ -543,14 +613,22 @@
 preset.temperature = Temperatura
 preset.untitled = (bez nazwy)
 preset.use = Użyj
 preset.user_name = Imię użytkownika
 preset.vision = Wizja (Vision)
 profile.current.suffix = (bieżący)
 screenshot.capture.name.prefix = Zrzut ekranu z
+settings.access.voice_control = Włącz kontrolę głosową (przy użyciu mikrofonu)
+settings.access.voice_control.model = Model
+settings.access.voice_control.model.desc = Model do używania w rozpoznawaniu poleceń w kontroli głosowej
+settings.access.audio.event.speech = Użyj syntezy mowy do opisywania zdarzeń na ekranie.
+settings.access.audio.notify.execute = Powiadomienie audio wykonania polecenia głosowego
+settings.access.microphone.notify = Powiadomienie audio startu/stopu nasłuchu mikrofonu
+settings.access.shortcuts = Skróty klawiszowe sterowania
+settings.access.shortcuts.desc = Ustaw skróty klawiszowe i polecenia głosowe do sterowania aplikacją przy użyciu głosu i mikrofonu.
 settings.advanced.collapse = Pokaż/ukryj zaawansowane opcje
 settings.agent.mode = Tryb wewnętrzny
 settings.agent.mode.desc = Tryb wewnętrzny do użycia w trybie Agenta (chat, completion, langchain, llama_index itp.)
 settings.agent.goal.notify = Wyświetl powiadomienie w zasobniku systemowym, gdy cel zostanie osiągnięty.
 settings.agent.idx = Indeks
 settings.agent.idx.desc = Tylko jeśli tryb wewnętrzny to llama_index (Czat z plikami), wybierz indeks do użycia w trybie Agenta
 settings.api_endpoint = Punkt końcowy API
@@ -646,15 +724,16 @@
 settings.prompt.expert = Ekspert: Główna wskazówka
 settings.prompt.expert.desc = Instrukcja (systemowa wskazówka) dla głównego eksperta, jak obsługiwać ekspertów pomocniczych. Instrukcje dla ekspertów pomocniczych są podawane z ich ustawień.
 settings.prompt.img = DALL-E: generowanie obrazu
 settings.prompt.img.desc = Prompt do generowania poleceń dla DALL-E (jeśli surowy tryb jest wyłączony). Tylko tryb obrazu.
 settings.render.code_syntax = Styl podświetlenia składni kodu
 settings.render.plain = Wyłącz formatowanie markdown w wyjściu (tryb plain-text)
 settings.restart.required = Restart aplikacji jest wymagany, aby zmiany dla tej opcji zostały wprowadzone.
-settings.section.agent = Agent (autonomiczny)
+settings.section.access = Dostępność
+settings.section.agent = Agenci i eksperci
 settings.section.files = Pliki i załączniki
 settings.section.general = Ogólne
 settings.section.layout = Wygląd
 settings.section.ctx = Kontekst
 settings.section.model = Modele
 settings.section.images = Obrazy
 settings.section.updates = Aktualizacje
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.uk.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.uk.ini`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 attachments_uploaded.btn.sync = Синхронізація
 attachments_uploaded.btn.sync.current = Лише поточний
 attachments_uploaded.btn.sync.all = Усі бази
 attachments_uploaded.clear.confirm = ПОПЕРЕДЖЕННЯ: ви впевнені, що хочете видалити всі ці файли з віддаленого сервера?
 attachments_uploaded.delete.confirm = ПОПЕРЕДЖЕННЯ: ви впевнені, що хочете видалити файл з віддаленого сервера?
 attachments_uploaded.sync.tip = Підказка: натисніть "Синхронізація", щоб отримати список файлів з OpenAI
 attachments_uploaded.tab = Завантажені файли
+audio.control.btn = Керування голосом
 audio.magic_word.detected = Магічне слово виявлено!
 audio.magic_word.invalid = Не магічне слово :(
 audio.magic_word.please = Магічне слово, будь ласка...
 audio.speak.btn = Мікрофон
 audio.speak.btn.stop = Стоп
 audio.speak.btn.tooltip = Натисніть, щоб почати слухання через мікрофон
 audio.speak.btn.stop.tooltip = Натисніть, щоб закінчити слухання через мікрофон
@@ -326,14 +327,81 @@
 dialog.workdir.result.directory_not_exists = Кінцевий каталог не існує!
 dt.days_ago = днів тому
 dt.month = місяць тому
 dt.today = сьогодні
 dt.week = тиждень тому
 dt.weeks = тижнів тому
 dt.yesterday = вчора
+event.audio.app.started = Ласкаво просимо!
+event.audio.app.status = Поточний режим: {mode}.\nПоточна розмова: {ctx}, останнє оновлення {last}.\nЗагальна кількість розмов: {total}.
+event.audio.ctx.created = Створено новий контекст.
+event.audio.ctx.current = Поточна розмова: {ctx}, останнє оновлення: {last}.
+event.audio.ctx.last = Ваш вхід: {input}. Відповідь ШІ: {output}.
+event.audio.ctx.end = Завершено.
+event.audio.ctx.selected = Вибраний контекст: {ctx}.
+event.audio.camera.enabled = Камера ввімкнута.
+event.audio.camera.disabled = Камера вимкнута.
+event.audio.camera.captured = З камери зроблено знімок.
+event.audio.output.enable = Аудіовихід ввімкнуто.
+event.audio.output.disable = Аудіовихід вимкнуто.
+event.audio.input.append = Текст додано до входу.
+event.audio.input.call = Вхідний виклик.
+event.audio.input.enable = Аудіовхід ввімкнуто.
+event.audio.input.disable = Аудіовхід вимкнуто.
+event.audio.input.error = Виникла помилка під час відправлення входу.
+event.audio.input.sent = Введення надіслано.
+event.audio.input.stopped = Введення зупинено.
+event.audio.input.voice.listen.started = Слухання. Будь ласка, говоріть зараз.
+event.audio.input.voice.listen.stopped = Слухання зупинено.
+event.audio.note.add = До блокнота додано нотатку.
+event.audio.tab.switch = Вибрана вкладка: {tab}.
+event.audio.voice.control.toggle = Керування голосом перемкнуто.
+event.audio.voice.control.started = Керування голосом активовано.
+event.audio.voice.control.stopped = Керування голосом деактивовано.
+event.audio.voice.control.sent = OK.
+event.audio.voice.control.unrecognized = Команду не впізнано.
+event.control.app.status = Додаток: Статус
+event.control.app.exit = Додаток: Вихід
+event.control.audio.output.enable = Аудіовихід: Увімкнуто
+event.control.audio.output.disable = Аудіовихід: Вимкнуто
+event.control.audio.input.enable = Аудіовхід: Увімкнуто
+event.control.audio.input.disable = Аудіовхід: Вимкнуто
+event.control.camera.enable = Камера: Увімкнути
+event.control.camera.disable = Камера: Вимкнути
+event.control.camera.capture = Камера: Зняти
+event.control.ctx.new = Контекст: Новий
+event.control.ctx.prev = Контекст: Попередній
+event.control.ctx.next = Контекст: Наступний
+event.control.ctx.last = Контекст: Останній
+event.control.ctx.input.focus = Введення: Фокус
+event.control.ctx.input.send = Введення: Надіслати
+event.control.ctx.input.clear = Введення: Очистити
+event.control.ctx.stop = Введення: Зупинити
+event.control.ctx.attachments.clear = Вкладення: Очистити
+event.control.input.sent = Введення надіслано.
+event.control.input.stopped = Введення зупинено.
+event.control.mode.chat = Режим: Чат
+event.control.mode.llama_index = Режим: Чат з файлами
+event.control.note.add = До блокнота додано нотатку.
+event.control.tab.chat = Вкладка: Чат
+event.control.tab.calendar = Вкладка: Календар
+event.control.tab.draw = Вкладка: Малювання
+event.control.tab.files = Вкладка: Файли
+event.control.tab.notepad = Вкладка: Блокнот
+event.control.tab.next = Вкладка: Наступна
+event.control.tab.prev = Вкладка: Попередня
+event.control.voice_msg.start = Голосовий вхід: Розпочати
+event.control.voice_msg.stop = Голосовий вхід: Зупинити
+event.control.voice_msg.toggle = Голосовий вхід: Перемкнути
+event.control.voice_cmd.start = Керування голосом: Розпочати
+event.control.voice_cmd.stop = Керування голосом: Зупинити
+event.control.voice_cmd.toggle = Керування голосом: Перемкнути
+dictionary.config.access.shortcuts.action = Дія для активації
+dictionary.config.access.shortcuts.key = Клавіша клавіатури
+dictionary.config.access.shortcuts.key_modifier = Модифікатор клавіатури
 error.assistant_not_selected = Будь ласка, спершу створіть, імпортуйте або оберіть помічника!
 files.local.upload = Завантажити файли
 files.local.dir.prefix = Каталог
 files.delete.confirm = Видалити файл/директорію?
 files.delete.recursive.confirm = Каталог не порожній! Ви впевнені, що хочете видалити каталог та всі файли в ньому?
 files.explorer.header.name = Ім'я
 files.explorer.header.size = Розмір
@@ -405,14 +473,15 @@
 interpreter.edit_label.output = Вивід
 interpreter.edit = Режим редагування
 interpreter.input.placeholder = Python код для виконання...
 menu.audio = Аудіо / Голос
 menu.audio.input = Введення: розпізнавання мови
 menu.audio.output = Вивід: синтез мови
 menu.config = Конфігурація
+menu.config.access = Доступність
 menu.config.edit.config = Редагувати config.json...
 menu.config.edit.models = Редагувати models.json...
 menu.config.edit.css = Редагувати CSS-стилі...
 menu.config.open_dir = Відкрити робочий каталог...
 menu.config.change_dir = Змінити робочий каталог...
 menu.config.profile = Профіль
 menu.config.profile.edit = Редагувати профілі...
@@ -543,14 +612,22 @@
 preset.temperature = Температура
 preset.untitled = (без назви)
 preset.use = Використовувати
 preset.user_name = Ім'я користувача
 preset.vision = Оптика
 profile.current.suffix = (поточний)
 screenshot.capture.name.prefix = Скріншот з
+settings.access.voice_control = Увімкнути голосове керування (за допомогою мікрофона)
+settings.access.voice_control.model = Модель
+settings.access.voice_control.model.desc = Модель для використання в розпізнаванні команд в голосовому керуванні
+settings.access.audio.event.speech = Використовувати синтез мовлення для
+settings.access.audio.notify.execute = Аудіо сповіщення виконання голосової команди
+settings.access.microphone.notify = Аудіо сповіщення початку/зупинки прослуховування мікрофону
+settings.access.shortcuts = Клавіші швидкого доступу
+settings.access.shortcuts.desc = Налаштування клавіш швидкого доступу та голосових команд для керування додатком за допомогою голосу та мікрофона.
 settings.advanced.collapse = Показати/сховати додаткові опції
 settings.agent.mode = Внутрішній режим
 settings.agent.mode.desc = Внутрішній режим для використання в режимі Агента (чат, завершення, langchain, llama_index тощо)
 settings.agent.goal.notify = Показати сповіщення в системному треї, коли мета досягнута.
 settings.agent.idx = Індекс
 settings.agent.idx.desc = Тільки якщо внутрішній режим є llama_index (Чат з файлами), виберіть індекс для використання в режимі Агента
 settings.api_endpoint = Кінцева точка API
@@ -646,15 +723,16 @@
 settings.prompt.img = DALL-E: генерація зображення
 settings.prompt.expert = Експерт: Основний запит
 settings.prompt.expert.desc = Інструкція (системний запит) для ведучого експерта, як керувати підеекспертами. Інструкції для підеекспертів даються з їхніх налаштувань.
 settings.prompt.img.desc = Підказка для генерації команддля DALL-E (якщо вимкнено сирівний режим). Тільки режим зображення.
 settings.render.code_syntax = Стиль підсвічування синтаксису коду
 settings.render.plain = Вимкнути форматування markdown у виводі (режим простого тексту RAW)
 settings.restart.required = Для внесення змін у цю опцію необхідно перезапустити програму.
-settings.section.agent = Агент (автономний)
+settings.section.access = Доступність
+settings.section.agent = Агенти та експерти
 settings.section.files = Файли та вкладення
 settings.section.general = Загальні
 settings.section.layout = Макет
 settings.section.ctx = Контекст
 settings.section.model = Моделі
 settings.section.images = Зображення
 settings.section.updates = Оновлення
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.zh.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.zh.ini`

 * *Files 9% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 attachments_uploaded.btn.sync = 同步
 attachments_uploaded.btn.sync.current = 仅当前
 attachments_uploaded.btn.sync.all = 所有存储
 attachments_uploaded.clear.confirm = 警告：您確定要從遠程服務器刪除所有這些文件嗎？
 attachments_uploaded.delete.confirm = 警告：您確定要從遠程服務器刪除文件嗎？
 attachments_uploaded.sync.tip = 提示：點擊“同步”以從OpenAI檢索文件列表。
 attachments_uploaded.tab = 已上傳的文件
+audio.control.btn = 语音控制
 audio.magic_word.detected = 檢測到魔法詞！
 audio.magic_word.invalid= 不是魔法詞 :(
 audio.magic_word.please= 請說出魔法詞...
 audio.speak.btn.stop = 停止
 audio.speak.btn.tooltip = 點擊開始麥克風聆聽
 audio.speak.btn.stop.tooltip = 點擊停止麥克風聆聽
 audio.speak.ignoring = 忽略（無前綴）
@@ -333,14 +334,17 @@
 dialog.workdir.result.success = [确定] 当前工作目录已设置为：{path}
 dialog.workdir.result.failed = 移动工作目录时发生错误。
 dialog.workdir.result.wait = 请稍等...正在移动当前工作目录...这可能需要一段时间...
 dialog.workdir.result.directory_not_exists = 目标目录不存在！
 dictionary.assistant.tool.function.name = 函數名稱
 dictionary.assistant.tool.function.params = 函數參數（JSON對象）
 dictionary.assistant.tool.function.desc = 描述（可選）
+dictionary.config.access.shortcuts.action = 触发行动
+dictionary.config.access.shortcuts.key = 键盘按键
+dictionary.config.access.shortcuts.key_modifier = 键盘修饰符
 dictionary.config.llama.idx.list.id = ID（索引目錄名稱）
 dictionary.config.llama.idx.list.name = 名稱
 dictionary.config.llama.idx.list.model_embed = 用於嵌入（索引）的模型，默認：gpt-3.5-turbo 
 dictionary.config.llama.idx.list.model_query = 查詢模型
 dictionary.config.llama.idx.storage.args.name = 額外參數名稱
 dictionary.config.llama.idx.storage.args.value = 額外參數值
 dictionary.config.llama.idx.storage.args.type = 類型，對於字典使用JSON字符串，對於列表：item1,item2等。
@@ -397,14 +401,79 @@
 dictionary.preset.tool.function.desc = 描述（可選）
 dt.days_ago = 天前
 dt.month = 月前
 dt.today = 今天
 dt.week = 周前
 dt.weeks = 周前
 dt.yesterday = 昨天
+event.audio.app.started = 欢迎！
+event.audio.app.status = 当前模式: {mode}。\n当前会话: {ctx}，最后更新 {last}。\n会话总数: {total}。
+event.audio.ctx.created = 已创建新上下文。
+event.audio.ctx.current = 当前会话: {ctx}，最后更新: {last}。
+event.audio.ctx.last = 您的输入: {input}。AI 回应: {output}。
+event.audio.ctx.end = 完成。
+event.audio.ctx.selected = 选定上下文: {ctx}。
+event.audio.ctx.attachments.clear = 附件列表为空。
+event.audio.camera.enabled = 摄像头已启用。
+event.audio.camera.disabled = 摄像头已禁用。
+event.audio.camera.captured = 已从摄像头捕获图像。
+event.audio.output.enable = 音频输出已启用。
+event.audio.output.disable = 音频输出已禁用。
+event.audio.input.append = 文本已附加到输入。
+event.audio.input.call = 输入调用。
+event.audio.input.enable = 音频输入已启用。
+event.audio.input.disable = 音频输入已启用。
+event.audio.input.error = 发送输入时发生错误。
+event.audio.input.sent = 输入已发送。
+event.audio.input.stopped = 输入已停止。
+event.audio.input.voice.listen.started = 正在监听。请现在说话。
+event.audio.input.voice.listen.stopped = 监听已停止。
+event.audio.note.add = 笔记已添加到记事本。
+event.audio.tab.switch = 选定标签是: {tab}。
+event.audio.voice.control.toggle = 语音控制已切换。
+event.audio.voice.control.started = 语音控制已激活。
+event.audio.voice.control.stopped = 语音控制已停用。
+event.audio.voice.control.sent = 好的。
+event.audio.voice.control.unrecognized = 无法识别的命令。
+event.control.app.status = 应用程序：状态
+event.control.app.exit = 应用程序：退出
+event.control.audio.output.enable = 音频输出：启用
+event.control.audio.output.disable = 音频输出：禁用
+event.control.audio.input.enable = 音频输入：启用
+event.control.audio.input.disable = 音频输入：禁用
+event.control.camera.enable = 摄像头：启用
+event.control.camera.disable = 摄像头：禁用
+event.control.camera.capture = 摄像头：捕捉
+event.control.ctx.new = 上下文：新建
+event.control.ctx.prev = 上下文：上一个
+event.control.ctx.next = 上下文：下一个
+event.control.ctx.last = 上下文：最后一个
+event.control.ctx.input.focus = 输入：焦点
+event.control.ctx.input.send = 输入：发送
+event.control.ctx.input.clear = 输入：清除
+event.control.ctx.stop = 输入：停止
+event.control.ctx.attachments.clear = 附件：清除
+event.control.input.sent = 输入已发送。
+event.control.input.stopped = 输入已停止。
+event.control.mode.chat = 模式：聊天
+event.control.mode.llama_index = 模式：带文件的聊天
+event.control.note.add = 笔记已添加到记事本。
+event.control.tab.chat = 标签：聊天
+event.control.tab.calendar = 标签：日历
+event.control.tab.draw = 标签：绘图
+event.control.tab.files = 标签：文件
+event.control.tab.notepad = 标签：记事本
+event.control.tab.next = 标签：下一个
+event.control.tab.prev = 标签：上一个
+event.control.voice_msg.start = 语音输入：开始
+event.control.voice_msg.stop = 语音输入：停止
+event.control.voice_msg.toggle = 语音输入：切换
+event.control.voice_cmd.start = 语音控制：开始
+event.control.voice_cmd.stop = 语音控制：停止
+event.control.voice_cmd.toggle = 语音控制：切换
 error.assistant_not_selected = 請首先創建、導入或選擇助手！
 files.local.upload = 上傳文件
 files.local.dir.prefix = 路徑
 files.delete.confirm = 刪除文件/目錄？
 files.delete.recursive.confirm = 目錄不是空的！您確定要刪除目錄及其中的所有文件嗎？
 files.explorer.header.name = 名稱
 files.explorer.header.size = 大小
@@ -478,14 +547,15 @@
 interpreter.edit_label.output = 输出
 interpreter.edit = 编辑模式
 interpreter.input.placeholder = 要执行的 Python 代码...
 menu.audio = 音頻/語音
 menu.audio.input = 輸入：語音識別
 menu.audio.output = 輸出：語音合成
 menu.config = 配置
+menu.config.access = 可访问性
 menu.config.edit.config = 編輯config.json...
 menu.config.edit.models = 編輯models.json...
 menu.config.edit.css = 編輯CSS樣式表...
 menu.config.edit.css.restore = 恢复默认CSS...
 menu.config.edit.json = 編輯JSON配置...
 menu.config.models = 模型...
 menu.config.open_dir = 打开工作目录...
@@ -646,14 +716,22 @@
 preset.untitled = （無標題）
 preset.use = 使用
 preset.user_name = 用戶名稱
 preset.vision = 視覺
 profile.current.suffix = （当前）
 screenshot.capture.name.prefix = 截圖來自
 settings.advanced.collapse = 顯示/隱藏高級選項
+settings.access.voice_control = 启用语音控制（使用麦克风）
+settings.access.voice_control.model = 模型
+settings.access.voice_control.model.desc = 用于语音控制命令识别的模型
+settings.access.audio.event.speech = 使用语音合成描述屏幕上的事件。
+settings.access.audio.notify.execute = 执行语音命令时的音频通知
+settings.access.microphone.notify = 启动/停止麦克风监听时的音频通知
+settings.access.shortcuts = 控制快捷键
+settings.access.shortcuts.desc = 设置键盘快捷键和语音命令，以使用语音和麦克风控制应用程序。
 settings.agent.mode = 要使用的子模式
 settings.agent.mode.desc = 在代理模式下使用的子模式（聊天、完成、langchain、llama_index等）
 settings.agent.goal.notify = 當目標達成時顯示托盤通知。
 settings.agent.idx = 要使用的索引
 settings.agent.idx.desc = 只有在子模式為llama_index（文件聊天）時，選擇在代理模式下使用的索引
 settings.api_endpoint = API端点
 settings.api_endpoint.desc = OpenAI API端点URL，默认为：https://api.openai.com/v1
@@ -756,15 +834,16 @@
 settings.prompt.expert = 专家：主提示
 settings.prompt.expert.desc = 对主专家如何处理奴隶专家的指令（系统提示）。奴隶专家的指令根据他们的预设给出。
 settings.prompt.img = DALL-E：生成图像
 settings.prompt.img.desc = 提示用于生成DALL-E的命令（如果原始模式被禁用）。仅图像模式。
 settings.render.code_syntax = 代码语法高亮样式
 settings.render.plain = 在輸出中禁用markdown格式化（RAW純文本模式）
 settings.restart.required = 此選項生效需要重新啟動應用程序。
-settings.section.agent = 代理（自主）
+settings.section.access = 可访问性
+settings.section.agent = 代理和专家
 settings.section.files = 文件和附件
 settings.section.general = 一般
 settings.section.layout = 布局
 settings.section.llama_index = 索引（llama-index）
 settings.section.ctx = 上下文
 settings.section.developer = 開發者
 settings.section.model = 模型
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.agent.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.agent.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.agent.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.agent.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_input.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_input.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_input.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_input.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_output.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_output.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_output.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_output.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_api.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_api.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_files.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_files.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_history.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_history.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_web.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_web.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.crontab.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.crontab.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.crontab.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.crontab.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_vision.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_vision.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.real_time.en.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.real_time.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.real_time.pl.ini` & `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.real_time.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/logo.png` & `pygpt_net-2.2.8/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/prompts.csv` & `pygpt_net-2.2.8/src/pygpt_net/data/prompts.csv`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/win32/README.rtf` & `pygpt_net-2.2.8/src/pygpt_net/data/win32/README.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/win32/USER-LICENSE.rtf` & `pygpt_net-2.2.8/src/pygpt_net/data/win32/USER-LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/data/win32/pygpt.aip` & `pygpt_net-2.2.8/src/pygpt_net/data/win32/pygpt.aip`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/icons.qrc` & `pygpt_net-2.2.8/src/pygpt_net/icons.qrc`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 <RCC>
     <qresource prefix="/icons">
         <file alias="abc.svg">/home/marcin/Dev/py-gpt/scripts/../src/pygpt_net/data/icons/abc.svg</file>
     </qresource>
     <qresource prefix="/icons">
+        <file alias="accessibility.svg">/home/marcin/Dev/py-gpt/scripts/../src/pygpt_net/data/icons/accessibility.svg</file>
+    </qresource>
+    <qresource prefix="/icons">
         <file alias="add.svg">/home/marcin/Dev/py-gpt/scripts/../src/pygpt_net/data/icons/add.svg</file>
     </qresource>
     <qresource prefix="/icons">
         <file alias="add_circle.svg">/home/marcin/Dev/py-gpt/scripts/../src/pygpt_net/data/icons/add_circle.svg</file>
     </qresource>
     <qresource prefix="/icons">
         <file alias="add_folder.svg">/home/marcin/Dev/py-gpt/scripts/../src/pygpt_net/data/icons/add_folder.svg</file>
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/icons_rc.py` & `pygpt_net-2.2.8/src/pygpt_net/icons_rc.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,14 +413,39 @@
 0H360Zm0-80h360v\
 -480H360v480ZM20\
 0-80q-33 0-56.5-\
 23.5T120-160v-56\
 0h80v560h440v80H\
 200Zm160-240v-48\
 0 480Z\x22/></svg>\
+\x00\x00\x01h\
+<\
+svg xmlns=\x22http:\
+//www.w3.org/200\
+0/svg\x22 height=\x222\
+4\x22 viewBox=\x220 -9\
+60 960 960\x22 widt\
+h=\x2224\x22><path fil\
+l=\x22#686868\x22 d=\x22M\
+480-720q-33 0-56\
+.5-23.5T400-800q\
+0-33 23.5-56.5T4\
+80-880q33 0 56.5\
+ 23.5T560-800q0 \
+33-23.5 56.5T480\
+-720ZM360-80v-52\
+0q-60-5-122-15t-\
+118-25l20-80q78 \
+21 166 30.5t174 \
+9.5q86 0 174-9.5\
+T820-720l20 80q-\
+56 15-118 25t-12\
+2 15v520h-80v-24\
+0h-80v240h-80Z\x22/\
+></svg>\
 \x00\x00\x00\xe0\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 height=\x222\
 4\x22 viewBox=\x220 -9\
 60 960 960\x22 widt\
@@ -3710,14 +3735,19 @@
 \x09s\xed\xc7\
 \x00w\
 \x00e\x00b\x00c\x00a\x00m\x00.\x00s\x00v\x00g\
 \x00\x08\
 \x06|W\x87\
 \x00c\
 \x00o\x00p\x00y\x00.\x00s\x00v\x00g\
+\x00\x11\
+\x04\x1d%\x87\
+\x00a\
+\x00c\x00c\x00e\x00s\x00s\x00i\x00b\x00i\x00l\x00i\x00t\x00y\x00.\x00s\x00v\x00g\
+\
 \x00\x08\
 \x05\xa8W\x87\
 \x00c\
 \x00o\x00d\x00e\x00.\x00s\x00v\x00g\
 \x00\x0c\
 \x09\x88\xc7\xa7\
 \x00l\
@@ -4191,285 +4221,287 @@
 \x00s\
 \x00y\x00n\x00c\x00.\x00s\x00v\x00g\
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x87\x00\x00\x00\x02\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x88\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x0cF\x00\x00\x00\x00\x00\x01\x00\x00\xb52\
+\x00\x00\x0cn\x00\x00\x00\x00\x00\x01\x00\x00\xb6\x9e\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0e,\x00\x00\x00\x00\x00\x01\x00\x00\xcf*\
+\x00\x00\x0eT\x00\x00\x00\x00\x00\x01\x00\x00\xd0\x96\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x0a\x8c\x00\x00\x00\x00\x00\x01\x00\x00\x9a\xe0\
+\x00\x00\x0a\xb4\x00\x00\x00\x00\x00\x01\x00\x00\x9cL\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x06l\x00\x00\x00\x00\x00\x01\x00\x00[(\
+\x00\x00\x06\x94\x00\x00\x00\x00\x00\x01\x00\x00\x5c\x94\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x02\x98\x00\x00\x00\x00\x00\x01\x00\x00#\xde\
+\x00\x00\x02\xc0\x00\x00\x00\x00\x00\x01\x00\x00%J\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x02\xae\x00\x00\x00\x00\x00\x01\x00\x00%\xcd\
+\x00\x00\x02\xd6\x00\x00\x00\x00\x00\x01\x00\x00'9\
 \x00\x00\x01\x8d[e\x92\xd5\
 \x00\x00\x00B\x00\x00\x00\x00\x00\x01\x00\x00\x02\xda\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x09\x16\x00\x00\x00\x00\x00\x01\x00\x00\x86\xa6\
+\x00\x00\x09>\x00\x00\x00\x00\x00\x01\x00\x00\x88\x12\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x08n\x00\x00\x00\x00\x00\x01\x00\x00}\xbf\
+\x00\x00\x08\x96\x00\x00\x00\x00\x00\x01\x00\x00\x7f+\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x08T\x00\x00\x00\x00\x00\x01\x00\x00|+\
+\x00\x00\x08|\x00\x00\x00\x00\x00\x01\x00\x00}\x97\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x07\xb8\x00\x00\x00\x00\x00\x01\x00\x00q\x04\
+\x00\x00\x07\xe0\x00\x00\x00\x00\x00\x01\x00\x00rp\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x08\x82\x00\x00\x00\x00\x00\x01\x00\x00\x7f\xe0\
+\x00\x00\x08\xaa\x00\x00\x00\x00\x00\x01\x00\x00\x81L\
 \x00\x00\x01\x8d\xf2\xd5$j\
-\x00\x00\x06L\x00\x00\x00\x00\x00\x01\x00\x00Z\x1b\
+\x00\x00\x06t\x00\x00\x00\x00\x00\x01\x00\x00[\x87\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x08\x08\x00\x00\x00\x00\x00\x01\x00\x00t\xb3\
+\x00\x00\x080\x00\x00\x00\x00\x00\x01\x00\x00v\x1f\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x06\xe6\x00\x00\x00\x00\x00\x01\x00\x00dT\
+\x00\x00\x07\x0e\x00\x00\x00\x00\x00\x01\x00\x00e\xc0\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x02\x10\x00\x00\x00\x00\x00\x01\x00\x00\x1b\xf1\
+\x00\x00\x028\x00\x00\x00\x00\x00\x01\x00\x00\x1d]\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x0c\x98\x00\x00\x00\x00\x00\x01\x00\x00\xba\xbf\
+\x00\x00\x0c\xc0\x00\x00\x00\x00\x00\x01\x00\x00\xbc+\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0ax\x00\x00\x00\x00\x00\x01\x00\x00\x99\x1d\
+\x00\x00\x0a\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x9a\x89\
 \x00\x00\x01\x8d[e\x92\xd1\
+\x00\x00\x01\xdc\x00\x00\x00\x00\x00\x01\x00\x00\x17=\
+\x00\x00\x01\x8f9\xc3\xae\xf0\
 \x00\x00\x00,\x00\x00\x00\x00\x00\x01\x00\x00\x01\xbc\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x04\x00\x00\x00\x00\x00\x00\x01\x00\x007\xbd\
+\x00\x00\x04(\x00\x00\x00\x00\x00\x01\x00\x009)\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x01$\x00\x00\x00\x00\x00\x01\x00\x00\x0d\x22\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x07\x10\x00\x00\x00\x00\x00\x01\x00\x00g\xcf\
+\x00\x00\x078\x00\x00\x00\x00\x00\x01\x00\x00i;\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x05\xba\x00\x00\x00\x00\x00\x01\x00\x00R\x1d\
+\x00\x00\x05\xe2\x00\x00\x00\x00\x00\x01\x00\x00S\x89\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x05,\x00\x00\x00\x00\x00\x01\x00\x00I\x8a\
+\x00\x00\x05T\x00\x00\x00\x00\x00\x01\x00\x00J\xf6\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x07B\x00\x00\x00\x00\x00\x01\x00\x00j\xfd\
+\x00\x00\x07j\x00\x00\x00\x00\x00\x01\x00\x00li\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x07\xce\x00\x00\x00\x00\x00\x01\x00\x00q\xc2\
+\x00\x00\x07\xf6\x00\x00\x00\x00\x00\x01\x00\x00s.\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x02\xca\x00\x00\x00\x00\x00\x01\x00\x00'\x07\
+\x00\x00\x02\xf2\x00\x00\x00\x00\x00\x01\x00\x00(s\
 \x00\x00\x01\x8d[e\x92\xcd\
 \x00\x00\x01p\x00\x00\x00\x00\x00\x01\x00\x00\x12f\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0a\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x9c\xc2\
+\x00\x00\x0a\xcc\x00\x00\x00\x00\x00\x01\x00\x00\x9e.\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x01\xdc\x00\x00\x00\x00\x00\x01\x00\x00\x17=\
+\x00\x00\x02\x04\x00\x00\x00\x00\x00\x01\x00\x00\x18\xa9\
 \x00\x00\x01\x8d[e\x92\xcd\
 \x00\x00\x01\x88\x00\x00\x00\x00\x00\x01\x00\x00\x14\x05\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0a\x10\x00\x00\x00\x00\x00\x01\x00\x00\x94\xf7\
+\x00\x00\x0a8\x00\x00\x00\x00\x00\x01\x00\x00\x96c\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x00\x10\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0b\xee\x00\x00\x00\x00\x00\x01\x00\x00\xb2\x18\
+\x00\x00\x0c\x16\x00\x00\x00\x00\x00\x01\x00\x00\xb3\x84\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0b\x92\x00\x00\x00\x00\x00\x01\x00\x00\xac\xc5\
+\x00\x00\x0b\xba\x00\x00\x00\x00\x00\x01\x00\x00\xae1\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x01\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x15\xe9\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0b4\x00\x00\x00\x00\x00\x01\x00\x00\xa6\x1b\
+\x00\x00\x0b\x5c\x00\x00\x00\x00\x00\x01\x00\x00\xa7\x87\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x02~\x00\x00\x00\x00\x00\x01\x00\x00\x22+\
+\x00\x00\x02\xa6\x00\x00\x00\x00\x00\x01\x00\x00#\x97\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0c\xba\x00\x00\x00\x00\x00\x01\x00\x00\xbb\xbc\
+\x00\x00\x0c\xe2\x00\x00\x00\x00\x00\x01\x00\x00\xbd(\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x04\xc0\x00\x00\x00\x00\x00\x01\x00\x00A\xec\
+\x00\x00\x04\xe8\x00\x00\x00\x00\x00\x01\x00\x00CX\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x08&\x00\x00\x00\x00\x00\x01\x00\x00v\x00\
+\x00\x00\x08N\x00\x00\x00\x00\x00\x01\x00\x00wl\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0b\x02\x00\x00\x00\x00\x00\x01\x00\x00\xa2\xd1\
+\x00\x00\x0b*\x00\x00\x00\x00\x00\x01\x00\x00\xa4=\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0d\xbe\x00\x00\x00\x00\x00\x01\x00\x00\xca4\
+\x00\x00\x0d\xe6\x00\x00\x00\x00\x00\x01\x00\x00\xcb\xa0\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0d\xf0\x00\x00\x00\x00\x00\x01\x00\x00\xcc\x8b\
+\x00\x00\x0e\x18\x00\x00\x00\x00\x00\x01\x00\x00\xcd\xf7\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x0c\xd0\x00\x00\x00\x00\x00\x01\x00\x00\xbc}\
+\x00\x00\x0c\xf8\x00\x00\x00\x00\x00\x01\x00\x00\xbd\xe9\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x0c\x1a\x00\x00\x00\x00\x00\x01\x00\x00\xb3\x87\
+\x00\x00\x0cB\x00\x00\x00\x00\x00\x01\x00\x00\xb4\xf3\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x04\xd8\x00\x00\x00\x00\x00\x01\x00\x00B\xca\
+\x00\x00\x05\x00\x00\x00\x00\x00\x00\x01\x00\x00D6\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x06\xc8\x00\x00\x00\x00\x00\x01\x00\x00b{\
+\x00\x00\x06\xf0\x00\x00\x00\x00\x00\x01\x00\x00c\xe7\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x01\x04\x00\x00\x00\x00\x00\x01\x00\x00\x0b\x93\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x09|\x00\x01\x00\x00\x00\x01\x00\x00\x8b\x09\
+\x00\x00\x09\xa4\x00\x01\x00\x00\x00\x01\x00\x00\x8cu\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0a\xd8\x00\x00\x00\x00\x00\x01\x00\x00\x9f\x94\
+\x00\x00\x0b\x00\x00\x00\x00\x00\x00\x01\x00\x00\xa1\x00\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x09^\x00\x00\x00\x00\x00\x01\x00\x00\x89\xdb\
+\x00\x00\x09\x86\x00\x00\x00\x00\x00\x01\x00\x00\x8bG\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0c\x04\x00\x00\x00\x00\x00\x01\x00\x00\xb2\xca\
+\x00\x00\x0c,\x00\x00\x00\x00\x00\x01\x00\x00\xb46\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x03\x0e\x00\x00\x00\x00\x00\x01\x00\x00*\xaf\
+\x00\x00\x036\x00\x00\x00\x00\x00\x01\x00\x00,\x1b\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x05F\x00\x00\x00\x00\x00\x01\x00\x00J\xd7\
+\x00\x00\x05n\x00\x00\x00\x00\x00\x01\x00\x00LC\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x05\x0e\x00\x00\x00\x00\x00\x01\x00\x00E\xe7\
+\x00\x00\x056\x00\x00\x00\x00\x00\x01\x00\x00GS\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0bz\x00\x00\x00\x00\x00\x01\x00\x00\xabp\
+\x00\x00\x0b\xa2\x00\x00\x00\x00\x00\x01\x00\x00\xac\xdc\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x04t\x00\x00\x00\x00\x00\x01\x00\x00=\xfc\
+\x00\x00\x04\x9c\x00\x00\x00\x00\x00\x01\x00\x00?h\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x05\x8a\x00\x00\x00\x00\x00\x01\x00\x00P$\
+\x00\x00\x05\xb2\x00\x00\x00\x00\x00\x01\x00\x00Q\x90\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x06\x08\x00\x00\x00\x00\x00\x01\x00\x00X\x0b\
+\x00\x00\x060\x00\x00\x00\x00\x00\x01\x00\x00Yw\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x06.\x00\x00\x00\x00\x00\x01\x00\x00Y\x05\
+\x00\x00\x06V\x00\x00\x00\x00\x00\x01\x00\x00Zq\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0a<\x00\x00\x00\x00\x00\x01\x00\x00\x96\xba\
+\x00\x00\x0ad\x00\x00\x00\x00\x00\x01\x00\x00\x98&\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x09\xc0\x00\x00\x00\x00\x00\x01\x00\x00\x91|\
+\x00\x00\x09\xe8\x00\x00\x00\x00\x00\x01\x00\x00\x92\xe8\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x00\x5c\x00\x00\x00\x00\x00\x01\x00\x00\x04o\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x09\x92\x00\x00\x00\x00\x00\x01\x00\x00\x8c6\
+\x00\x00\x09\xba\x00\x00\x00\x00\x00\x01\x00\x00\x8d\xa2\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0d$\x00\x00\x00\x00\x00\x01\x00\x00\xc1L\
+\x00\x00\x0dL\x00\x00\x00\x00\x00\x01\x00\x00\xc2\xb8\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0d<\x00\x00\x00\x00\x00\x01\x00\x00\xc3~\
+\x00\x00\x0dd\x00\x00\x00\x00\x00\x01\x00\x00\xc4\xea\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x02(\x00\x00\x00\x00\x00\x01\x00\x00\x1d\xd4\
+\x00\x00\x02P\x00\x00\x00\x00\x00\x01\x00\x00\x1f@\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x0b\xae\x00\x00\x00\x00\x00\x01\x00\x00\xaf]\
+\x00\x00\x0b\xd6\x00\x00\x00\x00\x00\x01\x00\x00\xb0\xc9\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x03\xbe\x00\x00\x00\x00\x00\x01\x00\x004\x8a\
+\x00\x00\x03\xe6\x00\x00\x00\x00\x00\x01\x00\x005\xf6\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x07,\x00\x00\x00\x00\x00\x01\x00\x00iy\
+\x00\x00\x07T\x00\x00\x00\x00\x00\x01\x00\x00j\xe5\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0a\xc2\x00\x00\x00\x00\x00\x01\x00\x00\x9d\xc5\
+\x00\x00\x0a\xea\x00\x00\x00\x00\x00\x01\x00\x00\x9f1\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x02\xf8\x00\x00\x00\x00\x00\x01\x00\x00)\xa3\
+\x00\x00\x03 \x00\x00\x00\x00\x00\x01\x00\x00+\x0f\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x07\xa0\x00\x00\x00\x00\x00\x01\x00\x00n\xeb\
+\x00\x00\x07\xc8\x00\x00\x00\x00\x00\x01\x00\x00pW\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x05\xf0\x00\x00\x00\x00\x00\x01\x00\x00U\xa0\
+\x00\x00\x06\x18\x00\x00\x00\x00\x00\x01\x00\x00W\x0c\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x01\xac\x00\x00\x00\x00\x00\x01\x00\x00\x14\xb9\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x01\xf2\x00\x00\x00\x00\x00\x01\x00\x00\x18!\
+\x00\x00\x02\x1a\x00\x00\x00\x00\x00\x01\x00\x00\x19\x8d\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x03\x82\x00\x00\x00\x00\x00\x01\x00\x002D\
+\x00\x00\x03\xaa\x00\x00\x00\x00\x00\x01\x00\x003\xb0\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x04<\x00\x00\x00\x00\x00\x01\x00\x00;\xec\
+\x00\x00\x04d\x00\x00\x00\x00\x00\x01\x00\x00=X\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x02d\x00\x00\x00\x00\x00\x01\x00\x00 \xf5\
+\x00\x00\x02\x8c\x00\x00\x00\x00\x00\x01\x00\x00\x22a\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x05\xd6\x00\x00\x00\x00\x00\x01\x00\x00T\x06\
+\x00\x00\x05\xfe\x00\x00\x00\x00\x00\x01\x00\x00Ur\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x04\x8c\x00\x00\x00\x00\x00\x01\x00\x00?\x1b\
+\x00\x00\x04\xb4\x00\x00\x00\x00\x00\x01\x00\x00@\x87\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x0d\x9c\x00\x00\x00\x00\x00\x01\x00\x00\xc8\xa4\
+\x00\x00\x0d\xc4\x00\x00\x00\x00\x00\x01\x00\x00\xca\x10\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0b \x00\x00\x00\x00\x00\x01\x00\x00\xa4\xda\
+\x00\x00\x0bH\x00\x00\x00\x00\x00\x01\x00\x00\xa6F\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x0c\xf4\x00\x00\x00\x00\x00\x01\x00\x00\xbe1\
+\x00\x00\x0d\x1c\x00\x00\x00\x00\x00\x01\x00\x00\xbf\x9d\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x04\xa8\x00\x00\x00\x00\x00\x01\x00\x00@\xa7\
+\x00\x00\x04\xd0\x00\x00\x00\x00\x00\x01\x00\x00B\x13\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x05r\x00\x00\x00\x00\x00\x01\x00\x00Nq\
+\x00\x00\x05\x9a\x00\x00\x00\x00\x00\x01\x00\x00O\xdd\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x03V\x00\x00\x00\x00\x00\x01\x00\x00.O\
+\x00\x00\x03~\x00\x00\x00\x00\x00\x01\x00\x00/\xbb\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x03n\x00\x00\x00\x00\x00\x01\x00\x00/\xa6\
+\x00\x00\x03\x96\x00\x00\x00\x00\x00\x01\x00\x001\x12\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0b`\x00\x00\x00\x00\x00\x01\x00\x00\xaaC\
+\x00\x00\x0b\x88\x00\x00\x00\x00\x00\x01\x00\x00\xab\xaf\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x06\x88\x00\x00\x00\x00\x00\x01\x00\x00]\x86\
+\x00\x00\x06\xb0\x00\x00\x00\x00\x00\x01\x00\x00^\xf2\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x00\x8a\x00\x00\x00\x00\x00\x01\x00\x00\x06\xb4\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x07\x5c\x00\x00\x00\x00\x00\x01\x00\x00l\x15\
+\x00\x00\x07\x84\x00\x00\x00\x00\x00\x01\x00\x00m\x81\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0dV\x00\x00\x00\x00\x00\x01\x00\x00\xc4\xf6\
+\x00\x00\x0d~\x00\x00\x00\x00\x00\x01\x00\x00\xc6b\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x088\x00\x00\x00\x00\x00\x01\x00\x00x\xd9\
+\x00\x00\x08`\x00\x00\x00\x00\x00\x01\x00\x00zE\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x02\xe2\x00\x00\x00\x00\x00\x01\x00\x00(\xe3\
+\x00\x00\x03\x0a\x00\x00\x00\x00\x00\x01\x00\x00*O\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x03&\x00\x00\x00\x00\x00\x01\x00\x00,5\
+\x00\x00\x03N\x00\x00\x00\x00\x00\x01\x00\x00-\xa1\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x03\xa4\x00\x00\x00\x00\x00\x01\x00\x003\x0d\
+\x00\x00\x03\xcc\x00\x00\x00\x00\x00\x01\x00\x004y\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x08\xbe\x00\x00\x00\x00\x00\x01\x00\x00\x82n\
+\x00\x00\x08\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x83\xda\
 \x00\x00\x01\x8d[e\x92\xcd\
 \x00\x00\x00\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x07\xfd\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x00\xba\x00\x00\x00\x00\x00\x01\x00\x00\x09\x05\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x05\xa2\x00\x00\x00\x00\x00\x01\x00\x00Qk\
+\x00\x00\x05\xca\x00\x00\x00\x00\x00\x01\x00\x00R\xd7\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x04\x5c\x00\x00\x00\x00\x00\x01\x00\x00<\xb3\
+\x00\x00\x04\x84\x00\x00\x00\x00\x00\x01\x00\x00>\x1f\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x0a\xec\x00\x00\x00\x00\x00\x01\x00\x00\xa1\xb2\
+\x00\x00\x0b\x14\x00\x00\x00\x00\x00\x01\x00\x00\xa3\x1e\
 \x00\x00\x01\x8d\x5c(\xc7\x04\
-\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x008\xe9\
+\x00\x00\x04F\x00\x00\x00\x00\x00\x01\x00\x00:U\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0b\xc8\x00\x00\x00\x00\x00\x01\x00\x00\xb1\x1d\
+\x00\x00\x0b\xf0\x00\x00\x00\x00\x00\x01\x00\x00\xb2\x89\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x03@\x00\x00\x00\x00\x00\x01\x00\x00-\x89\
+\x00\x00\x03h\x00\x00\x00\x00\x00\x01\x00\x00.\xf5\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0bJ\x00\x00\x00\x00\x00\x01\x00\x00\xa7\x8c\
+\x00\x00\x0br\x00\x00\x00\x00\x00\x01\x00\x00\xa8\xf8\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x08\xd6\x00\x00\x00\x00\x00\x01\x00\x00\x831\
+\x00\x00\x08\xfe\x00\x00\x00\x00\x00\x01\x00\x00\x84\x9d\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x0dt\x00\x00\x00\x00\x00\x01\x00\x00\xc6J\
+\x00\x00\x0d\x9c\x00\x00\x00\x00\x00\x01\x00\x00\xc7\xb6\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x00\x11.\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x09\xfa\x00\x00\x00\x00\x00\x01\x00\x00\x946\
+\x00\x00\x0a\x22\x00\x00\x00\x00\x00\x01\x00\x00\x95\xa2\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x09:\x00\x00\x00\x00\x00\x01\x00\x00\x88P\
+\x00\x00\x09b\x00\x00\x00\x00\x00\x01\x00\x00\x89\xbc\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0d\x0a\x00\x00\x00\x00\x00\x01\x00\x00\xbfX\
+\x00\x00\x0d2\x00\x00\x00\x00\x00\x01\x00\x00\xc0\xc4\
 \x00\x00\x01\x8d[e\x92\xcd\
 \x00\x00\x00r\x00\x00\x00\x00\x00\x01\x00\x00\x05\xb6\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0c\x80\x00\x00\x00\x00\x00\x01\x00\x00\xb9\x14\
+\x00\x00\x0c\xa8\x00\x00\x00\x00\x00\x01\x00\x00\xba\x80\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x06\xfa\x00\x00\x00\x00\x00\x01\x00\x00e\xe0\
+\x00\x00\x07\x22\x00\x00\x00\x00\x00\x01\x00\x00gL\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x08\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x81[\
+\x00\x00\x08\xcc\x00\x00\x00\x00\x00\x01\x00\x00\x82\xc7\
 \x00\x00\x01\x8d[e\x92\xd1\
 \x00\x00\x01:\x00\x00\x00\x00\x00\x01\x00\x00\x0f9\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x07\x84\x00\x00\x00\x00\x00\x01\x00\x00m\x12\
+\x00\x00\x07\xac\x00\x00\x00\x00\x00\x01\x00\x00n~\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x0a&\x00\x00\x00\x00\x00\x01\x00\x00\x95\xea\
+\x00\x00\x0aN\x00\x00\x00\x00\x00\x01\x00\x00\x97V\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x07\xe4\x00\x00\x00\x00\x00\x01\x00\x00s\xb5\
+\x00\x00\x08\x0c\x00\x00\x00\x00\x00\x01\x00\x00u!\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x09\xdc\x00\x00\x00\x00\x00\x01\x00\x00\x92:\
+\x00\x00\x0a\x04\x00\x00\x00\x00\x00\x01\x00\x00\x93\xa6\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x06\xa2\x00\x00\x00\x00\x00\x01\x00\x00`\xb1\
+\x00\x00\x06\xca\x00\x00\x00\x00\x00\x01\x00\x00b\x1d\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x08\xf0\x00\x00\x00\x00\x00\x01\x00\x00\x84\xab\
+\x00\x00\x09\x18\x00\x00\x00\x00\x00\x01\x00\x00\x86\x17\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0e\x0e\x00\x00\x00\x00\x00\x01\x00\x00\xce\x1b\
+\x00\x00\x0e6\x00\x00\x00\x00\x00\x01\x00\x00\xcf\x87\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0d\xd8\x00\x00\x00\x00\x00\x01\x00\x00\xcbI\
+\x00\x00\x0e\x00\x00\x00\x00\x00\x00\x01\x00\x00\xcc\xb5\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x02>\x00\x00\x00\x00\x00\x01\x00\x00\x1f&\
+\x00\x00\x02f\x00\x00\x00\x00\x00\x01\x00\x00 \x92\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x03\xea\x00\x00\x00\x00\x00\x01\x00\x006i\
+\x00\x00\x04\x12\x00\x00\x00\x00\x00\x01\x00\x007\xd5\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0aV\x00\x00\x00\x00\x00\x01\x00\x00\x97l\
+\x00\x00\x0a~\x00\x00\x00\x00\x00\x01\x00\x00\x98\xd8\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x0c^\x00\x00\x00\x00\x00\x01\x00\x00\xb7A\
+\x00\x00\x0c\x86\x00\x00\x00\x00\x00\x01\x00\x00\xb8\xad\
 \x00\x00\x01\x8d[e\x92\xcd\
-\x00\x00\x04\xec\x00\x00\x00\x00\x00\x01\x00\x00D\x87\
+\x00\x00\x05\x14\x00\x00\x00\x00\x00\x01\x00\x00E\xf3\
 \x00\x00\x01\x8d[e\x92\xcd\
 \x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x0a}\
 \x00\x00\x01\x8d[e\x92\xd1\
-\x00\x00\x05Z\x00\x00\x00\x00\x00\x01\x00\x00K\x8d\
+\x00\x00\x05\x82\x00\x00\x00\x00\x00\x01\x00\x00L\xf9\
 \x00\x00\x01\x8d[e\x92\xd5\
-\x00\x00\x09\xaa\x00\x00\x00\x00\x00\x01\x00\x00\x8fR\
+\x00\x00\x09\xd2\x00\x00\x00\x00\x00\x01\x00\x00\x90\xbe\
 \x00\x00\x01\x8d[e\x92\xd5\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/item/assistant.py` & `pygpt_net-2.2.8/src/pygpt_net/item/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/item/attachment.py` & `pygpt_net-2.2.8/src/pygpt_net/item/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/item/calendar_note.py` & `pygpt_net-2.2.8/src/pygpt_net/item/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/item/ctx.py` & `pygpt_net-2.2.8/src/pygpt_net/item/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/item/index.py` & `pygpt_net-2.2.8/src/pygpt_net/item/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/item/mode.py` & `pygpt_net-2.2.8/src/pygpt_net/item/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/item/model.py` & `pygpt_net-2.2.8/src/pygpt_net/item/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/item/notepad.py` & `pygpt_net-2.2.8/src/pygpt_net/item/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/item/preset.py` & `pygpt_net-2.2.8/src/pygpt_net/item/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/launcher.py` & `pygpt_net-2.2.8/src/pygpt_net/launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.20 06:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import sys
 import argparse
 from logging import ERROR, WARNING, INFO, DEBUG
 
 from PySide6.QtCore import QCoreApplication, Qt
 from PySide6.QtGui import QScreen
 from PySide6.QtWidgets import QApplication
 
+from pygpt_net.core.access.events import AppEvent
+from pygpt_net.core.access.shortcuts import GlobalShortcutFilter
 from pygpt_net.core.debug import Debug
 from pygpt_net.core.platforms import Platforms
 from pygpt_net.tools import BaseTool
 from pygpt_net.ui.main import MainWindow
 from pygpt_net.plugin.base import BasePlugin
 from pygpt_net.provider.llms.base import BaseLLM
 from pygpt_net.provider.loaders.base import BaseLoader
@@ -34,14 +36,15 @@
     def __init__(self):
         """Launcher"""
         self.app = None
         self.window = None
         self.debug = False
         self.force_legacy = False
         self.force_disable_gpu = False
+        self.shortcut_filter = None
 
     def setup(self) -> dict:
         """
         Setup launcher
 
         :return: dict with launcher arguments
         """
@@ -93,14 +96,15 @@
     def init(self):
         """Initialize app"""
         args = self.setup()
         Platforms.prepare()  # setup platform specific options
         QCoreApplication.setAttribute(Qt.AA_ShareOpenGLContexts)
         self.app = QApplication(sys.argv)
         self.window = MainWindow(self.app, args=args)
+        self.shortcut_filter = GlobalShortcutFilter(self.window)
 
     def add_plugin(self, plugin: BasePlugin):
         """
         Register plugin
 
         :param plugin: plugin instance
         """
@@ -227,8 +231,10 @@
         self.window.resize(geometry.width() - margin, geometry.height() - margin)
         self.window.show()
         self.window.move(pos)
         self.window.post_setup()
         self.app.setWindowIcon(self.window.ui.get_app_icon())
         self.window.ui.tray.setup(self.app)
         self.window.controller.after_setup()
+        self.window.core.dispatcher.dispatch(AppEvent(AppEvent.APP_STARTED))  # app event
+        self.window.installEventFilter(self.shortcut_filter)
         sys.exit(self.app.exec())
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231227152900.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231227152900.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231230095000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231230095000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231231230000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231231230000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240106060000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240106060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240107060000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240107060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240222160000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240222160000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240223050000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240223050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240303190000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240303190000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240408180000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240408180000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240426050000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240426050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240501030000.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240501030000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/migrations/base.py` & `pygpt_net-2.2.8/src/pygpt_net/migrations/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/agent/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/simple.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/simple.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.25 01:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import pyaudio
 import wave
 import os
 
 from PySide6.QtCore import QTimer
 
+from pygpt_net.core.access.events import AppEvent
 from pygpt_net.utils import trans
 
 
 class Simple:
 
     TIMEOUT_SECONDS = 120  # 2 minutes, max recording time before timeout
 
@@ -83,14 +84,15 @@
                                       channels=1,
                                       rate=44100,
                                       input=True,
                                       frames_per_buffer=1024,
                                       stream_callback=callback)
 
             self.plugin.window.ui.status(trans('audio.speak.now'))
+            self.plugin.window.core.dispatcher.dispatch(AppEvent(AppEvent.INPUT_VOICE_LISTEN_STARTED))  # app event
             self.stream.start_stream()
         except Exception as e:
             self.is_recording = False
             self.plugin.window.core.debug.log(e)
             self.plugin.window.ui.dialogs.alert(e)
             if self.plugin.window.core.platforms.is_snap():
                 self.plugin.window.ui.dialogs.open(
@@ -103,28 +105,29 @@
     def stop_recording(self, timeout: bool = False):
         """
         Stop recording
 
         :param timeout: True if stopped due to timeout
         """
         self.is_recording = False
+        self.plugin.window.core.dispatcher.dispatch(AppEvent(AppEvent.INPUT_VOICE_LISTEN_STOPPED))  # app event
         if self.timer:
             self.timer.stop()
             self.timer = None
         self.switch_btn_start()  # switch button to start
         path = os.path.join(self.plugin.window.core.config.path, self.plugin.input_file)
 
         if self.stream is not None:
             self.stream.stop_stream()
             self.stream.close()
             self.p.terminate()
 
             # abort if timeout
             if timeout:
-                self.plugin.window.ui.status("Timeout ({}s). Aborting...".format(self.TIMEOUT_SECONDS))
+                self.plugin.window.ui.status("Aborted.".format(self.TIMEOUT_SECONDS))
                 return
 
             if self.frames:
                 wf = wave.open(path, 'wb')
                 wf.setnchannels(1)
                 wf.setsampwidth(self.p.get_sample_size(pyaudio.paInt16))
                 wf.setframerate(44100)
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.19 06:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import os.path
 import time
 import speech_recognition as sr
 import audioop
 
@@ -250,7 +250,38 @@
 
             self.destroyed()
 
         except Exception as e:
             self.error(e)
             self.destroyed()
             print("Audio input thread error: {}".format(str(e)))
+
+
+class ControlWorker(BaseWorker):
+    def __init__(self, *args, **kwargs):
+        super(ControlWorker, self).__init__()
+        self.signals = WorkerSignals()
+        self.window = None
+        self.args = args
+        self.kwargs = kwargs
+        self.path = None
+        self.transcribe = False
+
+    @Slot()
+    def run(self):
+        """Handle mic simple mode."""
+        try:
+            # do transcribe
+            if os.path.exists(self.path):
+                # set status
+                self.status(trans('audio.speak.wait'))
+                # transcribe audio
+                transcript = self.window.core.plugins.get('audio_input').get_provider().transcribe(self.path)
+
+                # handle transcript
+                if transcript is not None and transcript.strip() != '':
+                    self.response(transcript)
+
+        except Exception as e:
+            self.error(e)
+            self.stopped()
+            self.status('Error: {}'.format(e))
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_output/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_output/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_output/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_output/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.09 10:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import Slot, Signal
 from pygpt_net.plugin.base import BaseWorker, BaseSignals
 
 
 class WorkerSignals(BaseSignals):
@@ -55,8 +55,30 @@
         self.stop()
 
     def stop(self):
         """Send stop signal to main thread"""
         self.signals.stop.emit()
 
 
+class PlayWorker(BaseWorker):
+    def __init__(self, *args, **kwargs):
+        super(PlayWorker, self).__init__()
+        self.signals = WorkerSignals()
+        self.args = args
+        self.kwargs = kwargs
+        self.window = None
+        self.path = None
+
+    @Slot()
+    def run(self):
+        from pygame import mixer
+        try:
+            if self.path:
+                mixer.init()
+                playback = mixer.Sound(self.path)
+                playback.play()
+        except Exception as e:
+            self.error(e)
+
+
+
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/base.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_api/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_api/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_api/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/runner.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/runner.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_custom/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_custom/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_custom/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_custom/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_files/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_files/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_files/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_files/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_history/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_history/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_history/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_history/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_serial/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_serial/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_serial/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_serial/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/websearch.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/websearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/crontab/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/crontab/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/experts/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/experts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from pygpt_net.plugin.base import BasePlugin
 from pygpt_net.core.dispatcher import Event
 
 
 class Plugin(BasePlugin):
     def __init__(self, *args, **kwargs):
         super(Plugin, self).__init__(*args, **kwargs)
         self.id = "experts"
         self.name = "Experts (inline)"
         self.description = "Enables inline experts in current mode."
         self.type = [
-            "experts",
+            "expert",
         ]
         self.allowed_cmds = [
             "expert_call",
         ]
         self.order = 9998
         self.use_locale = True
+        self.disallowed_modes = ["agent", "expert"]
         self.init_options()
 
     def init_options(self):
         """
         Initialize options
         """
         pass  # no options
@@ -53,30 +54,29 @@
 
     def is_allowed(self) -> bool:
         """
         Check if plugin is allowed to run
 
         :return: True if plugin is allowed to run
         """
-        return self.window.core.config.get("mode") != "expert"  # check global mode
+        return self.window.core.config.get("mode") not in self.disallowed_modes
 
     def handle(self, event: Event, *args, **kwargs):
         """
         Handle dispatched event
 
         :param event: event object
         :param args: event args
         :param kwargs: event kwargs
         """
-        name = event.name
-        data = event.data
-
-        if not self.is_allowed() and name != Event.DISABLE:
+        if not self.is_allowed():
             return
 
+        name = event.name
+        data = event.data
         if name == Event.SYSTEM_PROMPT:
             data['value'] = self.on_system_prompt(data['value'])
 
     def on_system_prompt(self, prompt: str) -> str:
         """
         Event: SYSTEM_PROMPT
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/extra_prompt/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/extra_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/idx_llama_index/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/idx_llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/idx_llama_index/worker.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/idx_llama_index/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/openai_dalle/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/openai_dalle/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/openai_vision/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/openai_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/plugin/real_time/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/plugin/real_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/bing_speech_recognition.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/bing_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/google_speech_recognition.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/google_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/openai_whisper.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/openai_whisper_local.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/openai_whisper_local.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/eleven_labs.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/google_tts.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/google_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/ms_azure_tts.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/ms_azure_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/openai_tts.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/openai_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/config/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/config/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/config/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/config/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/config/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/config/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import copy
 import os
 
 from packaging.version import parse as parse_version, Version
 
@@ -1428,14 +1428,62 @@
                 data["prompt.agent.instruction"] = self.window.core.config.get_base('prompt.agent.instruction')
                 data["prompt.agent.continue"] = self.window.core.config.get_base('prompt.agent.continue')
                 data["prompt.agent.goal"] = self.window.core.config.get_base('prompt.agent.goal')
                 data["prompt.expert"] = self.window.core.config.get_base('prompt.expert')
                 data["prompt.img"] = self.window.core.config.get_base('prompt.img')
                 updated = True
 
+            # < 2.2.8
+            if old < parse_version("2.2.8"):
+                print("Migrating config from < 2.2.8...")
+                if 'access.audio.event.speech' not in data:
+                    data["access.audio.event.speech"] = False
+                if 'access.audio.notify.execute' not in data:
+                    data["access.audio.notify.execute"] = True
+                if 'access.microphone.notify' not in data:
+                    data["access.microphone.notify"] = True
+                if 'access.shortcuts' not in data:
+                    data["access.shortcuts"] = [
+                        {
+                            "action": "voice_cmd.toggle",
+                            "key": "Space",
+                            "key_modifier": "Control"
+                        },
+                        {
+                            "action": "tab.chat",
+                            "key": "1",
+                            "key_modifier": "Control"
+                        },
+                        {
+                            "action": "tab.files",
+                            "key": "2",
+                            "key_modifier": "Control"
+                        },
+                        {
+                            "action": "tab.calendar",
+                            "key": "3",
+                            "key_modifier": "Control"
+                        },
+                        {
+                            "action": "tab.draw",
+                            "key": "4",
+                            "key_modifier": "Control"
+                        },
+                        {
+                            "action": "tab.notepad",
+                            "key": "5",
+                            "key_modifier": "Control"
+                        }
+                    ]
+                if 'access.voice_control' not in data:
+                    data["access.voice_control"] = False
+                if 'access.voice_control.model' not in data:
+                    data["access.voice_control.model"] = "gpt-3.5-turbo"
+                updated = True
+
         # update file
         migrated = False
         if updated:
             data = dict(sorted(data.items()))
             self.window.core.config.data = data
             self.window.core.config.save()
             migrated = True
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import time
 from uuid import uuid4
 from packaging.version import Version
 
 from pygpt_net.item.ctx import CtxMeta, CtxItem, CtxGroup
@@ -106,14 +106,22 @@
         """
         Return dict of ctx meta indexed by ID
 
         :return: dict of ctx meta indexed by ID
         """
         return self.storage.get_meta_indexed()
 
+    def get_last_meta_id(self) -> int:
+        """
+        Get last meta ID
+
+        :return: last meta ID
+        """
+        return self.storage.get_last_meta_id()
+
     def load(self, id: int) -> list:
         """
         Load items for ctx ID
 
         :param id: ctx ID
         :return: list of ctx items
         """
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.01 17:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from datetime import datetime
 import re
 import time
 
 from sqlalchemy import text
@@ -225,14 +225,31 @@
             row = result.fetchone()
             if row:
                 meta = CtxMeta()
                 unpack_meta(meta, row._asdict())
                 return meta
         return None
 
+    def get_last_meta_id(self) -> int:
+        """
+        Return last ctx meta ID
+
+        :return: int
+        """
+        stmt = text("""
+            SELECT id FROM ctx_meta ORDER BY updated_ts DESC LIMIT 1
+        """)
+        db = self.window.core.db.get_db()
+        with db.connect() as conn:
+            result = conn.execute(stmt)
+            row = result.fetchone()
+            if row:
+                return int(row.id)
+        return 0
+
     def get_items(self, id: int) -> list:
         """
         Return ctx items list by ctx meta ID
 
         :return: list of CtxItem
         """
         stmt = text("""
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/history/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/history/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/history/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/history/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/history/txt_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/history/txt_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/storage.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/utils.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/model/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/model/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/model/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/model/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/model/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/model/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/json_file.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/patch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,24 +193,27 @@
         if model is None:
             model = self.window.core.models.from_defaults()
 
         client = self.get_client()
         messages = []
         messages.append({"role": "system", "content": system_prompt})
         messages.append({"role": "user", "content": prompt})
+        additional_kwargs = {}
+        if max_tokens > 0:
+            additional_kwargs["max_tokens"] = max_tokens
         
         try:
             response = client.chat.completions.create(
                 messages=messages,
                 model=model.id,
-                max_tokens=max_tokens,
                 temperature=temperature,
                 top_p=1.0,
                 frequency_penalty=0.0,
                 presence_penalty=0.0,
+                **additional_kwargs,
             )
             return response.choices[0].message.content
         except Exception as e:
             self.window.core.debug.log(e)
             print("Error in GPT quick call: " + str(e))
 
     def stop(self):
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/assistants.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/chat.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/completion.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/image.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/store.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/summarizer.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/vision.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/assistants.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/importer.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/importer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/llms/anthropic.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/llms/azure_openai.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/llms/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/llms/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/llms/hugging_face.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/llms/hugging_face.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/llms/llama.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/llms/llama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/llms/ollama.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/llms/openai.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/llms/openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_csv.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_csv.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_docx.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_docx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_epub.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_epub.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_excel.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_excel.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_html.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_html.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_image_vision.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_image_vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_ipynb.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_ipynb.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_json.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_json.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_markdown.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_pdf.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_pdf.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_video_audio.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_video_audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_xml.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_xml.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/database/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/database/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/issues.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/repo.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/calendar.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/docs.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/gmail.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/keep.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/sheets.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/image_vision/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/image_vision/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/json/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/json/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/simple_csv/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/simple_csv/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/video_audio/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/video_audio/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/web_page/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/web_page/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/utils.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_bitbucket.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_bitbucket.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_database.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_database.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_github_issues.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_github_issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_github_repo.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_github_repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_calendar.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_docs.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_drive.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_drive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_gmail.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_keep.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_sheets.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_page.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_rss.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_rss.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_sitemap.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_sitemap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_twitter.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_twitter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_yt.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_yt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/chroma.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/elasticsearch.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/pinecode.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/pinecode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/redis.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/simple.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/temp.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/temp.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/web/base.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/web/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/web/google_custom_search.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/web/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/provider/web/microsoft_bing.py` & `pygpt_net-2.2.8/src/pygpt_net/provider/web/microsoft_bing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/base.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/dialogs.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/widgets.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/ui/dialogs.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/browse.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/browse.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/ctx.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/dialogs.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/files.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/web.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/widgets.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/media_player/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/media_player/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/dialogs.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/widgets.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/dialogs.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/widgets.py` & `pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/base/config_dialog.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/base/config_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.27 04:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QHBoxLayout, QLabel, QVBoxLayout, QSizePolicy, QWidget, QFrame
 
 from pygpt_net.ui.widget.element.labels import TitleLabel, UrlLabel
 from pygpt_net.ui.widget.option.checkbox import OptionCheckbox
@@ -66,14 +66,15 @@
                 self.window.controller.config.placeholder.apply(option)
                 widgets[key] = OptionDict(self.window, id, key, option)  # dictionary
                 widgets[key].setMinimumHeight(200)
                 widgets[key].setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
             elif option['type'] == 'combo':
                 self.window.controller.config.placeholder.apply(option)
                 widgets[key] = OptionCombo(self.window, id, key, option)  # combobox
+                widgets[key].fit_to_content()
 
         return widgets
 
     def add_option(self, widget: QWidget, option: dict) -> QHBoxLayout:
         """
         Add option
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/base/context_menu.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/base/context_menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/about.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/applog.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/assistant.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/assistant_store.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/changelog.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/changelog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/create.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/db.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/debug.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/dictionary.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/editor.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/find.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/image.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/license.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/logger.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/models.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/plugins.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/preset.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/preset_plugins.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/profile.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/rename.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/settings.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.28 22:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
+
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QStandardItemModel
 from PySide6.QtWidgets import QPushButton, QHBoxLayout, QLabel, QVBoxLayout, QScrollArea, QWidget, QSizePolicy, \
     QTabWidget, QSplitter
 
 from pygpt_net.ui.base.config_dialog import BaseConfigDialog
 from pygpt_net.ui.widget.dialog.settings import SettingsDialog
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/snap.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/start.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/start.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/update.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/workdir.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/dialogs.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/attachments.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/attachments_uploaded.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/attachments_uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/calendar.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/input.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/markdown.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/output.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/painter.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/ctx_list.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/ctx_list.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/search_input.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/video.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/status.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/status.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/agent.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.01.30 15:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtWidgets import QVBoxLayout, QLabel, QHBoxLayout, QWidget, QCheckBox
 
 from pygpt_net.ui.widget.option.slider import OptionSlider
 from pygpt_net.utils import trans
 
@@ -41,15 +41,15 @@
                 option,
             )
 
         # img raw
         self.window.ui.config['global']['agent.auto_stop'] = QCheckBox(trans("toolbox.agent.auto_stop.label"))
         self.window.ui.config['global']['agent.auto_stop'].stateChanged.connect(
             lambda:
-            self.window.controller.agent.toggle_auto_stop(
+            self.window.controller.agent.common.toggle_auto_stop(
                 self.window.ui.config['global']['agent.auto_stop'].isChecked())
         )
 
         # label
         label = QLabel(trans("toolbox.agent.iterations.label"))
 
         # options
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/assistants.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/footer.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/footer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.29 01:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtCore import QSize
-from PySide6.QtGui import Qt, QIcon
-from PySide6.QtWidgets import QVBoxLayout, QLabel, QHBoxLayout, QPushButton, QWidget, QSizePolicy
+from PySide6.QtGui import QIcon
+from PySide6.QtWidgets import QVBoxLayout, QLabel, QPushButton, QWidget, QSizePolicy
+
+from pygpt_net.ui.widget.textarea.name import NameInput
+from pygpt_net.ui.widget.option.slider import OptionSlider
+from pygpt_net.ui.widget.audio.input_button import VoiceControlButton
+from pygpt_net.utils import trans
 
 from .agent import Agent
 from .image import Image
 from .indexes import Indexes
 from .vision import Vision
-from pygpt_net.ui.widget.textarea.name import NameInput
-from pygpt_net.ui.widget.option.slider import OptionSlider
-from pygpt_net.utils import trans
 
 
 class Footer:
     def __init__(self, window=None):
         """
         Toolbox UI
 
@@ -51,22 +53,27 @@
         # bottom
         option = dict(self.window.controller.settings.editor.get_options()["temperature"])
         self.window.ui.nodes['temperature.label'] = QLabel(trans("toolbox.temperature.label"))
         self.window.ui.config['global']['current_temperature'] = \
             OptionSlider(self.window, 'global', 'current_temperature', option)
         self.window.ui.add_hook("update.global.current_temperature", self.window.controller.mode.hook_global_temperature)
 
+        # voice control btn
+        self.window.ui.nodes['voice.control.btn'] = VoiceControlButton(self.window)
+        self.window.ui.nodes['voice.control.btn'].setVisible(False)
+
         # per mode options
         rows = QVBoxLayout()
         # rows.addWidget(self.window.ui.nodes['temperature.label'])
         # rows.addWidget(self.window.ui.config['global']['current_temperature'])
         rows.addWidget(self.agent.setup())
         rows.addWidget(self.image.setup())
         # rows.addWidget(self.vision.setup())
         rows.addWidget(self.indexes.setup_options())
+        rows.addWidget(self.window.ui.nodes['voice.control.btn'])
         rows.setContentsMargins(0, 0, 0, 0)
 
         # logo
         logo_button = self.setup_logo()
 
         # bottom (options and logo)
         # bottom = QHBoxLayout()
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/image.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/indexes.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/mode.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/model.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/presets.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/prompt.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/vision.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/main.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/main.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/__init__.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/about.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/audio.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/config.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.09 23:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QMenu
 
 from pygpt_net.utils import trans
 import pygpt_net.icons_rc
@@ -35,14 +35,17 @@
         self.window.ui.menu['config.settings'] = QAction(QIcon(":/icons/settings_filled.svg"),
                                                          trans("menu.config.settings"), self.window)
         self.window.ui.menu['config.settings'].setMenuRole(QAction.MenuRole.NoRole)
 
         self.window.ui.menu['config.models'] = QAction(QIcon(":/icons/settings_filled.svg"),
                                                        trans("menu.config.models"), self.window)
 
+        self.window.ui.menu['config.access'] = QAction(QIcon(":/icons/accessibility.svg"),
+                                                       trans("menu.config.access"), self.window)
+
         css_files = []
         css_files.append("style.css")
         css_files.append("style.dark.css")
         css_files.append("style.light.css")
         css_files.append("markdown.css")
         css_files.append("markdown.dark.css")
         css_files.append("markdown.light.css")
@@ -125,14 +128,17 @@
 
         self.window.ui.menu['config.settings'].triggered.connect(
             lambda: self.window.controller.settings.toggle_editor('settings'))
 
         self.window.ui.menu['config.models'].triggered.connect(
             lambda: self.window.controller.model.editor.toggle_editor())
 
+        self.window.ui.menu['config.access'].triggered.connect(
+            lambda: self.window.controller.settings.open_section('access'))
+
         self.window.ui.menu['config.open_dir'].triggered.connect(
             lambda: self.window.controller.settings.open_config_dir())
 
         self.window.ui.menu['config.change_dir'].triggered.connect(
             lambda: self.window.controller.settings.workdir.change())
 
         self.window.ui.menu['config.save'].triggered.connect(
@@ -140,14 +146,15 @@
 
         self.lang.setup()
         self.theme.setup()
 
         self.window.ui.menu['menu.config'] = self.window.menuBar().addMenu(trans("menu.config"))
         self.window.ui.menu['menu.config'].addAction(self.window.ui.menu['config.settings'])
         self.window.ui.menu['menu.config'].addAction(self.window.ui.menu['config.models'])
+        self.window.ui.menu['menu.config'].addAction(self.window.ui.menu['config.access'])
 
         self.window.ui.menu['menu.config'].addMenu(self.window.ui.menu['menu.theme'])
         self.window.ui.menu['menu.config'].addMenu(self.window.ui.menu['menu.lang'])
         self.window.ui.menu['menu.config'].addMenu(self.window.ui.menu['config.edit.css'])
         self.window.ui.menu['menu.config'].addMenu(self.window.ui.menu['config.edit.json'])
         self.window.ui.menu['menu.config'].addMenu(self.window.ui.menu['config.profile'])
         self.window.ui.menu['menu.config'].addAction(self.window.ui.menu['config.open_dir'])
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/debug.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/file.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/lang.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/lang.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/plugins.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/theme.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/theme.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/tools.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/tools.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/menu/video.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/menu/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/tray.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/tray.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/input.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/input_button.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/output.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,67 +2,53 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.28 22:00:00                  #
+# Updated Date: 2023.12.25 21:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QLabel, QHBoxLayout, QWidget, QPushButton
+from PySide6.QtWidgets import QLabel, QHBoxLayout, QWidget
 
-from pygpt_net.core.dispatcher import Event
-from pygpt_net.utils import trans
 
-
-class AudioInputButton(QWidget):
+class AudioOutput(QWidget):
     def __init__(self, window=None):
         """
-        Audio input record button
+        Settings audio output options
 
-        :param window: Window instance
+        :param window: main window
         """
-        super(AudioInputButton, self).__init__(window)
+        super(AudioOutput, self).__init__(window)
         self.window = window
 
-        self.btn_toggle = QPushButton(trans('audio.speak.btn'))
-        self.btn_toggle.clicked.connect(self.toggle_recording)
-        self.btn_toggle.setToolTip(trans('audio.speak.btn.tooltip'))
-        self.btn_toggle.setCursor(Qt.PointingHandCursor)
-        self.btn_toggle.setMinimumWidth(200)
+        # stop button
+        # self.stop = QPushButton("STOP")
+        # self.stop.setVisible(False)
+        # self.stop.setMaximumHeight(40)
 
-        # status
         self.status = QLabel("")
-        self.status.setStyleSheet("color: #999; font-size: 10px; font-weight: 400; margin: 0; padding: 0; border: 0;")
-        self.status.setMaximumHeight(15)
-
         self.layout = QHBoxLayout(self)
-        self.layout.addWidget(self.btn_toggle)
         self.layout.addWidget(self.status)
-
         # self.layout.addWidget(self.stop)
         self.layout.setAlignment(Qt.AlignCenter)
         self.setLayout(self.layout)
-        self.setMaximumHeight(80)
+
+        self.setMinimumHeight(40)
+        self.setMaximumHeight(40)
 
     def add_widget(self, widget):
         """
         Add widget to layout
 
-        :param widget: widget
+        :param widget: QWidget
         """
         self.layout.addWidget(widget)
 
     def set_status(self, text):
         """
         Set status text
-
-        :param text: text
+        :param text: Text to set
         """
         self.status.setText(text)
-
-    def toggle_recording(self):
-        """Toggle recording"""
-        event = Event(Event.AUDIO_INPUT_RECORD_TOGGLE)
-        self.window.core.dispatcher.dispatch(event)
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/output.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/create.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,53 +2,42 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2023.12.25 21:00:00                  #
+# Updated Date: 2024.01.27 19:00:00                  #
 # ================================================== #
 
-from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QLabel, QHBoxLayout, QWidget
+from PySide6 import QtCore
+from PySide6.QtWidgets import QLineEdit
 
 
-class AudioOutput(QWidget):
-    def __init__(self, window=None):
+class CreateInput(QLineEdit):
+    def __init__(self, window=None, id=None):
         """
-        Settings audio output options
+        Create dialog input
 
         :param window: main window
+        :param id: info window id
         """
-        super(AudioOutput, self).__init__(window)
-        self.window = window
-
-        # stop button
-        # self.stop = QPushButton("STOP")
-        # self.stop.setVisible(False)
-        # self.stop.setMaximumHeight(40)
-
-        self.status = QLabel("")
-        self.layout = QHBoxLayout(self)
-        self.layout.addWidget(self.status)
-        # self.layout.addWidget(self.stop)
-        self.layout.setAlignment(Qt.AlignCenter)
-        self.setLayout(self.layout)
+        super(CreateInput, self).__init__(window)
 
-        self.setMinimumHeight(40)
-        self.setMaximumHeight(40)
+        self.window = window
+        self.id = id
 
-    def add_widget(self, widget):
+    def keyPressEvent(self, event):
         """
-        Add widget to layout
+        Key press event
 
-        :param widget: QWidget
+        :param event: key event
         """
-        self.layout.addWidget(widget)
+        super(CreateInput, self).keyPressEvent(event)
 
-    def set_status(self, text):
-        """
-        Set status text
-        :param text: Text to set
-        """
-        self.status.setText(text)
+        # save on Enter
+        if event.key() == QtCore.Qt.Key_Return or event.key() == QtCore.Qt.Key_Enter:
+            self.window.controller.dialogs.confirm.accept_create(
+                self.window.ui.dialog['create'].id,
+                self.window.ui.dialog['create'].current,
+                self.text(),
+            )
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/calendar/select.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/calendar/select.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/alert.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/alert.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/applog.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/assistant_store.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/audio.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/base.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/confirm.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/create.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/db.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/debug.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/editor.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/editor_file.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/editor_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/find.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/image.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/info.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/license.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/logger.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/model.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/preset_plugins.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/profile.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/rename.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/settings.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/settings_plugin.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/settings_plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/snap.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/update.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/workdir.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/draw/painter.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/draw/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/button.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/checkbox.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/group.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/group.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/labels.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/labels.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/filesystem/explorer.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/filesystem/explorer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/image/display.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/image/display.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/assistant.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/assistant_store.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/attachment.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/base.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/context.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/db.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/debug.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/experts.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/experts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/index.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/index_combo.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/index_combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/mode.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/model.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/model_editor.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/model_editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/plugin.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/preset.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/preset_plugins.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/profile.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/settings.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/uploaded.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/checkbox.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/cmd.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/combo.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/combo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.17 07:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtWidgets import QHBoxLayout, QWidget, QComboBox
 
 from pygpt_net.utils import trans
 
 
@@ -113,8 +113,9 @@
         :return:
         """
         self.current_id = self.combo.itemData(index)
         self.window.controller.config.combo.on_update(self.parent_id, self.id, self.option, self.current_id)
 
     def fit_to_content(self):
         """Fit to content"""
-        self.combo.setSizeAdjustPolicy(QComboBox.AdjustToContents)
+        self.combo.setSizeAdjustPolicy(QComboBox.AdjustToContents)
+
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/dictionary.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.11 01:00:00                  #
+# Updated Date: 2024.05.02 19:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import Qt, QAbstractItemModel, QModelIndex, QSize
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QWidget, QVBoxLayout, QPushButton, QTreeView, QMenu, QStyledItemDelegate, QComboBox, \
     QCheckBox, QSizePolicy
 
@@ -370,27 +370,38 @@
     def __init__(self, parent=None, keys=None):
         super(ComboBoxDelegate, self).__init__(parent)
         self.keys = keys
 
     def createEditor(self, parent, option, index):
         editor = QComboBox(parent)
         for item in self.keys:
-            if type(item) is dict:
+            if isinstance(item, dict):
                 for key, value in item.items():
                     editor.addItem(value, key)
             else:
                 editor.addItem(item)
         return editor
 
     def setEditorData(self, editor, index):
-        value = index.model().data(index, Qt.EditRole)
-        editor.setCurrentText(value)
+        key = index.model().data(index, Qt.EditRole)
+        if key is not None:
+            index = editor.findData(key)
+            if index >= 0:
+                editor.setCurrentIndex(index)
 
     def setModelData(self, editor, model, index):
-        model.setData(index, editor.currentText(), Qt.EditRole)
+        key = editor.currentData()
+        model.setData(index, key, Qt.EditRole)
+
+    def displayText(self, value, locale):
+        for item in self.keys:
+            if isinstance(item, dict):
+                if value in item:
+                    return item[value]
+        return value
 
 
 class MaxHeightDelegate(QStyledItemDelegate):
     def __init__(self, max, parent=None):
         super().__init__(parent)
         self.maxHeight = max
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/input.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/prompt.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/slider.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/textarea.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/Input.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/Input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/output.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/calendar_note.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/create.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/name.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,42 +2,34 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.01.27 19:00:00                  #
+# Updated Date: 2024.01.27 11:00:00                  #
 # ================================================== #
 
-from PySide6 import QtCore
 from PySide6.QtWidgets import QLineEdit
 
 
-class CreateInput(QLineEdit):
+class NameInput(QLineEdit):
     def __init__(self, window=None, id=None):
         """
-        Create dialog input
+        AI or user name input
 
-        :param window: main window
-        :param id: info window id
+        :param window: Window instance
+        :param id: input id
         """
-        super(CreateInput, self).__init__(window)
-
+        super(NameInput, self).__init__(window)
         self.window = window
         self.id = id
 
     def keyPressEvent(self, event):
         """
         Key press event
 
         :param event: key event
         """
-        super(CreateInput, self).keyPressEvent(event)
-
-        # save on Enter
-        if event.key() == QtCore.Qt.Key_Return or event.key() == QtCore.Qt.Key_Enter:
-            self.window.controller.dialogs.confirm.accept_create(
-                self.window.ui.dialog['create'].id,
-                self.window.ui.dialog['create'].current,
-                self.text(),
-            )
+        super(NameInput, self).keyPressEvent(event)
+        self.window.controller.ui.update_tokens()
+        self.window.controller.presets.editor.update_from_global(self.id, self.text())
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/editor.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/find.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/input.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/name.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/rename.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,34 +2,42 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.01.27 11:00:00                  #
+# Updated Date: 2024.01.27 19:00:00                  #
 # ================================================== #
 
+from PySide6 import QtCore
 from PySide6.QtWidgets import QLineEdit
 
 
-class NameInput(QLineEdit):
+class RenameInput(QLineEdit):
     def __init__(self, window=None, id=None):
         """
-        AI or user name input
+        Rename dialog input
 
-        :param window: Window instance
-        :param id: input id
+        :param window: main window
+        :param id: info window id
         """
-        super(NameInput, self).__init__(window)
+        super(RenameInput, self).__init__(window)
+
         self.window = window
         self.id = id
 
     def keyPressEvent(self, event):
         """
         Key press event
 
         :param event: key event
         """
-        super(NameInput, self).keyPressEvent(event)
-        self.window.controller.ui.update_tokens()
-        self.window.controller.presets.editor.update_from_global(self.id, self.text())
+        super(RenameInput, self).keyPressEvent(event)
+
+        # save on Enter
+        if event.key() == QtCore.Qt.Key_Return or event.key() == QtCore.Qt.Key_Enter:
+            self.window.controller.dialogs.confirm.accept_rename(
+                self.window.ui.dialog['rename'].id,
+                self.window.ui.dialog['rename'].current,
+                self.text(),
+            )
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/notepad.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/output.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/rename.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/search_input.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,42 +2,56 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.01.27 19:00:00                  #
+# Updated Date: 2024.04.12 10:00:00                  #
 # ================================================== #
 
-from PySide6 import QtCore
-from PySide6.QtWidgets import QLineEdit
+from PySide6.QtGui import QAction, QIcon
+from PySide6.QtWidgets import QLineEdit, QStyle
 
+from pygpt_net.utils import trans
+import pygpt_net.icons_rc
 
-class RenameInput(QLineEdit):
-    def __init__(self, window=None, id=None):
-        """
-        Rename dialog input
 
-        :param window: main window
-        :param id: info window id
+class CtxSearchInput(QLineEdit):
+    def __init__(self, window=None):
         """
-        super(RenameInput, self).__init__(window)
+        Search input
 
+        :param window: Window instance
+        """
+        super(CtxSearchInput, self).__init__(window)
         self.window = window
-        self.id = id
+        self.setPlaceholderText(trans('ctx.list.search.placeholder'))
+
+        self.clear_action = QAction(self)
+        self.clear_action.setIcon(QIcon(":/icons/close.svg"))
+        self.clear_action.triggered.connect(self.clear_search_string)
+        self.addAction(self.clear_action, QLineEdit.TrailingPosition)
+        self.clear_action.setVisible(False)
+
+        self.textChanged.connect(self.on_text_changed)
+
+    def clear_search_string(self):
+        """Clear input"""
+        self.clear()
+        self.window.controller.ctx.search_string_clear()
 
-    def keyPressEvent(self, event):
+    def on_text_changed(self, text):
         """
-        Key press event
+        On text changed
 
-        :param event: key event
+        :param text: text
         """
-        super(RenameInput, self).keyPressEvent(event)
+        self.window.controller.ctx.search_string_change(text)
+        self.clear_action.setVisible(bool(text))
+
+    def focusInEvent(self, event):
+        """Focus in event"""
+        super(CtxSearchInput, self).focusInEvent(event)
+        self.window.controller.ctx.search_focus_in()
+
 
-        # save on Enter
-        if event.key() == QtCore.Qt.Key_Return or event.key() == QtCore.Qt.Key_Enter:
-            self.window.controller.dialogs.confirm.accept_rename(
-                self.window.ui.dialog['rename'].id,
-                self.window.ui.dialog['rename'].current,
-                self.text(),
-            )
```

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/web.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/ui/widget/vision/camera.py` & `pygpt_net-2.2.8/src/pygpt_net/ui/widget/vision/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/src/pygpt_net/utils.py` & `pygpt_net-2.2.8/src/pygpt_net/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.7/PKG-INFO` & `pygpt_net-2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 2.2.7
+Version: 2.2.8
 Summary: Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more
 Home-page: https://github.com/szczyglis-dev/py-gpt
 License: MIT
 Keywords: py_gpt,py-gpt,pygpt,desktop,app,gpt,gpt4,gpt4-v,gpt3.5,gpt-4,gpt-4V,gpt-3.5,tts,whisper,vision,chatgpt,dall-e,chat,chatbot,assistant,text completion,image generation,ai,api,openai,api key,langchain,llama-index,presets,ui,qt,pyside
 Author: Marcin Szczyglinski
 Author-email: info@pygpt.net
 Requires-Python: >=3.10,<3.12
@@ -70,15 +70,15 @@
 Project-URL: Repository, https://github.com/szczyglis-dev/py-gpt
 Description-Content-Type: text/markdown
 
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.7** | build: **2024.05.01** | Python: **>=3.10, <3.12**
+Release: **2.2.8** | build: **2024.05.02** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -106,14 +106,15 @@
 
 ## Features
 
 - Desktop AI Assistant for `Linux`, `Windows` and `Mac`, written in Python.
 - Works similarly to `ChatGPT`, but locally (on a desktop computer).
 - 9 modes of operation: Chat, Vision, Completion, Assistant, Image generation, Langchain, Chat with files, Experts and Agent (autonomous).
 - Supports multiple models: `GPT-4`, `GPT-3.5`, and any model accessible through `Langchain`.
+- Included support for disabled people: voice control and translates actions on the screen using audio synthesis.
 - Handles and stores the full context of conversations (short-term memory).
 - Real-time video camera capture in Vision mode.
 - Internet access via `Google` and `Microsoft Bing`.
 - Speech synthesis via `Microsoft Azure`, `Google`, `Eleven Labs` and `OpenAI` Text-To-Speech services.
 - Speech recognition via `OpenAI Whisper`, `Google`, `Google Cloud` and `Microsoft Bing`.
 - Image analysis via `GPT-4 Vision`.
 - Crontab / Task scheduler included.
@@ -930,14 +931,112 @@
 
 You can also ask for a list of active experts at any time:
 
 ```bash
 Give me a list of active experts.
 ```
 
+# Accessibility
+
+Since version `2.2.8`, PyGPT has added beta support for disabled people and voice control. This may be very useful for blind people.
+
+
+In the `Config / Accessibility` menu, you can turn on accessibility features such as:
+
+
+- activating voice control
+
+- translating actions and events on the screen with audio speech
+
+- setting up keyboard shortcuts for actions.
+
+
+**To enable voice control:**
+
+
+Turn on the voice control option in `Config / Accessibility`:
+
+
+```bash
+Enable voice control (using microphone)
+```
+
+Once you enable this option, an `Audio Control` button will appear at the bottom right corner of the window. When you click on this button, the microphone will start listening; clicking it again stops listening and starts recognizing the voice command you said. You can cancel voice recording at any time with the `ESC` key. You can also set a keyboard shortcut to turn voice recording on/off.
+
+
+Voice command recognition works based on a model, so you don't have to worry about saying things perfectly.
+
+
+**Here's a list of commands you can ask for by voice:**
+
+- Get the current application status
+- Exit the application
+- Enable audio output
+- Disable audio output
+- Enable audio input
+- Disable audio input
+- Enable the camera
+- Disable the camera
+- Capture the camera
+- Create a new context
+- Go to the previous context
+- Go to the next context
+- Go to the last context
+- Focus on the input
+- Send the input
+- Clear the input
+- Get current conversation info
+- Stop executing current action
+- Clear the attachments
+- Read the last conversation entry
+- Read the whole conversation
+- Send the message to input
+- Append message to current input without sending it
+- Switch to chat mode
+- Switch to Chat with files (llama-index) mode
+- Add note to notepad
+- Read current notepad contents
+- Switch to the chat tab
+- Switch to the calendar tab
+- Switch to the draw (painter) tab
+- Switch to the files tab
+- Switch to the notepad tab
+- Switch to the next tab
+- Switch to the previous tab
+- Start listening for voice input
+- Stop listening for voice input
+- Toggle listening for voice input
+
+More commands coming soon.
+
+Just ask for an action that matches one of the descriptions above. These descriptions are also known to the model, and relevant commands are assigned to them. When you voice a command that fits one of those patterns, the model will trigger the appropriate action.
+
+
+For convenience, you can enable a short sound to play when voice recording starts and stops. To do this, turn on the option:
+
+
+```bash
+Audio notify microphone listening start/stop
+```
+
+To enable a sound notification when a voice command is recognized and command execution begins, turn on the option:
+
+
+```bash
+Audio notify voice command execution
+```
+
+For voice translation of on-screen events and information about completed commands via speech synthesis, you can turn on the option:
+
+```bash
+Use voice synthesis to describe events on the screen.
+```
+
+![v2_access](https://github.com/szczyglis-dev/py-gpt/assets/61396542/02dd161b-6fb1-48f9-9217-40c658888833)
+
 
 # Files and attachments
 
 ## Input attachments (upload)
 
 **PyGPT** makes it simple for users to upload files to the server and send them to the model for tasks like analysis, similar to attaching files in `ChatGPT`. There's a separate `Files` tab next to the text input area specifically for managing file uploads. Users can opt to have files automatically deleted after each upload or keep them on the list for repeated use.
 
@@ -3167,14 +3266,20 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.8 (2024-05-02)**
+
+- Added support for disabled people, including voice control and screen event translation with audio synthesis.
+- A new section in Settings called 'Accessibility' has been added with options for assistance: voice control, keyboard shortcut definitions for actions, and screen event translation using audio synthesis.
+- A new section called 'Accessibility' has been added to the Documentation.
+
 **2.2.7 (2024-05-01)**
 
 - A new experimental work mode has been added: 'Experts', which allows the creation of separate background instances with their own instructions that can be consulted for help. See the documentation: 'Work Modes / Experts'.
 - Added a new plugin: 'Experts (inline)`.
 - Improved the Agent mode by adding the ability to configure and invoke defined Experts.
 - Improved the prompts that control the autonomous mode.
 - The main prompt controlling the agents has been moved from presets to the application's settings window.
```

