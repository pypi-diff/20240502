# Comparing `tmp/plextraktsync-0.30.1.tar.gz` & `tmp/plextraktsync-0.30.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plextraktsync-0.30.1.tar", last modified: Mon Apr 29 19:52:38 2024, max compression
+gzip compressed data, was "plextraktsync-0.30.2.tar", last modified: Thu May  2 15:28:51 2024, max compression
```

## Comparing `plextraktsync-0.30.1.tar` & `plextraktsync-0.30.2.tar`

### file list

```diff
@@ -1,170 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    30005 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30005 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26812 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.466534 plextraktsync-0.30.1/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 19:52:35.000000 plextraktsync-0.30.1/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.466534 plextraktsync-0.30.1/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/ServerConfigFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/logger/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/media/
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/media/Media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/media/MediaFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/mixin/RichMarkup.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/mixin/SetWindowTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plan/WalkConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plan/WalkPlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plan/WalkPlanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plan/Walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.474534 plextraktsync-0.30.1/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderIMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderMbid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderTMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderTVDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexIdFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexPlaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexPlaylistCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexSectionPager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.474534 plextraktsync-0.30.1/plextraktsync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.474534 plextraktsync-0.30.1/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/TraktScrobbleWorker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.474534 plextraktsync-0.30.1/plextraktsync/rich/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/rich/RichHighlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/rich/RichProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.478534 plextraktsync-0.30.1/plextraktsync/sync/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/AddCollectionPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/ClearCollectedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/LikedListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/Sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/SyncRatingsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/SyncWatchedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/TraktListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/WatchListPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/WatchProgressPlugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.478534 plextraktsync-0.30.1/plextraktsync/sync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/plugin/SyncPluginInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/plugin/SyncPluginManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.478534 plextraktsync-0.30.1/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktUserList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktUserListCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/WatchProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.482534 plextraktsync-0.30.1/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/remove_empty_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.482534 plextraktsync-0.30.1/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-29 19:52:36.000000 plextraktsync-0.30.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_plex_id.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_rating.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.168800 plextraktsync-0.30.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    30188 2024-05-02 15:28:51.164800 plextraktsync-0.30.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.164800 plextraktsync-0.30.2/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30188 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26812 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.140799 plextraktsync-0.30.2/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.144799 plextraktsync-0.30.2/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.144799 plextraktsync-0.30.2/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/ServerConfigFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/coro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/logger/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/media/Media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/media/MediaFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/mixin/RichMarkup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/mixin/SetWindowTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plan/WalkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plan/WalkPlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plan/WalkPlanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plan/Walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.152799 plextraktsync-0.30.2/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderIMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderMbid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderTMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderTVDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexIdFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexPlaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexPlaylistCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexSectionPager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.152799 plextraktsync-0.30.2/plextraktsync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.152799 plextraktsync-0.30.2/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/TraktScrobbleWorker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.152799 plextraktsync-0.30.2/plextraktsync/rich/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/rich/RichHighlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/rich/RichProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.156799 plextraktsync-0.30.2/plextraktsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/AddCollectionPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/ClearCollectedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/LikedListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/Sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/SyncRatingsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/SyncWatchedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/TraktListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/WatchListPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/WatchProgressPlugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.156799 plextraktsync-0.30.2/plextraktsync/sync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/plugin/SyncPluginInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/plugin/SyncPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.160800 plextraktsync-0.30.2/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktUserList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktUserListCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/WatchProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.160800 plextraktsync-0.30.2/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/remove_empty_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.164800 plextraktsync-0.30.2/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-02 15:28:47.000000 plextraktsync-0.30.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 15:28:51.168800 plextraktsync-0.30.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.164800 plextraktsync-0.30.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_plex_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_rating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_walker.py
```

### Comparing `plextraktsync-0.30.1/LICENSE` & `plextraktsync-0.30.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/PKG-INFO` & `plextraktsync-0.30.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.1
+Version: 0.30.2
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,19 +14,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: apluggy==0.9.4; python_version >= "3.8"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: cattrs==23.2.3; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
+Requires-Dist: decorator==5.1.1; python_version >= "3.5"
 Requires-Dist: deprecated==1.2.14; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: exceptiongroup==1.2.1; python_version >= "3.7"
 Requires-Dist: humanize==4.9.0; python_version >= "3.8"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
