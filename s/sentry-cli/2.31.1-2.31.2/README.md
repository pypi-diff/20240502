# Comparing `tmp/sentry_cli-2.31.1.tar.gz` & `tmp/sentry_cli-2.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.31.1.tar", last modified: Tue Apr 30 15:03:35 2024, max compression
+gzip compressed data, was "sentry_cli-2.31.2.tar", last modified: Thu May  2 14:17:09 2024, max compression
```

## Comparing `sentry_cli-2.31.1.tar` & `sentry_cli-2.31.2.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/
--rw-r--r--   0 runner    (1001) docker     (127)    92408 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-30 15:03:35.000000 sentry_cli-2.31.1/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-30 15:03:35.000000 sentry_cli-2.31.1/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:03:35.000000 sentry_cli-2.31.1/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:03:35.000000 sentry_cli-2.31.1/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-30 15:03:35.949649 sentry_cli-2.31.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.929649 sentry_cli-2.31.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/connection_manager.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/encoding.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/api/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/errors/api_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/errors/sentry_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)    83574 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/pagination.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.941649 sentry_cli-2.31.1/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.941649 sentry_cli-2.31.1/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.941649 sentry_cli-2.31.1/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (127)    25588 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/args.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/src/utils/auth_token/
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/auth_token_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/org_auth_token.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/test.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/user_auth_token.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (127)    72264 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (127)    47198 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (127)    36324 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    92408 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-02 14:17:09.000000 sentry_cli-2.31.2/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-02 14:17:09.000000 sentry_cli-2.31.2/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:17:09.000000 sentry_cli-2.31.2/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:17:09.000000 sentry_cli-2.31.2/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.246627 sentry_cli-2.31.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.246627 sentry_cli-2.31.2/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/connection_manager.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/encoding.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.246627 sentry_cli-2.31.2/src/api/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/errors/api_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/errors/sentry_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    83793 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/pagination.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.246627 sentry_cli-2.31.2/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    25592 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.258627 sentry_cli-2.31.2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/args.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/src/utils/auth_token/
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/auth_token_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/org_auth_token.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/test.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/user_auth_token.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    72264 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    47198 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    36324 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.31.1/Cargo.lock` & `sentry_cli-2.31.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2428,15 +2428,15 @@
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.31.1"
+version = "2.31.2"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
```

### Comparing `sentry_cli-2.31.1/Cargo.toml` & `sentry_cli-2.31.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.31.1"
+version = "2.31.2"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
```

### Comparing `sentry_cli-2.31.1/LICENSE` & `sentry_cli-2.31.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/PKG-INFO` & `sentry_cli-2.31.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.31.1
+Version: 2.31.2
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.1 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.2 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.31.1/README.md` & `sentry_cli-2.31.2/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/build.rs` & `sentry_cli-2.31.2/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.31.2/sentry_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.31.1
+Version: 2.31.2
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.1 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.2 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.31.1/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.31.2/sentry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/setup.cfg` & `sentry_cli-2.31.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/setup.py` & `sentry_cli-2.31.2/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/api/connection_manager.rs` & `sentry_cli-2.31.2/src/api/connection_manager.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/api/encoding.rs` & `sentry_cli-2.31.2/src/api/encoding.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/api/errors/api_error.rs` & `sentry_cli-2.31.2/src/api/errors/api_error.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/api/errors/sentry_error.rs` & `sentry_cli-2.31.2/src/api/errors/sentry_error.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/api/mod.rs` & `sentry_cli-2.31.2/src/api/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 use crate::utils::file_upload::UploadContext;
 use crate::utils::http::{self, is_absolute_url};
 use crate::utils::progress::ProgressBar;
 use crate::utils::retry::{get_default_backoff, DurationAsMilliseconds};
 use crate::utils::sourcemaps::get_sourcemap_reference_from_headers;
 use crate::utils::ui::{capitalize_string, make_byte_progress_bar};
 
+use self::pagination::Pagination;
 use connection_manager::CurlConnectionManager;
 use encoding::{PathArg, QueryArg};
 use errors::{ApiError, ApiErrorKind, ApiResult, SentryError};
 
 lazy_static! {
     static ref API: Mutex<Option<Arc<Api>>> = Mutex::new(None);
 }
@@ -529,17 +530,17 @@
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ReleaseNotFound.into());
                 } else {
                     break;
                 }
             }
 
-            let next = resp.next_pagination_cursor();
+            let pagination = resp.pagination();
             rv.extend(resp.convert::<Vec<Artifact>>()?);
-            if let Some(next) = next {
+            if let Some(next) = pagination.into_next_cursor() {
                 cursor = next;
             } else {
                 break;
             }
         }
         Ok(rv)
     }