@@ -44,15 +46,16 @@
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
 Requires-Dist: requests-oauthlib==2.0.0; python_version >= "3.4"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
 Requires-Dist: tqdm==4.66.2; python_version >= "3.7"
-Requires-Dist: typing-extensions==4.11.0; python_version < "3.11"
+Requires-Dist: types-decorator==5.1.8.20240310; python_version >= "3.8"
+Requires-Dist: typing-extensions==4.11.0; python_version < "3.9"
 Requires-Dist: url-normalize==1.4.3; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: websocket-client==1.8.0; python_version >= "3.8"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.5" and python_version >= "3.6"
 
 # Plex-Trakt-Sync
```

### Comparing `plextraktsync-0.30.1/PlexTraktSync.egg-info/PKG-INFO` & `plextraktsync-0.30.2/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.1
+Version: 0.30.2
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,19 +14,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: apluggy==0.9.4; python_version >= "3.8"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: cattrs==23.2.3; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
+Requires-Dist: decorator==5.1.1; python_version >= "3.5"
 Requires-Dist: deprecated==1.2.14; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: exceptiongroup==1.2.1; python_version >= "3.7"
 Requires-Dist: humanize==4.9.0; python_version >= "3.8"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
@@ -44,15 +46,16 @@
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
 Requires-Dist: requests-oauthlib==2.0.0; python_version >= "3.4"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
 Requires-Dist: tqdm==4.66.2; python_version >= "3.7"
-Requires-Dist: typing-extensions==4.11.0; python_version < "3.11"
+Requires-Dist: types-decorator==5.1.8.20240310; python_version >= "3.8"
+Requires-Dist: typing-extensions==4.11.0; python_version < "3.9"
 Requires-Dist: url-normalize==1.4.3; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: websocket-client==1.8.0; python_version >= "3.8"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.5" and python_version >= "3.6"
 
 # Plex-Trakt-Sync
```

### Comparing `plextraktsync-0.30.1/PlexTraktSync.egg-info/SOURCES.txt` & `plextraktsync-0.30.2/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 plextraktsync/config/ConfigMergeMixin.py
 plextraktsync/config/HttpCacheConfig.py
 plextraktsync/config/PlexServerConfig.py
 plextraktsync/config/RunConfig.py
 plextraktsync/config/ServerConfigFactory.py
 plextraktsync/config/SyncConfig.py
 plextraktsync/config/__init__.py
+plextraktsync/decorators/coro.py
 plextraktsync/decorators/flatten.py
 plextraktsync/decorators/measure_time.py
 plextraktsync/decorators/memoize.py
 plextraktsync/decorators/nocache.py
 plextraktsync/decorators/rate_limit.py
 plextraktsync/decorators/retry.py
 plextraktsync/decorators/time_limit.py
```

### Comparing `plextraktsync-0.30.1/PlexTraktSync.egg-info/requires.txt` & `plextraktsync-0.30.2/PlexTraktSync.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 wcwidth==0.2.13
 
 [:python_full_version >= "3.7.0"]
 charset-normalizer==3.3.2
 prompt-toolkit==3.0.43
 rich==13.7.1
 
-[:python_version < "3.11"]
+[:python_version < "3.9"]
 typing-extensions==4.11.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 deprecated==1.2.14
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"]
 six==1.16.0
@@ -20,14 +20,15 @@
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"]
 url-normalize==1.4.3
 
 [:python_version >= "3.4"]
 requests-oauthlib==2.0.0
 
 [:python_version >= "3.5"]
+decorator==5.1.1
 idna==3.7
 
 [:python_version >= "3.5" and python_version >= "3.6"]
 wrapt==1.16.0
 
 [:python_version >= "3.6"]
 certifi==2024.2.2
@@ -48,15 +49,17 @@
 pfzy==0.3.4
 
 [:python_version >= "3.7" and python_version >= "3.8"]
 cattrs==23.2.3
 markdown-it-py==3.0.0
 
 [:python_version >= "3.8"]
+apluggy==0.9.4
 humanize==4.9.0
 platformdirs==4.2.1
 plexapi==4.15.12
 pluggy==1.5.0
 python-dotenv==1.0.1
 requests-cache==1.2.0
+types-decorator==5.1.8.20240310
 urllib3==2.2.1
 websocket-client==1.8.0
```

### Comparing `plextraktsync-0.30.1/README.md` & `plextraktsync-0.30.2/README.md`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/cli.py` & `plextraktsync-0.30.2/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/bug_report.py` & `plextraktsync-0.30.2/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/cache.py` & `plextraktsync-0.30.2/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/clear_collections.py` & `plextraktsync-0.30.2/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/config.py` & `plextraktsync-0.30.2/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/download.py` & `plextraktsync-0.30.2/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/imdb_import.py` & `plextraktsync-0.30.2/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/info.py` & `plextraktsync-0.30.2/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/inspect.py` & `plextraktsync-0.30.2/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/login.py` & `plextraktsync-0.30.2/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/plex_login.py` & `plextraktsync-0.30.2/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/self_update.py` & `plextraktsync-0.30.2/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/sync.py` & `plextraktsync-0.30.2/plextraktsync/commands/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from plextraktsync.commands.login import ensure_login
+from plextraktsync.decorators.coro import coro
 from plextraktsync.decorators.measure_time import measure_time
 from plextraktsync.factory import factory, logging
 
 logger = logging.getLogger(__name__)
 
 
-def sync(
+@coro
+async def sync(
     sync_option: str,
     library: str,
     show: str,
     movie: str,
     ids: list[str],
     server: str,
     batch_delay: int,
@@ -63,8 +65,8 @@
 
     with measure_time("Completed full sync"):
         runner = factory.sync
         if runner.config.need_library_walk:
             w.print_plan(print=logger.info)
         if dry_run:
             logger.info("Enabled dry-run mode: not making actual changes")
-        runner.sync(walker=w, dry_run=config.dry_run)
+        await runner.sync(walker=w, dry_run=config.dry_run)
```

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/trakt_login.py` & `plextraktsync-0.30.2/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/unmatched.py` & `plextraktsync-0.30.2/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/watch.py` & `plextraktsync-0.30.2/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/commands/watched_shows.py` & `plextraktsync-0.30.2/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/config/Config.py` & `plextraktsync-0.30.2/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/config/ConfigLoader.py` & `plextraktsync-0.30.2/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/config/HttpCacheConfig.py` & `plextraktsync-0.30.2/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/config/PlexServerConfig.py` & `plextraktsync-0.30.2/plextraktsync/config/PlexServerConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/config/ServerConfigFactory.py` & `plextraktsync-0.30.2/plextraktsync/config/ServerConfigFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/config/SyncConfig.py` & `plextraktsync-0.30.2/plextraktsync/config/SyncConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,21 @@
         return self.update_plex_wl or self.update_trakt_wl
 
     @cached_property
     def sync_liked_lists(self):
         return self.trakt_to_plex["liked_lists"]
 
     @cached_property