@@ -1130,17 +1131,17 @@
             if resp.status() == 404 || (resp.status() == 400 && !cursor.is_empty()) {
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ResourceNotFound.into());
                 } else {
                     break;
                 }
             }
-            let next = resp.next_pagination_cursor();
+            let pagination = resp.pagination();
             rv.extend(resp.convert::<Vec<Organization>>()?);
-            if let Some(next) = next {
+            if let Some(next) = pagination.into_next_cursor() {
                 cursor = next;
             } else {
                 break;
             }
         }
         Ok(rv)
     }
@@ -1174,17 +1175,17 @@
             if resp.status() == 404 || (resp.status() == 400 && !cursor.is_empty()) {
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ResourceNotFound.into());
                 } else {
                     break;
                 }
             }
-            let next = resp.next_pagination_cursor();
+            let pagination = resp.pagination();
             rv.extend(resp.convert::<Vec<Monitor>>()?);
-            if let Some(next) = next {
+            if let Some(next) = pagination.into_next_cursor() {
                 cursor = next;
             } else {
                 break;
             }
         }
         Ok(rv)
     }
@@ -1202,17 +1203,17 @@
             if resp.status() == 404 || (resp.status() == 400 && !cursor.is_empty()) {
                 if rv.is_empty() {
                     return Err(ApiErrorKind::OrganizationNotFound.into());
                 } else {
                     break;
                 }
             }
-            let next = resp.next_pagination_cursor();
+            let pagination = resp.pagination();
             rv.extend(resp.convert::<Vec<Project>>()?);
-            if let Some(next) = next {
+            if let Some(next) = pagination.into_next_cursor() {
                 cursor = next;
             } else {
                 break;
             }
         }
         Ok(rv)
     }
@@ -1242,22 +1243,22 @@
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ProjectNotFound.into());
                 } else {
                     break;
                 }
             }
 
-            let next = resp.next_pagination_cursor();
+            let pagination = resp.pagination();
             rv.extend(resp.convert::<Vec<ProcessedEvent>>()?);
 
             if requests_no == max_pages {
                 break;
             }
 
-            if let Some(next) = next {
+            if let Some(next) = pagination.into_next_cursor() {
                 cursor = next;
             } else {
                 break;
             }
         }
 
         Ok(rv)
@@ -1268,15 +1269,15 @@
         &self,
         org: &str,
         project: &str,
         max_pages: usize,
         query: Option<String>,
     ) -> ApiResult<Vec<Issue>> {
         let mut rv = vec![];
-        let mut cursor = String::from("");
+        let mut cursor = "".to_string();
         let mut requests_no = 0;
 
         let url = if let Some(query) = query {
             format!(
                 "/projects/{}/{}/issues/?query={}&",
                 PathArg(org),
                 PathArg(project),
@@ -1295,22 +1296,22 @@
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ProjectNotFound.into());
                 } else {
                     break;
                 }
             }
 
-            let next = resp.next_pagination_cursor();
+            let pagination = resp.pagination();
             rv.extend(resp.convert::<Vec<Issue>>()?);
 
             if requests_no == max_pages {
                 break;
             }
 
-            if let Some(next) = next {
+            if let Some(next) = pagination.into_next_cursor() {
                 cursor = next;
             } else {
                 break;
             }
         }
 
         Ok(rv)
@@ -1326,20 +1327,21 @@
                 PathArg(org),
                 QueryArg(&cursor)
             );
             let resp = self.request(Method::Get, &path)?.send()?;
             if resp.status() == 404 {
                 break;
             } else {
-                if let Some(next) = resp.next_pagination_cursor() {
+                let pagination = resp.pagination();
+                rv.extend(resp.convert::<Vec<Repo>>()?);
+                if let Some(next) = pagination.into_next_cursor() {
                     cursor = next;
                 } else {
                     break;
                 }
-                rv.extend(resp.convert::<Vec<Repo>>()?);
             }
         }
         Ok(rv)
     }
 
     /// Looks up an event, which was already processed by Sentry and returns it.
     /// If it does not exist `None` will be returned.
@@ -1964,18 +1966,19 @@
             if header_key.eq_ignore_ascii_case(key) {
                 return Some(header_value);
             }
         }
         None
     }
 
-    fn next_pagination_cursor(&self) -> Option<String> {
+    /// Returns the pagination info
+    pub fn pagination(&self) -> Pagination {
         self.get_header("link")
-            .and_then(pagination::next_cursor)
-            .map(String::from)
+            .and_then(|x| x.parse().ok())
+            .unwrap_or_default()
     }
 
     /// Returns true if the response is JSON.
     pub fn is_json(&self) -> bool {
         self.get_header("content-type")
             .and_then(|x| x.split(';').next())
             .unwrap_or("")
```

### Comparing `sentry_cli-2.31.1/src/bashsupport.sh` & `sentry_cli-2.31.2/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/bash_hook.rs` & `sentry_cli-2.31.2/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.31.2/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.31.2/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/debug_files/check.rs` & `sentry_cli-2.31.2/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/debug_files/find.rs` & `sentry_cli-2.31.2/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/debug_files/mod.rs` & `sentry_cli-2.31.2/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.31.2/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/debug_files/upload.rs` & `sentry_cli-2.31.2/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/deploys/list.rs` & `sentry_cli-2.31.2/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/deploys/mod.rs` & `sentry_cli-2.31.2/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/deploys/new.rs` & `sentry_cli-2.31.2/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/events/list.rs` & `sentry_cli-2.31.2/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/events/mod.rs` & `sentry_cli-2.31.2/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/files/delete.rs` & `sentry_cli-2.31.2/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/files/list.rs` & `sentry_cli-2.31.2/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/files/mod.rs` & `sentry_cli-2.31.2/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/files/upload.rs` & `sentry_cli-2.31.2/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/info.rs` & `sentry_cli-2.31.2/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/issues/list.rs` & `sentry_cli-2.31.2/src/commands/issues/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/issues/mod.rs` & `sentry_cli-2.31.2/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/issues/mute.rs` & `sentry_cli-2.31.2/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/issues/resolve.rs` & `sentry_cli-2.31.2/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/issues/unresolve.rs` & `sentry_cli-2.31.2/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/login.rs` & `sentry_cli-2.31.2/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/mod.rs` & `sentry_cli-2.31.2/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/monitors/list.rs` & `sentry_cli-2.31.2/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/monitors/mod.rs` & `sentry_cli-2.31.2/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/monitors/run.rs` & `sentry_cli-2.31.2/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/organizations/list.rs` & `sentry_cli-2.31.2/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/organizations/mod.rs` & `sentry_cli-2.31.2/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/projects/list.rs` & `sentry_cli-2.31.2/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/projects/mod.rs` & `sentry_cli-2.31.2/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/react_native/appcenter.rs` & `sentry_cli-2.31.2/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/react_native/gradle.rs` & `sentry_cli-2.31.2/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/react_native/mod.rs` & `sentry_cli-2.31.2/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/react_native/xcode.rs` & `sentry_cli-2.31.2/src/commands/react_native/xcode.rs`

 * *Files 2% similar despite different names*

```diff
@@ -369,18 +369,23 @@
                 (Err(_), Err(_)) => {
                     // Neither environment variable is present, attempt to parse Info.plist
                     info!("Parsing Info.plist");
                     match InfoPlist::discover_from_env() {
                         Ok(Some(plist)) => {
                             // Successfully discovered and parsed Info.plist
                             let dist_string = plist.build().to_string();
-                            let release_string = format!("{}@{}+{}", plist.bundle_id(), plist.version(), dist_string);
+                            let release_string = format!(
+                                "{}@{}+{}",
+                                plist.bundle_id(),
+                                plist.version(),
+                                dist_string
+                            );
                             info!("Parse result from Info.plist: {:?}", &plist);
                             (Some(dist_string), Some(release_string))
-                        },
+                        }
                         _ => {
                             bail!("Info.plist was not found or an parsing error occurred");
                         }
                     }
                 }
                 // At least one environment variable is present, use the values from the environment
                 _ => (dist_from_env.ok(), release_from_env.ok()),
@@ -552,16 +557,16 @@
                     hermes_sourcemap_path.as_path().display(),
                 );
             }
 
             if let (Ok(packager_sourcemap), Ok(mut hermes_sourcemap)) =
                 (packager_sourcemap_result, hermes_sourcemap_result)
             {
-                if hermes_sourcemap.get("debugId").is_none()
-                    && hermes_sourcemap.get("debug_id").is_none()
+                if !hermes_sourcemap.contains_key("debugId")
+                    && !hermes_sourcemap.contains_key("debug_id")
                 {
                     if let Some(debug_id) = packager_sourcemap
                         .get("debugId")
                         .or_else(|| packager_sourcemap.get("debug_id"))
                     {
                         hermes_sourcemap.insert("debugId".to_string(), debug_id.clone());
                         hermes_sourcemap.insert("debug_id".to_string(), debug_id.clone());
```

### Comparing `sentry_cli-2.31.1/src/commands/releases/archive.rs` & `sentry_cli-2.31.2/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/releases/delete.rs` & `sentry_cli-2.31.2/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/releases/finalize.rs` & `sentry_cli-2.31.2/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/releases/info.rs` & `sentry_cli-2.31.2/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/releases/list.rs` & `sentry_cli-2.31.2/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/releases/mod.rs` & `sentry_cli-2.31.2/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/releases/new.rs` & `sentry_cli-2.31.2/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/releases/restore.rs` & `sentry_cli-2.31.2/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/releases/set_commits.rs` & `sentry_cli-2.31.2/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/repos/list.rs` & `sentry_cli-2.31.2/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/repos/mod.rs` & `sentry_cli-2.31.2/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/send_envelope.rs` & `sentry_cli-2.31.2/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/send_event.rs` & `sentry_cli-2.31.2/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.31.2/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.31.2/src/commands/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.31.2/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.31.2/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.31.2/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/uninstall.rs` & `sentry_cli-2.31.2/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/update.rs` & `sentry_cli-2.31.2/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/commands/upload_proguard.rs` & `sentry_cli-2.31.2/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/config.rs` & `sentry_cli-2.31.2/src/config.rs`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
             .map(|td| td.url.as_str())
             .unwrap_or_default();
 
         if !token_url.is_empty() && url != token_url {
             bail!("Two different url values supplied: `{token_url}` (from token), `{url}`.");
         }
 
-        self.cached_base_url = url.to_owned();
+        url.clone_into(&mut self.cached_base_url);
         self.ini
             .set_to(Some("defaults"), "url".into(), self.cached_base_url.clone());
         Ok(())
     }
 
     /// Sets headers that should be attached to all requests
     pub fn set_headers(&mut self, headers: Vec<String>) {
```

### Comparing `sentry_cli-2.31.1/src/constants.rs` & `sentry_cli-2.31.2/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/android.rs` & `sentry_cli-2.31.2/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/appcenter.rs` & `sentry_cli-2.31.2/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/args.rs` & `sentry_cli-2.31.2/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/auth_token/auth_token_impl.rs` & `sentry_cli-2.31.2/src/utils/auth_token/auth_token_impl.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/auth_token/error.rs` & `sentry_cli-2.31.2/src/utils/auth_token/error.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/auth_token/org_auth_token.rs` & `sentry_cli-2.31.2/src/utils/auth_token/org_auth_token.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/auth_token/test.rs` & `sentry_cli-2.31.2/src/utils/auth_token/test.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/auth_token/user_auth_token.rs` & `sentry_cli-2.31.2/src/utils/auth_token/user_auth_token.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/chunks.rs` & `sentry_cli-2.31.2/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/cordova.rs` & `sentry_cli-2.31.2/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/dif.rs` & `sentry_cli-2.31.2/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/dif_upload.rs` & `sentry_cli-2.31.2/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/event.rs` & `sentry_cli-2.31.2/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/file_search.rs` & `sentry_cli-2.31.2/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/file_upload.rs` & `sentry_cli-2.31.2/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/formatting.rs` & `sentry_cli-2.31.2/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/fs.rs` & `sentry_cli-2.31.2/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/http.rs` & `sentry_cli-2.31.2/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/logging.rs` & `sentry_cli-2.31.2/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/progress.rs` & `sentry_cli-2.31.2/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/releases.rs` & `sentry_cli-2.31.2/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/retry.rs` & `sentry_cli-2.31.2/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.31.2/src/utils/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/sourcemaps.rs` & `sentry_cli-2.31.2/src/utils/sourcemaps.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/system.rs` & `sentry_cli-2.31.2/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/ui.rs` & `sentry_cli-2.31.2/src/utils/ui.rs`

 * *Files 11% similar despite different names*

```diff
@@ -41,22 +41,18 @@
     let mut bytes = s.as_bytes().to_vec();
     bytes.make_ascii_lowercase();
     bytes[0] = bytes[0].to_ascii_uppercase();
     String::from_utf8(bytes).unwrap()
 }
 
 /// Like ``io::copy`` but advances a progress bar set to bytes.
-pub fn copy_with_progress<R: ?Sized, W: ?Sized>(
-    pb: &ProgressBar,
-    reader: &mut R,
-    writer: &mut W,
-) -> io::Result<u64>
+pub fn copy_with_progress<R, W>(pb: &ProgressBar, reader: &mut R, writer: &mut W) -> io::Result<u64>
 where
-    R: Read,
-    W: Write,
+    R: Read + ?Sized,
+    W: Write + ?Sized,
 {
     let mut buf = [0; 16384];
     let mut written = 0;
     loop {
         let len = match reader.read(&mut buf) {
             Ok(0) => return Ok(written),
             Ok(len) => len,
```

### Comparing `sentry_cli-2.31.1/src/utils/update.rs` & `sentry_cli-2.31.2/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/vcs.rs` & `sentry_cli-2.31.2/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.1/src/utils/xcode.rs` & `sentry_cli-2.31.2/src/utils/xcode.rs`

 * *Files identical despite different names*