+    def sync_watchlists(self):
+        return any([
+            self.plex_to_trakt["watchlist"],
+            self.trakt_to_plex["watchlist"],
+        ])
+
+    @cached_property
     def need_library_walk(self):
         return any([
             self.update_plex_wl_as_pl,
             self.sync_watched_status,
             self.sync_ratings,
             self.plex_to_trakt["collection"],
             self.sync_liked_lists,
```

### Comparing `plextraktsync-0.30.1/plextraktsync/config.default.yml` & `plextraktsync-0.30.2/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/decorators/measure_time.py` & `plextraktsync-0.30.2/plextraktsync/decorators/measure_time.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/decorators/rate_limit.py` & `plextraktsync-0.30.2/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/decorators/retry.py` & `plextraktsync-0.30.2/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/logger/filter.py` & `plextraktsync-0.30.2/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/logger/init.py` & `plextraktsync-0.30.2/plextraktsync/logger/init.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/media/Media.py` & `plextraktsync-0.30.2/plextraktsync/media/Media.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/media/MediaFactory.py` & `plextraktsync-0.30.2/plextraktsync/media/MediaFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/mixin/ChangeNotifier.py` & `plextraktsync-0.30.2/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plan/WalkConfig.py` & `plextraktsync-0.30.2/plextraktsync/plan/WalkConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plan/WalkPlanner.py` & `plextraktsync-0.30.2/plextraktsync/plan/WalkPlanner.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plan/Walker.py` & `plextraktsync-0.30.2/plextraktsync/plan/Walker.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,22 +100,28 @@
         yield from shows
 
     def find_episodes(self):
         if self.plan.episodes:
             yield from self.get_plex_episodes(self.plan.episodes)
 
         # Preload plex shows
-        plex_shows = {}
-
+        plex_shows: dict[int, PlexLibraryItem] = {}
         self.logger.info("Preload shows data")
         for show in self.get_plex_shows():
             plex_shows[show.key] = show
         self.logger.info(f"Preloaded shows data ({len(plex_shows)} shows)")
 
-        show_cache = {}
+        # Preload matches for shows
+        show_cache: dict[int, Media] = {}
+        self.logger.info("Preload shows matches")
+        it = self.progressbar(plex_shows.items(), desc="Processing show matches")
+        for show_id, ps in it:
+            show_cache[show_id] = self.mf.resolve_any(ps)
+        self.logger.info(f"Preloaded shows matches ({len(show_cache)} shows)")
+
         for ep in self.episodes_from_sections(self.plan.show_sections):
             show_id = ep.show_id
             ep.show = plex_shows[show_id]
             show = show_cache[show_id] if show_id in show_cache else None
             m = self.mf.resolve_any(ep, show)
             if not m:
                 continue
```

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexApi.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexAudioCodec.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexGuid.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProvider.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProvider.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderMbid.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderMbid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderTMDB.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderTMDB.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexId.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexId.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexIdFactory.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexIdFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexLibraryItem.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexLibrarySection.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexPlaylist.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexPlaylist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexRatings.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexSectionPager.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexSectionPager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexServerConnection.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/PlexWatchList.py` & `plextraktsync-0.30.2/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/plex/SessionCollection.py` & `plextraktsync-0.30.2/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/pytrakt_extensions.py` & `plextraktsync-0.30.2/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/queue/BackgroundTask.py` & `plextraktsync-0.30.2/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/queue/Queue.py` & `plextraktsync-0.30.2/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/queue/TraktBatchWorker.py` & `plextraktsync-0.30.2/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/queue/TraktMarkWatchedWorker.py` & `plextraktsync-0.30.2/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/queue/TraktScrobbleWorker.py` & `plextraktsync-0.30.2/plextraktsync/queue/TraktScrobbleWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/rich/RichHighlighter.py` & `plextraktsync-0.30.2/plextraktsync/rich/RichHighlighter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/rich/RichProgressBar.py` & `plextraktsync-0.30.2/plextraktsync/rich/RichProgressBar.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,27 +6,49 @@
         self.options = options or {}
         self.desc = desc
         if total is None:
             total = len(iterable)
         self.total = total
         self.i = 0
 
-        if hasattr(iterable, "__next__"):
-            self.iterable_next = iterable.__next__
-        else:
-            self.iterable_next = iter(iterable).__next__
+        self.iterable_awaitable = False
+        if iterable is not None:
+            if hasattr(iterable, "__anext__"):
+                self.iterable_next = iterable.__anext__
+                self.iterable_awaitable = True
+            elif hasattr(iterable, "__next__"):
+                self.iterable_next = iterable.__next__
+            else:
+                self.iterable_next = iter(iterable).__next__
 
     def __iter__(self):
+        if self.iterable_awaitable:
+            raise RuntimeError("Iterable must be awaited")
+
+        return self
+
+    def __aiter__(self):
         return self
 
     def __next__(self):
         res = self.iterable_next()
         self.update()
         return res
 
+    async def __anext__(self):
+        try:
+            if self.iterable_awaitable:
+                res = await self.iterable_next()
+            else:
+                res = self.iterable_next()
+            self.update()
+            return res
+        except StopIteration:
+            raise StopAsyncIteration
+
     def __enter__(self):
         self.progress.__enter__()
         return self
 
     def __exit__(self, *exc):
         self.progress.__exit__(*exc)
```

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/AddCollectionPlugin.py` & `plextraktsync-0.30.2/plextraktsync/sync/AddCollectionPlugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,19 +17,19 @@
         return config.plex_to_trakt["collection"]
 
     @classmethod
     def factory(cls, sync):
         return cls()
 
     @hookimpl
-    def walk_movie(self, movie: Media, dry_run: bool):
+    async def walk_movie(self, movie: Media, dry_run: bool):
         self.sync_collection(movie, dry_run=dry_run)
 
     @hookimpl
-    def walk_episode(self, episode: Media, dry_run: bool):
+    async def walk_episode(self, episode: Media, dry_run: bool):
         self.sync_collection(episode, dry_run=dry_run)
 
     def sync_collection(self, m: Media, dry_run: bool):
         if m.is_collected:
             return
 
         self.logger.info(f"Adding to Trakt collection: {m.title_link}", extra={"markup": True})
```

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/ClearCollectedPlugin.py` & `plextraktsync-0.30.2/plextraktsync/sync/ClearCollectedPlugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,24 +34,24 @@
         if not is_partial:
             return
 
         self.logger.warning("Disabling Clear Collected: Running partial library sync")
         pm.unregister(self)
 
     @hookimpl
-    def fini(self, dry_run: bool):
+    async def fini(self, dry_run: bool):
         self.clear_collected(self.trakt.movie_collection, self.movie_trakt_ids, dry_run=dry_run)
         self.clear_collected(self.trakt.episodes_collection, self.episode_trakt_ids, dry_run=dry_run)
 
     @hookimpl
-    def walk_movie(self, movie: Media):
+    async def walk_movie(self, movie: Media):
         self.movie_trakt_ids.add(movie.trakt_id)
 
     @hookimpl
-    def walk_episode(self, episode: Media):
+    async def walk_episode(self, episode: Media):
         self.episode_trakt_ids.add(episode.trakt_id)
 
     def clear_collected(self, existing_items: Iterable[TraktMedia], keep_ids: set[int], dry_run):
         from plextraktsync.trakt.trakt_set import trakt_set
 
         existing_ids = trakt_set(existing_items)
         delete_ids = existing_ids - keep_ids
```

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/LikedListsPlugin.py` & `plextraktsync-0.30.2/plextraktsync/sync/LikedListsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/Sync.py` & `plextraktsync-0.30.2/plextraktsync/sync/Sync.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,25 +22,25 @@
         self.trakt = trakt
         self.walker = None
 
     @cached_property
     def trakt_lists(self):
         return TraktUserListCollection()
 
-    def sync(self, walker: Walker, dry_run=False):
+    async def sync(self, walker: Walker, dry_run=False):
         self.walker = walker
         is_partial = walker.is_partial
 
         from plextraktsync.sync.plugin import SyncPluginManager
         pm = SyncPluginManager()
         pm.register_plugins(self)
 
         pm.hook.init(sync=self, pm=pm, is_partial=is_partial, dry_run=dry_run)
 
         if self.config.need_library_walk:
             for movie in walker.find_movies():
-                pm.hook.walk_movie(movie=movie, dry_run=dry_run)
+                await pm.ahook.walk_movie(movie=movie, dry_run=dry_run)
 
             for episode in walker.find_episodes():
-                pm.hook.walk_episode(episode=episode, dry_run=dry_run)
+                await pm.ahook.walk_episode(episode=episode, dry_run=dry_run)
 
-        pm.hook.fini(walker=walker, dry_run=dry_run)
+        await pm.ahook.fini(walker=walker, dry_run=dry_run)
```

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/SyncRatingsPlugin.py` & `plextraktsync-0.30.2/plextraktsync/sync/SyncRatingsPlugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,24 @@
         return cls(config=sync.config)
 
     @hookimpl
     def init(self):
         self.shows = set()
 
     @hookimpl
-    def fini(self, walker: Walker, dry_run: bool):
+    async def fini(self, walker: Walker, dry_run: bool):
         for show in walker.walk_shows(self.shows, title="Syncing show ratings"):
             self.sync_ratings(show, dry_run=dry_run)
 
     @hookimpl
-    def walk_movie(self, movie: Media, dry_run: bool):
+    async def walk_movie(self, movie: Media, dry_run: bool):
         self.sync_ratings(movie, dry_run=dry_run)
 
     @hookimpl
-    def walk_episode(self, episode: Media, dry_run: bool):
+    async def walk_episode(self, episode: Media, dry_run: bool):
         self.sync_ratings(episode, dry_run=dry_run)
 
         if episode.show:
             self.shows.add(episode.show)
 
     def sync_ratings(self, m: Media, dry_run: bool):
         if m.plex_rating == m.trakt_rating:
```

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/SyncWatchedPlugin.py` & `plextraktsync-0.30.2/plextraktsync/sync/SyncWatchedPlugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,19 @@
         return config.sync_watched_status
 
     @classmethod
     def factory(cls, sync: Sync):
         return cls(config=sync.config)
 
     @hookimpl
-    def walk_movie(self, movie: Media, dry_run: bool):
+    async def walk_movie(self, movie: Media, dry_run: bool):
         self.sync_watched(movie, dry_run=dry_run)
 
     @hookimpl
-    def walk_episode(self, episode: Media, dry_run: bool):
+    async def walk_episode(self, episode: Media, dry_run: bool):
         self.sync_watched(episode, dry_run=dry_run)
 
     def sync_watched(self, m: Media, dry_run: bool):
         if m.watched_on_plex is m.watched_on_trakt:
             return
 
         if m.watched_on_plex:
```

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/WatchListPlugin.py` & `plextraktsync-0.30.2/plextraktsync/sync/WatchListPlugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,15 @@
     def __init__(self, config: SyncConfig, plex: PlexApi, trakt: TraktApi):
         self.config = config
         self.plex = plex
         self.trakt = trakt
 
     @staticmethod
     def enabled(config: SyncConfig):
-        return any([
-            config.plex_to_trakt["watchlist"],
-            config.trakt_to_plex["watchlist"],
-        ])
+        return config.sync_watchlists
 
     @classmethod
     def factory(cls, sync: Sync):
         return cls(
             config=sync.config,
             plex=sync.plex,
             trakt=sync.trakt,
@@ -42,15 +39,15 @@
         if self.config.update_plex_wl_as_pl:
             if is_partial:
                 self.logger.warning("Running partial library sync. "
                                     "Watchlist as playlist won't update because it needs full library sync.")
             else:
                 sync.trakt_lists.add_watchlist(self.trakt.watchlist_movies)
 
-    def fini(self, walker: Walker, dry_run: bool):
+    async def fini(self, walker: Walker, dry_run: bool):
         if walker.config.walk_watchlist and self.sync_wl:
             with measure_time("Updated watchlist"):
                 self.sync_watchlist(walker, dry_run=dry_run)
 
         if self.config.update_plex_wl_as_pl or self.config.sync_liked_lists:
             if dry_run:
                 self.logger.warning("Running partial library sync. "
```

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/WatchProgressPlugin.py` & `plextraktsync-0.30.2/plextraktsync/sync/WatchProgressPlugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,19 +24,19 @@
         return config.sync_playback_status
 
     @classmethod
     def factory(cls, sync: Sync):
         return cls(sync.trakt)
 
     @hookimpl
-    def walk_movie(self, movie: Media, dry_run: bool):
+    async def walk_movie(self, movie: Media, dry_run: bool):
         self.sync_progress(movie, dry_run=dry_run)
 
     @hookimpl
-    def walk_episode(self, episode: Media, dry_run: bool):
+    async def walk_episode(self, episode: Media, dry_run: bool):
         self.sync_progress(episode, dry_run=dry_run)
 
     def sync_progress(self, m: Media, dry_run=False):
         p = self.trakt.watch_progress.match(m)
         if not p:
             return
         progress = m.plex.progress_millis(p.progress)
```

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/plugin/SyncPluginInterface.py` & `plextraktsync-0.30.2/plextraktsync/sync/plugin/SyncPluginInterface.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     """A hook specification namespace."""
 
     @hookspec
     def init(self, pm: SyncPluginManager, sync: Sync, is_partial: bool, dry_run: bool):
         """Hook called at sync process initialization"""
 
     @hookspec
-    def fini(self, walker: Walker, dry_run: bool):
+    async def fini(self, walker: Walker, dry_run: bool):
         """Hook called at sync process finalization"""
 
     @hookspec
-    def walk_movie(self, movie: Media, dry_run: bool):
+    async def walk_movie(self, movie: Media, dry_run: bool):
         """Hook called walk a movie media object"""
 
     @hookspec
-    def walk_episode(self, episode: Media, dry_run: bool):
+    async def walk_episode(self, episode: Media, dry_run: bool):
         """Hook called walk a episode media object"""
```

### Comparing `plextraktsync-0.30.1/plextraktsync/sync/plugin/SyncPluginManager.py` & `plextraktsync-0.30.2/plextraktsync/sync/plugin/SyncPluginManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING
 
-import pluggy
+import apluggy as pluggy
 
 from plextraktsync.decorators.measure_time import measure_time
 from plextraktsync.factory import logging
 
 if TYPE_CHECKING:
     from plextraktsync.sync.Sync import Sync
 
@@ -21,14 +21,18 @@
 
         pm = pluggy.PluginManager("PlexTraktSync")
         pm.add_hookspecs(SyncPluginInterface)
 
         return pm
 
     @cached_property
+    def ahook(self):
+        return self.pm.ahook
+
+    @cached_property
     def hook(self):
         return self.pm.hook
 
     @cached_property
     def unregister(self):
         return self.pm.unregister
```

### Comparing `plextraktsync-0.30.1/plextraktsync/trakt/ScrobblerCollection.py` & `plextraktsync-0.30.2/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/trakt/ScrobblerProxy.py` & `plextraktsync-0.30.2/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/trakt/TraktApi.py` & `plextraktsync-0.30.2/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/trakt/TraktLookup.py` & `plextraktsync-0.30.2/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/trakt/TraktRatingCollection.py` & `plextraktsync-0.30.2/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/trakt/TraktUserList.py` & `plextraktsync-0.30.2/plextraktsync/trakt/TraktUserList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/trakt/TraktWatchlist.py` & `plextraktsync-0.30.2/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/trakt/WatchProgress.py` & `plextraktsync-0.30.2/plextraktsync/trakt/WatchProgress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/util/Factory.py` & `plextraktsync-0.30.2/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/util/Path.py` & `plextraktsync-0.30.2/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/util/Rating.py` & `plextraktsync-0.30.2/plextraktsync/util/Rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/util/Timer.py` & `plextraktsync-0.30.2/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/util/Version.py` & `plextraktsync-0.30.2/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/util/local_url.py` & `plextraktsync-0.30.2/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/util/openurl.py` & `plextraktsync-0.30.2/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/util/packaging.py` & `plextraktsync-0.30.2/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/util/remove_empty_values.py` & `plextraktsync-0.30.2/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/watch/EventDispatcher.py` & `plextraktsync-0.30.2/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/watch/EventFactory.py` & `plextraktsync-0.30.2/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/watch/ProgressBar.py` & `plextraktsync-0.30.2/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/watch/WatchStateUpdater.py` & `plextraktsync-0.30.2/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/watch/WebSocketListener.py` & `plextraktsync-0.30.2/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/plextraktsync/watch/events.py` & `plextraktsync-0.30.2/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/requirements.txt` & `plextraktsync-0.30.2/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+apluggy==0.9.4; python_version >= '3.8'
 attrs==23.2.0; python_version >= '3.7'
 cattrs==23.2.3; python_version >= '3.7' and python_version >= '3.8'
 certifi==2024.2.2; python_version >= '3.6'
 charset-normalizer==3.3.2; python_full_version >= '3.7.0'
 click==8.1.7; python_version >= '3.7'
+decorator==5.1.1; python_version >= '3.5'
 deprecated==1.2.14; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 exceptiongroup==1.2.1; python_version >= '3.7'
 humanize==4.9.0; python_version >= '3.8'
 idna==3.7; python_version >= '3.5'
 inquirerpy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 markdown-it-py==3.0.0; python_version >= '3.7' and python_version >= '3.8'
 mdurl==0.1.2; python_version >= '3.7'
@@ -24,13 +26,14 @@
 pyyaml==6.0.1; python_version >= '3.6'
 requests==2.31.0; python_version >= '3.7'
 requests-cache==1.2.0; python_version >= '3.8'
 requests-oauthlib==2.0.0; python_version >= '3.4'
 rich==13.7.1; python_full_version >= '3.7.0'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3' and python_version >= '3.4'
 tqdm==4.66.2; python_version >= '3.7'
-typing-extensions==4.11.0; python_version < '3.11'
+types-decorator==5.1.8.20240310; python_version >= '3.8'
+typing-extensions==4.11.0; python_version < '3.9'
 url-normalize==1.4.3; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version >= '3.6'
 urllib3==2.2.1; python_version >= '3.8'
 wcwidth==0.2.13
 websocket-client==1.8.0; python_version >= '3.8'
 wrapt==1.16.0; python_version >= '3.5' and python_version >= '3.6'
```

### Comparing `plextraktsync-0.30.1/setup.cfg` & `plextraktsync-0.30.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_collection_metadata.py` & `plextraktsync-0.30.2/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_config.py` & `plextraktsync-0.30.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_events.py` & `plextraktsync-0.30.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_new_agent.py` & `plextraktsync-0.30.2/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_plex_id.py` & `plextraktsync-0.30.2/tests/test_plex_id.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_rating.py` & `plextraktsync-0.30.2/tests/test_rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_timer.py` & `plextraktsync-0.30.2/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_trakt_progress.py` & `plextraktsync-0.30.2/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_tv_lookup.py` & `plextraktsync-0.30.2/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.1/tests/test_walker.py` & `plextraktsync-0.30.2/tests/test_walker.py`

 * *Files identical despite different names*

