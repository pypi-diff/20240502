# Comparing `tmp/stepup-1.0.0.tar.gz` & `tmp/stepup-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepup-1.0.0.tar", last modified: Thu Apr 25 17:28:17 2024, max compression
+gzip compressed data, was "stepup-1.1.0.tar", last modified: Thu May  2 09:17:23 2024, max compression
```

## Comparing `stepup-1.0.0.tar` & `stepup-1.1.0.tar`

### file list

```diff
@@ -1,921 +1,949 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.766806 stepup-1.0.0/
--rw-r--r--   0 toon      (1000) toon      (1000)      283 2024-02-08 02:51:50.000000 stepup-1.0.0/.editorconfig
--rw-r--r--   0 toon      (1000) toon      (1000)      181 2024-04-25 17:11:07.000000 stepup-1.0.0/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)     1022 2024-04-10 05:36:26.000000 stepup-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2024-04-24 20:23:46.000000 stepup-1.0.0/LICENSE
--rw-r--r--   0 toon      (1000) toon      (1000)     2279 2024-04-25 17:28:17.765806 stepup-1.0.0/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      915 2024-04-25 17:09:51.000000 stepup-1.0.0/README.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.647806 stepup-1.0.0/docs/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.648806 stepup-1.0.0/docs/advanced_topics/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.648806 stepup-1.0.0/docs/advanced_topics/amending_steps/
--rw-r--r--   0 toon      (1000) toon      (1000)       30 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/amending_steps/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      114 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/amending_steps/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      262 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/amending_steps/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1472 2024-04-25 17:26:14.000000 stepup-1.0.0/docs/advanced_topics/amending_steps/stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      465 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/amending_steps/step.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3178 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/amending_steps.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.649806 stepup-1.0.0/docs/advanced_topics/blocked_steps/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-04-23 18:06:07.000000 stepup-1.0.0/docs/advanced_topics/blocked_steps/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      114 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/blocked_steps/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      161 2024-04-23 18:14:36.000000 stepup-1.0.0/docs/advanced_topics/blocked_steps/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      947 2024-04-25 17:26:13.000000 stepup-1.0.0/docs/advanced_topics/blocked_steps/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2576 2024-04-23 18:15:40.000000 stepup-1.0.0/docs/advanced_topics/blocked_steps.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.650806 stepup-1.0.0/docs/advanced_topics/environment_variables/
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/environment_variables/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      124 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/environment_variables/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)       91 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/environment_variables/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      797 2024-04-25 17:26:13.000000 stepup-1.0.0/docs/advanced_topics/environment_variables/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1345 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/environment_variables.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.650806 stepup-1.0.0/docs/advanced_topics/here_and_root/
--rw-r--r--   0 toon      (1000) toon      (1000)       15 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/here_and_root/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      127 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/here_and_root/main.sh
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.650806 stepup-1.0.0/docs/advanced_topics/here_and_root/source/
--rwxr-xr-x   0 toon      (1000) toon      (1000)      134 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/here_and_root/source/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.650806 stepup-1.0.0/docs/advanced_topics/here_and_root/source/sub/
--rw-r--r--   0 toon      (1000) toon      (1000)       25 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/here_and_root/source/sub/example.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      164 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/here_and_root/source/sub/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      683 2024-04-25 17:27:50.000000 stepup-1.0.0/docs/advanced_topics/here_and_root/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3081 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/here_and_root.md
--rw-r--r--   0 toon      (1000) toon      (1000)      330 2024-04-23 13:53:11.000000 stepup-1.0.0/docs/advanced_topics/introduction.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.652806 stepup-1.0.0/docs/advanced_topics/optional_steps/
--rw-r--r--   0 toon      (1000) toon      (1000)       21 2024-04-23 17:11:07.000000 stepup-1.0.0/docs/advanced_topics/optional_steps/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      438 2024-04-23 17:05:47.000000 stepup-1.0.0/docs/advanced_topics/optional_steps/generate.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      114 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/optional_steps/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)      151 2024-04-23 09:13:57.000000 stepup-1.0.0/docs/advanced_topics/optional_steps/matplotlibrc
--rwxr-xr-x   0 toon      (1000) toon      (1000)      170 2024-04-23 17:43:58.000000 stepup-1.0.0/docs/advanced_topics/optional_steps/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      503 2024-04-23 18:16:31.000000 stepup-1.0.0/docs/advanced_topics/optional_steps/plot.py
--rw-r--r--   0 toon      (1000) toon      (1000)    62802 2024-04-25 17:27:50.000000 stepup-1.0.0/docs/advanced_topics/optional_steps/plot_logmap.png
--rw-r--r--   0 toon      (1000) toon      (1000)      597 2024-04-25 17:26:15.000000 stepup-1.0.0/docs/advanced_topics/optional_steps/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3621 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/optional_steps.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.652806 stepup-1.0.0/docs/advanced_topics/pools/
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2024-04-24 03:53:02.000000 stepup-1.0.0/docs/advanced_topics/pools/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      114 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/pools/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      195 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/pools/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1934 2024-04-25 17:26:13.000000 stepup-1.0.0/docs/advanced_topics/pools/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2563 2024-04-24 04:17:42.000000 stepup-1.0.0/docs/advanced_topics/pools.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.653806 stepup-1.0.0/docs/advanced_topics/static_deferred_glob/
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2024-04-23 13:56:08.000000 stepup-1.0.0/docs/advanced_topics/static_deferred_glob/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       13 2024-04-23 15:40:36.000000 stepup-1.0.0/docs/advanced_topics/static_deferred_glob/bar.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       13 2024-04-23 15:40:36.000000 stepup-1.0.0/docs/advanced_topics/static_deferred_glob/foo.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1310 2024-04-25 17:27:50.000000 stepup-1.0.0/docs/advanced_topics/static_deferred_glob/graph.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/static_deferred_glob/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      182 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/static_deferred_glob/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      802 2024-04-25 17:26:13.000000 stepup-1.0.0/docs/advanced_topics/static_deferred_glob/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1915 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/static_deferred_glob.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.654806 stepup-1.0.0/docs/advanced_topics/static_named_glob/
--rw-r--r--   0 toon      (1000) toon      (1000)       24 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/.gitignore
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.654806 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch1/
--rw-r--r--   0 toon      (1000) toon      (1000)       23 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch1/sec1_1_introduction.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       21 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch1/sec1_2_objectives.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch1/unused.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.655806 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch2/
--rw-r--r--   0 toon      (1000) toon      (1000)       34 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch2/sec2_1_mathematical_requisites.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       17 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch2/sec2_2_theory.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.655806 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch3/
--rw-r--r--   0 toon      (1000) toon      (1000)       23 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch3/sec3_1_applications.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       21 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch3/sec3_2_discussion.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.655806 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch4/
--rw-r--r--   0 toon      (1000) toon      (1000)       18 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/ch4/sec4_1_summary.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      647 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2063 2024-04-25 17:26:13.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1818 2024-04-25 15:31:00.000000 stepup-1.0.0/docs/advanced_topics/static_named_glob.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.656806 stepup-1.0.0/docs/advanced_topics/variable_substitution/
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/variable_substitution/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       45 2024-04-25 17:27:50.000000 stepup-1.0.0/docs/advanced_topics/variable_substitution/dst_foo.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      125 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/variable_substitution/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      186 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/variable_substitution/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)       16 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/variable_substitution/src_foo.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      393 2024-04-25 17:26:14.000000 stepup-1.0.0/docs/advanced_topics/variable_substitution/stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      177 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/variable_substitution/step.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2238 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/variable_substitution.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.657806 stepup-1.0.0/docs/advanced_topics/volatile_outputs/
--rw-r--r--   0 toon      (1000) toon      (1000)       17 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/volatile_outputs/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/volatile_outputs/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)       96 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/volatile_outputs/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      349 2024-04-25 17:26:14.000000 stepup-1.0.0/docs/advanced_topics/volatile_outputs/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1725 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/advanced_topics/volatile_outputs.md
--rw-r--r--   0 toon      (1000) toon      (1000)      294 2024-04-25 17:24:35.000000 stepup-1.0.0/docs/changelog.md
--rw-r--r--   0 toon      (1000) toon      (1000)       63 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/clean_stdout.sed
--rw-r--r--   0 toon      (1000) toon      (1000)      585 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/development.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.660806 stepup-1.0.0/docs/getting_started/
--rw-r--r--   0 toon      (1000) toon      (1000)     1176 2024-04-23 18:16:30.000000 stepup-1.0.0/docs/getting_started/automatic_cleaning.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.661806 stepup-1.0.0/docs/getting_started/copy_mkdir/
--rw-r--r--   0 toon      (1000) toon      (1000)       23 2024-04-23 05:29:14.000000 stepup-1.0.0/docs/getting_started/copy_mkdir/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/copy_mkdir/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      157 2024-04-23 13:42:30.000000 stepup-1.0.0/docs/getting_started/copy_mkdir/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      546 2024-04-23 13:42:57.000000 stepup-1.0.0/docs/getting_started/copy_mkdir/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1105 2024-04-23 05:34:02.000000 stepup-1.0.0/docs/getting_started/copy_mkdir.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.661806 stepup-1.0.0/docs/getting_started/dependencies/
--rw-r--r--   0 toon      (1000) toon      (1000)       18 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/getting_started/dependencies/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/dependencies/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      179 2024-04-22 02:59:32.000000 stepup-1.0.0/docs/getting_started/dependencies/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1004 2024-04-25 17:27:50.000000 stepup-1.0.0/docs/getting_started/dependencies/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1553 2024-04-23 05:35:12.000000 stepup-1.0.0/docs/getting_started/dependencies.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.662806 stepup-1.0.0/docs/getting_started/distributed_plans/
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2024-04-23 09:58:27.000000 stepup-1.0.0/docs/getting_started/distributed_plans/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/distributed_plans/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)       16 2024-04-23 10:04:33.000000 stepup-1.0.0/docs/getting_started/distributed_plans/part1.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      137 2024-04-23 10:03:24.000000 stepup-1.0.0/docs/getting_started/distributed_plans/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1453 2024-04-25 17:26:11.000000 stepup-1.0.0/docs/getting_started/distributed_plans/stdout.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.662806 stepup-1.0.0/docs/getting_started/distributed_plans/sub/
--rw-r--r--   0 toon      (1000) toon      (1000)       16 2024-04-23 10:04:33.000000 stepup-1.0.0/docs/getting_started/distributed_plans/sub/part2.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      140 2024-04-23 10:12:15.000000 stepup-1.0.0/docs/getting_started/distributed_plans/sub/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1453 2024-04-23 10:12:15.000000 stepup-1.0.0/docs/getting_started/distributed_plans.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.663806 stepup-1.0.0/docs/getting_started/first_step/
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/getting_started/first_step/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      177 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/first_step/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)       81 2024-04-22 01:47:01.000000 stepup-1.0.0/docs/getting_started/first_step/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      811 2024-04-25 17:26:11.000000 stepup-1.0.0/docs/getting_started/first_step/stdout1.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      345 2024-04-25 17:26:12.000000 stepup-1.0.0/docs/getting_started/first_step/stdout2.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2907 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/first_step.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2414 2024-04-23 05:39:58.000000 stepup-1.0.0/docs/getting_started/interactive_usage.md
--rw-r--r--   0 toon      (1000) toon      (1000)     5349 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/introduction.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.664806 stepup-1.0.0/docs/getting_started/no_rules/
--rw-r--r--   0 toon      (1000) toon      (1000)       30 2024-04-23 09:48:59.000000 stepup-1.0.0/docs/getting_started/no_rules/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       22 2024-04-23 09:48:48.000000 stepup-1.0.0/docs/getting_started/no_rules/lower1.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-04-23 09:48:51.000000 stepup-1.0.0/docs/getting_started/no_rules/lower2.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/no_rules/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      229 2024-04-23 09:48:15.000000 stepup-1.0.0/docs/getting_started/no_rules/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      559 2024-04-25 17:26:11.000000 stepup-1.0.0/docs/getting_started/no_rules/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1130 2024-04-24 04:15:58.000000 stepup-1.0.0/docs/getting_started/no_rules.md
--rw-r--r--   0 toon      (1000) toon      (1000)    16830 2024-04-21 18:51:43.000000 stepup-1.0.0/docs/getting_started/processes.svg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.665806 stepup-1.0.0/docs/getting_started/script_multiple/
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2024-04-23 09:09:42.000000 stepup-1.0.0/docs/getting_started/script_multiple/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)    13493 2024-04-23 09:13:25.000000 stepup-1.0.0/docs/getting_started/script_multiple/ebbr.csv
--rw-r--r--   0 toon      (1000) toon      (1000)    13550 2024-04-23 09:13:25.000000 stepup-1.0.0/docs/getting_started/script_multiple/ebos.csv
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/script_multiple/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)      151 2024-04-23 09:13:57.000000 stepup-1.0.0/docs/getting_started/script_multiple/matplotlibrc
--rwxr-xr-x   0 toon      (1000) toon      (1000)      142 2024-04-23 08:56:59.000000 stepup-1.0.0/docs/getting_started/script_multiple/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      962 2024-04-23 16:52:19.000000 stepup-1.0.0/docs/getting_started/script_multiple/plot.py
--rw-r--r--   0 toon      (1000) toon      (1000)    60122 2024-04-25 17:27:50.000000 stepup-1.0.0/docs/getting_started/script_multiple/plot_ebbr.png
--rw-r--r--   0 toon      (1000) toon      (1000)    70028 2024-04-25 17:27:50.000000 stepup-1.0.0/docs/getting_started/script_multiple/plot_ebos.png
--rw-r--r--   0 toon      (1000) toon      (1000)      523 2024-04-25 17:26:15.000000 stepup-1.0.0/docs/getting_started/script_multiple/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     4044 2024-04-23 09:36:33.000000 stepup-1.0.0/docs/getting_started/script_multiple.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.666806 stepup-1.0.0/docs/getting_started/script_single/
--rw-r--r--   0 toon      (1000) toon      (1000)       35 2024-04-22 17:39:51.000000 stepup-1.0.0/docs/getting_started/script_single/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       34 2024-04-22 17:54:33.000000 stepup-1.0.0/docs/getting_started/script_single/config.json
--rwxr-xr-x   0 toon      (1000) toon      (1000)      508 2024-04-22 17:37:22.000000 stepup-1.0.0/docs/getting_started/script_single/generate.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/script_single/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      125 2024-04-22 17:38:13.000000 stepup-1.0.0/docs/getting_started/script_single/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3959 2024-04-23 07:46:42.000000 stepup-1.0.0/docs/getting_started/script_single.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.666806 stepup-1.0.0/docs/getting_started/static_files/
--rw-r--r--   0 toon      (1000) toon      (1000)       21 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/getting_started/static_files/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      164 2024-04-22 03:31:06.000000 stepup-1.0.0/docs/getting_started/static_files/limerick.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/static_files/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      154 2024-04-22 03:37:22.000000 stepup-1.0.0/docs/getting_started/static_files/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      379 2024-04-25 17:26:11.000000 stepup-1.0.0/docs/getting_started/static_files/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1598 2024-04-23 05:44:35.000000 stepup-1.0.0/docs/getting_started/static_files.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.667806 stepup-1.0.0/docs/getting_started/static_glob/
--rw-r--r--   0 toon      (1000) toon      (1000)       12 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/getting_started/static_glob/.gitignore
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/static_glob/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      168 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/getting_started/static_glob/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.667806 stepup-1.0.0/docs/getting_started/static_glob/src/
--rw-r--r--   0 toon      (1000) toon      (1000)       13 2024-04-22 14:25:54.000000 stepup-1.0.0/docs/getting_started/static_glob/src/bar.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       13 2024-04-22 16:55:16.000000 stepup-1.0.0/docs/getting_started/static_glob/src/foo.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      529 2024-04-25 17:26:11.000000 stepup-1.0.0/docs/getting_started/static_glob/stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2061 2024-04-23 05:45:37.000000 stepup-1.0.0/docs/getting_started/static_glob.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.668806 stepup-1.0.0/docs/getting_started/static_glob_conditional/
--rw-r--r--   0 toon      (1000) toon      (1000)       20 2024-04-23 07:18:10.000000 stepup-1.0.0/docs/getting_started/static_glob_conditional/.gitignore
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.668806 stepup-1.0.0/docs/getting_started/static_glob_conditional/dataset/
--rw-r--r--   0 toon      (1000) toon      (1000)       21 2024-04-23 07:17:45.000000 stepup-1.0.0/docs/getting_started/static_glob_conditional/dataset/bigfile.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      232 2024-04-23 07:22:31.000000 stepup-1.0.0/docs/getting_started/static_glob_conditional/expensive.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      207 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/getting_started/static_glob_conditional/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      339 2024-04-23 07:22:46.000000 stepup-1.0.0/docs/getting_started/static_glob_conditional/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      866 2024-04-25 17:26:11.000000 stepup-1.0.0/docs/getting_started/static_glob_conditional/stdout1.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      369 2024-04-25 17:26:13.000000 stepup-1.0.0/docs/getting_started/static_glob_conditional/stdout2.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3372 2024-04-23 09:15:45.000000 stepup-1.0.0/docs/getting_started/static_glob_conditional.md
--rw-r--r--   0 toon      (1000) toon      (1000)     5769 2024-04-25 17:07:06.000000 stepup-1.0.0/docs/index.md
--rw-r--r--   0 toon      (1000) toon      (1000)      666 2024-04-22 17:08:37.000000 stepup-1.0.0/docs/installation.md
--rw-r--r--   0 toon      (1000) toon      (1000)      831 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/license.md
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1964 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.668806 stepup-1.0.0/docs/reference/
--rw-r--r--   0 toon      (1000) toon      (1000)     1922 2024-04-22 17:54:33.000000 stepup-1.0.0/docs/reference/interactive.md
--rw-r--r--   0 toon      (1000) toon      (1000)      731 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/reference/stepup.core.api.md
--rw-r--r--   0 toon      (1000) toon      (1000)      128 2024-04-24 20:23:46.000000 stepup-1.0.0/docs/reference/stepup.core.interact.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2600 2024-04-24 20:23:46.000000 stepup-1.0.0/mkdocs.yml
--rw-r--r--   0 toon      (1000) toon      (1000)     1752 2024-04-25 17:16:41.000000 stepup-1.0.0/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2024-04-25 17:28:17.766806 stepup-1.0.0/setup.cfg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.639806 stepup-1.0.0/stepup/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.674806 stepup-1.0.0/stepup/core/
--rw-r--r--   0 toon      (1000) toon      (1000)     1019 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)      411 2024-04-25 17:28:17.000000 stepup-1.0.0/stepup/core/_version.py
--rw-r--r--   0 toon      (1000) toon      (1000)    21187 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/api.py
--rw-r--r--   0 toon      (1000) toon      (1000)     6986 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/assoc.py
--rw-r--r--   0 toon      (1000) toon      (1000)    18834 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/cascade.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2670 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/deferred_glob.py
--rw-r--r--   0 toon      (1000) toon      (1000)    15234 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/director.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1122 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/exceptions.py
--rw-r--r--   0 toon      (1000) toon      (1000)     7072 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/file.py
--rw-r--r--   0 toon      (1000) toon      (1000)    12143 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/hash.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1952 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/interact.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3725 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/job.py
--rw-r--r--   0 toon      (1000) toon      (1000)    20162 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/nglob.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4557 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/pytest.py
--rw-r--r--   0 toon      (1000) toon      (1000)     6475 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/reporter.py
--rw-r--r--   0 toon      (1000) toon      (1000)    19031 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/rpc.py
--rw-r--r--   0 toon      (1000) toon      (1000)    11417 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/runner.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5308 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/scheduler.py
--rw-r--r--   0 toon      (1000) toon      (1000)    11450 2024-04-23 08:09:00.000000 stepup-1.0.0/stepup/core/script.py
--rw-r--r--   0 toon      (1000) toon      (1000)    27061 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/step.py
--rw-r--r--   0 toon      (1000) toon      (1000)     8819 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/tui.py
--rw-r--r--   0 toon      (1000) toon      (1000)     7368 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/utils.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2930 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/watcher.py
--rw-r--r--   0 toon      (1000) toon      (1000)    19287 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/worker.py
--rw-r--r--   0 toon      (1000) toon      (1000)    31121 2024-04-25 17:08:00.000000 stepup-1.0.0/stepup/core/workflow.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.764805 stepup-1.0.0/stepup.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)     2279 2024-04-25 17:28:17.000000 stepup-1.0.0/stepup.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)    32294 2024-04-25 17:28:17.000000 stepup-1.0.0/stepup.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2024-04-25 17:28:17.000000 stepup-1.0.0/stepup.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       48 2024-04-25 17:28:17.000000 stepup-1.0.0/stepup.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      165 2024-04-25 17:28:17.000000 stepup-1.0.0/stepup.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        7 2024-04-25 17:28:17.000000 stepup-1.0.0/stepup.egg-info/top_level.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.676806 stepup-1.0.0/tests/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.676806 stepup-1.0.0/tests/cases/
--rw-r--r--   0 toon      (1000) toon      (1000)     1866 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/README.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.678806 stepup-1.0.0/tests/cases/amend/
--rw-r--r--   0 toon      (1000) toon      (1000)      119 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/amend/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      308 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/amend/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2430 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/amend/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2430 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/amend/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2430 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/amend/expected_graph_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2430 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/amend/expected_graph_04.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     4462 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/amend/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2092 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/amend/expected_stdout_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     4038 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/amend/expected_stdout_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        6 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/amend/inp1.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     2079 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/amend/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      185 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/amend/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      249 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/amend/step.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.679806 stepup-1.0.0/tests/cases/amend_delay/
--rw-r--r--   0 toon      (1000) toon      (1000)      115 2024-04-18 22:28:13.000000 stepup-1.0.0/tests/cases/amend_delay/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      197 2024-04-18 20:13:06.000000 stepup-1.0.0/tests/cases/amend_delay/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3755 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/amend_delay/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3755 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/amend_delay/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3755 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/amend_delay/expected_graph_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     4954 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/amend_delay/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1605 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/amend_delay/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      308 2024-04-18 22:28:13.000000 stepup-1.0.0/tests/cases/amend_delay/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      307 2024-04-18 22:29:00.000000 stepup-1.0.0/tests/cases/amend_delay/step.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.680806 stepup-1.0.0/tests/cases/amend_env_vars/
--rw-r--r--   0 toon      (1000) toon      (1000)       42 2024-03-23 20:28:52.000000 stepup-1.0.0/tests/cases/amend_env_vars/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      156 2024-03-23 20:19:14.000000 stepup-1.0.0/tests/cases/amend_env_vars/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1860 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/amend_env_vars/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      279 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/amend_env_vars/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       24 2024-03-23 20:24:41.000000 stepup-1.0.0/tests/cases/amend_env_vars/foo.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      696 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/amend_env_vars/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      100 2024-03-24 06:59:03.000000 stepup-1.0.0/tests/cases/amend_env_vars/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      475 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/amend_env_vars/step.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.681806 stepup-1.0.0/tests/cases/amend_missing/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-04-18 21:56:44.000000 stepup-1.0.0/tests/cases/amend_missing/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      156 2024-04-21 07:24:13.000000 stepup-1.0.0/tests/cases/amend_missing/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2009 2024-04-25 17:19:38.000000 stepup-1.0.0/tests/cases/amend_missing/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2051 2024-04-25 17:19:38.000000 stepup-1.0.0/tests/cases/amend_missing/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      566 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/amend_missing/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      189 2024-04-22 14:25:54.000000 stepup-1.0.0/tests/cases/amend_missing/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      203 2024-04-22 14:25:54.000000 stepup-1.0.0/tests/cases/amend_missing/step.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.682806 stepup-1.0.0/tests/cases/amend_outdir_pending/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-16 15:07:29.000000 stepup-1.0.0/tests/cases/amend_outdir_pending/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      176 2024-04-21 07:23:44.000000 stepup-1.0.0/tests/cases/amend_outdir_pending/README.md
--rwxr-xr-x   0 toon      (1000) toon      (1000)       92 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/amend_outdir_pending/demo.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1542 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/amend_outdir_pending/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1694 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/amend_outdir_pending/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      538 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/amend_outdir_pending/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)       74 2024-03-24 06:59:03.000000 stepup-1.0.0/tests/cases/amend_outdir_pending/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.683806 stepup-1.0.0/tests/cases/amend_voldir_pending/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-16 15:07:29.000000 stepup-1.0.0/tests/cases/amend_voldir_pending/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      176 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/amend_voldir_pending/README.md
--rwxr-xr-x   0 toon      (1000) toon      (1000)       92 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/amend_voldir_pending/demo.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1543 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/amend_voldir_pending/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1419 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/amend_voldir_pending/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      538 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/amend_voldir_pending/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)       74 2024-03-24 06:59:03.000000 stepup-1.0.0/tests/cases/amend_voldir_pending/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.684806 stepup-1.0.0/tests/cases/deferred_glob1/
--rw-r--r--   0 toon      (1000) toon      (1000)       59 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/deferred_glob1/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      213 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob1/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2250 2024-04-25 17:19:44.000000 stepup-1.0.0/tests/cases/deferred_glob1/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2250 2024-04-25 17:19:44.000000 stepup-1.0.0/tests/cases/deferred_glob1/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      329 2024-04-25 17:19:44.000000 stepup-1.0.0/tests/cases/deferred_glob1/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      380 2024-04-25 17:19:44.000000 stepup-1.0.0/tests/cases/deferred_glob1/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1221 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/deferred_glob1/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      153 2024-03-29 17:35:46.000000 stepup-1.0.0/tests/cases/deferred_glob1/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.684806 stepup-1.0.0/tests/cases/deferred_glob1/static/
--rw-r--r--   0 toon      (1000) toon      (1000)        6 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob1/static/data1.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        6 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob1/static/data2.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.684806 stepup-1.0.0/tests/cases/deferred_glob1/static/sub/
--rw-r--r--   0 toon      (1000) toon      (1000)        4 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob1/static/sub/bar.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        4 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob1/static/sub/foo.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.685806 stepup-1.0.0/tests/cases/deferred_glob2/
--rw-r--r--   0 toon      (1000) toon      (1000)       67 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/deferred_glob2/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      213 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob2/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2203 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/deferred_glob2/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      774 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/deferred_glob2/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      538 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/deferred_glob2/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      989 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/deferred_glob2/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      132 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/deferred_glob2/plan_01.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)       87 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/deferred_glob2/plan_02.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.685806 stepup-1.0.0/tests/cases/deferred_glob2/static/
--rw-r--r--   0 toon      (1000) toon      (1000)        6 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob2/static/data1.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        6 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob2/static/data2.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.686806 stepup-1.0.0/tests/cases/deferred_glob2/static/sub/
--rw-r--r--   0 toon      (1000) toon      (1000)        4 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob2/static/sub/bar.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        4 2024-03-25 23:52:39.000000 stepup-1.0.0/tests/cases/deferred_glob2/static/sub/foo.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.687806 stepup-1.0.0/tests/cases/deferred_subdir/
--rw-r--r--   0 toon      (1000) toon      (1000)       39 2024-03-31 14:36:45.000000 stepup-1.0.0/tests/cases/deferred_subdir/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       70 2024-03-31 14:38:18.000000 stepup-1.0.0/tests/cases/deferred_subdir/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2572 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/deferred_subdir/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      403 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/deferred_subdir/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      603 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/deferred_subdir/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      107 2024-04-20 04:14:34.000000 stepup-1.0.0/tests/cases/deferred_subdir/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.688806 stepup-1.0.0/tests/cases/deferred_subdir/sub/
--rwxr-xr-x   0 toon      (1000) toon      (1000)      119 2024-03-31 14:40:11.000000 stepup-1.0.0/tests/cases/deferred_subdir/sub/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)       23 2024-03-31 14:34:42.000000 stepup-1.0.0/tests/cases/deferred_subdir/sub/unused.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       19 2024-03-31 14:34:47.000000 stepup-1.0.0/tests/cases/deferred_subdir/sub/used.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.691806 stepup-1.0.0/tests/cases/env_vars/
--rw-r--r--   0 toon      (1000) toon      (1000)      321 2024-03-23 11:31:24.000000 stepup-1.0.0/tests/cases/env_vars/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      391 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/env_vars/README.md
--rwxr-xr-x   0 toon      (1000) toon      (1000)      242 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/env_vars/demovars.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2598 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2648 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2648 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_graph_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2648 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_graph_04.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2648 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_graph_05.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3046 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_stdout_a.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2494 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_stdout_b.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2494 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_stdout_c.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2494 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_stdout_d.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       68 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_variables_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       68 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_variables_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       68 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_variables_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       68 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_variables_04.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       34 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/env_vars/expected_variables_05.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     3211 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/env_vars/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      183 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/env_vars/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      224 2024-03-23 19:42:59.000000 stepup-1.0.0/tests/cases/env_vars/printvars.py
--rw-r--r--   0 toon      (1000) toon      (1000)       35 2024-03-23 19:43:00.000000 stepup-1.0.0/tests/cases/env_vars/variables_01.json
--rw-r--r--   0 toon      (1000) toon      (1000)       67 2024-03-23 19:42:59.000000 stepup-1.0.0/tests/cases/env_vars/variables_02.json
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.692806 stepup-1.0.0/tests/cases/env_vars_amend/
--rw-r--r--   0 toon      (1000) toon      (1000)       61 2024-03-23 13:28:49.000000 stepup-1.0.0/tests/cases/env_vars_amend/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      176 2024-03-23 13:25:17.000000 stepup-1.0.0/tests/cases/env_vars_amend/README.md
--rwxr-xr-x   0 toon      (1000) toon      (1000)      102 2024-03-29 17:37:38.000000 stepup-1.0.0/tests/cases/env_vars_amend/demovars.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1678 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/env_vars_amend/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1678 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/env_vars_amend/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      313 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/env_vars_amend/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1832 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/env_vars_amend/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1033 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/env_vars_amend/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      162 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/env_vars_amend/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.694806 stepup-1.0.0/tests/cases/env_vars_path/
--rw-r--r--   0 toon      (1000) toon      (1000)      116 2024-03-23 16:38:59.000000 stepup-1.0.0/tests/cases/env_vars_path/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       54 2024-03-23 16:35:17.000000 stepup-1.0.0/tests/cases/env_vars_path/FOO.md
--rw-r--r--   0 toon      (1000) toon      (1000)       60 2024-03-23 16:35:17.000000 stepup-1.0.0/tests/cases/env_vars_path/FOO.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      495 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/env_vars_path/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2497 2024-04-25 17:19:39.000000 stepup-1.0.0/tests/cases/env_vars_path/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2423 2024-04-25 17:19:39.000000 stepup-1.0.0/tests/cases/env_vars_path/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1177 2024-04-25 17:19:39.000000 stepup-1.0.0/tests/cases/env_vars_path/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1436 2024-04-25 17:19:39.000000 stepup-1.0.0/tests/cases/env_vars_path/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1263 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/env_vars_path/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      480 2024-03-29 18:17:05.000000 stepup-1.0.0/tests/cases/env_vars_path/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.695806 stepup-1.0.0/tests/cases/env_vars_subs/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-30 06:15:34.000000 stepup-1.0.0/tests/cases/env_vars_subs/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      136 2024-03-30 06:12:55.000000 stepup-1.0.0/tests/cases/env_vars_subs/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1641 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/env_vars_subs/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1223 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/env_vars_subs/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      620 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/env_vars_subs/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      159 2024-04-20 04:20:55.000000 stepup-1.0.0/tests/cases/env_vars_subs/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.695806 stepup-1.0.0/tests/cases/env_vars_subs/sub/
--rwxr-xr-x   0 toon      (1000) toon      (1000)      133 2024-03-30 06:15:01.000000 stepup-1.0.0/tests/cases/env_vars_subs/sub/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.696806 stepup-1.0.0/tests/cases/env_vars_workdir/
--rw-r--r--   0 toon      (1000) toon      (1000)       41 2024-03-23 19:37:42.000000 stepup-1.0.0/tests/cases/env_vars_workdir/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       70 2024-03-23 19:32:50.000000 stepup-1.0.0/tests/cases/env_vars_workdir/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1918 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/env_vars_workdir/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      335 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/env_vars_workdir/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      648 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/env_vars_workdir/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      355 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/env_vars_workdir/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.697806 stepup-1.0.0/tests/cases/env_vars_workdir/sub/
--rw-r--r--   0 toon      (1000) toon      (1000)       40 2024-03-23 19:34:02.000000 stepup-1.0.0/tests/cases/env_vars_workdir/sub/input.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.698806 stepup-1.0.0/tests/cases/error_cyclic_early/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_cyclic_early/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      156 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_cyclic_early/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      903 2024-04-25 17:19:43.000000 stepup-1.0.0/tests/cases/error_cyclic_early/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2771 2024-04-25 17:19:43.000000 stepup-1.0.0/tests/cases/error_cyclic_early/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      568 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/error_cyclic_early/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      108 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_cyclic_early/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.698806 stepup-1.0.0/tests/cases/error_cyclic_late/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_cyclic_late/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      156 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_cyclic_late/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      827 2024-04-25 17:19:45.000000 stepup-1.0.0/tests/cases/error_cyclic_late/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3041 2024-04-25 17:19:45.000000 stepup-1.0.0/tests/cases/error_cyclic_late/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      595 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/error_cyclic_late/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      164 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_cyclic_late/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.699806 stepup-1.0.0/tests/cases/error_deferred_nonexisting/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_deferred_nonexisting/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      156 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_deferred_nonexisting/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2217 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/error_deferred_nonexisting/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1161 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/error_deferred_nonexisting/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      568 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/error_deferred_nonexisting/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      162 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_deferred_nonexisting/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.701806 stepup-1.0.0/tests/cases/error_env_var/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-23 19:48:25.000000 stepup-1.0.0/tests/cases/error_env_var/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       67 2024-03-23 19:46:10.000000 stepup-1.0.0/tests/cases/error_env_var/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      679 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/error_env_var/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1575 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/error_env_var/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      538 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/error_env_var/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      124 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_env_var/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.702806 stepup-1.0.0/tests/cases/error_main_fails/
--rw-r--r--   0 toon      (1000) toon      (1000)       69 2024-03-30 16:48:21.000000 stepup-1.0.0/tests/cases/error_main_fails/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       31 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/error_main_fails/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1251 2024-04-25 17:19:49.000000 stepup-1.0.0/tests/cases/error_main_fails/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      984 2024-04-25 17:19:49.000000 stepup-1.0.0/tests/cases/error_main_fails/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      293 2024-04-25 17:19:49.000000 stepup-1.0.0/tests/cases/error_main_fails/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2096 2024-04-25 17:19:49.000000 stepup-1.0.0/tests/cases/error_main_fails/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1052 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/error_main_fails/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      101 2024-03-30 16:46:36.000000 stepup-1.0.0/tests/cases/error_main_fails/plan_01.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)       36 2024-03-30 16:46:36.000000 stepup-1.0.0/tests/cases/error_main_fails/plan_02.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.703806 stepup-1.0.0/tests/cases/error_not_executable/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/error_not_executable/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       31 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/error_not_executable/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      903 2024-04-25 17:19:49.000000 stepup-1.0.0/tests/cases/error_not_executable/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      385 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/error_not_executable/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)      107 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_not_executable/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.705806 stepup-1.0.0/tests/cases/error_overlap_deferred/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_overlap_deferred/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      156 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_overlap_deferred/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      501 2024-04-25 17:19:27.000000 stepup-1.0.0/tests/cases/error_overlap_deferred/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2727 2024-04-25 17:19:27.000000 stepup-1.0.0/tests/cases/error_overlap_deferred/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      568 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/error_overlap_deferred/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      157 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_overlap_deferred/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.706806 stepup-1.0.0/tests/cases/error_static_dir/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-16 15:07:29.000000 stepup-1.0.0/tests/cases/error_static_dir/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      117 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/error_static_dir/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      679 2024-04-25 17:19:28.000000 stepup-1.0.0/tests/cases/error_static_dir/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1430 2024-04-25 17:19:28.000000 stepup-1.0.0/tests/cases/error_static_dir/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      538 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/error_static_dir/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      114 2024-04-01 08:45:34.000000 stepup-1.0.0/tests/cases/error_static_dir/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.706806 stepup-1.0.0/tests/cases/error_static_dir/subdir/
--rw-r--r--   0 toon      (1000) toon      (1000)        0 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/error_static_dir/subdir/.keep
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.707805 stepup-1.0.0/tests/cases/error_step/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-16 15:07:29.000000 stepup-1.0.0/tests/cases/error_step/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      117 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/error_step/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1228 2024-04-25 17:19:30.000000 stepup-1.0.0/tests/cases/error_step/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1423 2024-04-25 17:19:30.000000 stepup-1.0.0/tests/cases/error_step/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      538 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/error_step/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      107 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/error_step/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.708806 stepup-1.0.0/tests/cases/here/
--rw-r--r--   0 toon      (1000) toon      (1000)       41 2024-03-24 05:24:41.000000 stepup-1.0.0/tests/cases/here/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      186 2024-03-23 21:01:41.000000 stepup-1.0.0/tests/cases/here/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     4364 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/here/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      612 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/here/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      728 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/here/main.sh
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.708806 stepup-1.0.0/tests/cases/here/source/
--rwxr-xr-x   0 toon      (1000) toon      (1000)      198 2024-04-24 20:23:46.000000 stepup-1.0.0/tests/cases/here/source/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.708806 stepup-1.0.0/tests/cases/here/source/www/
--rw-r--r--   0 toon      (1000) toon      (1000)       28 2024-03-23 21:06:49.000000 stepup-1.0.0/tests/cases/here/source/www/index.md
--rwxr-xr-x   0 toon      (1000) toon      (1000)      130 2024-03-24 05:41:23.000000 stepup-1.0.0/tests/cases/here/source/www/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.709806 stepup-1.0.0/tests/cases/makedirs/
--rw-r--r--   0 toon      (1000) toon      (1000)       31 2024-03-31 13:16:16.000000 stepup-1.0.0/tests/cases/makedirs/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       86 2024-03-31 13:12:50.000000 stepup-1.0.0/tests/cases/makedirs/README.md
--rwxr-xr-x   0 toon      (1000) toon      (1000)      456 2024-03-31 13:27:55.000000 stepup-1.0.0/tests/cases/makedirs/bunch.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2966 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/makedirs/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      281 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/makedirs/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      614 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/makedirs/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      170 2024-03-31 13:29:44.000000 stepup-1.0.0/tests/cases/makedirs/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.710806 stepup-1.0.0/tests/cases/mkdir/
--rw-r--r--   0 toon      (1000) toon      (1000)       42 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/mkdir/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       56 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/mkdir/README.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.710806 stepup-1.0.0/tests/cases/mkdir/exists/
--rw-r--r--   0 toon      (1000) toon      (1000)        0 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/mkdir/exists/.keep
--rw-r--r--   0 toon      (1000) toon      (1000)     2266 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/mkdir/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      417 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/mkdir/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      603 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/mkdir/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      237 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/mkdir/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.711806 stepup-1.0.0/tests/cases/mkdir_error/
--rw-r--r--   0 toon      (1000) toon      (1000)       42 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/mkdir_error/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      229 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/mkdir_error/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1634 2024-04-25 17:19:37.000000 stepup-1.0.0/tests/cases/mkdir_error/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      974 2024-04-25 17:19:37.000000 stepup-1.0.0/tests/cases/mkdir_error/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      538 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/mkdir_error/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)       79 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/mkdir_error/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.712806 stepup-1.0.0/tests/cases/nodata/
--rw-r--r--   0 toon      (1000) toon      (1000)       93 2024-03-25 03:11:01.000000 stepup-1.0.0/tests/cases/nodata/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      217 2024-03-24 10:16:56.000000 stepup-1.0.0/tests/cases/nodata/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2108 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/nodata/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1378 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/nodata/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2108 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/nodata/expected_graph_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1662 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/nodata/expected_stdout_a.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      980 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/nodata/expected_stdout_b.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1504 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/nodata/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)       85 2024-03-24 10:09:08.000000 stepup-1.0.0/tests/cases/nodata/original.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      259 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/nodata/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.713806 stepup-1.0.0/tests/cases/noplan/
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/noplan/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       62 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/noplan/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      885 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/noplan/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      294 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/noplan/main.sh
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.713806 stepup-1.0.0/tests/cases/nostatic/
--rw-r--r--   0 toon      (1000) toon      (1000)       47 2024-03-16 15:07:29.000000 stepup-1.0.0/tests/cases/nostatic/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      231 2024-04-21 07:23:44.000000 stepup-1.0.0/tests/cases/nostatic/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1886 2024-04-25 17:19:43.000000 stepup-1.0.0/tests/cases/nostatic/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      867 2024-04-25 17:19:43.000000 stepup-1.0.0/tests/cases/nostatic/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      599 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/nostatic/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      181 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/nostatic/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.715806 stepup-1.0.0/tests/cases/optional_convert/
--rw-r--r--   0 toon      (1000) toon      (1000)      145 2024-04-15 14:34:12.000000 stepup-1.0.0/tests/cases/optional_convert/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      471 2024-03-24 15:24:38.000000 stepup-1.0.0/tests/cases/optional_convert/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3217 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/optional_convert/expected_graph_a.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3217 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/optional_convert/expected_graph_b.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3217 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/optional_convert/expected_graph_c.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      514 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/optional_convert/expected_stdout_a.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      508 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/optional_convert/expected_stdout_b.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1552 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/optional_convert/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      253 2024-03-29 17:37:38.000000 stepup-1.0.0/tests/cases/optional_convert/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)        7 2024-03-24 16:16:29.000000 stepup-1.0.0/tests/cases/optional_convert/raw_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        7 2024-03-24 16:16:29.000000 stepup-1.0.0/tests/cases/optional_convert/raw_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        7 2024-03-24 16:16:29.000000 stepup-1.0.0/tests/cases/optional_convert/raw_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        7 2024-03-24 16:16:29.000000 stepup-1.0.0/tests/cases/optional_convert/raw_04.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.716806 stepup-1.0.0/tests/cases/output_not_created/
--rw-r--r--   0 toon      (1000) toon      (1000)       46 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/output_not_created/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      138 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/output_not_created/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1821 2024-04-25 17:19:27.000000 stepup-1.0.0/tests/cases/output_not_created/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1203 2024-04-25 17:19:27.000000 stepup-1.0.0/tests/cases/output_not_created/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      631 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/output_not_created/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      169 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/output_not_created/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.716806 stepup-1.0.0/tests/cases/pending/
--rw-r--r--   0 toon      (1000) toon      (1000)       47 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/pending/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      158 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/pending/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1738 2024-04-25 17:19:29.000000 stepup-1.0.0/tests/cases/pending/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1007 2024-04-25 17:19:29.000000 stepup-1.0.0/tests/cases/pending/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      538 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/pending/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      143 2024-04-01 10:26:22.000000 stepup-1.0.0/tests/cases/pending/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.717805 stepup-1.0.0/tests/cases/permissions_file_rerun/
--rw-r--r--   0 toon      (1000) toon      (1000)       61 2024-04-01 12:01:03.000000 stepup-1.0.0/tests/cases/permissions_file_rerun/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      114 2024-04-01 11:59:36.000000 stepup-1.0.0/tests/cases/permissions_file_rerun/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1570 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/permissions_file_rerun/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1570 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/permissions_file_rerun/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      540 2024-04-25 17:19:31.000000 stepup-1.0.0/tests/cases/permissions_file_rerun/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       51 2024-04-01 11:59:36.000000 stepup-1.0.0/tests/cases/permissions_file_rerun/input.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1203 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/permissions_file_rerun/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      116 2024-04-01 12:00:24.000000 stepup-1.0.0/tests/cases/permissions_file_rerun/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.718806 stepup-1.0.0/tests/cases/permissions_plan_rerun/
--rw-r--r--   0 toon      (1000) toon      (1000)       63 2024-04-01 11:38:30.000000 stepup-1.0.0/tests/cases/permissions_plan_rerun/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      150 2024-04-01 03:33:17.000000 stepup-1.0.0/tests/cases/permissions_plan_rerun/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1496 2024-04-25 17:19:33.000000 stepup-1.0.0/tests/cases/permissions_plan_rerun/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2073 2024-04-25 17:19:33.000000 stepup-1.0.0/tests/cases/permissions_plan_rerun/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1513 2024-04-25 17:19:33.000000 stepup-1.0.0/tests/cases/permissions_plan_rerun/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      989 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/permissions_plan_rerun/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      107 2024-04-20 04:20:55.000000 stepup-1.0.0/tests/cases/permissions_plan_rerun/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.718806 stepup-1.0.0/tests/cases/permissions_plan_rerun/sub/
--rwxr-xr-x   0 toon      (1000) toon      (1000)       95 2024-04-01 11:38:30.000000 stepup-1.0.0/tests/cases/permissions_plan_rerun/sub/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.719806 stepup-1.0.0/tests/cases/permissions_plan_restart/
--rw-r--r--   0 toon      (1000) toon      (1000)       63 2024-04-01 11:47:30.000000 stepup-1.0.0/tests/cases/permissions_plan_restart/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      150 2024-04-01 03:33:17.000000 stepup-1.0.0/tests/cases/permissions_plan_restart/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1523 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/permissions_plan_restart/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2154 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/permissions_plan_restart/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1216 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/permissions_plan_restart/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      970 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/permissions_plan_restart/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1148 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/permissions_plan_restart/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      107 2024-04-20 04:20:55.000000 stepup-1.0.0/tests/cases/permissions_plan_restart/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.720806 stepup-1.0.0/tests/cases/permissions_plan_restart/sub/
--rwxr-xr-x   0 toon      (1000) toon      (1000)       95 2024-04-01 11:47:30.000000 stepup-1.0.0/tests/cases/permissions_plan_restart/sub/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.722806 stepup-1.0.0/tests/cases/permissions_step_rerun/
--rw-r--r--   0 toon      (1000) toon      (1000)       62 2024-04-01 03:39:50.000000 stepup-1.0.0/tests/cases/permissions_step_rerun/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      150 2024-04-01 03:33:17.000000 stepup-1.0.0/tests/cases/permissions_step_rerun/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1222 2024-04-25 17:19:38.000000 stepup-1.0.0/tests/cases/permissions_step_rerun/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1225 2024-04-25 17:19:38.000000 stepup-1.0.0/tests/cases/permissions_step_rerun/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1352 2024-04-25 17:19:38.000000 stepup-1.0.0/tests/cases/permissions_step_rerun/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      967 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/permissions_step_rerun/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-01 04:33:50.000000 stepup-1.0.0/tests/cases/permissions_step_rerun/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)       95 2024-04-01 03:37:39.000000 stepup-1.0.0/tests/cases/permissions_step_rerun/step.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.723806 stepup-1.0.0/tests/cases/permissions_step_restart/
--rw-r--r--   0 toon      (1000) toon      (1000)       62 2024-04-01 03:39:50.000000 stepup-1.0.0/tests/cases/permissions_step_restart/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      150 2024-04-01 03:33:17.000000 stepup-1.0.0/tests/cases/permissions_step_restart/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1249 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/permissions_step_restart/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1279 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/permissions_step_restart/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1167 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/permissions_step_restart/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      866 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/permissions_step_restart/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1066 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/permissions_step_restart/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-04-01 04:33:50.000000 stepup-1.0.0/tests/cases/permissions_step_restart/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)       95 2024-04-01 03:37:39.000000 stepup-1.0.0/tests/cases/permissions_step_restart/step.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.724805 stepup-1.0.0/tests/cases/pool/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/pool/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      164 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/pool/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1574 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/pool/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1422 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/pool/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      592 2024-04-21 12:39:21.000000 stepup-1.0.0/tests/cases/pool/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      316 2024-03-24 06:59:03.000000 stepup-1.0.0/tests/cases/pool/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)       46 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/pool/r.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.725806 stepup-1.0.0/tests/cases/reqdir_missing/
--rw-r--r--   0 toon      (1000) toon      (1000)       30 2024-03-26 02:00:30.000000 stepup-1.0.0/tests/cases/reqdir_missing/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      181 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/reqdir_missing/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1956 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/reqdir_missing/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1006 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/reqdir_missing/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      609 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/reqdir_missing/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      136 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/reqdir_missing/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.727805 stepup-1.0.0/tests/cases/restart_blocked/
--rw-r--r--   0 toon      (1000) toon      (1000)       89 2024-04-14 09:58:27.000000 stepup-1.0.0/tests/cases/restart_blocked/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      175 2024-04-14 09:52:15.000000 stepup-1.0.0/tests/cases/restart_blocked/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3177 2024-04-25 17:19:45.000000 stepup-1.0.0/tests/cases/restart_blocked/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3149 2024-04-25 17:19:45.000000 stepup-1.0.0/tests/cases/restart_blocked/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      905 2024-04-25 17:19:45.000000 stepup-1.0.0/tests/cases/restart_blocked/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      936 2024-04-25 17:19:45.000000 stepup-1.0.0/tests/cases/restart_blocked/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      210 2024-04-14 09:58:52.000000 stepup-1.0.0/tests/cases/restart_blocked/expensive.py
--rw-r--r--   0 toon      (1000) toon      (1000)       18 2024-04-14 09:52:36.000000 stepup-1.0.0/tests/cases/restart_blocked/initial.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1060 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/restart_blocked/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      261 2024-04-14 09:58:36.000000 stepup-1.0.0/tests/cases/restart_blocked/plan_blocked.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      249 2024-04-14 09:58:36.000000 stepup-1.0.0/tests/cases/restart_blocked/plan_unblocked.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.728806 stepup-1.0.0/tests/cases/restart_changes/
--rw-r--r--   0 toon      (1000) toon      (1000)      104 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/restart_changes/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      447 2024-04-21 07:23:44.000000 stepup-1.0.0/tests/cases/restart_changes/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2693 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/restart_changes/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2693 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/restart_changes/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      421 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/restart_changes/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      529 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/restart_changes/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1402 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/restart_changes/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      301 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/restart_changes/plan_01.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      301 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/restart_changes/plan_02.py
--rw-r--r--   0 toon      (1000) toon      (1000)       48 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/restart_changes/source_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       40 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/restart_changes/source_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       60 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/restart_changes/source_both.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.730805 stepup-1.0.0/tests/cases/restart_deferred_glob/
--rw-r--r--   0 toon      (1000) toon      (1000)       86 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/restart_deferred_glob/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       70 2024-03-31 12:08:51.000000 stepup-1.0.0/tests/cases/restart_deferred_glob/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1672 2024-04-25 17:19:29.000000 stepup-1.0.0/tests/cases/restart_deferred_glob/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1672 2024-04-25 17:19:29.000000 stepup-1.0.0/tests/cases/restart_deferred_glob/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      777 2024-04-25 17:19:29.000000 stepup-1.0.0/tests/cases/restart_deferred_glob/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1418 2024-04-25 17:19:29.000000 stepup-1.0.0/tests/cases/restart_deferred_glob/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      952 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/restart_deferred_glob/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      142 2024-03-31 12:10:13.000000 stepup-1.0.0/tests/cases/restart_deferred_glob/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.730805 stepup-1.0.0/tests/cases/restart_deferred_glob/static/
--rw-r--r--   0 toon      (1000) toon      (1000)       32 2024-03-31 12:09:10.000000 stepup-1.0.0/tests/cases/restart_deferred_glob/static/foo.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.731806 stepup-1.0.0/tests/cases/restart_nochanges/
--rw-r--r--   0 toon      (1000) toon      (1000)       86 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/restart_nochanges/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      278 2024-04-21 07:23:44.000000 stepup-1.0.0/tests/cases/restart_nochanges/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2852 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/restart_nochanges/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2852 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/restart_nochanges/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      537 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/restart_nochanges/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2729 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/restart_nochanges/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1074 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/restart_nochanges/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      296 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/restart_nochanges/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.732806 stepup-1.0.0/tests/cases/restart_orphan/
--rw-r--r--   0 toon      (1000) toon      (1000)       66 2024-03-31 06:13:26.000000 stepup-1.0.0/tests/cases/restart_orphan/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       70 2024-03-31 06:11:49.000000 stepup-1.0.0/tests/cases/restart_orphan/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1901 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/restart_orphan/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1901 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/restart_orphan/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      375 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/restart_orphan/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2040 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/restart_orphan/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      994 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/restart_orphan/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      132 2024-03-31 06:12:30.000000 stepup-1.0.0/tests/cases/restart_orphan/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.733806 stepup-1.0.0/tests/cases/restart_outdated_amend/
--rw-r--r--   0 toon      (1000) toon      (1000)       86 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/restart_outdated_amend/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       90 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/restart_outdated_amend/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2177 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/restart_outdated_amend/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2177 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/restart_outdated_amend/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      279 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/restart_outdated_amend/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1719 2024-04-25 17:19:35.000000 stepup-1.0.0/tests/cases/restart_outdated_amend/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1147 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/restart_outdated_amend/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      164 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/restart_outdated_amend/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      271 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/restart_outdated_amend/step.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.734805 stepup-1.0.0/tests/cases/restart_output/
--rw-r--r--   0 toon      (1000) toon      (1000)       59 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/restart_output/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      278 2024-04-21 07:23:44.000000 stepup-1.0.0/tests/cases/restart_output/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1637 2024-04-25 17:19:38.000000 stepup-1.0.0/tests/cases/restart_output/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1637 2024-04-25 17:19:38.000000 stepup-1.0.0/tests/cases/restart_output/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      317 2024-04-25 17:19:38.000000 stepup-1.0.0/tests/cases/restart_output/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1754 2024-04-25 17:19:38.000000 stepup-1.0.0/tests/cases/restart_output/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      972 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/restart_output/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)       10 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/restart_output/original.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      120 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/restart_output/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.735806 stepup-1.0.0/tests/cases/script_cases/
--rw-r--r--   0 toon      (1000) toon      (1000)       52 2024-03-16 15:07:29.000000 stepup-1.0.0/tests/cases/script_cases/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      262 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/script_cases/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3075 2024-04-25 17:19:44.000000 stepup-1.0.0/tests/cases/script_cases/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      445 2024-04-25 17:19:44.000000 stepup-1.0.0/tests/cases/script_cases/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       67 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/script_cases/helper.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      662 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/script_cases/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      115 2024-03-30 05:44:08.000000 stepup-1.0.0/tests/cases/script_cases/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      397 2024-04-16 22:11:52.000000 stepup-1.0.0/tests/cases/script_cases/work.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.736806 stepup-1.0.0/tests/cases/script_cases_settings/
--rw-r--r--   0 toon      (1000) toon      (1000)       52 2024-04-16 21:54:11.000000 stepup-1.0.0/tests/cases/script_cases_settings/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      596 2024-04-21 07:24:13.000000 stepup-1.0.0/tests/cases/script_cases_settings/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3430 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/script_cases_settings/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      445 2024-04-25 17:19:46.000000 stepup-1.0.0/tests/cases/script_cases_settings/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       67 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/script_cases_settings/helper.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      662 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/script_cases_settings/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      130 2024-04-16 21:53:36.000000 stepup-1.0.0/tests/cases/script_cases_settings/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)       21 2024-04-16 21:52:31.000000 stepup-1.0.0/tests/cases/script_cases_settings/settings.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      423 2024-04-16 22:11:52.000000 stepup-1.0.0/tests/cases/script_cases_settings/work.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.737805 stepup-1.0.0/tests/cases/script_single/
--rw-r--r--   0 toon      (1000) toon      (1000)       54 2024-03-28 16:30:28.000000 stepup-1.0.0/tests/cases/script_single/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      163 2024-04-21 07:23:44.000000 stepup-1.0.0/tests/cases/script_single/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3602 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/script_single/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      533 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/script_single/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      643 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/script_single/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      193 2024-04-20 04:56:16.000000 stepup-1.0.0/tests/cases/script_single/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.738806 stepup-1.0.0/tests/cases/script_single/work/
--rw-r--r--   0 toon      (1000) toon      (1000)       33 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/script_single/work/config.json
--rwxr-xr-x   0 toon      (1000) toon      (1000)      554 2024-04-16 22:11:52.000000 stepup-1.0.0/tests/cases/script_single/work/generate.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.739806 stepup-1.0.0/tests/cases/static/
--rw-r--r--   0 toon      (1000) toon      (1000)       33 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/static/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      166 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/static/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      918 2024-04-25 17:19:48.000000 stepup-1.0.0/tests/cases/static/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      229 2024-04-25 17:19:48.000000 stepup-1.0.0/tests/cases/static/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      571 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/static/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)       10 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static/original.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)       81 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/static/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.741805 stepup-1.0.0/tests/cases/static_abs/
--rw-r--r--   0 toon      (1000) toon      (1000)       33 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/static_abs/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      172 2024-04-21 07:24:14.000000 stepup-1.0.0/tests/cases/static_abs/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1481 2024-04-25 17:19:29.000000 stepup-1.0.0/tests/cases/static_abs/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      229 2024-04-25 17:19:29.000000 stepup-1.0.0/tests/cases/static_abs/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      571 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/static_abs/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)       10 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static_abs/original.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      103 2024-04-24 20:23:46.000000 stepup-1.0.0/tests/cases/static_abs/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.742806 stepup-1.0.0/tests/cases/static_dir/
--rw-r--r--   0 toon      (1000) toon      (1000)       33 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/static_dir/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       41 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static_dir/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      898 2024-04-25 17:19:30.000000 stepup-1.0.0/tests/cases/static_dir/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      229 2024-04-25 17:19:30.000000 stepup-1.0.0/tests/cases/static_dir/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      599 2024-04-21 12:39:13.000000 stepup-1.0.0/tests/cases/static_dir/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)       76 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/static_dir/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.744805 stepup-1.0.0/tests/cases/static_glob/
--rw-r--r--   0 toon      (1000) toon      (1000)      150 2024-03-25 02:56:32.000000 stepup-1.0.0/tests/cases/static_glob/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      137 2024-04-21 07:23:44.000000 stepup-1.0.0/tests/cases/static_glob/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2516 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/static_glob/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2516 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/static_glob/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2516 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/static_glob/expected_graph_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1312 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/static_glob/expected_stdout_a.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1016 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/static_glob/expected_stdout_b.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1692 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/static_glob/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      137 2024-03-24 09:53:01.000000 stepup-1.0.0/tests/cases/static_glob/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.746806 stepup-1.0.0/tests/cases/static_nglob/
--rw-r--r--   0 toon      (1000) toon      (1000)      442 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/static_nglob/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      134 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static_nglob/README.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.746806 stepup-1.0.0/tests/cases/static_nglob/ch-1-intro/
--rw-r--r--   0 toon      (1000) toon      (1000)       17 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static_nglob/ch-1-intro/sec-1-1-blabla.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       22 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static_nglob/ch-1-intro/sec-1-2-some-more.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.746806 stepup-1.0.0/tests/cases/static_nglob/ch-2-theory/
--rw-r--r--   0 toon      (1000) toon      (1000)       30 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static_nglob/ch-2-theory/sec-2-1-basics.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.746806 stepup-1.0.0/tests/cases/static_nglob/ch-3-conclusions/
--rw-r--r--   0 toon      (1000) toon      (1000)       24 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static_nglob/ch-3-conclusions/sec-3-1-summary.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       19 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static_nglob/ch-3-conclusions/sec-3-2-outlook.txt
--rw-r--r--   0 toon      (1000) toon      (1000)    17182 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/static_nglob/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)    17182 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/static_nglob/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     5129 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/static_nglob/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     2370 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/static_nglob/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      972 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/static_nglob/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)       24 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/static_nglob/sec-2-2.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.748806 stepup-1.0.0/tests/cases/static_nglob_partial/
--rw-r--r--   0 toon      (1000) toon      (1000)      228 2024-03-25 03:42:01.000000 stepup-1.0.0/tests/cases/static_nglob_partial/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      302 2024-03-25 03:28:04.000000 stepup-1.0.0/tests/cases/static_nglob_partial/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2411 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/static_nglob_partial/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3805 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/static_nglob_partial/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2639 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/static_nglob_partial/expected_graph_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     4971 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/static_nglob_partial/expected_graph_04.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2254 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/static_nglob_partial/expected_stdout_a.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1229 2024-04-25 17:19:40.000000 stepup-1.0.0/tests/cases/static_nglob_partial/expected_stdout_b.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     2139 2024-04-22 14:25:54.000000 stepup-1.0.0/tests/cases/static_nglob_partial/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      297 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/static_nglob_partial/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.748806 stepup-1.0.0/tests/cases/static_nglob_subdir/
--rw-r--r--   0 toon      (1000) toon      (1000)       52 2024-03-31 14:52:44.000000 stepup-1.0.0/tests/cases/static_nglob_subdir/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       57 2024-03-31 14:48:55.000000 stepup-1.0.0/tests/cases/static_nglob_subdir/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3514 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/static_nglob_subdir/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      505 2024-04-25 17:19:42.000000 stepup-1.0.0/tests/cases/static_nglob_subdir/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      746 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/static_nglob_subdir/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      107 2024-03-31 14:49:42.000000 stepup-1.0.0/tests/cases/static_nglob_subdir/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.748806 stepup-1.0.0/tests/cases/static_nglob_subdir/sub/
--rw-r--r--   0 toon      (1000) toon      (1000)        4 2024-03-31 14:52:44.000000 stepup-1.0.0/tests/cases/static_nglob_subdir/sub/inp1.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        4 2024-03-31 14:52:44.000000 stepup-1.0.0/tests/cases/static_nglob_subdir/sub/inp2.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      151 2024-03-31 14:52:44.000000 stepup-1.0.0/tests/cases/static_nglob_subdir/sub/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.749806 stepup-1.0.0/tests/cases/subdir/
--rw-r--r--   0 toon      (1000) toon      (1000)       56 2024-03-16 15:07:28.000000 stepup-1.0.0/tests/cases/subdir/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      267 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/subdir/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)       10 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/subdir/example.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3872 2024-04-25 17:19:44.000000 stepup-1.0.0/tests/cases/subdir/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1259 2024-04-25 17:19:44.000000 stepup-1.0.0/tests/cases/subdir/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      640 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/subdir/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      170 2024-04-20 04:20:55.000000 stepup-1.0.0/tests/cases/subdir/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.749806 stepup-1.0.0/tests/cases/subdir/sub/
--rwxr-xr-x   0 toon      (1000) toon      (1000)      448 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/subdir/sub/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.750805 stepup-1.0.0/tests/cases/watch_blocked/
--rw-r--r--   0 toon      (1000) toon      (1000)       89 2024-04-14 09:58:27.000000 stepup-1.0.0/tests/cases/watch_blocked/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      175 2024-04-14 09:52:15.000000 stepup-1.0.0/tests/cases/watch_blocked/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3177 2024-04-25 17:19:45.000000 stepup-1.0.0/tests/cases/watch_blocked/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3149 2024-04-25 17:19:45.000000 stepup-1.0.0/tests/cases/watch_blocked/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1746 2024-04-25 17:19:45.000000 stepup-1.0.0/tests/cases/watch_blocked/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      210 2024-04-14 09:58:52.000000 stepup-1.0.0/tests/cases/watch_blocked/expensive.py
--rw-r--r--   0 toon      (1000) toon      (1000)       18 2024-04-14 09:52:36.000000 stepup-1.0.0/tests/cases/watch_blocked/initial.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      966 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_blocked/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      261 2024-04-14 09:58:36.000000 stepup-1.0.0/tests/cases/watch_blocked/plan_blocked.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      249 2024-04-14 09:58:36.000000 stepup-1.0.0/tests/cases/watch_blocked/plan_unblocked.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.752806 stepup-1.0.0/tests/cases/watch_boot/
--rw-r--r--   0 toon      (1000) toon      (1000)       89 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_boot/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      191 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/watch_boot/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1868 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/watch_boot/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1884 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/watch_boot/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      759 2024-04-25 17:19:47.000000 stepup-1.0.0/tests/cases/watch_boot/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      988 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_boot/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      178 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_boot/plan_01.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      182 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_boot/plan_02.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.754805 stepup-1.0.0/tests/cases/watch_chain/
--rw-r--r--   0 toon      (1000) toon      (1000)      114 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/watch_chain/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      967 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_chain/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)       81 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_chain/config_01.json
--rw-r--r--   0 toon      (1000) toon      (1000)       85 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_chain/config_02.json
--rw-r--r--   0 toon      (1000) toon      (1000)     3737 2024-04-25 17:19:48.000000 stepup-1.0.0/tests/cases/watch_chain/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3723 2024-04-25 17:19:48.000000 stepup-1.0.0/tests/cases/watch_chain/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1110 2024-04-25 17:19:48.000000 stepup-1.0.0/tests/cases/watch_chain/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1074 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_chain/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      229 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_chain/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      545 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_chain/use_config.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.756806 stepup-1.0.0/tests/cases/watch_input/
--rw-r--r--   0 toon      (1000) toon      (1000)       92 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_input/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      124 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/watch_input/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1546 2024-04-25 17:19:28.000000 stepup-1.0.0/tests/cases/watch_input/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1547 2024-04-25 17:19:28.000000 stepup-1.0.0/tests/cases/watch_input/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1546 2024-04-25 17:19:28.000000 stepup-1.0.0/tests/cases/watch_input/expected_graph_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1354 2024-04-25 17:19:28.000000 stepup-1.0.0/tests/cases/watch_input/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       55 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/watch_input/first.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      946 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_input/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      155 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_input/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)       42 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/watch_input/second.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.758806 stepup-1.0.0/tests/cases/watch_middle/
--rw-r--r--   0 toon      (1000) toon      (1000)      112 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_middle/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      294 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/watch_middle/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2202 2024-04-25 17:19:30.000000 stepup-1.0.0/tests/cases/watch_middle/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1787 2024-04-25 17:19:30.000000 stepup-1.0.0/tests/cases/watch_middle/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2253 2024-04-25 17:19:30.000000 stepup-1.0.0/tests/cases/watch_middle/expected_graph_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1547 2024-04-25 17:19:30.000000 stepup-1.0.0/tests/cases/watch_middle/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1164 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_middle/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)       10 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/watch_middle/original.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      235 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_middle/plan_01.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      247 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_middle/plan_02.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.759806 stepup-1.0.0/tests/cases/watch_mixed/
--rw-r--r--   0 toon      (1000) toon      (1000)       87 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_mixed/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      216 2024-04-10 05:36:26.000000 stepup-1.0.0/tests/cases/watch_mixed/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)       10 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/watch_mixed/backup.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2155 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/watch_mixed/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1923 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/watch_mixed/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1329 2024-04-25 17:19:32.000000 stepup-1.0.0/tests/cases/watch_mixed/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      827 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_mixed/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      219 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_mixed/plan_full.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      125 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_mixed/plan_trimmed.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.760805 stepup-1.0.0/tests/cases/watch_nochanges/
--rw-r--r--   0 toon      (1000) toon      (1000)       61 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_nochanges/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       94 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/watch_nochanges/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1546 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/watch_nochanges/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1546 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/watch_nochanges/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      396 2024-04-25 17:19:34.000000 stepup-1.0.0/tests/cases/watch_nochanges/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       42 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/watch_nochanges/input.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      884 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_nochanges/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      155 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_nochanges/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.761805 stepup-1.0.0/tests/cases/watch_outdated_amend1/
--rw-r--r--   0 toon      (1000) toon      (1000)       86 2024-04-12 20:27:48.000000 stepup-1.0.0/tests/cases/watch_outdated_amend1/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       90 2024-04-12 20:27:48.000000 stepup-1.0.0/tests/cases/watch_outdated_amend1/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2177 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/watch_outdated_amend1/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2177 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/watch_outdated_amend1/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1343 2024-04-25 17:19:36.000000 stepup-1.0.0/tests/cases/watch_outdated_amend1/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1073 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_outdated_amend1/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      164 2024-04-12 20:27:48.000000 stepup-1.0.0/tests/cases/watch_outdated_amend1/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      271 2024-04-12 20:27:48.000000 stepup-1.0.0/tests/cases/watch_outdated_amend1/step.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.762806 stepup-1.0.0/tests/cases/watch_outdated_amend2/
--rw-r--r--   0 toon      (1000) toon      (1000)      118 2024-04-12 20:27:48.000000 stepup-1.0.0/tests/cases/watch_outdated_amend2/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       90 2024-04-12 20:27:48.000000 stepup-1.0.0/tests/cases/watch_outdated_amend2/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3776 2024-04-25 17:19:39.000000 stepup-1.0.0/tests/cases/watch_outdated_amend2/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3776 2024-04-25 17:19:39.000000 stepup-1.0.0/tests/cases/watch_outdated_amend2/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2787 2024-04-25 17:19:39.000000 stepup-1.0.0/tests/cases/watch_outdated_amend2/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1262 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_outdated_amend2/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      331 2024-04-12 20:27:48.000000 stepup-1.0.0/tests/cases/watch_outdated_amend2/plan.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      167 2024-04-12 20:27:48.000000 stepup-1.0.0/tests/cases/watch_outdated_amend2/step.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.763805 stepup-1.0.0/tests/cases/watch_output/
--rw-r--r--   0 toon      (1000) toon      (1000)       61 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_output/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      185 2024-04-21 07:23:43.000000 stepup-1.0.0/tests/cases/watch_output/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1570 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/watch_output/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1570 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/watch_output/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      516 2024-04-25 17:19:41.000000 stepup-1.0.0/tests/cases/watch_output/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       55 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/watch_output/input.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      925 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_output/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      116 2024-03-24 07:02:12.000000 stepup-1.0.0/tests/cases/watch_output/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)       42 2024-03-15 14:33:02.000000 stepup-1.0.0/tests/cases/watch_output/second.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 17:28:17.764805 stepup-1.0.0/tests/cases/watch_wanted/
--rw-r--r--   0 toon      (1000) toon      (1000)      112 2024-03-19 16:46:37.000000 stepup-1.0.0/tests/cases/watch_wanted/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       77 2024-03-22 16:09:26.000000 stepup-1.0.0/tests/cases/watch_wanted/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2540 2024-04-25 17:19:43.000000 stepup-1.0.0/tests/cases/watch_wanted/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2114 2024-04-25 17:19:43.000000 stepup-1.0.0/tests/cases/watch_wanted/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      910 2024-04-25 17:19:43.000000 stepup-1.0.0/tests/cases/watch_wanted/expected_graph_03.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2322 2024-04-25 17:19:43.000000 stepup-1.0.0/tests/cases/watch_wanted/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1544 2024-04-21 12:39:12.000000 stepup-1.0.0/tests/cases/watch_wanted/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      328 2024-03-27 20:48:00.000000 stepup-1.0.0/tests/cases/watch_wanted/plan_01.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      105 2024-03-24 07:02:12.000000 stepup-1.0.0/tests/cases/watch_wanted/plan_02.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2445 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/conftest.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1833 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/core_common.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1154 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/echo_server_socket.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1106 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/echo_server_stdio.py
--rw-r--r--   0 toon      (1000) toon      (1000)     9480 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/test_assoc.py
--rw-r--r--   0 toon      (1000) toon      (1000)     6724 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/test_basics.py
--rw-r--r--   0 toon      (1000) toon      (1000)    14605 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/test_cascade.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2963 2024-04-25 17:15:32.000000 stepup-1.0.0/tests/test_cases.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2513 2024-04-25 17:18:13.000000 stepup-1.0.0/tests/test_hash.py
--rw-r--r--   0 toon      (1000) toon      (1000)    21262 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/test_nglob.py
--rw-r--r--   0 toon      (1000) toon      (1000)     7965 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/test_rpc.py
--rw-r--r--   0 toon      (1000) toon      (1000)     9091 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/test_scheduler.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3646 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/test_utils.py
--rw-r--r--   0 toon      (1000) toon      (1000)    64288 2024-04-25 17:08:00.000000 stepup-1.0.0/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.207486 stepup-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 09:17:18.000000 stepup-1.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.059485 stepup-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.075485 stepup-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-02 09:17:18.000000 stepup-1.1.0/.github/workflows/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 09:17:18.000000 stepup-1.1.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-02 09:17:18.000000 stepup-1.1.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 09:17:18.000000 stepup-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-02 09:17:18.000000 stepup-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 09:17:18.000000 stepup-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-02 09:17:23.207486 stepup-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-02 09:17:18.000000 stepup-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.079485 stepup-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.079485 stepup-1.1.0/docs/advanced_topics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.083485 stepup-1.1.0/docs/advanced_topics/amending_static_inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_static_inputs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_static_inputs/config.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      149 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_static_inputs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_static_inputs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_static_inputs/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_static_inputs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.083485 stepup-1.1.0/docs/advanced_topics/amending_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_steps/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_steps/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_steps/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/amending_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.083485 stepup-1.1.0/docs/advanced_topics/blocked_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/blocked_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/blocked_steps/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/blocked_steps/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/blocked_steps/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/blocked_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.083485 stepup-1.1.0/docs/advanced_topics/cyclic_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/cyclic_dependencies/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/cyclic_dependencies/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/cyclic_dependencies/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/cyclic_dependencies/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/cyclic_dependencies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.083485 stepup-1.1.0/docs/advanced_topics/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/environment_variables/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/environment_variables/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/environment_variables/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/environment_variables/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/environment_variables.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.083485 stepup-1.1.0/docs/advanced_topics/here_and_root/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/here_and_root/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/here_and_root/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.083485 stepup-1.1.0/docs/advanced_topics/here_and_root/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/here_and_root/source/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.087485 stepup-1.1.0/docs/advanced_topics/here_and_root/source/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/here_and_root/source/sub/example.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/here_and_root/source/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/here_and_root/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/here_and_root.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/manual_cleaning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.087485 stepup-1.1.0/docs/advanced_topics/optional_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/optional_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/optional_steps/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/optional_steps/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/optional_steps/matplotlibrc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/optional_steps/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/optional_steps/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62512 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/optional_steps/plot_logmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/optional_steps/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/optional_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.087485 stepup-1.1.0/docs/advanced_topics/pools/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/pools/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/pools/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/pools/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/pools/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/pools.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.087485 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/graph_creator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/graph_supplier.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_deferred_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.091485 stepup-1.1.0/docs/advanced_topics/static_named_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.091485 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch1/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch1/sec1_1_introduction.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch1/sec1_2_objectives.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch1/unused.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.091485 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch2/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch2/sec2_1_mathematical_requisites.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch2/sec2_2_theory.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.091485 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch3/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch3/sec3_1_applications.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch3/sec3_2_discussion.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.091485 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch4/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/ch4/sec4_1_summary.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      647 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/static_named_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.091485 stepup-1.1.0/docs/advanced_topics/variable_substitution/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/variable_substitution/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/variable_substitution/dst_foo.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/variable_substitution/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/variable_substitution/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/variable_substitution/src_foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/variable_substitution/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/variable_substitution/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/variable_substitution.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.091485 stepup-1.1.0/docs/advanced_topics/volatile_outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/volatile_outputs/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/volatile_outputs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/volatile_outputs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/volatile_outputs/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/advanced_topics/volatile_outputs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/clean_stdout.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.095485 stepup-1.1.0/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/automatic_cleaning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.095485 stepup-1.1.0/docs/getting_started/copy_mkdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/copy_mkdir/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/copy_mkdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/copy_mkdir/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/copy_mkdir/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/copy_mkdir.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.095485 stepup-1.1.0/docs/getting_started/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/dependencies/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/dependencies/graph_creator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/dependencies/graph_supplier.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      286 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/dependencies/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/dependencies/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/dependencies/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/dependencies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.099485 stepup-1.1.0/docs/getting_started/distributed_plans/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/distributed_plans/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/distributed_plans/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/distributed_plans/part1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/distributed_plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/distributed_plans/stdout.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.099485 stepup-1.1.0/docs/getting_started/distributed_plans/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/distributed_plans/sub/part2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/distributed_plans/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/distributed_plans.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.099485 stepup-1.1.0/docs/getting_started/first_step/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/first_step/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/first_step/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/first_step/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/first_step/stdout1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/first_step/stdout2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/first_step.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/interactive_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.099485 stepup-1.1.0/docs/getting_started/no_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/no_rules/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/no_rules/lower1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/no_rules/lower2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/no_rules/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/no_rules/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/no_rules/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/no_rules.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/processes.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.103485 stepup-1.1.0/docs/getting_started/script_multiple/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/ebbr.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/ebos.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/matplotlibrc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      962 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60027 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/plot_ebbr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69904 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/plot_ebos.png
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_multiple.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.103485 stepup-1.1.0/docs/getting_started/script_single/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_single/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_single/config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      508 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_single/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_single/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_single/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_single/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/script_single.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.103485 stepup-1.1.0/docs/getting_started/static_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_files/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_files/limerick.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_files/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      154 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_files/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_files/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_files.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.103485 stepup-1.1.0/docs/getting_started/static_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.103485 stepup-1.1.0/docs/getting_started/static_glob/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob/src/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob/src/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.107485 stepup-1.1.0/docs/getting_started/static_glob_conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob_conditional/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.107485 stepup-1.1.0/docs/getting_started/static_glob_conditional/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob_conditional/dataset/bigfile.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      232 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob_conditional/expensive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob_conditional/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob_conditional/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob_conditional/stdout1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob_conditional/stdout2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/getting_started/static_glob_conditional.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/license.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1846 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.107485 stepup-1.1.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/reference/interactive.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/reference/stepup.core.api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/reference/stepup.core.interact.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      913 2024-05-02 09:17:18.000000 stepup-1.1.0/docs/run_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-02 09:17:18.000000 stepup-1.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-02 09:17:18.000000 stepup-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:17:23.207486 stepup-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.063485 stepup-1.1.0/stepup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.111485 stepup-1.1.0/stepup/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 09:17:22.000000 stepup-1.1.0/stepup/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21298 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/assoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19643 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/deferred_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/interact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21319 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/nglob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16273 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27113 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/tui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19950 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32915 2024-05-02 09:17:18.000000 stepup-1.1.0/stepup/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.207486 stepup-1.1.0/stepup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-02 09:17:22.000000 stepup-1.1.0/stepup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33312 2024-05-02 09:17:23.000000 stepup-1.1.0/stepup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:17:22.000000 stepup-1.1.0/stepup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 09:17:22.000000 stepup-1.1.0/stepup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 09:17:22.000000 stepup-1.1.0/stepup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:17:22.000000 stepup-1.1.0/stepup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.115485 stepup-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.115485 stepup-1.1.0/tests/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.119485 stepup-1.1.0/tests/cases/amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/expected_stdout_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/expected_stdout_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/inp1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2066 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.119485 stepup-1.1.0/tests/cases/amend_delay/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_delay/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_delay/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_delay/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_delay/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_delay/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_delay/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1602 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_delay/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_delay/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      307 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_delay/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.119485 stepup-1.1.0/tests/cases/amend_env_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_env_vars/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_env_vars/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_env_vars/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_env_vars/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_env_vars/foo.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      692 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_env_vars/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_env_vars/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_env_vars/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.123485 stepup-1.1.0/tests/cases/amend_missing/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_missing/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_missing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_missing/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_missing/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      562 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_missing/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_missing/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      203 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_missing/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.123485 stepup-1.1.0/tests/cases/amend_outdir_pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_outdir_pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_outdir_pending/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_outdir_pending/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_outdir_pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_outdir_pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_outdir_pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_outdir_pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.123485 stepup-1.1.0/tests/cases/amend_voldir_pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_voldir_pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_voldir_pending/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_voldir_pending/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_voldir_pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_voldir_pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_voldir_pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/amend_voldir_pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.127485 stepup-1.1.0/tests/cases/deferred_glob1/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1213 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.127485 stepup-1.1.0/tests/cases/deferred_glob1/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/static/data1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/static/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.127485 stepup-1.1.0/tests/cases/deferred_glob1/static/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/static/sub/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob1/static/sub/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.127485 stepup-1.1.0/tests/cases/deferred_glob2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      984 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.127485 stepup-1.1.0/tests/cases/deferred_glob2/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/static/data1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/static/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.127485 stepup-1.1.0/tests/cases/deferred_glob2/static/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/static/sub/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_glob2/static/sub/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.131485 stepup-1.1.0/tests/cases/deferred_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      599 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.131485 stepup-1.1.0/tests/cases/deferred_subdir/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_subdir/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_subdir/sub/unused.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/deferred_subdir/sub/used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.135485 stepup-1.1.0/tests/cases/env_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/demovars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_graph_05.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_stdout_b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_stdout_c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_stdout_d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_variables_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_variables_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_variables_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_variables_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/expected_variables_05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3193 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/printvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/variables_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars/variables_02.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.135485 stepup-1.1.0/tests/cases/env_vars_amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_amend/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_amend/demovars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_amend/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1025 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_amend/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.139485 stepup-1.1.0/tests/cases/env_vars_path/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/FOO.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/FOO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1255 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_path/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.139485 stepup-1.1.0/tests/cases/env_vars_subs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_subs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_subs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_subs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_subs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_subs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_subs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.139485 stepup-1.1.0/tests/cases/env_vars_subs/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      133 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_subs/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.139485 stepup-1.1.0/tests/cases/env_vars_workdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_workdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_workdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_workdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_workdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      644 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_workdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_workdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.139485 stepup-1.1.0/tests/cases/env_vars_workdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/env_vars_workdir/sub/input.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.139485 stepup-1.1.0/tests/cases/error_cyclic_late/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_cyclic_late/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_cyclic_late/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_cyclic_late/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_cyclic_late/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      591 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_cyclic_late/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_cyclic_late/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.143485 stepup-1.1.0/tests/cases/error_deferred_nonexisting/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_deferred_nonexisting/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_deferred_nonexisting/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_deferred_nonexisting/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      573 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_deferred_nonexisting/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_deferred_nonexisting/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.143485 stepup-1.1.0/tests/cases/error_env_var/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_env_var/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_env_var/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_env_var/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_env_var/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_env_var/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_env_var/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.143485 stepup-1.1.0/tests/cases/error_main_fails/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_main_fails/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_main_fails/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_main_fails/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_main_fails/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_main_fails/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_main_fails/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1044 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_main_fails/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_main_fails/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       36 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_main_fails/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.147485 stepup-1.1.0/tests/cases/error_not_executable/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_not_executable/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_not_executable/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_not_executable/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_not_executable/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_not_executable/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.147485 stepup-1.1.0/tests/cases/error_overlap_deferred/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_overlap_deferred/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_overlap_deferred/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_overlap_deferred/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_overlap_deferred/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      564 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_overlap_deferred/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_overlap_deferred/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.147485 stepup-1.1.0/tests/cases/error_static_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_static_dir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_static_dir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_static_dir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_static_dir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_static_dir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_static_dir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.147485 stepup-1.1.0/tests/cases/error_static_dir/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_static_dir/subdir/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.147485 stepup-1.1.0/tests/cases/error_step/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_step/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_step/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_step/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_step/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_step/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/error_step/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.151485 stepup-1.1.0/tests/cases/here/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/here/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/here/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/here/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/here/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/here/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.151485 stepup-1.1.0/tests/cases/here/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/here/source/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.151485 stepup-1.1.0/tests/cases/here/source/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/here/source/www/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/here/source/www/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.151485 stepup-1.1.0/tests/cases/makedirs/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/makedirs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/makedirs/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      456 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/makedirs/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/makedirs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/makedirs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      610 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/makedirs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/makedirs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.151485 stepup-1.1.0/tests/cases/mkdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.151485 stepup-1.1.0/tests/cases/mkdir/exists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir/exists/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      599 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.151485 stepup-1.1.0/tests/cases/mkdir_error/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir_error/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir_error/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir_error/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir_error/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir_error/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       79 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/mkdir_error/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.155485 stepup-1.1.0/tests/cases/nodata/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1495 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nodata/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.155485 stepup-1.1.0/tests/cases/noplan/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/noplan/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/noplan/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/noplan/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/noplan/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.155485 stepup-1.1.0/tests/cases/nostatic/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nostatic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nostatic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nostatic/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nostatic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nostatic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/nostatic/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.155485 stepup-1.1.0/tests/cases/not_cyclic/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/not_cyclic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/not_cyclic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/not_cyclic/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/not_cyclic/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/not_cyclic/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/not_cyclic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1386 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/not_cyclic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/not_cyclic/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.159485 stepup-1.1.0/tests/cases/optional_convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/expected_graph_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/expected_graph_b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/expected_graph_c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1540 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/raw_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/raw_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/raw_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/optional_convert/raw_04.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.159485 stepup-1.1.0/tests/cases/output_not_created/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/output_not_created/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/output_not_created/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/output_not_created/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/output_not_created/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      627 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/output_not_created/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/output_not_created/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.159485 stepup-1.1.0/tests/cases/pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pending/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.163485 stepup-1.1.0/tests/cases/permissions_file_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_file_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_file_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_file_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_file_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_file_rerun/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_file_rerun/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1198 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_file_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_file_rerun/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.163485 stepup-1.1.0/tests/cases/permissions_plan_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_rerun/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      984 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_rerun/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.163485 stepup-1.1.0/tests/cases/permissions_plan_rerun/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_rerun/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.163485 stepup-1.1.0/tests/cases/permissions_plan_restart/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_restart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_restart/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_restart/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_restart/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_restart/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_restart/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1140 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_restart/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_restart/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.163485 stepup-1.1.0/tests/cases/permissions_plan_restart/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_plan_restart/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.167485 stepup-1.1.0/tests/cases/permissions_step_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_rerun/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      962 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_rerun/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_rerun/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.167485 stepup-1.1.0/tests/cases/permissions_step_restart/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_restart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_restart/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_restart/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_restart/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_restart/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_restart/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1058 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_restart/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_restart/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/permissions_step_restart/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.167485 stepup-1.1.0/tests/cases/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pool/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pool/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pool/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pool/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pool/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pool/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/pool/r.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.167485 stepup-1.1.0/tests/cases/reqdir_missing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/reqdir_missing/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/reqdir_missing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/reqdir_missing/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/reqdir_missing/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      605 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/reqdir_missing/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/reqdir_missing/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.171485 stepup-1.1.0/tests/cases/restart_blocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/expensive.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/initial.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1052 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/plan_blocked.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_blocked/plan_unblocked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.171485 stepup-1.1.0/tests/cases/restart_changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1394 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/plan_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/source_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/source_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_changes/source_both.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.171485 stepup-1.1.0/tests/cases/restart_deferred_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_deferred_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_deferred_glob/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_deferred_glob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_deferred_glob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_deferred_glob/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_deferred_glob/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_deferred_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_deferred_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.171485 stepup-1.1.0/tests/cases/restart_deferred_glob/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_deferred_glob/static/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.175485 stepup-1.1.0/tests/cases/restart_nochanges/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_nochanges/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_nochanges/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_nochanges/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_nochanges/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_nochanges/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_nochanges/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1066 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_nochanges/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_nochanges/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.175485 stepup-1.1.0/tests/cases/restart_orphan/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_orphan/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_orphan/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_orphan/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_orphan/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_orphan/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_orphan/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_orphan/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_orphan/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.175485 stepup-1.1.0/tests/cases/restart_outdated_amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_outdated_amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_outdated_amend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_outdated_amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_outdated_amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_outdated_amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_outdated_amend/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_outdated_amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_outdated_amend/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_outdated_amend/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.179485 stepup-1.1.0/tests/cases/restart_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_output/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_output/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_output/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_output/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_output/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      964 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_output/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_output/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/restart_output/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.179485 stepup-1.1.0/tests/cases/script_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.179485 stepup-1.1.0/tests/cases/script_cases_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases_settings/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases_settings/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases_settings/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases_settings/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases_settings/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases_settings/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases_settings/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases_settings/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_cases_settings/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.183485 stepup-1.1.0/tests/cases/script_single/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_single/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_single/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_single/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_single/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      639 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_single/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_single/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.183485 stepup-1.1.0/tests/cases/script_single/work/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_single/work/config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/script_single/work/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.183485 stepup-1.1.0/tests/cases/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      567 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.183485 stepup-1.1.0/tests/cases/static_abs/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_abs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_abs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_abs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_abs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      567 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_abs/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_abs/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_abs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.183485 stepup-1.1.0/tests/cases/static_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_dir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_dir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_dir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_dir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      595 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_dir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_dir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.187485 stepup-1.1.0/tests/cases/static_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_glob/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_glob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_glob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_glob/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_glob/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_glob/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1686 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.187485 stepup-1.1.0/tests/cases/static_nglob/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.187485 stepup-1.1.0/tests/cases/static_nglob/ch-1-intro/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/ch-1-intro/sec-1-1-blabla.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/ch-1-intro/sec-1-2-some-more.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.187485 stepup-1.1.0/tests/cases/static_nglob/ch-2-theory/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/ch-2-theory/sec-2-1-basics.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.187485 stepup-1.1.0/tests/cases/static_nglob/ch-3-conclusions/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/ch-3-conclusions/sec-3-1-summary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/ch-3-conclusions/sec-3-2-outlook.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2740 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob/sec-2-2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.191486 stepup-1.1.0/tests/cases/static_nglob_partial/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_partial/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.191486 stepup-1.1.0/tests/cases/static_nglob_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      742 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.191486 stepup-1.1.0/tests/cases/static_nglob_subdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_subdir/sub/inp1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_subdir/sub/inp2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/static_nglob_subdir/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.191486 stepup-1.1.0/tests/cases/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/subdir/example.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      636 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.191486 stepup-1.1.0/tests/cases/subdir/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/subdir/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.195485 stepup-1.1.0/tests/cases/watch_blocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/expensive.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/initial.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      961 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/plan_blocked.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_blocked/plan_unblocked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.195485 stepup-1.1.0/tests/cases/watch_boot/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_boot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_boot/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_boot/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_boot/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_boot/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      983 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_boot/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_boot/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_boot/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.195485 stepup-1.1.0/tests/cases/watch_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/config_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/config_02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      545 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_chain/use_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.199485 stepup-1.1.0/tests/cases/watch_input/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/first.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_input/second.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.199485 stepup-1.1.0/tests/cases/watch_middle/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      235 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_middle/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.199485 stepup-1.1.0/tests/cases/watch_mixed/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_mixed/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_mixed/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_mixed/backup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_mixed/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_mixed/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_mixed/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_mixed/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      219 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_mixed/plan_full.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_mixed/plan_trimmed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.203486 stepup-1.1.0/tests/cases/watch_nochanges/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_nochanges/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_nochanges/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_nochanges/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_nochanges/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_nochanges/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_nochanges/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      876 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_nochanges/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_nochanges/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.203486 stepup-1.1.0/tests/cases/watch_outdated_amend1/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend1/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend1/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend1/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend1/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend1/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend1/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.203486 stepup-1.1.0/tests/cases/watch_outdated_amend2/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend2/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend2/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend2/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1260 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend2/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend2/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_outdated_amend2/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.207486 stepup-1.1.0/tests/cases/watch_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_output/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_output/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_output/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_output/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_output/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      920 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_output/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_output/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_output/second.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:17:23.207486 stepup-1.1.0/tests/cases/watch_wanted/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_wanted/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_wanted/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_wanted/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_wanted/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_wanted/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_wanted/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1538 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_wanted/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      328 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_wanted/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/cases/watch_wanted/plan_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/core_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/echo_server_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/echo_server_stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_assoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21262 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_nglob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65158 2024-05-02 09:17:18.000000 stepup-1.1.0/tests/test_workflow.py
```

### Comparing `stepup-1.0.0/.pre-commit-config.yaml` & `stepup-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/LICENSE` & `stepup-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/PKG-INFO` & `stepup-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: stepup
-Version: 1.0.0
+Version: 1.1.0
 Summary: StepUp Core provides the basic framework for the StepUp build tool
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
+Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-core/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-core/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-core/
-Project-URL: Changelog, https://github.com/reproducible-reporting/stepup-core/blob/main/CHANGELOG.md
+Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-core/changelog/
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: msgpack
 Requires-Dist: parse
 Requires-Dist: path
 Requires-Dist: rich
-Requires-Dist: watchfiles
+Requires-Dist: watchdog
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-macros-plugin; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 
-[![PyPI Upload](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pypi.yaml)
+[![release](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml)
 [![pytest](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml)
-[![PyPI Version](https://img.shields.io/pypi/v/stepup-core)](https://pypi.org/project/stepup-core/)
+[![PyPI Version](https://img.shields.io/pypi/v/stepup)](https://pypi.org/project/stepup/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-core)
 
 # StepUp Core
 
 StepUp is a simple, powerful and universal build tool.
 StepUp Core provides the basic framework for StepUp, without any domain-specific features.
```

### Comparing `stepup-1.0.0/README.md` & `stepup-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![PyPI Upload](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pypi.yaml)
+[![release](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml)
 [![pytest](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml)
-[![PyPI Version](https://img.shields.io/pypi/v/stepup-core)](https://pypi.org/project/stepup-core/)
+[![PyPI Version](https://img.shields.io/pypi/v/stepup)](https://pypi.org/project/stepup/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-core)
 
 # StepUp Core
 
 StepUp is a simple, powerful and universal build tool.
 StepUp Core provides the basic framework for StepUp, without any domain-specific features.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/amending_steps/stdout.txt` & `stepup-1.1.0/docs/advanced_topics/amending_steps/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ echo input.txt > sources.txt
    SUCCESS │ echo input.txt > sources.txt
      START │ ./step.py
 RESCHEDULE │ ./step.py
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
```

### Comparing `stepup-1.0.0/docs/advanced_topics/amending_steps.md` & `stepup-1.1.0/docs/advanced_topics/amending_steps.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Amending steps
 
 Every step in StepUp can inform the director process of additional inputs or environment variables it uses, or of additional (volatile) outputs it creates.
-Defining an amended input may not always be successful, if that file is not yet built nor known as a static file.
+However, defining an amended input will fail when that file is not yet built nor known as a static file.
 In this case, the step can end early and will be rescheduled by the director process when the amended input becomes available.
 
 The [`amend()`][stepup.core.api.amend] function implements this feature and is convenient in various scenarios:
 
-- This is particularly useful when a step uses input files that refer to other inputs files.
+- This is particularly useful when a step uses input files that refer to other input files.
   It may happen that some of these other input files still need to be generated by other steps.
   Once built, the other inputs may again refer to more input files, etc.
   Such dependencies cannot be discovered in advance, simply because not all inputs are available before running the steps that generate them.
   (This is a common scenario when writing LaTeX documents of which parts are generated by scripts.)
 
 - Another use case is that some steps may take their default configuration from environment variables if some command-line options are missing.
   In this case, `amend` can be used to specify the environment variables used.
@@ -20,19 +20,21 @@
 
 To the best of our knowledge, there is no equivalent of `amend` in other build tools.
 Some features in Ninja cover what can be achieved with `amend`.
 
 
 ## Example
 
+Example source files: [advanced_topics/amending_steps/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/advanced_topics/amending_steps)
+
 This example intentionally creates a simple scenario with an amended input.
 This is a somewhat silly example to illustrate the concept.
 You may achieve the same result without amending, because you have full control over all scripts in the example.
 
-Create the following `plan.py`, of which the first step is a script that will discover it needs an additional input.
+Create the following `plan.py`, where the first step is a script that will discover it needs an additional input.
 
 ```python
 {% include 'advanced_topics/amending_steps/plan.py' %}
 ```
 
 In addition, create a file `input.txt` with some arbitrary contents and the following `step.py` script:
 
@@ -53,16 +55,19 @@
 {% include 'advanced_topics/amending_steps/stdout.txt' %}
 ```
 
 The output shows that `./step.py` first stopped early due to the missing file `input.txt`.
 Once this became clear, StepUp scheduled the optional step to generate the requested input.
 Later, StepUp ran `./step.py` again.
 
-## Try the following
 
-- Rerun StepUp without making changes. As expected, all steps are skipped.
-  The file `workflow.mpk.xz` also stores the amended information,
-  so it does not need to be rediscovered later.
-- Change the file `plan.py` to include a second amended input, e.g. `other.txt`.
-  Rerun StepUp with these changes.
-  Because `sources.txt` contains a new file, StepUp will try rerunning
-  `./step.py`, which will amend new inputs that require the step to be rescheduled.
+## Try the Following
+
+- Run StepUp again without making any changes.
+  As expected, all steps are skipped.
+  The `workflow.mpk.xz` file also stores the amended information,
+  so these don't need to be rediscovered later.
+
+- Modify the `plan.py` file to include a second amended input, for example, `other.txt`.
+  Run StepUp with these changes.
+  Because `sources.txt` contains a new file, StepUp will try re-running
+  `./step.py`, which will amend new inputs that require the step to be rescheduled again.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/blocked_steps/stdout.txt` & `stepup-1.1.0/docs/advanced_topics/blocked_steps/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ echo hello > a.txt
    SUCCESS │ echo hello > a.txt
    WARNING │ 2 steps remain pending due to blocked steps
 ──────────────────────────────── Blocked steps ─────────────────────────────────
 step:cp -aT a.txt b.txt
```

### Comparing `stepup-1.0.0/docs/advanced_topics/blocked_steps.md` & `stepup-1.1.0/docs/advanced_topics/blocked_steps.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-# Blocked steps
+# Blocked Steps
 
 As discussed in the [previous tutorial](optional_steps.md),
 StepUp has several mechanisms to ignore certain steps.
 As a rule, StepUp will always try to execute all steps, and not doing so is the exception.
 
 A valid reason for ignoring some steps is illustrated in the following schematic:
 
 ```
      File           In development            File                 Costly
 |-------------|      |----------|      |-----------------|      |----------|
 |  input.txt  |  =>  |  Step 1  |  =>  |  converted.txt  |  =>  |  Step 2  |
 |-------------|      |----------|      |-----------------|      |----------|
 ```
 
-Imagine that you are the `Step 2` is very expensive and you are developing a script for `Step 1`.
+Imagine that `Step 2` is very expensive and you are developing a script for `Step 1`.
 In practice, it takes several iterations to get `Step 1` working properly.
-This can, for example, be verified by analyzing the file `converted.txt` or with unit tests.
+This can be verified by analyzing the file `converted.txt` or with unit tests.
 
-To avoid that `Step 2` is executed at every iteration in the development of `Step 1`,
+To avoid executing `Step 2` at every iteration in the development of `Step 1`,
 you can **block** this step.
-All step-creating functions accept an optional `block=True` keyword argument to these prevent step(s) from being executed.
-Blocking steps is obviously a temporary measure, meant to be reverted once you're done with `Step 1`.
+All step-creating functions accept an optional `block=True` keyword argument to prevent them from being executed.
+Blocking steps is a temporary measure, meant to be reverted once you're done with `Step 1`.
 
 Blocking steps has some consequences:
 
 - Blocked steps remain in the PENDING state, meaning that outdated output files are not cleaned up automatically.
-- At the end of the *run phase* a list of blocked steps is shown, to remind the user that some steps are blocked.
+- At the end of the *run phase*, a list of blocked steps is shown, to remind the user that some steps are blocked.
 - Subsequent steps, which use outputs of blocked or pending steps, also remain pending.
 
 
 ## Example
 
+Example source files: [advanced_topics/blocked_steps/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/advanced_topics/blocked_steps)
+
 The following `plan.py` illustrates the blocking mechanism.
 The copy commands are too simple and cheap to justify blocking,
 so this is just an example to illustrate the mechanism only.
 
 ```python
 {% include 'advanced_topics/blocked_steps/plan.py' %}
 ```
@@ -49,16 +51,17 @@
 You should get the following terminal output:
 
 ```
 {% include 'advanced_topics/blocked_steps/stdout.txt' %}
 ```
 
 
-## Try the following
+## Try the Following
 
 - Unblock the copy step, run StepUp, block it again, and run StepUp again.
-  Even though the copy commands are no longer executed, their outputs (`b.txt` and `c.txt`)
+  Although the copy commands are no longer executed, their outputs (`b.txt` and `c.txt`)
   are not cleaned up.
-  This is the expected behavior because the automatic cleaning is only performed when all
-  (non-optional) steps have been executed succesfully.
+  This is the expected behavior because automatic cleaning is only performed when all
+  (non-optional) steps have been executed successfully.
+
 - Unblock the copy step, run StepUp, and then make the last copy command optional.
   In this case, the output of the optional step (`c.txt`) will be removed.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/environment_variables/stdout.txt` & `stepup-1.1.0/docs/advanced_topics/environment_variables/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ echo ${MYVAR}
    SUCCESS │ echo ${MYVAR}
 ─────────────────────────────── Standard output ────────────────────────────────
 foo
 ────────────────────────────────────────────────────────────────────────────────
```

### Comparing `stepup-1.0.0/docs/advanced_topics/environment_variables.md` & `stepup-1.1.0/docs/advanced_topics/environment_variables.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# Environment variables
+# Environment Variables
 
-When defining a step, one may specify environment variables it uses (not their values).
+When defining a step, one can specify the environment variables it uses (not their values).
 When starting StepUp with a different value for any of these variables, StepUp will know that it has to repeat the step instead of skipping it.
 
-One can only change an environment variable by stopping StepUp, changing the variable and starting StepUp again.
+One can only change an environment variable by stopping StepUp, changing the variable, and then starting StepUp again.
 One cannot modify environment variables while StepUp is running.
 
 
 ## Example
 
+Example source files: [advanced_topics/environment_variables/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/advanced_topics/environment_variables)
+
 Create the following `plan.py`:
 
 ```python
 {% include 'advanced_topics/environment_variables/plan.py' %}
 ```
 
 Make it executable and run StepUp with a specific value of the variable:
@@ -25,17 +27,19 @@
 You will see the following output:
 
 ```
 {% include 'advanced_topics/environment_variables/stdout.txt' %}
 ```
 
 The variable substitution is performed in the subshell of the worker.
-StepUp will not try substitute `${MYVAR}` before starting the step.
-The special variables `${inp}` and `${out}` are the exceptions to this rule as discussed in the [tutorial on dependencies](../getting_started/dependencies.md).
+StepUp will not try to substitute `${MYVAR}` before starting the step.
+The special variables `${inp}` and `${out}` are exceptions to this rule,
+as discussed in the [tutorial on dependencies](../getting_started/dependencies.md).
 
 
-## Try the following
+## Try the Following
 
 - Repeat `MYVAR=foo stepup -n -w1` without making changes.
   You will see that the `echo` step is skipped as expected.
+
 - Now run `MYVAR=bar stepup -n -w1`.
   This time, the variable change will cause the step to be executed.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/here_and_root/stdout.txt` & `stepup-1.1.0/docs/advanced_topics/here_and_root/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
-     START │ ./plan.py  # wd=sub/
-   SUCCESS │ ./plan.py  # wd=sub/
      START │ mkdir -p ../public/
    SUCCESS │ mkdir -p ../public/
+     START │ ./plan.py  # wd=sub/
+   SUCCESS │ ./plan.py  # wd=sub/
      START │ mkdir -p ../../public/sub/  # wd=sub/
    SUCCESS │ mkdir -p ../../public/sub/  # wd=sub/
      START │ cp -aT example.txt ../../public/sub/example.txt  # wd=sub/
    SUCCESS │ cp -aT example.txt ../../public/sub/example.txt  # wd=sub/
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/here_and_root.md` & `stepup-1.1.0/docs/advanced_topics/here_and_root.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # HERE and ROOT variables
 
-When a worker runs a step, it defines several environment variables, of which `HERE` and `ROOT` can be relevant for writing advanced scripts.
-(The workers also defines variables starting with `STEPUP_`, but these are only useful to StepUp itself, not to end users.)
+When a worker runs a step, it defines several environment variables, including `HERE` and `ROOT`, which can be relevant for writing advanced scripts.
+(The workers also define variables starting with `STEPUP_`, but these are only useful to StepUp itself, not to end users.)
 
 The two variables are defined as follows:
 
 - `HERE` contains the relative path from the directory where StepUp was started to the current working directory of the step.
 - `ROOT` contains the opposite: the relative directory from the current working directory to the directory where StepUp was started.
 
 Hence, `HERE/ROOT` and `ROOT/HERE` normalize to the current directory: `./`.
 
 These variables can be useful in the following cases:
 
 - For out-of-source builds, where you want to replicate the directory structure of the source material.
   (See example below.)
-- To refeference a local script that is stored in the top-level directory of your project: `${ROOT}/script.py`
+- To reference a local script that is stored in the top-level directory of your project: `${ROOT}/script.py`
 
 
 ## Example
 
+Example source files: [advanced_topics/here_and_root/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/advanced_topics/here_and_root)
+
 This example represents a minimal out-of-source build, which is nevertheless involving several files, due to the inherent complexity of out-of-source builds.
 
 Create a `source/` directory with the following `source/plan.py`:
 
 ```python
 {% include 'advanced_topics/here_and_root/source/plan.py' %}
 ```
@@ -59,18 +61,19 @@
 
 ```python
 from stepup.core.api import getenv
 dst = getenv("DST", is_path=True)
 ```
 
 The `is_path=True` option implies that the variable is a path defined globally.
-If it is a relative path, it will be interpreted relative to the sorking directory where StepUp was started and will be translated to the working directory of the script calling `getenv`.
+If it is a relative path, it will be interpreted relative to the working directory where StepUp was started and will be translated to the working directory of the script calling `getenv`.
 Any variables present in the environment variable will also be substituted once.
 
 
-## Try the following
+## Try the Following
+
+- Modify the scripts `plan.py` and `sub/plan.py` to utilize a `DST` variable as explained above.
+  To achieve this, define `DST` externally, for instance, by starting StepUp as `DST='../public/${HERE}' stepup -n -w1`.
 
-- Change the scripts `plan.py` and `sub/plan.py` such that they make use of a `DST` variable as explained above.
-  To make this work, you need to define `DST` externally, e.g. by starting StepUp as `DST='../public/${HERE}' stepup -n -w1`.
-- After the previous point, run StepUp with a different `DST` value.
+- As a follow-up to the previous point, run StepUp with a different `DST` value.
   For example: `DST='../out/${HERE}' stepup -n -w1`.
-  You will see that all the old output files get cleaned up after the new output is created
+  You will see that all old output files get cleaned up after the new output is created.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/optional_steps/stdout.txt` & `stepup-1.1.0/docs/advanced_topics/optional_steps/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./generate.py plan --optional
    SUCCESS │ ./generate.py plan --optional
      START │ ./plot.py plan
    SUCCESS │ ./plot.py plan
      START │ ./generate.py run -- 'logmap_3.200'
```

### Comparing `stepup-1.0.0/docs/advanced_topics/optional_steps.md` & `stepup-1.1.0/docs/advanced_topics/optional_steps.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,67 @@
-# Optional steps
+# Optional Steps
 
-By default StepUp will build all steps created.
+By default, StepUp will build all steps created.
 As an exception, steps can be made optional by adding the `optional=True` option.
 This is the opposite of most build tools, where steps are only executed when they are *targets*.
 
 The reason for this difference is that conventional build tools work with rigid predefined graphs.
 By accepting command-line arguments with target steps, they introduce some flexibility:
 this lets the user control which part of the graph is executed.
 
 StepUp offers such flexibility in a different way.
 The basic premise is that all outdated or missing outputs need to be (re)built.
 It is the responsibility of the build tool to figure out which steps need executing.
 This responsibility should not be shifted to users by expecting them to specify targets.
-That said, some legit exceptions exist, in which ignoring steps is a desirable feature.
+That said, some legitimate exceptions exist, in which ignoring steps is a desirable feature.
 These are supported by StepUp as follows:
 
-- One can define **steps conditionally**, e.g. as in the tutorial [Static glob conditional](../getting_started/static_glob_conditional.md).
+- One can define **steps conditionally**, e.g., as in the tutorial [Static Glob Conditional](../getting_started/static_glob_conditional.md).
   Such conditionals are controlled by external factors and
   are picked up by your `plan.py` without manual interventions.
+
 - One can make **steps optional**, as in this tutorial.
-  This is useful when multiple steps are defined in a loop, as in the [Static glob](../getting_started/static_glob.md) tutorial, of which not all steps are required for the end result.
+  This is useful when multiple steps are defined in a loop, as in the [Static Glob](../getting_started/static_glob.md) tutorial, of which not all steps are required for the end result.
   Use this feature wisely:
   It is obviously inefficient to define a few thousand steps of which only a handful are needed.
+
 - As shown in the [next tutorial](blocked_steps.md), one may also **block steps**,
   as a temporary measure to speed up the edit-build cycle.
 
 
 ## Example
 
+Example source files: [advanced_topics/optional_steps/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/advanced_topics/optional_steps)
+
 The example below uses the `script()` feature introduced in
-[Script (single case)](../getting_started/script_single.md) and
-[Script (multiple cases)](../getting_started/script_multiple.md)
+[Script (Single Case)](../getting_started/script_single.md) and
+[Script (Multiple Cases)](../getting_started/script_multiple.md)
 to create a somewhat entertaining example.
-However, practically all step generating functions support the `optional` argument,
+However, practically all step-generating functions support the `optional` argument,
 and can thus be made optional in the same way.
 
-Create a first script `generate.py` to generates sequences of the [logistic map](https://en.wikipedia.org/wiki/Logistic_map) for different values of the parameter *r*:
+Create a first script `generate.py` that generates sequences of the [logistic map](https://en.wikipedia.org/wiki/Logistic_map) for different values of the parameter *r*:
 
 ```python
 {% include 'advanced_topics/optional_steps/generate.py' %}
 ```
 
-Then write a `plot.py` script that plots only one of these sequences:
+Then, write a `plot.py` script that plots only one of these sequences:
 
 ```python
 {% include 'advanced_topics/optional_steps/plot.py' %}
 ```
 
 The `plan.py` file adds steps for both scripts, but makes the data generation optional:
 
 ```python
 {% include 'advanced_topics/optional_steps/plan.py' %}
 ```
 
-Finally make the scripts executable and run StepUp:
+Finally, make the scripts executable and run StepUp:
 
 ```bash
 chmod +x generate.py plot.py plan.py
 stepup -n -w1
 ```
 
 You should get the following output:
@@ -68,14 +72,15 @@
 
 Note that, in this case, it would be trivial to modify the `generate.py` script to only generate the sequence of interest.
 Whenever such a simpler approach is possible, it is always preferable.
 However, in more complex use cases, it is not always possible to figure out which steps are going to be needed or not.
 In such situations, optional steps can be convenient.
 
 
-## Try the following
+## Try the Following
 
 - Remove the `optional=True` keyword argument and rerun the plan.
-  As expected, additional text files with sequences are created.
+  As expected, additional text files with sequences will be created.
+
 - Restore the `optional=True` keyword argument and rerun the plan.
-  As expected, the [Automatic cleaning](../getting_started/automatic_cleaning.md) feature
+  As expected, the [Automatic Cleaning](../getting_started/automatic_cleaning.md) feature
   removes the outputs that were generated by steps that are no longer present in the workflow.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/pools/stdout.txt` & `stepup-1.1.0/docs/advanced_topics/pools/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
   DIRECTOR │ Launched worker 1
   DIRECTOR │ Launched worker 2
   DIRECTOR │ Launched worker 3
+     PHASE │ run
      START │ ./plan.py
-     START │ sleep 0.1; echo A
      START │ sleep 0.1; echo B
+     START │ sleep 0.1; echo A
    SUCCESS │ ./plan.py
-   SUCCESS │ sleep 0.1; echo A
-─────────────────────────────── Standard output ────────────────────────────────
-A
-────────────────────────────────────────────────────────────────────────────────
    SUCCESS │ sleep 0.1; echo B
 ─────────────────────────────── Standard output ────────────────────────────────
 B
 ────────────────────────────────────────────────────────────────────────────────
      START │ sleep 0.1; echo C
+   SUCCESS │ sleep 0.1; echo A
+─────────────────────────────── Standard output ────────────────────────────────
+A
+────────────────────────────────────────────────────────────────────────────────
    SUCCESS │ sleep 0.1; echo C
 ─────────────────────────────── Standard output ────────────────────────────────
 C
 ────────────────────────────────────────────────────────────────────────────────
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/pools.md` & `stepup-1.1.0/docs/advanced_topics/pools.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,39 +4,43 @@
 so StepUp will launch any queued step as soon as a worker becomes available.
 A "pool" is a simple mechanism to limit parallelization in the few cases that this would be counterproductive:
 
 1. Some programs behave poorly (have bugs) when multiple instances are running in parallel.
    Here are a few examples encountered in the development of StepUp RepRep:
     - [Inkscape/issue4716](https://gitlab.com/inkscape/inkscape/-/issues/4716)
     - [markdown-katex/issue16](https://github.com/mbarkhau/markdown-katex/issues/16)
-2. Some steps may consume a lot of resources, e.g. memory,
+
+2. Some steps may consume a lot of resources, such as memory,
    and would require more resources than available when running in parallel.
+
 3. Software licenses may not allow for more than a given number of instances running in parallel.
 
 One defines a pool with [`pool(name, size)`][stepup.core.api.pool].
 The size is the maximum number of steps running concurrently within the pool.
 Steps are assigned to a pool by defining them with the `pool=name` keyword argument.
 
 For StepUp, mainly the first use case (working around concurrency bugs) is relevant,
 for which the pool size is 1.
 
 
 ## Example
 
-The example here is a simple test case illustrating the use of a pool.
-The steps can also run easily in parallel, so you can experiment with the pool size.
+Example source files: [advanced_topics/pools/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/advanced_topics/pools)
+
+The example here illustrates the use of a pool in a simple test case.
+The steps can run easily in parallel, so you can experiment with the pool size.
 
 Create the following `plan.py`:
 
 ```python
 {% include 'advanced_topics/pools/plan.py' %}
 ```
 
-The `sleep` command assures the step last sufficient long,
-which guarantees they will run in parallel when allowed.
+The `sleep` command ensures that each step lasts long enough to guarantee they will run in parallel when allowed.
+
 
 Make the plan executable and run it with StepUp:
 
 ```bash
 chmod +x plan.py
 stepup -n -w4
 ```
@@ -44,23 +48,24 @@
 You should get the following output:
 
 ```
 {% include 'advanced_topics/pools/stdout.txt' %}
 ```
 
 Initially, the `./plan.py` step and two `sleep+echo` commands are running in parallel.
-Despite the fact that there are four workers,
-the third `sleep+echo` is only started after the previous two.
+Despite having four workers,
+the third `sleep+echo` is only started after the previous two have finished.
 
 
-## Try the following
+## Try the Following
 
 - Run `stepup -n -w4` again without making changes.
-  Skipping of steps is never subject to pool size restrictions.
-  (It does require some computation and comparison of hashes,
-  which is done by the worker processes.)
+  Skipping of steps requires some computation and comparison of hashes,
+  which is done by worker processes.
+  However, these hash computations are never subject to pool size restrictions.
+
 - Change the pool size to `1` or `3` and verify that the output matches your expectations.
-  When you try this, StepUp will keep skipping steps.
+  When you try this, StepUp will continue skipping steps.
   To forcibly re-execute steps, you have two options:
 
     1. Remove the file `.stepup/workflow.mpk.xz` and start StepUp.
-    2. Run StepUp interactively (wihout `-n`) and use the `f` key to start the workflow from scratch.
+    2. Run StepUp interactively (without `-n`) and use the `f` key to start the workflow from scratch.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/static_deferred_glob/graph.txt` & `stepup-1.1.0/docs/advanced_topics/static_deferred_glob/graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/docs/advanced_topics/static_deferred_glob/stdout.txt` & `stepup-1.1.0/docs/advanced_topics/static_deferred_glob/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cat foo.txt
    SUCCESS │ cat foo.txt
 ─────────────────────────────── Standard output ────────────────────────────────
 This is foo.
 ────────────────────────────────────────────────────────────────────────────────
```

### Comparing `stepup-1.0.0/docs/advanced_topics/static_deferred_glob.md` & `stepup-1.1.0/docs/advanced_topics/static_deferred_glob.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,68 @@
-# Static deferred glob
+# Static Deferred Glob
 
-When working with large datasets (many thousands of files),
-it is not desirable to make all these files static when only a few of them are used.
-This can be solved with StepUp's *deferred glob*,
-which will only declare static files matching a glob pattern when they are used as inputs.
+When dealing with massive datasets comprising tens of thousands of files, it doesn't make sense to render all of them as static when only a handful will actually be utilized.
+StepUp addresses this issue with the *deferred glob* feature,
+which makes previously unknown files static when:
+
+1. they are used as inputs of a new step and
+2. they match a deferred glob pattern.
 
 
 ## Example
 
+Example source files: [advanced_topics/static_deferred_glob/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/advanced_topics/static_deferred_glob)
+
 Create two text files with some content: `foo.txt` and `bar.txt`,
-and alsos the following `plan.py`:
+and also the following `plan.py`:
 
 ```python
 {% include 'advanced_topics/static_deferred_glob/plan.py' %}
 ```
 
 Run the plan interactively with StepUp:
 
 ```bash
 chmod +x plan.py
 stepup -n -w1
 ```
 
-You should have the following screen output:
+You should get the following screen output:
 
 ```
 {% include 'advanced_topics/static_deferred_glob/stdout.txt' %}
 ```
 
-As expected, `foo.txt` is used as a static file,
-but this would also have been the case without the `_defer=True` option.
-The key difference is that, internally, StepUp does not build a list of all matching `*.txt` files.
-This can be seen when inspecting the file `graph.txt`, which has no trace of `bar.txt`:
+As expected, `foo.txt` is used as a static file.
+Of course, this would also have been the case without the `_defer=True` option.
+The key difference is that with `_defer=True`, StepUp does not create a list of all matching `*.txt` files.
+This can be seen when examining the file `graph.txt`, which has no trace of `bar.txt`:
 
 ```
 {% include 'advanced_topics/static_deferred_glob/graph.txt' %}
 ```
 
-The node `dg:'*.txt;` in the graph is the result of adding the `_defer=True` option.
+The node `dg:'*.txt;` in the graph (green octagon in the figures below) is the result of adding the `_defer=True` option.
 This node will create static files as they are needed by other steps.
-This option is ideal when there are a large number of files that could match the pattern,
+The deferred glob is ideal when there are a large number of files that could match the pattern,
 of which most are irrelevant for the build.
-In this example, there could be thousands of `.txt` files and
+For example, there could be thousands of `.txt` files in this scenario, but
 this would not have any effect on the resources consumed by StepUp.
 
+The **supplier graph**:
+
+![graph_supplier.svg](static_deferred_glob/graph_supplier.svg)
+
+The **creator graph**:
 
-## Try the following
+![graph_creator.svg](static_deferred_glob/graph_creator.svg)
+
+
+## Try the Following
 
 - When using deferred globs, steps cannot create outputs that match the deferred glob.
-  It would mean that a built file must be made static, which is obviously inconsistent.
-  Cause this error by adding a step `copy("foo.txt", "foo2.txt")`.
-- Remove the `_defer=True` option and inspect the corresponding `graph.txt`
-  to observe that now `bar.txt` is indeed included in the graph.
+  This would mean that a built file could be made static when used as input later,
+  which is clearly inconsistent.
+  Try causing this error by adding a step `copy("foo.txt", "foo2.txt")`.
+
+- Remove the `_defer=True` option and inspect the corresponding `graph.txt`.
+  You should see that `bar.txt` is now indeed included in the graph.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/static_named_glob/plan.py` & `stepup-1.1.0/docs/advanced_topics/static_named_glob/plan.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/docs/advanced_topics/static_named_glob/stdout.txt` & `stepup-1.1.0/docs/advanced_topics/static_named_glob/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp -aT ch1/sec1_1_introduction.txt ch1/sec1_1_introduction.md
    SUCCESS │ cp -aT ch1/sec1_1_introduction.txt ch1/sec1_1_introduction.md
      START │ cp -aT ch1/sec1_2_objectives.txt ch1/sec1_2_objectives.md
    SUCCESS │ cp -aT ch1/sec1_2_objectives.txt ch1/sec1_2_objectives.md
      START │ cp -aT ch2/sec2_1_mathematical_requisites.txt ch2/sec2_1_mathematical_requisites.md
```

### Comparing `stepup-1.0.0/docs/advanced_topics/variable_substitution.md` & `stepup-1.1.0/docs/advanced_topics/variable_substitution.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# Variable substitution
+# Variable Substitution
 
-StepUp does not susbtitute environment variables is the command (first argument) of the [`step()`][stepup.core.api.step] function.
-As discussed in the tutorial on [envorinment variables](environment_variables.md), the executing shell takes care of such substitutions.
+StepUp does not substitute environment variables is the command (first argument) of the [`step()`][stepup.core.api.step] function.
+As discussed in the tutorial on [environment variables](environment_variables.md), the executing shell takes care of such substitutions.
 
 However, environment variables in all path-like arguments (e.g. `workdir`, `inp`, `out` and `vol`) of functions that take such arguments ([`step()`][stepup.core.api.step], [`amend()`][stepup.core.api.amend] etc.) are automatically substituted.
 This substitution takes place before the commands are sent to the director process and all used variables are communicated to the director with an `amend()` call.
 
 If a script needs an environment variable elsewhere, the function [`getenv()`][stepup.core.api.getenv] is recommended:
 It returns the value of the variable and calls `amend()` to tell the director that the current step depends on this variable.
 
 
 ## Example
 
+Example source files: [advanced_topics/variable_substitution/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/advanced_topics/variable_substitution)
+
 Create a `plan.py` with the following contents:
 
 ```python
 {% include 'advanced_topics/variable_substitution/plan.py' %}
 ```
 
 In addition, create a script `step.py` as follows:
@@ -43,14 +45,14 @@
 {% include 'advanced_topics/variable_substitution/dst_foo.txt' %}
 ```
 
 As shown in this example, the function [`getenv()`][stepup.core.api.getenv] returns `None` when a variable does not exist (or any other default you specify).
 When using variables like `${MYVAR}` in path-like arguments, the variable must exist or an exception is raised.
 
 
-## Try the following
+## Try the Following
 
-- Run StepUp without defining `MYVAR`, i.e. just `stepup -n -w1`.
+- Run StepUp without defining `MYVAR`: `stepup -n -w1`.
   As explained above, this raises an exception.
-- Run StepUp by also defining `MYNAME`, i.e. `MYVAR=foo MYNUM=1 stepup -n -w1`.
+- Run StepUp by also defining `MYNUM`: `MYVAR=foo MYNUM=1 stepup -n -w1`.
   Now the string `'1'` is shown in the output `dst_foo.txt`.
-  Note that environment variables are always strings, and need to converted to other types is needed.
+  Note that environment variables are always strings, and need to be converted to other types if needed.
```

### Comparing `stepup-1.0.0/docs/advanced_topics/volatile_outputs.md` & `stepup-1.1.0/docs/advanced_topics/volatile_outputs.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-# Volatile outputs
+# Volatile Outputs
 
-It may happen that steps produce auxiliary outputs that are not really of interest, but just happen to be created as a side effect.
+It may happen that steps produce auxiliary outputs that are not really of interest,
+but rather occur as a side effect.
 For example, LaTeX is notoriously productive in terms of output files.
-Some of these files will change with every run, e.g. because they contain timestamps.
+Some of these files will change with every run, e.g., because they contain timestamps.
 
-It is useful to inform StepUp of the existence of such volatile files, so they are cleaned up when appropriate.
-However, there is no point in computing file hashes for them, because these files are not used as inputs later and may change for no good reason.
+It is useful to inform StepUp of the existence of such volatile files, so they can be cleaned up when appropriate.
+However, there is no point in computing file hashes for them,
+as these files are not used as inputs later and may change for no good reason.
 One may pass a list of such files to the `vol` argument of the [`step()`][stepup.core.api.step] function.
 
 
 ## Example
 
+Example source files: [advanced_topics/volatile_outputs/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/advanced_topics/volatile_outputs)
+
 Create the following `plan.py`, with a single step that produces a trivially volatile output:
 
 ```python
 {% include 'advanced_topics/volatile_outputs/plan.py' %}
 ```
 
 Make the plan executable and run it as follows:
@@ -28,19 +32,21 @@
 You should get the following terminal output:
 
 ```
 {% include 'advanced_topics/volatile_outputs/stdout.txt' %}
 ```
 
 
-## Try the following
+## Try the Following
 
 - Remove the file `date.txt` and run StepUp again.
   You will see that the step gets ignored:
-  StepUp does not care much about the state of the volatile files.
+  StepUp does not care much about the state of volatile files.
   It only keeps track of them, so they can be removed when needed.
+
 - Manually recreate the file `date.txt` with some arbitrary contents,
   and run StepUp.
-  Again, the step gets skipped because also the contents of the
-  volatile `date.txt` is not considered when deciding if a step is outdated.
-- Comment out the the step in `plan.py` and run StepUp again.
+  Again, the step gets skipped because the contents of the
+  volatile `date.txt` are not considered when deciding if a step is outdated.
+
+- Comment out the step in `plan.py` and run StepUp again.
   Because the step is removed, the volatile output is also removed.
```

### Comparing `stepup-1.0.0/docs/getting_started/automatic_cleaning.md` & `stepup-1.1.0/docs/getting_started/automatic_cleaning.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-# Automatic cleaning
+# Automatic Cleaning
 
 StepUp follows the same cleanup strategy as [tup](https://gittup.org/tup/index.html):
 If a step is removed or modified so that an output file is no longer created,
 StepUp will remove this output.
-This is also similar to [Ninja](https://ninja-build.org/)'s `cleandead` command, but is not optional in StepUp.
-Thou shalt be clean!
+This is also similar to [Ninja](https://ninja-build.org/)'s `cleandead` command, but it is not optional in StepUp.
 
+The main advantage of automatic cleaning is that it eliminates potential bugs and confusion related to old output files that are no longer relevant.
 
-## Try the following
+
+## Try the Following
 
 To illustrate the automatic cleanup, take the files from the example [Copy and mkdir](copy_mkdir.md)
 and start StepUp in interactive mode.
-Make te following changes and rerun the affected steps after each point by pressing `r` in the terminal.
+Make the following changes and rerun the affected steps after each point by pressing `r` in the terminal:
 
 - Change the directory `sub/` to `foo/` in `plan.py`.
   Rerunning StepUp will not only create `foo/` and `foo/hello.txt`.
   After completing all pending steps, `sub/` and `sub/hello.txt` are removed.
-- Change all occurrences of `hello.txt` in `plan.py` by `hi.txt`.
+
+- Change all occurrences of `hello.txt` in `plan.py` to `hi.txt`.
   Rerunning StepUp will not only create `hi.txt` and `foo/hi.txt`.
   After completing all pending steps, `hello.txt` and `foo/hello.txt` are removed.
+
 - Undo all changes and rerun StepUp again.
   You should end up with the original outputs without any leftovers from the previous two steps.
```

### Comparing `stepup-1.0.0/docs/getting_started/copy_mkdir/stdout.txt` & `stepup-1.1.0/docs/getting_started/copy_mkdir/stdout.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-  DIRECTOR │ Listening on /tmp/stepup-qx0niv5o/director
-     PHASE │ run
+  DIRECTOR │ Listening on /tmp/stepup-########/director
   DIRECTOR │ Launched worker 0
   DIRECTOR │ Launched worker 1
+     PHASE │ run
      START │ ./plan.py
      START │ echo hello > hello.txt
    SUCCESS │ echo hello > hello.txt
      START │ mkdir -p sub/
+   SUCCESS │ ./plan.py
    SUCCESS │ mkdir -p sub/
      START │ cp -aT hello.txt sub/hello.txt
-   SUCCESS │ ./plan.py
    SUCCESS │ cp -aT hello.txt sub/hello.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/docs/getting_started/dependencies/stdout.txt` & `stepup-1.1.0/docs/getting_started/dependencies/stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
   DIRECTOR │ Launched worker 1
+     PHASE │ run
      START │ ./plan.py
      START │ echo First line. > story.txt; echo Second line. >> story.txt
-   SUCCESS │ ./plan.py
    SUCCESS │ echo First line. > story.txt; echo Second line. >> story.txt
      START │ grep First story.txt
    SUCCESS │ grep First story.txt
 ─────────────────────────────── Standard output ────────────────────────────────
 First line.
 ────────────────────────────────────────────────────────────────────────────────
+   SUCCESS │ ./plan.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/docs/getting_started/dependencies.md` & `stepup-1.1.0/docs/getting_started/static_files.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,53 @@
-# Dependencies
+# Static Files
 
-This tutorial shows how StepUp keeps track of dependencies.
+When steps use input files written by you, this must be explicitly stated in `plan.py`
+by declaring the human-written files as *static files*.
+This informs StepUp that it does not need to wait for other steps whose outputs are the required files.
 
 
 ## Example
 
-The following `plan.py` defines two steps, the second making use of the output from the first.
+Example source files: [getting_started/static_files/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/getting_started/static_files)
+
+Create a file `limerick.txt` with the following contents:
+
+```
+{% include 'getting_started/static_files/limerick.txt' %}
+```
+
+Also create the following `plan.py`:
 
 ```python
-{% include 'getting_started/dependencies/plan.py' %}
+{% include 'getting_started/static_files/plan.py' %}
 ```
 
-The placeholders `${inp}` and `${out}` are replaced by the `inp` and `out` keyword arguments.
-(This happens early, before the steps are sent to the director process.)
+The [`static()`][stepup.core.api.static] function declares a static file,
+i.e. one that you have created.
 
-Now run StepUp with two workers:
+Make the plan executable and run it with StepUp as follows:
 
 ```bash
-stepup -n -w2
+chmod +x plan.py
+stepup -n -w1
 ```
-
-You will see the following output:
+You should get the following output:
 
 ```
-{% include 'getting_started/dependencies/stdout.txt' %}
+{% include 'getting_started/static_files/stdout.txt' %}
 ```
 
-Despite the fact that StepUp launched two workers, it carries out the steps sequentially,
-because it knows that the output of the first step is used by the second.
+As expected, StepUp does not wait for another step to create `limerick.txt` because the file is static.
+The file `numbered.txt` will contain a copy of the limerick with line numbers.
+
+
+## Try the Following
 
-Note, however, that the `echo` commands are already started before `./plan.py` has completed.
-This is the expected behavior: even without a complete overview of all build steps,
-StepUp will start steps for which it has sufficient information.
+- Replace `gloom` by `boom` in `limerick.txt` and run `stepup -n -w1` again.
+  The line numbering is repeated, but the step `./plan.py` is skipped as it did not change.
 
-## Try the following
+- Change the order of `static` and `step` in `plan.py` and run `stepup -n -w1` again.
+  This has no apparent effect, but the step is only sent to the worker process after the director
+  is informed that the file `limerick.txt` is static.
 
-- Just run `stepup -n -w2` again. As expected, the steps are now skipped.
-- Modify the `grep` command to select the second line and run `stepup -n -w2` again.
-  The `echo` commands are skipped, since they have not changed.
-- Change the order of the two steps in `plan.py` and run `stepup -n -w2`.
-  The step `./plan.py` is executed because the file changed,
-  but the `echo` and `grep` steps are skipped.
-  This illustrates that `plan.py` is nothing but a plan being communicated to the director process.
-  It does not execute the steps.
+- Comment out the `static` function call and run `stepup -n -w1` again.
+  StepUp will refuse to execute the line numbering step and will show a warning explaining why.
```

### Comparing `stepup-1.0.0/docs/getting_started/distributed_plans/stdout.txt` & `stepup-1.1.0/docs/getting_started/distributed_plans/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./plan.py  # wd=sub/
    SUCCESS │ ./plan.py  # wd=sub/
      START │ cat part2.txt  # wd=sub/
    SUCCESS │ cat part2.txt  # wd=sub/
 ─────────────────────────────── Standard output ────────────────────────────────
```

### Comparing `stepup-1.0.0/docs/getting_started/distributed_plans.md` & `stepup-1.1.0/docs/getting_started/distributed_plans.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-# Distributed plans
+# Distributed Plans
 
-When your project grows, defining the whole workflow in a single `plan.py` may become inconvenient.
-Especially working with nested directories for different parts of the project,
-it may be convenient to distribute the workflow over multiple files.
+When your project grows, defining the entire workflow in a single `plan.py` file may become inconvenient.
+Especially when working with nested directories for different parts of the project,
+it may be convenient to distribute the workflow over multiple `plan.py` files.
 
 
 ## Example
 
+Example source files: [getting_started/distributed_plans/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/getting_started/distributed_plans)
+
 Create a simple example with a top-level `plan.py` as follows:
 
 ```python
 {% include 'getting_started/distributed_plans/plan.py' %}
 ```
 
 The top-level plan defines a few static files and then calls another plan in `sub/`.
-Create a files `sub/plan.py` as follows:
+Create a file `sub/plan.py` as follows:
 
 ```python
 {% include 'getting_started/distributed_plans/sub/plan.py' %}
 ```
 
 Also create two files `part1.txt` and `sub/part2.txt` with a bit of text.
 Make both plans executable and run StepUp as follows:
@@ -30,15 +32,18 @@
 You will get the following output:
 
 ```
 {% include 'getting_started/distributed_plans/stdout.txt' %}
 ```
 
 
-## Practical considerations
+## Practical Considerations
 
-- The main benefit of multiple plan.py files is to improve the logical structure of your project.
+- The main benefit of having multiple `plan.py` files
+  is to improve the logical structure of your project.
   It may also be helpful when a part of your `plan.py` is computationally demanding, in which
-  case it can be factored out such that it does not slow down the rest of the build.
+  case it can be factored out so that it does not slow down the rest of the build.
   However, ideally, the `plan.py` scripts execute quickly, leaving the hard work to other steps.
-- When there are multiple `plan.py`, keep in mind that their order of execution cannot be relied upon.
-  In general, they are executed in parallel.
+- When there are multiple `plan.py` files,
+  keep in mind that their order of execution cannot be relied upon.
+  They are executed in parallel, and their relative starting times depend
+  on factors unknown a priori, such as system load and number of workers.
```

### Comparing `stepup-1.0.0/docs/getting_started/first_step/stdout1.txt` & `stepup-1.1.0/docs/getting_started/first_step/stdout1.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ echo Hello World
    SUCCESS │ echo Hello World
 ─────────────────────────────── Standard output ────────────────────────────────
 Hello World
 ────────────────────────────────────────────────────────────────────────────────
```

### Comparing `stepup-1.0.0/docs/getting_started/first_step.md` & `stepup-1.1.0/docs/getting_started/first_step.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# First step
+# First Step
 
 The goal of the first tutorial is to introduce the basic usage of StepUp.
-For the sake of simplicity, a minimal workflow will be defined that won't achieve much.
+For the sake of simplicity, a minimal workflow will be defined that does not achieve much.
 
 
 ## Example
 
+Example source files: [getting_started/first_step/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/getting_started/first_step)
+
 Create a file `plan.py` with the following contents:
 
 ```python
 {% include 'getting_started/first_step/plan.py' %}
 ```
 
 Make this file executable with `chmod +x plan.py`.
@@ -43,15 +45,15 @@
 - The `START` and `SUCCESS` lines are shown for steps executed by StepUp:
     - The step `./plan.py` is created by default and runs the script that you just created.
     - Then the step `echo Hello World` is the step defined in `plan.py`.
 - When a step produces output, it is shown after the step has completed.
 - When no more steps can be executed, StepUp wraps up by saving the worklow for future runs.
 - Because of the `-n` option, StepUp immediately shuts down.
 
-Now repeat the execution of StepUp with
+Now repeat the execution of StepUp with:
 
 ```bash
 stepup -n -w1
 ```
 
 You will see a slightly different output:
 
@@ -62,11 +64,12 @@
 The steps are skipped (no longer executed) because their inputs have not changed.
 This is achieved by loading the file `.stepup/workflow.mpk.xz`, which contains the state of the
 most recent execution of all steps.
 StepUp determines if a step can be skipped by comparing a [Blake2 hash](https://en.wikipedia.org/wiki/BLAKE_(hash_function)#BLAKE2) including inputs, used environment variables and produced outputs.
 When you manually remove `.stepup/workflow.mpk.xz`,
 StepUp will not know anymore that it already executed some steps and runs all of them again.
 
-## Try the following
 
-Now change the arguments of the `echo` command in `plan.py` and run `stepup -n -w1` again.
-You will see that it detected the change and reruns both `plan.py` and the `echo` command.
+## Try the Following
+
+Now, change the arguments of the `echo` command in `plan.py` and run `stepup -n -w1` again.
+As expected, StepUp will detect the change and repeat the `plan.py` and `echo` steps.
```

### Comparing `stepup-1.0.0/docs/getting_started/interactive_usage.md` & `stepup-1.1.0/docs/getting_started/interactive_usage.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,66 @@
-# Interactive usage
+# Interactive Usage
 
-All previous tutorials ran StepUp non-interatively, for the sake of simplicity.
-In practice this is mainly useful for build projects in batch jobs, e.g. in the cloud.
-When working on a project, interative usage is more efficient and convenient,
+All previous tutorials have run StepUp non-interactively, for the sake of simplicity.
+In practice, this is mainly useful when building projects in batch jobs, e.g., in the cloud.
+When working on a project, interactive usage is more efficient and convenient,
 but requires a little more explanation.
-(For this reason most tutorials here will use the non-interactive option.)
+(For this reason, most of the tutorials use the non-interactive option.)
 
-The tutorial [Static glob](static_glob.md) is in fact a good showcase for StepUp's interactive usage.
-When running StepUp as follows, the terminal user interface will not exit:
+The [Static Glob](static_glob.md) tutorial is a good example to demonstrate the interactive use of StepUp.
+Running StepUp as follows will not exit the terminal user interface:
 
 ```bash
 stepup
 ```
 
-In fact, `stepup` without any arguments is the recommended way of running StepUp in most cases.
+In fact, running the `stepup` command without any arguments is the recommended way to run StepUp in most cases.
 
 After the line `PHASE │ watch` appears, StepUp just waits for changes to the (static) files.
 
-## Change an existing file
 
-For example, while StepUp is still running, change the file `src/foo.txt`.
-You will at least see the following:
+## Change an Existing File
+
+For example, while StepUp is still running, edit and save the file `src/foo.txt`.
+You will see at least the following:
 
 ```
-     ADDED │ src/foo.txt
+    UPDATED │ src/foo.txt
 ```
 
-Now go back to the terminal and press the character `?`,
-which will show the supported keys with interactive commands:
+Now go back to the terminal and press the character `?`
+to display the supported keys with interactive commands:
 
 ```
 ───────────────────────────────────── Keys ─────────────────────────────────────
 
    q = shutdown       d = drain        j = join   g = graph
    f = from scratch   t = try replay   r = run
 
 ────────────────────────────────────────────────────────────────────────────────
 ```
 
 Now press (lower case) `r` to run steps whose (indirect) inputs have changed.
-The new file `src/foo.txt` is copied again to `dst/foo.txt` while other step are ignored.
+The new file `src/foo.txt` is copied again to `dst/foo.txt`, while other steps are ignored.
+
+The interactive commands are described in detail in the [Interactive Command Reference](../reference/interactive.md).
 
-The interactive commands are described in detail in the [Interactive command reference](../reference/interactive.md)
 
-## Add a new file that matches `glob("src/*.txt")`
+## Add a New File That Matches `glob("src/*.txt")`
 
-Create a new file `src/spam.txt` with some contents to your liking, still while StepUp is running.
-You will at least see the following:
+Create a new file `src/spam.txt` with content of your choice while StepUp is still running.
+You will see at least the following:
 
 ```
-     ADDED │ src/spam.txt
+    UPDATED │ src/spam.txt
 ```
 
 Now press (lower case) `r` again.
-The `./plan.py` step is executed again because a new file appeared that matches a glob pattern used in `plan.py`.
-Rerunning `./plan.py` will in turn create a new step to copy `src/spam.txt` to `dst/spam.txt`.
+The `./plan.py` step is executed again because a new file has appeared that matches a glob pattern used in `plan.py`.
+Running `./plan.py` again will, in turn, create a new step to copy `src/spam.txt` to `dst/spam.txt`.
+
+
+## Screen Recording
+
+The following recording shows the terminal output when starting StepUp from scratch with two workers, changing `src/foo.txt` and re-running, followed by adding `src/spam.txt` and re-running:
+
+[![asciicast](https://asciinema.org/a/657277.svg)](https://asciinema.org/a/657277)
```

### Comparing `stepup-1.0.0/docs/getting_started/introduction.md` & `stepup-1.1.0/docs/getting_started/introduction.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,107 +1,125 @@
 # Introduction
 
 The "Getting Started" section consists of a series of short tutorials.
 Each tutorial introduces a few concepts at a time to maintain a gentle learning curve.
-The following initial competences are assumed:
+The following initial competencies are assumed:
 
 - Basic Python programming.
 - Working with a virtual terminal.
 - Editing text files.
 
 Note that the examples in the tutorials are all small and use StepUp non-interactively.
 We believe this offers the best learning experience.
 However, StepUp really shines in more complex use cases and when used interactively.
 Once you know how StepUp works, you can impress yourself by effortlessly mastering the daunting complexity of your projects. :)
 
 
 ## Tutorial source files
 
-Input files for each tutorial are stored in a corresponding subdirectory under `docs/getting_started/` in the source code of StepUp Core.
-Each directory contains a script `main.sh` that simply runs the example in non-interactive mode,
-to generate output that can be included in the documentation.
+Input files for each tutorial are stored in a corresponding subdirectory under `docs/getting_started/` within StepUp Core's source code.
+Each directory contains a script named `main.sh`,
+which simply runs the example in non-interactive mode,
+generating output that can be included in the documentation.
 
 
 ## StepUp architecture
 
-The tutorials use terminology defined in this mini architecture overview.
-The overview merely summarizes the internals of StepUp and omits plenty of details for the sake of clarity.
-It provides just enough to get a basic understanding of its core concepts.
+The tutorials use terminology defined in this small architecture overview.
+This overview summarizes the internals of StepUp, omitting many details for the sake of clarity.
+It provides just enough to give a basic understanding of its core concepts.
 
 
-### Workflow (graph)
+### Workflow (graphs)
 
-StepUp keeps track of what it must do and has already done in a workflow data structure.
-This workflow is represented by a [direct acyclic graph](https://en.wikipedia.org/wiki/Directed_acyclic_graph).
+StepUp keeps track of what it needs to do and what it has already done in a workflow data structure.
+This workflow is represented by *two* [direct acyclic graphs (DAGs)](https://en.wikipedia.org/wiki/Directed_acyclic_graph), which comprise the same nodes.
 
 
 #### Nodes
 
 The nodes of the graph can be instances of the following main classes:
 
-- A `Step` defines a program that can be executed with all information for a specific execution:
+- A `Step` defines a program that can be executed with all the information for a specific execution:
   working directory, command, arguments, inputs, outputs, etc.
   A step can also be in one of the following states:
-    - `PENDING`: the step cannot be scheduled yet because some inputs are not declared or built yet.
+
+    - `PENDING`: the step cannot yet be scheduled because some inputs have not been declared or built yet.
     - `QUEUED`: all inputs are available and the step is waiting to be executed.
     - `RUNNING`: the step is being executed by one of the workers.
-    - `SUCCEEDED`: the step has completed successfully.
-    - `FAILED`: the subprocess exited with a nonzero exitcode or some output files were not created.
-- A `File` defines a path and a status, which can be any of:
-    - `PENDING`: the file is an output of a step that sill needs to be executed.
-    - `BUILT`: the file is an output of a step that has been executed successfully.
-    - `VOLATILE`: the file is (or may be) created by a step, but it is volatile.
+    - `SUCCEEDED`: the step has been successfully completed.
+    - `FAILED`: the subprocess exited with a non-zero exit code or some output files were not created.
+
+- A `File` defines a path and a status, which can be any of the following:
+
+    - `PENDING`: the file is the output of a step that still needs to be executed.
+    - `BUILT`: the file is the output of a step that has been successfully executed.
+    - `VOLATILE`: the file is (or can be) created by a step, but it is volatile.
       It cannot be used as input, no hashes are computed for it.
-      These files are only registered to remove them when appropriate.
-    - `STATIC`: the file is written by you, and can only be an input to a step.
-      (Note that step inputs may also be outputs of other steps.)
+      These files are only registered so that they can be removed when appropriate.
+    - `STATIC`: the file is written by you and can only be an input to a step.
+      (Note that step inputs can also be outputs of previous steps.)
     - `MISSING`: a static file that has gone missing.
 
 There are also a few special nodes:
 
 - The `Root` node is the top-level node, of which there is only one.
-- The `Vacuum` node is also unique and collects other nodes that will soon be deleted.
-- A `DeferredGlob` node contains a [glob](https://en.wikipedia.org/wiki/Glob_(programming)) pattern of files that are made static when they are used as inputs.
+- The `Vacuum` node is also unique and collects other nodes that will be deleted soon.
+- A `DeferredGlob` node contains a [glob](https://en.wikipedia.org/wiki/Glob_(programming)) pattern of files that are made static when they are used as input.
 
 
 #### Edges
 
-The StepUp workflow has two types of directed edges (arrows) that connect a pair of nodes:
+The StepUp workflow has two types of directed edges (arrows) connecting pairs of nodes.
+Each type of edge forms a graph with its own rules and logic.
 
-- A **creator** edge is an arrow pointing from a node to its creator.
-  It is added whenever the workflow is extended with a new node:
-  every node must have a creator.
-  The inverse arrows are also used in StepUp and are called **product** edges.
+- A **"supplier ➜ consumer"** edge points from a node that provides *something* to a node that uses that *something*.
   A few examples:
+
+    - If a step uses a file as its input, it is the consumer of that file.
+    - Likewise, a step is the supplier of its outputs
+    - Every file is the consumer of its parent directory.
+      (The only exceptions are `./` and `/`.)
+    - A step is the consumer of its working directory.
+
+    The following diagram from the [Dependencies tutorial](dependencies.md) illustrates this type of edge.
+    (Directories are not included, steps are blue ellipses, files are grey rectangles.)
+
+    ![graph_supplier.svg](dependencies/graph_supplier.svg)
+
+    The build algorithm in StepUp will traverse *up*wards through this graph as it executes the steps,
+    similarly to [tup](https://gittup.org/tup/)
+
+- A **"creator ➜ product"** edge is added whenever a new node is added to the workflow:
+  Each node must have **one** creator, but nodes can have multiple products.
+  Examples include:
+
     - A step is the creator of its output files.
-    - When a `plan.py` (or other step) defines new steps, then `plan.py` step is the creator of
+    - If a `plan.py` (or other step) defines new steps, then the `./plan.py` step is the creator of
       the new steps.
-    - When a step declares a static file, the step is the creator of the static file.
+    - If a step declares a static file, the step is the creator of the static file.
     - The initial `plan.py` step has the `Root` node as its creator.
     - Only the `Root` node is its own creator, making it the top-level node by construction.
     - When nodes are slated for removal, the `Vacuum` node becomes their creator.
 
-- A **consumer** edge is an arrow pointing from a node to other nodes that use it (as input).
-  The inverse arrows are also present in StepUp and are called **supplier** edges.
-  A few examples:
-    - When a step uses a file as input, it is the consumer of that file.
-    - Each file is the consumer of its parent directory,
-      except for `./` (for relative paths) and `/` (for absolute paths).
-    - A step is the consumer of its working directory.
+    The following graph from the [Dependencies tutorial](dependencies.md) illustrates this type of edge.
+    (Steps are blue ellipses, files are grey rectangles, root and vacuum are orange hexagons.)
+
+    ![graph_creator.svg](dependencies/graph_creator.svg)
 
 
 ### Processes
 
-The following schematic visualizes how the components of StepUp interact. Legend:
+The following diagram illustrates how the components of StepUp interact. Legend:
 
 - White boxes: your fingers and eyes
 - Grey boxes: processes
-    - The **terminal user interface** is the part of StepUp that you interact when when running the `stepup` command.
-    - The **director** holds the workflow datastructure and is responsible for running steps and watching for file changes.
+    - The **terminal user interface** is the part of StepUp that you interact with when you run the `stepup` command.
+    - The **director** holds the workflow data structure and is responsible for running steps and watching for file changes.
     - The **worker** processes execute steps and compute file and step hashes.
 - Grey arrows: standard input (interactively usage only) and standard output.
 - Yellow arrows: startup of subprocesses
 - Blue arrows: remote procedure calls to control the director and the workers
 - Purple arrows: remote procedure calls for progress updates
-- Geen arrows: remote procedure calls to extend the workflow
+- Green arrows: remote procedure calls to extend the workflow
 
 ![processes](processes.svg)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stepup-1.0.0/docs/getting_started/no_rules/stdout.txt` & `stepup-1.1.0/docs/getting_started/no_rules/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ tr '[:lower:]' '[:upper:]' < lower1.txt > upper1.txt
    SUCCESS │ tr '[:lower:]' '[:upper:]' < lower1.txt > upper1.txt
      START │ tr '[:lower:]' '[:upper:]' < lower2.txt > upper2.txt
    SUCCESS │ tr '[:lower:]' '[:upper:]' < lower2.txt > upper2.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
```

### Comparing `stepup-1.0.0/docs/getting_started/processes.svg` & `stepup-1.1.0/docs/getting_started/processes.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/docs/getting_started/script_multiple/ebbr.csv` & `stepup-1.1.0/docs/getting_started/script_multiple/ebbr.csv`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/docs/getting_started/script_multiple/ebos.csv` & `stepup-1.1.0/docs/getting_started/script_multiple/ebos.csv`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/docs/getting_started/script_multiple/plot.py` & `stepup-1.1.0/docs/getting_started/script_multiple/plot.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/docs/getting_started/script_multiple/stdout.txt` & `stepup-1.1.0/docs/getting_started/script_multiple/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./plot.py plan
    SUCCESS │ ./plot.py plan
      START │ ./plot.py run -- 'plot_ebbr'
    SUCCESS │ ./plot.py run -- 'plot_ebbr'
      START │ ./plot.py run -- 'plot_ebos'
```

### Comparing `stepup-1.0.0/docs/getting_started/script_multiple.md` & `stepup-1.1.0/docs/getting_started/script_multiple.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Script (multiple cases)
+# Script (Multiple Cases)
 
 In the [previous tutorial](script_single.md), the script protocol and driver
 were illustrated with a single use case of a script.
 The driver also handles scripts that can be executed with different combinations of inputs.
 
 
-## Multiple case script driver
+## Multiple Cases Script Driver
 
 A Python script using the driver for multiple cases has the following structure.
 
 ```python
 #!/usr/bin/env python
 from stepup.core.script import driver
 
@@ -47,29 +47,31 @@
 - The cases will be represented by a string argument on the command line formatted with
   `CASE_FMT.format(*args, **kwargs)`, where `args` and `kwargs` are derived from the iterates
   from the `cases()` generator.
   The formatted string must retain all information of `args` and `kwargs`,
   so that they can be derived again from the formatted string
   with the [parse](https://github.com/r1chardj0n3s/parse) library.
 
-    - Here, the two string representations will `foo1` and `foo2`.
+    - Here, the two string representations will be `foo1` and `foo2`.
     - The corresponding steps will be `./script.py run foo1` and `./script.py run foo2`
 
 - The function `case_info()` is used to translate `args` and `kwargs` into a more detailed
   planning of the run steps.
 
 - The function `run()` works in the same way as for the single case script driver.
 
 
 ## Example
 
-To make the example a little more entertaining,
-it makes use of [NumPy](https://numpy.org/) and [Matplotlib](https://matplotlib.org/).
+Example source files: [getting_started/script_multiple/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/getting_started/script_multiple)
+
+To make the example more engaging,
+it leverages [NumPy](https://numpy.org/) and [Matplotlib](https://matplotlib.org/).
 The same plotting function is applied to two datasets of hourly temperatures recorded at
-the airports of Brussels and Ostend in the month of February 2024, downloaded from the
+the airports of Brussels and Ostend in February 2024, downloaded from the
 [ASOS network hosted by Iowa State University](https://mesonet.agron.iastate.edu/request/download.phtml).
 
 
 Create a script `plan.py` that just calls the plotting script:
 
 ```python
 {% include 'getting_started/script_multiple/plan.py' %}
@@ -96,25 +98,23 @@
 
 This produces the following figures:
 
 ![EBBR](script_multiple/plot_ebbr.png)
 ![EBOS](script_multiple/plot_ebos.png)
 
 
-## Try the following
+## Try the Following
 
-- Download temperature data for the same month of an airport close to your home and put it in
-  the same format as the `*.csv` already present.
+- Download temperature data for the same month of an airport close to your home and format it
+  similarly to the `*.csv` already present.
   Extend the `cases()` generator to also process your temperature data.
 
-- It is common that iterates of `cases()` are reused by multiple scripts.
+- It is common for iterates of `cases()` to be reused by multiple scripts.
   One way to centralize this information is by defining a list `airports` in a `settings.py` module.
   By locally importing this module in the `cases()` function,
-  the driver will make `settings.py` an input of (only) the planning step of the script:
+  the driver will make `settings.py` an input only of the planning step of the script:
 
     ```python
     def cases():
         from settings import airports
         yield from airports
     ```
-
-    A change in `settings.py` will only affect the relevant run steps.
```

### Comparing `stepup-1.0.0/docs/getting_started/script_single.md` & `stepup-1.1.0/docs/getting_started/script_single.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# Script (single case)
+# Script (Single Case)
 
 StepUp Core implements a simple *script protocol* for defining scripts that combine planning and execution in a single source file.
-This is sometimes more convenient than putting a lot of detail in the `plan.py` file.
+This can be more convenient than putting a lot of detail in the `plan.py` file.
 
 
-## Script protocol
+## Script Protocol
 
 The [`script()`][stepup.core.api.script] protocol itself is rather simple.
 The following line in `plan.py`:
 
 ```python
 script("sub/executable")
 ```
 
-is roughly equivalent to
+is roughly equivalent to:
 
 ```python
-step("./excutable plan", inp="sub/executable", workdir="sub/")
+step("./executable plan", inp="sub/executable", workdir="sub/")
 ```
 
 where the subdirectory is optional.
-The step `./excutable plan` is expected to define additional steps to actually run something useful with the executable.
+The step `./executable plan` is expected to define additional steps to actually run something useful with the executable.
 A common scenario is that it plans a single step `./executable run` with appropriate inputs and outputs.
 
 
 ## Script driver
 
 StepUp implements a `driver` function in the module `stepup.core.script` that greatly facilitates
 writing Python scripts that adhere to the script protocol.
 
 It can be used in two ways:
 
 1. To run the executable for just one specific case of inputs and outputs (this tutorial).
+
 2. To run the same script with multiple combinations of inputs and outputs ([next tutorial](script_multiple.md)).
 
 
-## Single case script driver
+## Single Case Script Driver
 
 A Python script using the driver for a single case has the following structure.
 
 
 ```python
 #!/usr/bin/env python
 from stepup.core.script import driver
@@ -54,25 +55,30 @@
 def run(inp, out, just_any):
     ...
 
 if __name__ == "__main__":
     driver()
 ```
 
-- The `info` function provides the necessary data to implement the planning of the running of script.
-  It is executed when calling the script as `./script.py plan`
-- The `run` function is called to perform the useful work and is executed when running he script with `./script.py run`.
+- The `info` function provides the necessary data to implement
+  the planning of the execution of the script.
+  It is executed when calling the script as `./script.py plan`.
+
+- The `run` function is called to perform the useful work and
+  is executed when running the script with `./script.py run`.
 
 Note that the `run` function can have any argument defined in the dictionary return by `info`,
 but it does not have to specify all of them.
-The argument list of `run` may also contain less arguments (or even none at all).
+The argument list of `run` may also contain fewer arguments (or even none at all).
 
 
 ## Example
 
+Example source files: [getting_started/script_single/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/getting_started/script_single)
+
 Consider a script that has parameters defined in a config file `config.json`,
 which may be used by multiple script, e.g. for reasons of consistency.
 For this example, the configuration contains a number of steps and a frequency in arbitrary units,
 serialized in a JSON file:
 
 ```json
 {% include 'getting_started/script_single/config.json' %}
@@ -101,21 +107,24 @@
 
 ```
 {% include 'getting_started/script_single/stdout.txt' %}
 ```
 
 As expected, this creates two files: `cos.npy` and `sin.npy`.
 
-Now, try the following:
 
-- Change the file `config.json` and rerun StepUp.
+## Try the Following:
+
+- Modify the file `config.json` and re-run StepUp.
   The planning is skipped because the script itself did not change.
   Only the run function is called to work with the updated `config.json`.
+
 - Delete one of the outputs and rerun StepUp.
   Again, the planning is skipped and the computation is repeated to recreate the missing output.
+
 - Create a new module `utils.py` with a `compute` function to calculate the cosine and sine arrays
   with parameters `nstep` and `freq`.
-  Import this module into `generate.py`, use it in `run` and rerun StepUp.
+  Import this module into `generate.py`, use it in `run` and re-run StepUp.
   This will automatically make `utils.py` an input for the planning and running of `generate.py`.
-  Test this by making a small change to `utils.py` and rerunning it.
+  Test this by making a small change to `utils.py` and re-running it.
   (Note that local imports inside the `run` function will not be identified automatically and
-  are therefore note recommended.)
+  are therefore not recommended.)
```

### Comparing `stepup-1.0.0/docs/getting_started/static_glob/stdout.txt` & `stepup-1.1.0/docs/getting_started/static_glob/stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ mkdir -p dst/
    SUCCESS │ mkdir -p dst/
      START │ cp -aT src/bar.txt dst/bar.txt
    SUCCESS │ cp -aT src/bar.txt dst/bar.txt
      START │ cp -aT src/foo.txt dst/foo.txt
```

### Comparing `stepup-1.0.0/docs/getting_started/static_glob.md` & `stepup-1.1.0/docs/getting_started/static_glob.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-# Static glob
+# Static Glob
 
 Explicitly declaring static files with the `static` function from the previous tutorial becomes tedious when dealing with many static files.
-To simplify matters, StepUp supports ["glob"](https://en.wikipedia.org/wiki/Glob_(programming)) patterns, i.e. wildcards such as `*` and `?`.
+To simplify matters, StepUp supports ["glob"](https://en.wikipedia.org/wiki/Glob_(programming)) patterns, i.e., wildcards such as `*` and `?`.
 
 The [`glob()`][stepup.core.api.glob] function is similar to [`static()`][stepup.core.api.static] and supports globbing, including some non-standard glob techniques discussed in the following tutorials.
 
 Here, only the basic usage of [`glob()`][stepup.core.api.glob] is covered.
 In the [following tutorial](static_glob_conditional.md), the use of `glob` in conditionals is discussed.
-See [Static named glob](../advanced_topics/static_named_glob.md) and [Static deferred glob](../advanced_topics/static_deferred_glob.md) for more advanced use cases.
+See [Static Named Glob](../advanced_topics/static_named_glob.md) and
+[Static Deferred Glob](../advanced_topics/static_deferred_glob.md) for more advanced use cases.
+
 
 ## Example
 
+Example source files: [getting_started/static_glob/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/getting_started/static_glob)
+
 Create a subdirectory `src/` with two files: `sub/foo.txt` and `sub/bar.txt`.
-Also create a `plan.py` with the following contents:
+Also, create a `plan.py` file with the following contents:
 
 ```python
 {% include 'getting_started/static_glob/plan.py' %}
 ```
 
 Make the plan executable and run it non-interactively:
 
@@ -32,17 +36,18 @@
 ```
 
 Note that all files found by the `glob` function are declared static in the workflow.
 Hence, they cannot be outputs of other steps.
 (This is not optional.)
 
 
-## Try the following
+## Try the Following
 
 - Run StepUp again without making any changes.
-  You will notice that the `plan.py` step is executed again despite not having changed it.
+  You will notice that the `./plan.py` step is executed again despite not having changed it.
   When StepUp starts from scratch, it has to assume that new files could have been added (since the last run) that match the glob pattern.
   Hence, a step calling the `glob` function cannot be skipped.
   (This can be avoided when using StepUp interactively. More on that later.)
+
 - Add a file `src/egg.txt` and run StepUp again with the same arguments.
   You will notice that known steps for `sub/foo.txt` and `sub/bar.txt` are skipped.
   A new step is added for `src/egg.txt`.
```

### Comparing `stepup-1.0.0/docs/getting_started/static_glob_conditional/stdout1.txt` & `stepup-1.1.0/docs/getting_started/static_glob_conditional/stdout1.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   DIRECTOR │ Listening on /tmp/stepup-########/director
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./expensive.py
    SUCCESS │ ./expensive.py
      START │ cat average.txt
    SUCCESS │ cat average.txt
 ─────────────────────────────── Standard output ────────────────────────────────
```

### Comparing `stepup-1.0.0/docs/getting_started/static_glob_conditional.md` & `stepup-1.1.0/docs/getting_started/static_glob_conditional.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Static glob conditional
+# Static Glob Conditional
 
 The [`glob()`][stepup.core.api.glob] function introduced in the previous tutorial
 also works in conditional expressions.
 This is particularly useful when not using any wildcards at all:
 
 ```python
 from stepup.core.api import glob
@@ -19,14 +19,16 @@
 
 A similar conditional would not work with the [`static()`][stepup.core.api.static] function
 because it would raise an exception when the file does not exist.
 
 
 ## Example
 
+Example source files: [getting_started/static_glob_conditional/](https://github.com/reproducible-reporting/stepup-core/tree/main/docs/getting_started/static_glob_conditional)
+
 Let's simulate a scenario where `dataset/`, if it exists, is remote storage with a huge dataset.
 Plan A is to extract useful information from the dataset.
 However, there may be reasons why this is not always possible or desirable:
 
 - Not all your collaborators may have access to this storage at all times.
 - The extraction is slow or expensive otherwise.
 
@@ -62,15 +64,15 @@
 
 You should get the following output:
 
 ```
 {% include 'getting_started/static_glob_conditional/stdout1.txt' %}
 ```
 
-Now, simulate the situation the absence of the dataset by renaming the directory:
+Now, simulate the situation where the dataset is absent by renaming the directory:
 
 ```bash
 mv dataset tmp
 stepup -n -w1
 ```
 
 The new output reveals that the dataset is completely ignored while the file `average.txt` is still used:
@@ -78,24 +80,24 @@
 ```
 {% include 'getting_started/static_glob_conditional/stdout2.txt' %}
 ```
 
 Since the file `average.txt` did not change, the step `cat average.txt` is skipped.
 
 
-## Practical considerations
+## Practical Considerations
 
-- The example involves few calculations for the sake of simplicity.
+- For simplity's sake, the example involves few calculations.
   In a more realistic setting, the step `cat average.txt` is replaced by several scripts that
   make graphs of the information extracted from the large dataset.
   Tweaking these graphs for clarity usually takes some iterations,
-  for which access to the big dataset is not relevant.
+  for which access to the large dataset is not necessary.
 
 - A StepUp project practically always resides in a Git repository.
-  While the files extract from the big dataset can be reproduced easily,
-  it may still be relevant to commit the data extracted from the big data set into the Git repository:
+  While the files extracted from the large dataset can be reproduced easily,
+  it may still be relevant to commit them into the Git repository:
 
-    - Not all your collaborators may have access to the dataset,
+    - Not all collaborators may have access to the dataset,
       but you still want them to be able to reproduce the workflow.
 
-    - In the long run, the big dataset may be removed because it is too big and old keep around.
-      The extracted data are then a relevant and compact subset that you can easily store for longer times.
+    - In the long run, the large dataset might be removed because it is too big and old to keep around.
+      The extracted data then become a relevant and compact subset that can be easily stored for longer periods.
```

### Comparing `stepup-1.0.0/docs/installation.md` & `stepup-1.1.0/docs/installation.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Installation
 
 Requirements:
 
-- [POSIX](https://en.wikipedia.org/wiki/POSIX) operating system: Linux, macOS or WSL. StepUp cannot not run natively on Windows.
+- [POSIX](https://en.wikipedia.org/wiki/POSIX) operating system: Linux, macOS or WSL. StepUp cannot run natively on Windows.
 - [Python](https://www.python.org/) ≥ 3.11
 - [Pip](https://pip.pypa.io/)
 
-It is assumed you know how to use [Pip](https://pip.pypa.io/).
-We recommend to perform the installation in a [Python virtual environment](https://docs.python.org/3/library/venv.html) and to activate such environments with [direnv](https://direnv.net/).
+It is assumed that you know how to use [Pip](https://pip.pypa.io/).
+We recommend performing the installation in a [Python virtual environment](https://docs.python.org/3/library/venv.html) and activating such environments with [direnv](https://direnv.net/).
 
-The core package is installed with
+The core package can be installed with:
 
 ```bash
 pip install stepup
 ```
 
-The RepRep extension (for reproducible reporting) is installed with:
+The [StepUp RepRep](https://reproducible-reporting.github.io/stepup-reprep/) extension
+(for reproducible reporting) is installed with:
 
 ```bash
 pip install stepup-reprep
 ```
```

### Comparing `stepup-1.0.0/docs/license.md` & `stepup-1.1.0/docs/license.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # License
 
 ## Source code license
 
-StepUp is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+StepUp Core is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
-StepUp is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+StepUp Core is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see [https://www.gnu.org/licenses/](https://www.gnu.org/licenses/).
 
 
 ## Documentation license
 
-StepUp's documentation is distributed under the [Creative Commons CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).
+StepUp Core's documentation is distributed under the [Creative Commons CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).
```

### Comparing `stepup-1.0.0/docs/reference/interactive.md` & `stepup-1.1.0/docs/reference/interactive.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-# Interactive command reference
+# Interactive Command Reference
 
-By default StepUp runs in interactive mode.
-When pressing a key on the keyboard, it will respond by executing a corresponding command.
-If the key is not associated with some command, the following help message is shown:
+By default, StepUp runs in interactive mode.
+When pressing a key on the keyboard, it responds by executing a corresponding command.
+If the key is not associated with any command, the following help message appears:
 
 ```
 ───────────────────────────────────── Keys ─────────────────────────────────────
 
    q = shutdown       d = drain        j = join   g = graph
    f = from scratch   t = try replay   r = run
 
 ────────────────────────────────────────────────────────────────────────────────
 ```
 
 These commands are defined as follows:
 
 - `q = shutdown`:
-  StepUp waits for the workers to complete their current job but will not start new jobs.
-  As soon as all workers are idle, StepUp exists.
+  StepUp waits for the workers to complete their current job and will not start new jobs.
+  As soon as all workers are idle, StepUp exits.
 - `d = drain`:
-  StepUp waits for the workers to complete their current job but will not start new jobs.
-  As soon as all workers are idle, StepUp switches to *watch phase*.
+  StepUp waits for the workers to complete their current job and will not start new jobs.
+  As soon as all workers are idle, StepUp transitions into the *watch phase*.
 - `j = join`:
-  StepUp keeps running jobs until no new jobs can be found to send to the workers.
-  As soon as all workers are idle, StepUp exists.
+  StepUp continues running jobs until no new jobs can be found to send to the workers.
+  As soon as all workers are idle, StepUp terminates.
 - `g = graph`:
-  Write out the workflow graph in text format to a file `graph.txt`.
-  (This is a human readable file containing most of the information in `.stepup/workflow.mp.xz`)
+  Writes out the workflow graph in text format to a file named `graph.txt`.
+  (This human-readable file contains most of the information from `.stepup/workflow.mp.xz`)
 - `f = from scratch`:
-  Discard all hashes and rerun all steps.
-  No attempts are made to skip steps and everything is executed from scratch.
+  Discards all hashes and reruns all steps.
+  No attempts are made to skip steps, and everything is executed from scratch.
 - `t = try replay`:
-  Check the hash of each step and skip it if no changes were detected. Run otherwise.
-  (Normally, this command is never needed.)
+  Checks the hash of each step and skips it if no changes were detected.
+  Otherwise, run the step.
+  (Normally, this command is not needed.)
 - `r = run`:
-  Run steps that are affected by file changes registered in *watch phase*.
+  Runs steps that are affected by file changes registered during the *watch phase*.
```

### Comparing `stepup-1.0.0/docs/reference/stepup.core.api.md` & `stepup-1.1.0/docs/reference/stepup.core.api.md`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/mkdocs.yml` & `stepup-1.1.0/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,17 @@
     - advanced_topics/blocked_steps.md
     - advanced_topics/pools.md
     - advanced_topics/environment_variables.md
     - advanced_topics/volatile_outputs.md
     - advanced_topics/amending_steps.md
     - advanced_topics/variable_substitution.md
     - advanced_topics/here_and_root.md
+    - advanced_topics/cyclic_dependencies.md
+    - advanced_topics/amending_static_inputs.md
+    - advanced_topics/manual_cleaning.md
   - Reference:
     - reference/stepup.core.api.md
     - reference/stepup.core.interact.md
     - reference/interactive.md
   - changelog.md
   - development.md
   - license.md
@@ -86,14 +89,15 @@
         paths: ["stepup-core"]
         options:
           docstring_style: numpy
           show_root_heading: true
           docstring_section_style: list
 
 markdown_extensions:
+  - admonition
   - smarty
   - pymdownx.highlight:
       anchor_linenums: true
       line_spans: __span
       pygments_lang_class: true
   - pymdownx.inlinehilite
   - pymdownx.snippets
```

### Comparing `stepup-1.0.0/pyproject.toml` & `stepup-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ]
 dependencies = [
     "attrs",
     "msgpack",
     "parse",
     "path",
     "rich",
-    "watchfiles",
+    "watchdog",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-asyncio",
@@ -39,20 +39,22 @@
     "mkdocs-macros-plugin",
     "mkdocs-material",
     "numpy",
     "matplotlib",
 ]
 
 [project.urls]
+Documentation = "https://reproducible-reporting.github.io/stepup-core/"
 Issues = "https://github.com/reproducible-reporting/stepup-core/issues"
 Source = "https://github.com/reproducible-reporting/stepup-core/"
-Changelog = "https://github.com/reproducible-reporting/stepup-core/blob/main/CHANGELOG.md"
+Changelog = "https://reproducible-reporting.github.io/stepup-core/changelog/"
 
 [project.scripts]
 stepup = "stepup.core.tui:main"
+cleanup = "stepup.core.cleanup:main"
 
 [tool.pytest.ini_options]
 addopts = "-n auto"
 
 [tool.black]
 line-length = 100
 target-version = ['py311']
@@ -61,11 +63,14 @@
 line-length = 100
 target-version = "py311"
 
 [too.ruff.lint]
 select = ["E", "F", "UP", "B", "I", "PGH", "PL", "RUF", "C"]
 ignore = ["PLR0911", "PLR0912", "PLR0913", "PLR0915", "PLR2004", "PLW2901", "C901"]
 
+[tool.setuptools]
+packages = ["stepup.core"]
+
 [tool.setuptools_scm]
 write_to = "stepup/core/_version.py"
 version_scheme = "post-release"
 local_scheme = "no-local-version"
```

### Comparing `stepup-1.0.0/stepup/core/__init__.py` & `stepup-1.1.0/stepup/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/stepup/core/api.py` & `stepup-1.1.0/stepup/core/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         When True, static files are not added yet.
         Instead, the glob is installed in the workflow as a deferred glob.
         As soon as any file is needed as input and matches the pattern,
         it will be made static.
         This is not compatible with `_required=True`.
         Named wildcards are not supported in deferred globs.
     **subs
-        When using named wildcards, they will match the pattern ``*`` by default.
+        When using named wildcards, they will match the pattern `*` by default.
         Through the subs argument each name can be associated with another glob pattern.
         Names starting with underscores are not allowed.
 
     Raises
     ------
     FileNotFoundError
         when no matches were found and _required is True.
@@ -202,15 +202,15 @@
         ngm_data = nglob_multi.unstructure(lookup)
         tr_strings = [str(translate(path)) for path in lookup.get_list()]
         RPC_CLIENT.call.nglob(_get_step_key(), ngm_data, tr_strings)
         return nglob_multi
 
 
 def _str_to_list(arg: Collection[str] | str) -> list[str]:
-    return [arg] if isinstance(arg, str) else arg
+    return [arg] if isinstance(arg, str) else list(arg)
 
 
 def step(
     command: str,
     *,
     inp: Collection[str] | str = (),
     env: Collection[str] | str = (),
@@ -382,15 +382,15 @@
 
 def plan(subdir: str, block: bool = False):
     """Run a `plan.py` script in a subdirectory.
 
     Parameters
     ----------
     subdir
-        The subdirectory in which another ``plan.py`` script can be found.
+        The subdirectory in which another `plan.py` script can be found.
         The file must be executable and have `#!/usr/bin/env python` as its first line.
     block
         When True, the step will always remain pending.
     """
     with subs_env_vars() as subs:
         subdir = subs(subdir)
     path_subdir = Path(subdir)
@@ -490,15 +490,15 @@
         The path of a local executable that will be called with the argument `plan`.
         The file must be executable.
     workdir
         The subdirectory in which the script is to be executed.
         The path of the executable is assumed to be relative to this directory.
     optional
         When True, the steps planned by the executable are made optional.
-        The planing itself is never optional.
+        The planning itself is never optional.
     block
         When True, the planning will always remain pending.
     """
     with subs_env_vars() as subs:
         executable = subs(executable)
         workdir = subs(workdir)
     path_workdir = Path(workdir)
@@ -511,15 +511,15 @@
 
 #
 # API development utilities
 #
 
 
 @contextlib.contextmanager
-def subs_env_vars() -> Iterator[Callable]:
+def subs_env_vars() -> Iterator[Callable[[str | None], str | None]]:
     """A context manager for substituting environment variables and tracking the used variables.
 
     The context manager yields a function, `subs`, which takes a string with variables and
     returns the substituted form.
     All used variables are recorded and sent to the director with `amend(env=...)`.
     For example:
 
@@ -620,14 +620,15 @@
     return SocketSyncRPCClient(STEPUP_DIRECTOR_SOCKET)
 
 
 RPC_CLIENT = _get_rpc_client()
 
 
 def _get_step_key():
+    """Get the current step key from the STEPUP_STEP_KEY environment variable."""
     stepup_step_key = os.getenv("STEPUP_STEP_KEY")
     if stepup_step_key is None:
         if isinstance(RPC_CLIENT, DummySyncRPCClient):
             return "dummy:"
         else:
             raise RuntimeError("The STEPUP_STEP_KEY environment variable is not defined.")
     return stepup_step_key
```

### Comparing `stepup-1.0.0/stepup/core/assoc.py` & `stepup-1.1.0/stepup/core/assoc.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/stepup/core/cascade.py` & `stepup-1.1.0/stepup/core/cascade.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,23 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""A Cascade instance is StepUp's abstract dependency graph."""
+"""A Cascade instance is StepUp's abstract implementation of the workflow graph.
+
+It introduces two types of edges (creator-product) and (supplier-consumer),
+and several essential `Node` classes: `Root` and `Vacuum`.
+All other nodes and their logic are implemented in `stepup.core.workflow`.
+
+The separation between `Cascade` and `Workflow` allows for testing a well-defined subset,
+before building more complexity on top of it.
+"""
 
 import lzma
 from typing import Any, Self, Iterator
 
 import attrs
 import msgpack
 
@@ -147,15 +155,15 @@
 
 @attrs.define
 class Cascade:
     # Dictionary of all nodes in their key
     nodes: dict[str, Node] = attrs.field(factory=dict)
     # Association (kind, keys_of_kind)
     kinds: Assoc[str, str] = attrs.field(factory=one_to_many)
-    # Association (creator, products) and its inverse
+    # Association (creator, product) and its inverse
     products: Assoc[str, str] = attrs.field(factory=one_to_many)
     creators: AssocView[str, str] = attrs.field(init=False)
     # Association (supplier, consumer) and its inverse
     consumers: Assoc[str, str] = attrs.field(factory=many_to_many)
     suppliers: AssocView[str, str] = attrs.field(init=False)
     # The types of nodes that are allowed
     node_classes: dict[str, type[Node]] = attrs.field(init=False)
@@ -365,31 +373,36 @@
         keys = sorted(key for key in keys if (include_orphans or not self.is_orphan(key)))
         return [self.nodes[key] for key in keys]
 
     #
     # Graph modifications
     #
 
-    def _iter_cycles(self, src_key, dst_key):
+    def _iter_cycles(self, src_key: str, dst_key: str) -> Iterator[tuple[str]]:
+        """Iterate over cycles that point from `dst_key` back to `src_key`.
+
+        Notes
+        -----
+        This method only consider supplier-consumer edges.
+        """
         if src_key != "root:":
             if src_key == dst_key:
                 yield (src_key,)
-            creator_key = self.creators.get(src_key)
-            if creator_key is not None:
-                for cycle in self._iter_cycles(creator_key, dst_key):
-                    yield (src_key,) + cycle
             for supplier_key in self.suppliers.get(src_key, ()):
                 for cycle in self._iter_cycles(supplier_key, dst_key):
                     yield (src_key,) + cycle
 
-    def report_cyclic(self, src_key, dst_key):
+    def report_cyclic(self, src_key: str, dst_key: str):
         """Raise an informative exception when the new edge would make the directed graph cyclic.
 
-        This method is rather slow and only called when there is a known problem.
-        It is helpful because it provides more useful (and expensive) feedback.
+        Notes
+        -----
+        - This method is rather slow and only called when there is a known problem.
+          It is helpful because it provides more useful (and expensive) feedback.
+        - This method only consider supplier-consumer edges.
         """
         lines = []
         for cycle in self._iter_cycles(src_key, dst_key):
             lines.append("cycle:")
             for key in cycle:
                 lines.append(f"  {key}")
             lines.append("")
@@ -399,28 +412,36 @@
                 "",
                 f"src = {src_key}",
                 f"dst = {dst_key}",
                 "",
             ] + lines
             raise CyclicError("\n".join(lines))
 
-    def _iter_predecessors(self, key: str, visited: set):
-        if key != "root:":
-            visited.add(key)
-            creator_key = self.creators.get(key)
-            if creator_key not in visited:
-                self._iter_predecessors(creator_key, visited)
-            for supplier_key in self.suppliers.get(key, ()):
-                if supplier_key not in visited:
-                    self._iter_predecessors(supplier_key, visited)
+    def walk_suppliers(self, key: str, visited: set[str]):
+        """Efficiently collect all suppliers of `key` and add them to `visited`."""
+        if key in ["root:", "vacuum:"]:
+            return
+        visited.add(key)
+        for supplier_key in self.suppliers.get(key, ()):
+            if supplier_key not in visited:
+                self.walk_suppliers(supplier_key, visited)
+
+    def walk_consumers(self, key: str, visited: set[str]):
+        """Efficiently collect all consumers of `key` and add them to `visited`."""
+        if key in ["root:", "vacuum:"]:
+            return
+        visited.add(key)
+        for consumer_key in self.consumers.get(key, ()):
+            if consumer_key not in visited:
+                self.walk_consumers(consumer_key, visited)
 
-    def check_cyclic(self, src_key, dst_key):
-        """Raise an informative exception when the new edge would make the directed graph cyclic."""
+    def check_cyclic(self, src_key: str, dst_key: str):
+        """Raise an informative exception when the new edge would introduce a cyclic dependency."""
         visited = set()
-        self._iter_predecessors(src_key, visited)
+        self.walk_suppliers(src_key, visited)
         if dst_key in visited:
             self.report_cyclic(src_key, dst_key)
 
     def create(self, node: Node, creator_key: str) -> str:
         """Add a newly created node with reference to its creator."""
         # Sanity checking
         if not isinstance(creator_key, str):
```

### Comparing `stepup-1.0.0/stepup/core/deferred_glob.py` & `stepup-1.1.0/stepup/core/deferred_glob.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""StepUp deferred patterns for static files."""
+"""Deferred patterns for static files."""
 
 from typing import Any, Self, Iterator, TYPE_CHECKING
 
 import attrs
 
 from .cascade import Node
 from .nglob import NGlobMulti
```

### Comparing `stepup-1.0.0/stepup/core/director.py` & `stepup-1.1.0/stepup/core/director.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,36 +13,37 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""director."""
+"""The director process manages the workflow and sends jobs to the worker processes."""
 
 import asyncio
 import contextlib
 import os
 import argparse
 import shutil
 import sys
 import traceback
 from decimal import Decimal
 
 import attrs
 from path import Path
 
+from stepup.core.file import FileState
 from stepup.core.nglob import NGlobMulti
 from .rpc import serve_socket_rpc, allow_rpc
 from .workflow import Workflow
 from .exceptions import GraphError
 from .reporter import ReporterClient
-from .runner import Runner, Phase
+from .runner import Runner
 from .scheduler import Scheduler
-from .utils import check_plan, mynormpath
+from .utils import check_plan, mynormpath, remove_path
 from .watcher import Watcher
 
 
 __all__ = ("interpret_num_workers", "serve")
 
 
 def main():
@@ -54,15 +55,15 @@
     print(f"PID {os.getpid()}", file=sys.stderr)
     async with ReporterClient.socket(args.reporter_socket) as reporter:
         num_workers = interpret_num_workers(args.num_workers)
         await reporter.set_num_workers(num_workers)
         await reporter("DIRECTOR", f"Listening on {args.director_socket}")
         try:
             await serve(
-                args.director_socket,
+                Path(args.director_socket),
                 num_workers,
                 args.workflow,
                 args.plan,
                 reporter,
                 args.show_perf,
                 args.explain_rerun,
             )
@@ -144,15 +145,15 @@
 Please open an issue at https://github.com/reproducible-reporting/stepup-core/issues
 Copy paste the traceback below and explain how to reproduce the problem.
 The broken workflow file was copied to {}.
 """
 
 
 async def serve(
-    director_socket_path: str,
+    director_socket_path: Path,
     num_workers: int,
     path_workflow: str,
     path_plan: str,
     reporter: ReporterClient,
     show_perf: bool,
     explain_rerun: bool,
 ):
@@ -163,14 +164,16 @@
     director_socket_path
         The socket to listen to for remote calls.
     num_workers
         The number of worker processes.
     path_workflow
         The path where the workflow file will be written to
         (and read from if there was a previous run).
+    path_plan
+        The initial `plan.py` file.
     reporter
         The reporter client for sending information back to
         the terminal user interface.
     show_perf
         Show performance details after each completed step.
     explain_rerun
         Let workers explain why steps with recording info cannot be skipped.
@@ -178,15 +181,15 @@
     if num_workers < 1:
         raise ValueError(f"Number of workers must be strictly positive, got {num_workers}")
 
     # Process paths
     path_workflow = Path(path_workflow)
     check_plan(path_plan)
 
-    # Initialize components
+    # Initialize workflow
     workflow = None
     if path_workflow.exists():
         try:
             workflow = Workflow.from_file(path_workflow)
             workflow.check_consistency()
             workflow.dissolve(not explain_rerun)
             await reporter("WORKFLOW", f"Loaded from {path_workflow}")
@@ -204,44 +207,43 @@
             await reporter("WORKFLOW", f"Exception while loading workflow {path_workflow}.", pages)
             workflow = None
     if workflow is None:
         dir_workflow = path_workflow.dirname()
         if len(dir_workflow) > 0 and dir_workflow != ".":
             dir_workflow.makedirs_p()
         workflow = Workflow.from_scratch()
-    scheduler = Scheduler(workflow.queue, workflow.queue_changed)
+
+    # Create components
+    scheduler = Scheduler(workflow.job_queue, workflow.job_queue_changed)
     scheduler.num_workers = num_workers
+    watcher = Watcher(workflow, reporter, workflow.dir_queue)
     runner = Runner(
-        scheduler, workflow, path_workflow, reporter, director_socket_path, show_perf, explain_rerun
+        watcher,
+        scheduler,
+        workflow,
+        path_workflow,
+        reporter,
+        director_socket_path,
+        show_perf,
+        explain_rerun,
     )
-    watcher = Watcher(workflow, reporter)
-
-    # Start tasks and wait for them to complete
     stop_event = asyncio.Event()
-    cycle = asyncio.create_task(cycle_run_watch(runner, watcher, stop_event), name="run-watch loop")
     director_handler = DirectorHandler(scheduler, workflow, runner, watcher, path_plan, stop_event)
-
-    # Add the initial plan
     director_handler.define_boot()
 
-    # Start RPC task
-    rpc_director = asyncio.create_task(
-        serve_socket_rpc(director_handler, director_socket_path, stop_event), name="director-rpc"
-    )
+    # Start tasks and wait for them to complete
+    watcher_loop = watcher.loop(stop_event)
+    runner_loop = runner.loop(stop_event)
+    rpc_director = serve_socket_rpc(director_handler, director_socket_path, stop_event)
     try:
-        await asyncio.gather(cycle, rpc_director)
+        await asyncio.gather(watcher_loop, runner_loop, rpc_director)
     finally:
         await reporter("DIRECTOR", "Stopping workers.")
         await runner.stop_workers()
-
-
-async def cycle_run_watch(runner: Runner, watcher: Watcher, stop_event: asyncio.Event):
-    while not stop_event.is_set():
-        await runner.loop()
-        await watcher.loop()
+        director_socket_path.remove_p()
 
 
 @attrs.define
 class DirectorHandler:
     _scheduler: Scheduler = attrs.field()
     _workflow: Workflow = attrs.field()
     _runner: Runner = attrs.field()
@@ -250,14 +252,15 @@
     _stop_event: asyncio.Event = attrs.field()
 
     #
     # For building up the workflow
     #
 
     def define_boot(self):
+        """Define the initial plan.py as static file and create a step for it."""
         if Path(self._path_plan).absolute().parent != Path.cwd():
             raise ValueError("The plan script must be in the current directory.")
         self.static("root:", [self._path_plan])
         self.step(
             "root:",
             f"./{self._path_plan}",
             [self._path_plan],
@@ -268,14 +271,15 @@
             False,
             None,
             False,
         )
 
     @contextlib.contextmanager
     def _dissolve_if_graph_changed(self):
+        """A context manager that will dissolve the workflow is errors were after making changes."""
         self._workflow.graph_changed = False
         try:
             yield
         except Exception:
             if self._workflow.graph_changed:
                 self._scheduler.drain()
                 self._runner.dissolve_after_dump = True
@@ -283,28 +287,27 @@
 
     @allow_rpc
     def static(self, creator_key: str, paths: list[str]):
         """Add a list of absolute static paths to the workflow.
 
         They are stored internal as paths relative to STEPUP_ROOT.
         """
-        if self._runner.phase.is_set(Phase.WATCH):
-            raise GraphError("A static file cannot be declared in watch phase.")
         with self._dissolve_if_graph_changed():
             self._workflow.declare_static(creator_key, paths)
 
     @allow_rpc
     def nglob(self, creator_key: str, ngm_data: list, strings: list[str]):
-        """Register a number of glob patterns to be watched."""
+        """Register a glob patterns to be watched."""
         with self._dissolve_if_graph_changed():
             ngm = NGlobMulti.structure(ngm_data, strings)
             self._workflow.register_nglob(creator_key, ngm)
 
     @allow_rpc
     def defer(self, creator_key: str, patterns: list[str]):
+        """Register a deferred glob."""
         with self._dissolve_if_graph_changed():
             self._workflow.defer_glob(creator_key, patterns)
 
     @allow_rpc
     def step(
         self,
         creator_key: str,
@@ -314,18 +317,23 @@
         out_paths: list[str],
         vol_paths: list[str],
         workdir: str,
         optional: bool,
         pool: str | None,
         block: bool,
     ) -> str:
-        """See ``stepup.core.api.step``."""
+        """Create a step in the workflow.
+
+        Notes
+        -----
+        This is an RPC wrapper for `Workflow.define_step` with a few additional sanity checks:
+        - The pool must exist.
+        - The working directory must exist.
+        """
         # If the pool is unknown, raise an error
-        if self._runner.phase.is_set(Phase.WATCH):
-            raise GraphError(f"A step cannot be defined in watch phase: {command}")
         if not self._scheduler.has_pool(pool):
             raise GraphError(f"Unknown pool name: {pool}")
         if not workdir.endswith(os.sep):
             raise GraphError(f"A working directory must end with a separator, got: {workdir}")
         with self._dissolve_if_graph_changed():
             return self._workflow.define_step(
                 creator_key,
@@ -338,118 +346,183 @@
                 optional,
                 pool,
                 block,
             )
 
     @allow_rpc
     def pool(self, name: str, size: int):
-        """See ``stepup.core.api.pool``."""
+        """Define a pool with given name and size.
+
+        Notes
+        -----
+        This is an RPC wrapper for `Scheduler.set_pool`.
+        """
         self._scheduler.set_pool(name, size)
 
     @allow_rpc
     def amend(
         self,
         step_key: str,
         inp_paths: list[str],
         env_vars: set[str],
         out_paths: list[str],
         vol_paths: list[str],
     ) -> bool:
-        """See ``stepup.core.api.amend``."""
-        if self._runner.phase.is_set(Phase.WATCH):
-            raise GraphError(f"A step cannot be amended in watch phase: {step_key}")
+        """Amend a step.
+
+        Notes
+        -----
+        This is an RPC wrapper for `Workflow.amend_step`.
+        """
         with self._dissolve_if_graph_changed():
             return self._workflow.amend_step(step_key, inp_paths, env_vars, out_paths, vol_paths)
 
     #
     # For interactive use
     #
 
     @allow_rpc
     async def shutdown(self):
-        """See ``stepup.core.api.shutdown``."""
+        """Shut down the director and worker processes."""
+        self._stop_event.set()
         self._scheduler.drain()
         self._watcher.interrupt.set()
-        self._stop_event.set()
 
     @allow_rpc
     async def drain(self):
-        """See ``stepup.core.api.shutdown``."""
+        """Do not start new steps and switch to the watch phase after the steps completed.
+
+        Notes
+        -----
+        This RPC blocks until all running steps have completed.
+        """
         self._scheduler.drain()
-        await self._runner.phase.wait(Phase.WATCH)
+        await self._watcher.active.wait()
 
     @allow_rpc
     async def join(self):
-        """See ``stepup.core.api.join``."""
-        await self._runner.phase.wait(Phase.WATCH)
+        """Block until the runner completed all (runnable) steps and shut down."""
+        await self._watcher.active.wait()
         await self.shutdown()
 
     @allow_rpc
-    async def run(self):
-        """See ``stepup.core.api.run``."""
-        # No point in starting run phase when the runner is active.
-        if self._runner.phase.is_set(Phase.RUN):
-            return
-        self._watcher.interrupt.set()
-        # Only return after the runner loop has started.
-        self._scheduler.resume()
-        await self._runner.phase.wait(Phase.RUN)
-
-    @allow_rpc
-    def graph(self, path_graph: str):
+    def graph(self, prefix: str):
         """Write out the graph in text format."""
-        with open(path_graph, "w") as fh:
+        with open(f"{prefix}.txt", "w") as fh:
             print(self._workflow.format_str(), file=fh)
+        with open(f"{prefix}_creator.dot", "w") as fh:
+            print(self._workflow.format_dot_creator(), file=fh)
+        with open(f"{prefix}_supplier.dot", "w") as fh:
+            print(self._workflow.format_dot_supplier(), file=fh)
 
     @allow_rpc
-    async def from_scratch(self):
-        """Remove all recordings and run everything again."""
-        # No point in starting run phase when the runner is active.
-        if self._runner.phase.is_set(Phase.RUN):
+    def from_scratch(self):
+        """Remove all recordings and run everything again.
+
+        Notes
+        -----
+        This has no effect during the run phase.
+        """
+        if not self._watcher.active.is_set():
             return
         self._workflow.discard_recordings()
-        await self.try_replay()
+        self.try_replay()
 
     @allow_rpc
-    async def try_replay(self):
-        """Make all steps pending and try replaying them. When needed, steps are rerun instead."""
-        # No point in starting run phase when the runner is active.
-        if self._runner.phase.is_set(Phase.RUN):
+    def try_replay(self):
+        """Make all steps pending and try replaying them. When needed, steps are rerun instead.
+
+        Notes
+        -----
+        This has no effect during the run phase.
+        """
+        if not self._watcher.active.is_set():
             return
         self._workflow.dissolve()
-        self._watcher.interrupt.set()
-        # This is a bit hacky: make runner active to be able to modify the workflow,
-        # which is normally only done in run phase.
-        self._runner.phase.set(Phase.RUN)
         self.define_boot()
-        self._runner.phase.set(Phase.WATCH)
+        self.run()
+
+    @allow_rpc
+    def run(self):
+        """Run pending steps (based on file changes observed in the watch phase).
+
+        Notes
+        -----
+        This has no effect during the run phase.
+        """
+        if not self._watcher.active.is_set():
+            return
+        self._watcher.interrupt.set()
         self._scheduler.resume()
-        await self._runner.phase.wait(Phase.RUN)
+        self._runner.resume.set()
+
+    @allow_rpc
+    async def cleanup(self, paths: list[str]) -> tuple[int, int]:
+        """Recursively clean up outputs (consumer files and directories).
+
+        Parameters
+        ----------
+        paths
+            A list of paths to consider for removal.
+
+        Returns
+        -------
+        numf
+            The number of files effectively removed.
+        numd
+            The number of directories effectively removed.
+        """
+        if not self._watcher.active.is_set():
+            raise ValueError("Cleanup is only allowed in the watch phase.")
+        initial_keys = []
+        for path in paths:
+            key = f"file:{path}"
+            if key not in self._workflow.nodes:
+                raise ValueError(f"Path not known to workflow: {path}")
+            initial_keys.append(key)
+        visited = set()
+        for key in initial_keys:
+            self._workflow.walk_consumers(key, visited)
+
+        numf = 0
+        numd = 0
+        for key in sorted(visited, reverse=True):
+            if key.startswith("file:"):
+                file = self._workflow.get_file(key)
+                if file.get_state(self._workflow) not in (FileState.STATIC, FileState.MISSING):
+                    remove_path(file.path)
+                    if file.path.endswith("/"):
+                        numd += 1
+                    else:
+                        numf += 1
+        return numf, numd
 
     @allow_rpc
-    async def watch_add(self, path: str):
-        """Wait for a file to be added by the watcher."""
+    async def watch_update(self, path: str):
+        """Block until the watcher observed an update of the file."""
         path = mynormpath(path)
-        while not self._watcher.interrupt.is_set():
-            if path in self._watcher.added:
+        await self._watcher.active.wait()
+        while True:
+            if path in self._watcher.updated:
                 return
-            self._watcher.changed.clear()
-            await self._watcher.changed.wait()
+            self._watcher.files_changed.clear()
+            await self._watcher.files_changed.wait()
 
     @allow_rpc
-    async def watch_del(self, path: str):
-        """Wait for a file to be deleted by the watcher."""
+    async def watch_delete(self, path: str):
+        """Block until the watcher observed the deletion of the file."""
         path = mynormpath(path)
-        while not self._watcher.interrupt.is_set():
+        await self._watcher.active.wait()
+        while True:
             if path in self._watcher.deleted:
                 return
-            self._watcher.changed.clear()
-            await self._watcher.changed.wait()
+            self._watcher.files_changed.clear()
+            await self._watcher.files_changed.wait()
 
     @allow_rpc
     async def wait(self):
-        """See ``stepup.core.api.wait``."""
-        await self._runner.phase.wait(Phase.WATCH)
+        """Block until the runner completed all (runnable) steps."""
+        await self._watcher.active.wait()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `stepup-1.0.0/stepup/core/exceptions.py` & `stepup-1.1.0/stepup/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/stepup/core/file.py` & `stepup-1.1.0/stepup/core/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""StepUp files are inputs or outputs of steps."""
+"""A `File` is StepUp's node for an input or output file of a step."""
 
 import enum
 from typing import Any, Self, Iterator, TYPE_CHECKING
 
 import attrs
 from path import Path
 
@@ -84,16 +84,14 @@
         return path
 
     @classmethod
     def structure(cls, workflow: "Workflow", strings: list[str], data: dict) -> Self:
         state = FileState(data.pop("s"))
         file = cls(path=strings[data["p"]], hash=FileHash.structure(data["h"]))
         file.set_state(workflow, state)
-        if file._path.endswith("/"):
-            workflow._used_directories.add(file._path)
         return file
 
     def unstructure(self, workflow: "Workflow", lookup: dict[str, int]) -> dict:
         return {
             "p": lookup[self._path],
             "s": self.get_state(workflow).value,
             "h": self.hash.unstructure(),
@@ -108,35 +106,35 @@
             yield "", l2
 
     #
     # Overridden from base class
     #
 
     def recycle(self, workflow: "Workflow", old: Self | None):
-        if old is None:
-            # Bookkeeping relevant directories
-            if self._path.endswith("/"):
-                workflow._used_directories.add(self._path)
-        else:
+        if old is not None:
             # Recycle hash
             self.hash = old.hash
 
     def orphan(self, workflow: "Workflow"):
         for step_key in workflow.get_consumers(self.key, kind="step"):
             step = workflow.get_step(step_key)
             step.make_pending(workflow)
+            # When inputs of a step are orphaned,
+            # amended information becomes unreliable because the orphaned
+            # nodes may have been created by the step.
+            step.clean_before_run(workflow)
 
     def cleanup(self, workflow: "Workflow"):
         if self._path.endswith("/"):
-            workflow._used_directories.discard(self._path)
+            workflow.dir_queue.put_nowait((True, self._path))
         state = self.get_state(workflow)
         if state == FileState.VOLATILE:
             workflow.to_be_deleted.append((self._path, None))
         elif state in (FileState.PENDING, FileState.BUILT):
-            if self.hash.digest not in (b"u", b"m"):
+            if self.hash.digest != b"u":
                 workflow.to_be_deleted.append((self._path, self.hash))
         workflow.file_states.discard(self.key, insist=True)
 
     #
     # File state
     #
 
@@ -147,25 +145,34 @@
         workflow.file_states[self.key] = new_state
 
     #
     # Run phase
     #
 
     def release_pending(self, workflow: "Workflow"):
-        """Check all steps using this one as input and queue them if possible."""
+        """Check all steps using this one as input and queue them if possible.
+
+        In case of a directory, also notify the watcher by putting it on the dir_queue.
+        """
         for step_key in sorted(workflow.get_consumers(self.key, kind="step")):
             step = workflow.get_step(step_key)
             step.validate_amended = True
             step.queue_if_appropriate(workflow)
+        if self.path.endswith("/"):
+            workflow.dir_queue.put_nowait((False, self.path))
 
     #
     # Watch phase
     #
 
     def watcher_deleted(self, workflow: "Workflow"):
+        """Modify the graph to account for the fact this was deleted.
+
+        Hashes are not removed in case the file is restored by the user with the same contents.
+        """
         state = self.get_state(workflow)
         if state == FileState.MISSING:
             raise ValueError(f"Cannot delete a path that is already MISSING: {self._path}")
         if state == FileState.STATIC:
             self.set_state(workflow, FileState.MISSING)
         elif state == FileState.BUILT:
             self.set_state(workflow, FileState.PENDING)
@@ -174,15 +181,20 @@
         else:
             # No action needed when a PENDING or VOLATILE file is deleted.
             return
         # Make all consumers pending
         for step_key in workflow.get_consumers(self.key, kind="step"):
             workflow.get_step(step_key).make_pending(workflow)
 
-    def watcher_added(self, workflow: "Workflow"):
+    def watcher_updated(self, workflow: "Workflow"):
+        """Modify the graph to account for the fact that this file changed on disk.
+
+        Hashes are not updated until needed, to allow for reverting the file in its original
+        form. (This is more common than one may thing, e.g. when switching Git branches.)
+        """
         state = self.get_state(workflow)
         if state == FileState.MISSING:
             self.set_state(workflow, FileState.STATIC)
             state = FileState.STATIC
         if state == FileState.STATIC:
             # Make all consumers pending
             for step_key in workflow.get_consumers(self.key, kind="step"):
```

### Comparing `stepup-1.0.0/stepup/core/hash.py` & `stepup-1.1.0/stepup/core/hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""File and Step hashing."""
+"""File and step hashing."""
 
 import hashlib
 import os
 import stat
 from typing import Self
 
 import attrs
```

### Comparing `stepup-1.0.0/stepup/core/interact.py` & `stepup-1.1.0/stepup/core/interact.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,45 +13,74 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Application programming interface to the director to simulate interactive use.
+"""Application Programming Interface (API) for interactive use of the director process.
 
 Most of these functions are used for writing tests.
-They can also be used to create keyboard shortcuts in your IDE to control StepUp.
-"""
+They can also be employed to create keyboard shortcuts within your IDE.
+
+For example, one may bind the following command to an IDE's keyboard shortcut:
 
+```bash
+python -c 'from stepup.core.interact import run; run()'
+```
+
+This command must be executed in the top-level directory
+where a `stepup` command is running in interactive mode.
+"""
 
-from .api import RPC_CLIENT
 
+from .api import RPC_CLIENT, translate
 
-__all__ = ("run", "graph", "watch_add", "watch_del", "wait", "join")
+__all__ = ("run", "cleanup", "graph", "watch_update", "watch_delete", "wait", "join")
 
 
 def run():
     """Exit the watch phase and start running steps whose inputs have changed."""
     RPC_CLIENT.call.run()
 
 
-def graph(path: str):
-    """Write the workflow graph in text format to a file."""
-    return RPC_CLIENT.call.graph(path)
-
-
-def watch_add(path: str):
-    """Block until the watcher has observed the addition of file."""
-    RPC_CLIENT.call.watch_add(path, _rpc_timeout=None)
-
+def cleanup(*paths: str) -> tuple[int, int]:
+    """Remove paths (if they are outputs), recursively removing all consumer files and directories.
 
-def watch_del(path: str):
-    """Block until the watcher has observed the deletion of a file."""
-    RPC_CLIENT.call.watch_del(path, _rpc_timeout=None)
+    Parameters
+    ----------
+    paths
+        A list of paths to consider for removal.
+        Variable substitutions are not supported.
+
+    Returns
+    -------
+    numf
+        The number of files effectively removed.
+    numd
+        The number of directories effectively removed.
+    """
+    # Translate paths to directory working dir and make RPC call
+    tr_paths = sorted(translate(path) for path in paths)
+    return RPC_CLIENT.call.cleanup(tr_paths)
+
+
+def graph(prefix: str):
+    """Write the workflow graph files in text and dot formats."""
+    return RPC_CLIENT.call.graph(prefix)
+
+
+def watch_update(path: str):
+    """Block until the watcher has observed an update of the file."""
+    RPC_CLIENT.call.watch_update(path, _rpc_timeout=None)
+
+
+def watch_delete(path: str):
+    """Block until the watcher has observed the deletion of the file."""
+    RPC_CLIENT.call.watch_delete(path, _rpc_timeout=None)
 
 
 def wait():
     """Block until the runner has become idle."""
     RPC_CLIENT.call.wait(_rpc_timeout=None)
```

### Comparing `stepup-1.0.0/stepup/core/job.py` & `stepup-1.1.0/stepup/core/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Definition of a job to be executed by a worker."""
+"""Definition of jobs to be executed by a worker."""
 
 
 from typing import TYPE_CHECKING
 import attrs
 
 if TYPE_CHECKING:
     from .worker import WorkerClient
@@ -69,15 +69,14 @@
     def coro(self, worker: "WorkerClient"):
         return worker.validate_amended_job(self._step_key)
 
     def finalize(self, must_run: bool, scheduler: "Scheduler", workflow: "Workflow"):
         if must_run:
             run_job = RunJob(self._step_key, self._pool)
             scheduler.inqueue.put_nowait(run_job)
-            # TODO: needed?
             scheduler.changed.set()
 
 
 @attrs.define
 class TryReplayJob(Job):
     _step_key: str = attrs.field()
     _pool: str | None = attrs.field()
@@ -96,15 +95,14 @@
     def coro(self, worker: "WorkerClient"):
         return worker.try_replay_job(self._step_key)
 
     def finalize(self, must_run: bool, scheduler: "Scheduler", workflow: "Workflow"):
         if must_run:
             run_job = RunJob(self._step_key, self._pool)
             scheduler.inqueue.put_nowait(run_job)
-            # TODO: needed?
             scheduler.changed.set()
 
 
 @attrs.define
 class RunJob(Job):
     _step_key: str = attrs.field()
     _pool: str | None = attrs.field()
```

### Comparing `stepup-1.0.0/stepup/core/nglob.py` & `stepup-1.1.0/stepup/core/nglob.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,72 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Glob with named back-reference support.
 
-A named glob (nglob) pattern may contain the following:
+Named glob (NGlob) patterns are an advanced form of pattern matching
+that supports back referencing of previously matched substrings.
 
-- ``${*name}`` is a named wildcard. Optionally, the name can be associated with a glob pattern.
-  When no pattern is specified for a name, the default is ``*``.
-  When a name appears twice in a named glob pattern (or multiple named glob patterns),
-  the same value must be present for each placeholder to get a match.
-- One may also specify a set of named glob patterns, enforcing consistency between their names.
-- Regular wildcards are also allowed and are called "anonymous wildcards"
-  to clarify the distinction with named wildcards.
+It has the following use cases:
+
+- **Single named wildcard:**
+    By default, the wildcard `${*name}` is a placeholder for any string.
+    One may also specify a pattern for `${*name}` through optional arguments.
+    For example:
+
+    ```python
+    ngs = NGlobSingle("feedback_${*idx}.md", idx="[0-9][0-9][0-9]")
+    ngs.glob()
+    print(ngs.results)
+    ```
+
+- **Consistency within one pattern:**
+    If a pattern uses the same named globs multiple times,
+    the matching substring must also be consistent.
+    For example:
+
+    ```python
+    ngs = NGlobSingle("archive_${*idx}/feedback_${*idx}.md", idx="[0-9][0-9][0-9]")
+    ngs.glob()
+    print(ngs.results)
+    ```
+
+    These would match:
+
+    - `archive_042/feedback_042.md`
+    - `archive_777/feedback_777.md`
+
+    This won't match:
+
+    - `archive_042/feedback_777.md`
+
+- **Consistency across multiple patterns:**
+    One can define multiple patterns and enforce consistency between their matches.
+    For example:
+
+    ```python
+    ngm = NGlobMulti("feedback_${*idx}.md", "report_${*idx}.pdf", idx="[0-9][0-9][0-9]")
+    ngm.glob()
+    print(ngm.results)
+    ```
+
+    This will produce pairs of matches (provided the files are present).
+    For example, the following would match:
+
+    - `feedback_001.md` with `report_001.pdf`
+    - `feedback_123.md` with `report_123.pdf`
+
+    The following won't be in the results, despite the fact that the files exist:
+
+    - `feedback_001.md` with `report_123.pdf`
+
+- Conventional glob wildcards are also allowed and are called "anonymous wildcards"
+  to clarify the distinction from named wildcards.
 """
 
 import copy
 import glob
 import re
 from typing import Iterator, Iterable, Self, Collection, Any
 
@@ -423,31 +472,31 @@
                 added_new.difference_update(paths)
         for ngs in self._nglob_singles:
             for path in added_new:
                 if ngs.regex.fullmatch(path):
                     return True
         return False
 
-    def will_change(self, deleted: Collection[str], added: Collection[str]) -> bool:
+    def will_change(self, deleted: Collection[str], updated: Collection[str]) -> bool:
         """Determine whether the results may change after deleting or adding files.
 
         Parameters
         ----------
         deleted
             Set of files to be deleted.
-        added
-            Set of files to be added.
+        updated
+            Set of files to be added or changed.
 
         Returns
         -------
         will_change
             True if the NGlobMulti results will change.
         """
         evolved = self.deepcopy()
-        evolved.extend(added)
+        evolved.extend(updated)
         evolved.reduce(deleted)
         return not evolved.equals(self)
 
 
 def convert_nglob_to_regex(
     pattern: str, subs: dict[str, str] | None = None, allow_names: bool = True
 ) -> str:
```

### Comparing `stepup-1.0.0/stepup/core/reporter.py` & `stepup-1.1.0/stepup/core/reporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Progress monitoring."""
+"""Terminal output of StepUp's runner progress and observed file changes."""
 
 
 import asyncio
 import contextlib
 from collections import Counter
 from time import perf_counter
 from typing import Self
@@ -54,15 +54,15 @@
 
     async def __call__(
         self, action: str, description: str, pages: list[tuple[str, str]] | None = None
     ):
         if self.client is not None:
             if pages is None:
                 pages = {}
-            await self.client.call.reporter(action, description, pages)
+            await self.client.call.report(action, description, pages)
 
     async def set_num_workers(self, num_workers: int):
         if self.client is not None:
             await self.client.call.set_num_workers(num_workers)
 
     async def update_step_counts(self, step_counter: Counter[StepState, int]):
         if self.client is not None:
@@ -88,15 +88,15 @@
     show_perf: bool = attrs.field()
     stop_event: asyncio.Event = attrs.field(factory=asyncio.Event)
     _num_workers: int = attrs.field(init=False, default=0)
     _step_counts: Counter[StepState, int] = attrs.field(init=False, factory=Counter)
     _num_digits: int = attrs.field(init=False, default=3)
     console: Console = attrs.field(init=False)
     progress_bar: ProgressBar = attrs.field(init=False)
-    running_id_step: TaskID = attrs.field(init=False)
+    task_id_running: TaskID = attrs.field(init=False)
     task_id_step: TaskID = attrs.field(init=False)
     start: float = attrs.field(init=False, factory=perf_counter)
 
     @console.default
     def _default_console(self):
         theme = Theme(
             {
@@ -107,52 +107,54 @@
         )
         return Console(highlight=False, theme=theme)
 
     @progress_bar.default
     def _default_progress_bar(self):
         progress_bar = ProgressBar(
             TextColumn("{task.description}"),
-            BarColumn(self.console.width),
+            BarColumn(None),
             MofNCompleteColumn(),
             transient=True,
             console=self.console,
         )
         progress_bar.start()
         return progress_bar
 
-    @running_id_step.default
-    def _default_running_id_step(self):
-        return self.progress_bar.add_task("🛠️ ", total=0, visible=True)
+    @task_id_running.default
+    def _default_task_id_running(self):
+        return self.progress_bar.add_task("🛠 ", total=0, visible=True)
 
     @task_id_step.default
     def _default_task_id_step(self):
-        return self.progress_bar.add_task("✔️ ", total=0, visible=True)
+        return self.progress_bar.add_task("✔ ", total=0, visible=True)
 
     @allow_rpc
     def shutdown(self):
         self.progress_bar.stop()
         self.stop_event.set()
 
     @allow_rpc
-    def reporter(self, action: str, description: str, pages: list[tuple[str, str]]):
+    def report(self, action: str, description: str, pages: list[tuple[str, str]]):
         # Progress bar
         nsuc = self._step_counts[StepState.SUCCEEDED]
         nrun = self._step_counts[StepState.RUNNING]
         npen = self._step_counts[StepState.PENDING] + self._step_counts[StepState.QUEUED]
         nd = max(self._num_digits, len(str(nsuc)), len(str(nrun)), len(str(npen)))
         self._num_digits = nd
-        self.progress_bar.update(self.running_id_step, completed=nrun, total=self._num_workers)
+        self.progress_bar.update(self.task_id_running, completed=nrun, total=self._num_workers)
         self.progress_bar.update(self.task_id_step, completed=nsuc, total=nsuc + nrun + npen)
 
         # Action info
         action_color = {
             "START": "blue",
             "FAIL": "red",
             "ERROR": "red",
             "SUCCESS": "green",
+            "DELETED": "yellow",
+            "UPDATED": "yellow",
             "SKIP": "cyan",
             "NOSKIP": "cyan",
             "RESCHEDULE": "yellow",
             "DROPAMEND": "yellow",
             "WARNING": "yellow",
             "PHASE": "white",
         }.get(action, "magenta")
```

### Comparing `stepup-1.0.0/stepup/core/rpc.py` & `stepup-1.1.0/stepup/core/rpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,35 +20,31 @@
 """Lightweight and versatile RPC implementation using asyncio stream reader and writer.
 
 This module also includes a synchronous RPC client to support simple client APIs.
 """
 
 
 import inspect
-import os
-import sys
 import traceback
 import asyncio
 import subprocess
 import pickle
 import socket
 from functools import partial
 from typing import Any, Callable, Collection, Awaitable
 
 import attrs
 
+from .asyncio import stoppable_iterator, stdio
 from .exceptions import RPCError
 
 
 __all__ = (
     "fmt_rpc_call",
     "allow_rpc",
-    "stoppable_iterator",
-    "stdio",
-    "pipe",
     "serve_rpc",
     "serve_socket_rpc",
     "serve_stdio_rpc",
     "BaseAsyncRPCClient",
     "AsyncRPCClient",
     "DummyAsyncRPCClient",
     "BaseSyncRPCClient",
@@ -77,120 +73,14 @@
 
 def allow_rpc(func):
     func._allow_rpc = True
     return func
 
 
 #
-# Stoppable async loop
-#
-
-
-async def stoppable_iterator(get_next, stop_event: asyncio.Event, args=()):
-    """Iterate over messages received by calling awaitable get_next until stop_event is set.
-
-    Parameters
-    ----------
-    get_next
-        An awaitable that returns the next iteration.
-    stop_event
-        When set, the loop is interrupted.
-    args
-        A list of arguments to pass into get_next.
-    """
-    stop_task = asyncio.create_task(stop_event.wait(), name="stop_task")
-    while True:
-        future = asyncio.ensure_future(get_next(*args))
-        done, pending = await asyncio.wait([future, stop_task], return_when=asyncio.FIRST_COMPLETED)
-        if stop_task in done and future in pending:
-            await stop_task
-            stop_task.result()
-            future.cancel()
-            break
-        yield await future
-
-
-#
-# Setting up reader and writer pairs, other than those provided by asyncio.
-#
-
-
-async def stdio(
-    limit=asyncio.streams._DEFAULT_LIMIT, loop=None
-) -> tuple[asyncio.StreamReader, asyncio.StreamWriter]:
-    """Create a reader and writer connected to stdin and stdout.
-
-    Adapted from:
-    https://stackoverflow.com/questions/52089869/
-    how-to-create-asyncio-stream-reader-writer-for-stdin-stdout
-
-    Parameters
-    ----------
-    limit
-        The maximum buffers size.
-    loop
-        The event loop. When not given `asyncio.get_event_loop()` is
-        called, which is usually just fine.
-
-    Returns
-    -------
-    reader
-        The StreamReader connected to standard input.
-    writer
-        The StreamWriter connected to standard output.
-    """
-    if loop is None:
-        loop = asyncio.get_event_loop()
-    reader = asyncio.StreamReader(limit=limit, loop=loop)
-    await loop.connect_read_pipe(lambda: asyncio.StreamReaderProtocol(reader, loop=loop), sys.stdin)
-    writer_transport, writer_protocol = await loop.connect_write_pipe(
-        lambda: asyncio.streams.FlowControlMixin(loop=loop), os.fdopen(sys.stdout.fileno(), "wb")
-    )
-    writer = asyncio.streams.StreamWriter(writer_transport, writer_protocol, None, loop)
-    return reader, writer
-
-
-async def pipe(
-    limit=asyncio.streams._DEFAULT_LIMIT, loop=None
-) -> tuple[asyncio.StreamReader, asyncio.StreamWriter]:
-    """Create a connected reader and writer through `os.pipe`.
-
-    This is mainly useful for testing, to setup an RPC client and server within one test function.
-    Testing the RPC code involves two of these pipes, to set up bidirectional communication.
-
-    Parameters
-    ----------
-    limit
-        The maximum buffers size.
-    loop
-        The event loop. When not given `asyncio.get_event_loop()` is
-        called, which is usually just fine.
-
-    Returns
-    -------
-    reader
-        The StreamReader taking data out of the pipe.
-    writer
-        The StreamWriter putting data into the pipe.
-    """
-    if loop is None:
-        loop = asyncio.get_event_loop()
-    fd_in, fd_out = os.pipe()
-    pipe_in = open(fd_in)
-    pipe_out = open(fd_out)
-    reader = asyncio.StreamReader(limit=limit, loop=loop)
-    await loop.connect_read_pipe(lambda: asyncio.StreamReaderProtocol(reader, loop=loop), pipe_in)
-    writer_transport, writer_protocol = await loop.connect_write_pipe(
-        lambda: asyncio.streams.FlowControlMixin(loop=loop), pipe_out
-    )
-    writer = asyncio.streams.StreamWriter(writer_transport, writer_protocol, None, loop)
-    return reader, writer
-
-
-#
 # RPC message protocol
 #
 
 
 async def _recv_rpc_message(reader: asyncio.StreamReader) -> tuple[int | None, bytes | None]:
     """Read a single RPC request.
 
@@ -576,16 +466,38 @@
         size = int.from_bytes(self._readexactly(8))
         if size == 0:
             raise ValueError("RPC clients should never receive a closing message.")
         body = self._readexactly(size)
         return body
 
     def _readexactly(self, size: int) -> bytes:
+        """Keep reading from the socket until (at least) size bytes were received.
+
+        Parameters
+        ----------
+        size
+            The length of the byte sequence to receive.
+
+        Raises
+        ------
+        ConectionResetError
+            When the socket returns zero bytes, the connection is lost and this error is raised.
+
+        Returns
+        -------
+        data
+            The bytes read from the socket of the requested size.
+            Any additional data received from the socket is stored for the
+            following call to `_readexactly`.
+        """
         while len(self._partial_recv) < size:
-            self._partial_recv += self._socket.recv(4096)
+            fragment = self._socket.recv(4096)
+            if len(fragment) == 0:
+                raise ConnectionResetError()
+            self._partial_recv += fragment
         result = self._partial_recv[:size]
         self._partial_recv = self._partial_recv[size:]
         return result
 
 
 @attrs.define
 class DummySyncRPCClient(BaseSyncRPCClient):
```

### Comparing `stepup-1.0.0/stepup/core/runner.py` & `stepup-1.1.0/stepup/core/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,103 +13,161 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Execute tasks."""
+"""The `Runner` delegates the execution of jobs by the workers."""
+
 
 import asyncio
-import enum
 import logging
 from functools import partial
 
 import attrs
 from path import Path
 
+from .asyncio import wait_for_events
 from .hash import FileHash
 from .job import Job
 from .reporter import ReporterClient
 from .scheduler import Scheduler
 from .step import StepState, Mandatory
-from .utils import MultiEvent
+from .utils import remove_path
+from .watcher import Watcher
 from .worker import WorkerClient
 from .workflow import Workflow
 
 
-__all__ = ("Runner", "Phase")
-
-
-class Phase(enum.Enum):
-    RUN = 1000
-    WATCH = 2000
+__all__ = ("Runner",)
 
 
 @attrs.define
 class Runner:
+    # The watcher instance, used to start the watcher when the runner becomes idle.
+    watcher: Watcher = attrs.field()
+
+    # The scheduler providing jobs to the runner.
     scheduler: Scheduler = attrs.field()
+
+    # The workflow which generated the jobs and which gets updated as a result of the jobs.
     workflow: Workflow = attrs.field()
+
+    # The location of the workflow file (is written after the runner becomes idle).
     path_workflow: Path = attrs.field()
+
+    # A reporter client for sending progress info to.
     reporter: ReporterClient = attrs.field()
+
+    # The path of the director socket, passed on to worker processes.
     director_socket_path: str = attrs.field()
+
+    # Flag to enable performance output after a worker executed a step.
     show_perf: bool = attrs.field()
+
+    # Flag to enable more details on why steps cannot be skipped.
     explain_rerun: bool = attrs.field()
-    phase: MultiEvent = attrs.field(init=False)
-    workers: dict[int, WorkerClient] = attrs.field(init=False, factory=dict)
+
+    # Other parts of StepUp can set the resume event to put the runner back to work.
+    resume: asyncio.Event = attrs.field(init=False, factory=asyncio.Event)
+
+    # A list of worker client objects, one for each worker process.
+    workers: list[WorkerClient] = attrs.field(init=False, factory=list)
+
+    # The list of active and idle workers (just integer indexes of the workers list).
     active_workers: set[int] = attrs.field(init=False, factory=set)
     idle_workers: set[int] = attrs.field(init=False, factory=set)
+
+    # Dictionary of asyncio tasks that interact with a worker client.
     running_worker_tasks: dict[asyncio.Task, Job] = attrs.field(init=False, factory=dict)
     done_worker_tasks: dict[asyncio.Task, Job] = attrs.field(init=False, factory=dict)
+
+    # Flag set when an error is raised halfway an RPC that changes the workflow.
+    # StepUp has no rollback mechanism, so this is the nuclear option to prevent
+    # StepUp from continuing with a half-baked workflow.
     dissolve_after_dump: bool = attrs.field(init=False, default=False)
 
-    @phase.default
-    def _default_phase(self):
-        return MultiEvent.from_values(Phase.RUN, Phase.WATCH)
+    async def loop(self, stop_event: asyncio.Event):
+        """The main runner loop.
 
-    async def loop(self):
+        Parameters
+        ----------
+        stop_event
+            The main runner loop is interrupted by this event.
+
+        Notes
+        -----
+        One iteration in the main runner loop consists of running a bunch of jobs:
+        All runnable jobs are executed unless the user interrupts the runner (drain command).
+        """
+        # Start workers
+        self.idle_workers.update(
+            await asyncio.gather(
+                *[self._launch_worker() for _ in range(self.scheduler.num_workers)]
+            )
+        )
+        # Loop through runner phases.
+        while True:
+            await self.job_loop()
+            await self.finalize()
+            self.resume.clear()
+            await wait_for_events(self.resume, stop_event, return_when=asyncio.FIRST_COMPLETED)
+            if stop_event.is_set():
+                return
+
+    async def job_loop(self):
+        """Run all runnable jobs unless the scheduler is drained while the runner is in progress."""
         await self.reporter.update_step_counts(self.workflow.get_step_counters())
         await self.reporter("PHASE", "run")
 
-        # Make clear to the rest of the code that the runner is working.
-        self.phase.set(Phase.RUN)
-
-        # Pre-launch workers (if more are needed)
-        num_launch = self.scheduler.num_workers - len(self.workers)
-        if num_launch > 0:
-            self.idle_workers.update(
-                await asyncio.gather(*[self._launch_worker() for _ in range(num_launch)])
-            )
-
         # Get step jobs and run them on the workers.
         while True:
-            # Get next step job and send it to workers if there is such a job.
+            # Get the next job and send it to workers if there is such a job.
             job, pool_name = self.scheduler.pop_runnable_job()
             if job is not None:
                 await self.send_to_worker(job, pool_name)
                 continue
 
             # When there is nothing left to do, the runner must stop.
             if (
                 self.scheduler.queues_empty
                 and len(self.running_worker_tasks) == 0
                 and len(self.done_worker_tasks) == 0
             ):
-                # Time to stop
-                await self.finalize()
                 return
 
             # If the runner needs to wait, there is time to handle exceptions of done tasks.
             self.handle_done_tasks()
 
             # After handling done tasks, the runner just waits until the scheduler has a new job,
             # or a task has completed.
             await self.scheduler.changed.wait()
             self.scheduler.changed.clear()
 
+    async def finalize(self):
+        """Final steps after the runner has executed a bunch of jobs."""
+        success = await report_completion(self.workflow, self.scheduler, self.reporter)
+        if success:
+            self.workflow.clean()
+            await remove_files(self.workflow.to_be_deleted, self.reporter)
+        else:
+            await self.reporter("WARNING", "Skipping cleanup due to incomplete build.")
+        self.workflow.to_file(self.path_workflow)
+        await self.reporter.update_step_counts(self.workflow.get_step_counters())
+        await self.reporter("WORKFLOW", f"Dumped to {self.path_workflow}")
+        if self.dissolve_after_dump:
+            await self.reporter(
+                "WARNING",
+                "Dissolving the workflow due to an exceptions while the graph was being changed.",
+            )
+            self.workflow.dissolve()
+            self.dissolve_after_dump = False
+        self.watcher.resume.set()
+
     async def send_to_worker(self, job: Job, pool_name: str):
         if len(self.idle_workers) > 0:
             worker_idx = self.idle_workers.pop()
         else:
             # Normally never needed because workers are pre-launched, but keeping to play safe.
             worker_idx = await self._launch_worker()
         worker = self.workers[worker_idx]
@@ -123,15 +181,15 @@
             self.workflow,
             self.reporter,
             self.director_socket_path,
             self.show_perf,
             self.explain_rerun,
             len(self.workers),
         )
-        self.workers[worker.idx] = worker
+        self.workers.append(worker)
         await worker.boot()
         await self.reporter("DIRECTOR", f"Launched worker {worker.idx}")
         return worker.idx
 
     def _task_done(self, task: asyncio.Task, worker_idx: int):
         job = self.running_worker_tasks.pop(task)
         self.done_worker_tasks[task] = job
@@ -147,70 +205,35 @@
             if exc is not None:
                 self.scheduler.drain()
                 msg = f"Exception in worker task {task.get_name()}"
                 raise RuntimeError(msg) from exc
             job.finalize(task.result(), self.scheduler, self.workflow)
             self.scheduler.changed.set()
 
-    async def finalize(self):
-        success = await report_completion(self.workflow, self.scheduler, self.reporter)
-        if success:
-            self.workflow.clean()
-            await remove_files(self.workflow.to_be_deleted, self.reporter)
-        else:
-            await self.reporter("WARNING", "Skipping cleanup due to incomplete build.")
-        self.workflow.to_file(self.path_workflow)
-        await self.reporter.update_step_counts(self.workflow.get_step_counters())
-        await self.reporter("WORKFLOW", f"Dumped to {self.path_workflow}")
-        if self.dissolve_after_dump:
-            await self.reporter(
-                "WARNING",
-                "Dissolving the workflow due to an exceptions while the graph was being changed.",
-            )
-            self.workflow.dissolve()
-            self.dissolve_after_dump = False
-        self.phase.set(Phase.WATCH)
-
     async def stop_workers(self):
         waits = []
         while len(self.idle_workers) > 0:
             worker_idx = self.idle_workers.pop()
-            worker = self.workers.pop(worker_idx)
+            worker = self.workers[worker_idx]
             await worker.shutdown()
             waits.append(worker.close())
         while len(self.active_workers) > 0:
             worker_idx = self.active_workers.pop()
-            worker = self.workers.pop(worker_idx)
+            worker = self.workers[worker_idx]
             await worker.shutdown()
             waits.append(worker.close())
         await asyncio.gather(*waits)
 
 
 async def remove_files(to_be_deleted: list[tuple[str, FileHash | None]], reporter: ReporterClient):
     to_be_deleted.sort(reverse=True)
     for path, file_hash in to_be_deleted:
-        path = Path(path)
-        if path.endswith("/"):
-            try:
-                path.rmdir()
+        if path.endswith("/") or file_hash is None or file_hash.update(path) is False:
+            if remove_path(Path(path)):
                 await reporter("CLEAN", path)
-            except FileNotFoundError:
-                logging.error(f"Stale directory not found: {path}")
-            except OSError:
-                logging.error(f"Stale directory not empty: {path}")
-        else:
-            # Volatile outputs have no hash, and are always cleaned up
-            if file_hash is None or file_hash.update(path) is False:
-                try:
-                    path.remove()
-                    await reporter("CLEAN", path)
-                except FileNotFoundError:
-                    logging.error(f"Stale file not found: {path}")
-                except OSError:
-                    logging.error(f"Stale file is a directory: {path}")
     to_be_deleted.clear()
 
 
 async def report_completion(workflow: Workflow, scheduler: Scheduler, reporter: ReporterClient):
     """Report parts of the workflow that could not be executed."""
     success = True
     step_keys_failed = workflow.step_states.inverse.get(StepState.FAILED, ())
```

### Comparing `stepup-1.0.0/stepup/core/scheduler.py` & `stepup-1.1.0/stepup/core/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Schedule steps."""
+"""The `Scheduler` plans the execution of jobs by the worker processes."""
 
 import asyncio
 import itertools
 
 import attrs
 
 from .job import Job
```

### Comparing `stepup-1.0.0/stepup/core/script.py` & `stepup-1.1.0/stepup/core/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,23 @@
 from path import Path
 
 
 __all__ = ("driver",)
 
 
 def driver(obj=None) -> int:
-    """Driver function to be called from script as ``driver()`` or ``driver(obj)``."""
+    """Driver function to be called from a script as `driver()` or `driver(obj)`.
+
+    Parameters
+    ----------
+    obj
+        When not provided, the namespace of the module where `driver` is defined
+        will be searched for names like 'info' and 'run' to implement the script protocol.
+        When an object is given as a parameter, its attributes are searched instead.
+    """
     frame = inspect.currentframe().f_back
     script_path = Path(frame.f_locals["__file__"]).relpath()
     if obj is None:
         # Get the calling module and use it as obj
         module_name = frame.f_locals["__name__"]
         obj = sys.modules.get(module_name)
         if obj is None:
```

### Comparing `stepup-1.0.0/stepup/core/step.py` & `stepup-1.1.0/stepup/core/step.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""StepUp steps are things that can be executed and have inputs and outputs."""
+"""A `Step` is a shell command that can be executed and that has inputs and outputs."""
 
 import enum
 from typing import Any, Self, Iterator, TYPE_CHECKING, Collection
 
 import attrs
 
 from .cascade import Node
@@ -78,15 +78,15 @@
     _pool: str | None = attrs.field(kw_only=True, default=None)
     # When True, the step will behave as it never has all dependencies satisfied.
     # This is convenient for lowering the build time when working on intermediate steps.
     _block: bool = attrs.field(kw_only=True, default=False)
 
     # Augment information in Workflow instance
     _amended_suppliers: set[str] = attrs.field(kw_only=True, factory=set)
-    _amended_products: set[str] = attrs.field(kw_only=True, factory=set)
+    _amended_consumers: set[str] = attrs.field(kw_only=True, factory=set)
 
     # Extra information, not in Workflow instance
     _initial_env_vars: set[str] = attrs.field(kw_only=True, factory=set)
     _amended_env_vars: set[str] = attrs.field(kw_only=True, factory=set)
     _nglob_multis: list[NGlobMulti] = attrs.field(kw_only=True, factory=list)
 
     # List of missing amended files causing reschedule
@@ -123,16 +123,16 @@
         return self._initial_env_vars
 
     @property
     def amended_suppliers(self) -> set[str]:
         return self._amended_suppliers
 
     @property
-    def amended_products(self) -> set[str]:
-        return self._amended_products
+    def amended_consumers(self) -> set[str]:
+        return self._amended_consumers
 
     @property
     def amended_env_vars(self) -> set[str]:
         return self._amended_env_vars
 
     @property
     def nglob_multis(self) -> list[NGlobMulti]:
@@ -172,15 +172,15 @@
         pool = data.get("p")
         if pool is not None:
             kwargs["pool"] = pool
         kwargs["block"] = data.get("b", False)
         initial_env_vars = data.get("i")
         if initial_env_vars is not None:
             kwargs["initial_env_vars"] = set(initial_env_vars)
-        for short, name in ("as", "amended_suppliers"), ("ao", "amended_products"):
+        for short, name in ("as", "amended_suppliers"), ("ac", "amended_consumers"):
             idxs = data.get(short)
             if idxs is not None:
                 kwargs[name] = {strings[idx] for idx in idxs}
         amended_env_vars = data.get("ai")
         if amended_env_vars is not None:
             kwargs["amended_env_vars"] = set(amended_env_vars)
         ngm_datas = data.get("g")
@@ -211,16 +211,16 @@
             data["p"] = self._pool
         if self._block:
             data["b"] = True
         if len(self._initial_env_vars) > 0:
             data["i"] = sorted(self._initial_env_vars)
         if len(self._amended_suppliers) > 0:
             data["as"] = sorted(lookup[key] for key in self._amended_suppliers)
-        if len(self._amended_products) > 0:
-            data["ao"] = sorted(lookup[key] for key in self._amended_products)
+        if len(self._amended_consumers) > 0:
+            data["ac"] = sorted(lookup[key] for key in self._amended_consumers)
         if len(self._amended_env_vars) > 0:
             data["ai"] = sorted(self._amended_env_vars)
         if len(self._nglob_multis) > 0:
             data["g"] = [nglob_multi.unstructure(lookup) for nglob_multi in self._nglob_multis]
         if self._hash is not None:
             data["h"] = self._hash.unstructure(lookup)
         return data
@@ -240,16 +240,16 @@
         for env_var in sorted(self._initial_env_vars):
             yield label, env_var
             label = ""
         label = "consumes (amended)"
         for supplier in sorted(self._amended_suppliers):
             yield label, supplier
             label = ""
-        label = "creates (amended)"
-        for product in sorted(self._amended_products):
+        label = "supplies (amended)"
+        for product in sorted(self._amended_consumers):
             yield label, product
             label = ""
         label = "env_var (amended)"
         for env_var in sorted(self._amended_env_vars):
             yield label, env_var
             label = ""
         for ngm in self._nglob_multis:
@@ -405,30 +405,30 @@
         self,
         workflow: "Workflow",
         *,
         state=False,
         file_hash=False,
         only_initial=False,
     ) -> list:
-        file_keys = workflow.get_products(self.key, kind="file")
+        file_keys = workflow.get_consumers(self.key, kind="file")
         if only_initial:
-            file_keys = [fk for fk in file_keys if fk not in self._amended_products]
+            file_keys = [fk for fk in file_keys if fk not in self._amended_consumers]
         filter_states = (FileState.PENDING, FileState.BUILT)
         return self._get_paths(workflow, file_keys, state, file_hash, False, filter_states)
 
     def get_vol_paths(
         self,
         workflow: "Workflow",
         *,
         file_hash=False,
         only_initial=False,
     ) -> list:
-        file_keys = workflow.get_products(self.key, kind="file")
+        file_keys = workflow.get_consumers(self.key, kind="file")
         if only_initial:
-            file_keys = [fk for fk in file_keys if fk not in self._amended_products]
+            file_keys = [fk for fk in file_keys if fk not in self._amended_consumers]
         filter_states = (FileState.VOLATILE,)
         return self._get_paths(workflow, file_keys, False, file_hash, False, filter_states)
 
     def get_static_paths(self, workflow: "Workflow", *, state=False, file_hash=False) -> list:
         file_keys = workflow.get_products(self.key, kind="file")
         filter_states = (FileState.STATIC, FileState.MISSING)
         return self._get_paths(workflow, file_keys, state, file_hash, False, filter_states)
@@ -473,31 +473,33 @@
             if self._hash is None or self._recording is None:
                 job = RunJob(self._key, self._pool)
             else:
                 job = TryReplayJob(self._key, self._pool)
         self.set_state(workflow, StepState.QUEUED)
         self.reschedule_due_to = set()
         self.validate_amended = False
-        workflow.queue.put_nowait(job)
-        workflow.queue_changed.set()
+        workflow.job_queue.put_nowait(job)
+        workflow.job_queue_changed.set()
 
     def clean_before_run(self, workflow: "Workflow"):
         """Drop amended inputs and (volatile) outputs.
 
-        This method is called right before (re)running a step, which will effectively recreate
+        This method is called right before (re)running a step.
+        Running the step will effectively recreate
         the same or different amended inputs and (volatile) outputs.
         """
         for supplier_key in self._amended_suppliers:
             workflow.consumers.discard(supplier_key, self._key, insist=True)
         self._amended_suppliers.clear()
-        for product_key in sorted(self._amended_products):
-            product = workflow.get_file(product_key)
-            assert product.get_state(workflow) in (FileState.PENDING, FileState.VOLATILE)
-            workflow.orphan(product_key)
-        self._amended_products.clear()
+        for consumer_key in sorted(self._amended_consumers):
+            consumer = workflow.get_file(consumer_key)
+            assert consumer.get_state(workflow) in (FileState.PENDING, FileState.VOLATILE)
+            workflow.suppliers.discard(consumer_key, self.key, insist=True)
+            workflow.orphan(consumer_key)
+        self._amended_consumers.clear()
         self._amended_env_vars.clear()
         self._nglob_multis = []
 
     def completed(self, workflow: "Workflow", success: bool, new_hash: StepHash | None) -> set[str]:
         """Set a step as completed (succeeded or failed) and trigger the consequences.
 
         Parameters
@@ -552,22 +554,22 @@
                 recording.initial_inp_paths.append(inp_path)
 
         recording.initial_env_vars = set(self._initial_env_vars)
         recording.amend_args["env_vars"] = set(self._amended_env_vars)
 
         for out_path in self.get_out_paths(workflow):
             file_key = f"file:{out_path}"
-            if file_key in self.amended_products:
+            if file_key in self.amended_consumers:
                 recording.amend_args.setdefault("out_paths", []).append(out_path)
             else:
                 recording.initial_out_paths.append(out_path)
 
         for vol_path in self.get_vol_paths(workflow):
             file_key = f"file:{vol_path}"
-            if file_key in self.amended_products:
+            if file_key in self.amended_consumers:
                 recording.amend_args.setdefault("vol_paths", []).append(vol_path)
             else:
                 recording.initial_vol_paths.append(vol_path)
 
         if len(recording.amend_args) > 0:
             recording.amend_args["step_key"] = self.key
             recording.amend_args.setdefault("inp_paths", [])
@@ -604,21 +606,20 @@
         """
         # Don't bother if there is no recording.
         if self._recording is None:
             return
         if self._recording.key != self.key:
             raise ValueError("The recorded key is not consistent with the step key")
         if (
-            len(self._amended_products) != 0
+            len(self._amended_consumers) != 0
             or len(self._amended_suppliers) != 0
             or len(self._amended_env_vars) != 0
         ):
             raise ValueError("Cannot restore amended info if step is already amended")
         if (
-            # TODO: get_inp_paths must include orphans!
             self._recording.initial_inp_paths == self.get_inp_paths(workflow, only_initial=True)
             and self._recording.initial_env_vars == self.initial_env_vars
             and self._recording.initial_out_paths == self.get_out_paths(workflow, only_initial=True)
             and self._recording.initial_vol_paths == self.get_vol_paths(workflow, only_initial=True)
         ):
             if len(self._recording.amend_args) > 0:
                 workflow.amend_step(**self._recording.amend_args)
@@ -649,15 +650,15 @@
             workflow.define_step(**step_args)
         for ngm in recording.nglob_multis:
             workflow.register_nglob(self.key, ngm)
         for patterns in recording.deferred_glob_args:
             workflow.defer_glob(self.key, patterns)
         # Mark the step as succeeded and mark outputs as BUILT
         self.set_state(workflow, StepState.SUCCEEDED)
-        for file_key in workflow.get_products(self.key, kind="file"):
+        for file_key in workflow.get_consumers(self.key, kind="file"):
             file = workflow.get_file(file_key)
             if file.get_state(workflow) == FileState.PENDING:
                 file.set_state(workflow, FileState.BUILT)
             file.release_pending(workflow)
 
     def register_nglob(self, workflow, nglob_multi):
         self.nglob_multis.append(nglob_multi)
@@ -667,24 +668,24 @@
     # Watch phase
     #
 
     def make_pending(self, workflow: "Workflow", *, input_changed: bool = False):
         self.validate_amended |= input_changed
         if self.get_state(workflow) != StepState.PENDING:
             self.set_state(workflow, StepState.PENDING)
-            other_keys = []
-            for key in workflow.get_products(self.key):
+            # First make all consumers (output files) pending
+            for key in workflow.get_consumers(self.key):
                 if key.startswith("file:"):
                     file = workflow.get_file(key)
-                    state = file.get_state(workflow)
-                    if state in (FileState.STATIC, FileState.MISSING):
-                        workflow.orphan(key)
-                    elif state == FileState.BUILT:
+                    if file.get_state(workflow) == FileState.BUILT:
                         file.make_pending(workflow)
-                else:
-                    # Postpone orphaning other things than files, so
-                    # steps are made pending before they are orphaned.
-                    # This is a slightly better (and order-independent)
-                    # representation of the current status.
-                    other_keys.append(key)
-            for key in other_keys:
+            # Then orphan all products that are not (volatile) output files
+            for key in workflow.get_products(self.key):
+                if key.startswith("file:"):
+                    file = workflow.get_file(key)
+                    if file.get_state(workflow) in (
+                        FileState.BUILT,
+                        FileState.PENDING,
+                        FileState.VOLATILE,
+                    ):
+                        continue
                 workflow.orphan(key)
```

### Comparing `stepup-1.0.0/stepup/core/tui.py` & `stepup-1.1.0/stepup/core/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,17 @@
 import tempfile
 import termios
 from decimal import Decimal
 
 import attrs
 from path import Path
 
+from .asyncio import stoppable_iterator
 from .director import interpret_num_workers
-from .rpc import serve_socket_rpc, stoppable_iterator, AsyncRPCClient
+from .rpc import serve_socket_rpc, AsyncRPCClient
 from .reporter import ReporterHandler, ReporterClient
 
 
 __all__ = ()
 
 
 def main():
@@ -73,21 +74,14 @@
         reporter_handler = ReporterHandler(args.show_perf > 0, stop_event)
         task_reporter = asyncio.create_task(
             serve_socket_rpc(reporter_handler, reporter_socket_path, stop_event),
             name="reporter-rpc",
         )
         tasks = [task_reporter]
 
-        # Instantiate keyboard interaction
-        if sys.stdin.isatty() and args.interactive:
-            task_keyboard = asyncio.create_task(
-                keyboard(director_socket_path, reporter_socket_path, stop_event), name="keyboard"
-            )
-            tasks.append(task_keyboard)
-
         # Launch director as background process
         log_file = open(".stepup/logs/director", "w")
         argv = [
             "-m",
             "stepup.core.director",
             args.plan_py,
             director_socket_path,
@@ -102,29 +96,40 @@
             process_director = await asyncio.create_subprocess_exec(
                 sys.executable,
                 *argv,
                 stdin=subprocess.DEVNULL,
                 stdout=log_file,
                 stderr=subprocess.STDOUT,
             )
-            if not args.interactive:
+            # Instantiate keyboard interaction or work non-interactively
+            if args.interactive:
+                if sys.stdin.isatty():
+                    await wait_for_path(director_socket_path, stop_event)
+                    task_keyboard = asyncio.create_task(
+                        keyboard(director_socket_path, reporter_socket_path, stop_event),
+                        name="keyboard",
+                    )
+                    tasks.append(task_keyboard)
+            else:
                 await wait_for_path(director_socket_path, stop_event)
                 async with await AsyncRPCClient.socket(director_socket_path) as client:
                     await client.call.join()
             await process_director.wait()
             stop_event.set()
         finally:
             try:
                 await asyncio.gather(*tasks)
+            except ConnectionRefusedError:
+                reporter_handler.report("ERROR", "Could not connect to director", [])
             finally:
                 log_file.close()
                 path_tmpsock.remove_p()
 
 
-async def wait_for_path(path: str, stop_event: asyncio.Event):
+async def wait_for_path(path: Path, stop_event: asyncio.Event):
     while not path.exists():
         if stop_event.is_set():
             return
         await asyncio.sleep(0.1)
 
 
 @attrs.define
@@ -165,15 +170,14 @@
 
 
 async def keyboard(
     director_socket_path: Path,
     reporter_socket_path: Path,
     stop_event: asyncio.Event,
 ):
-    await wait_for_path(director_socket_path, stop_event)
     async with (
         ReporterClient.socket(reporter_socket_path) as reporter,
         await AsyncRPCClient.socket(director_socket_path) as client,
         AsyncReadChar() as readchar,
     ):
         async for ch in stoppable_iterator(readchar, stop_event):
             if ch == "q":
@@ -189,15 +193,15 @@
                 break
             elif ch == "r":
                 await reporter("KEYBOARD", "Restarting the runner.")
                 async with asyncio.timeout(5):
                     await client.call.run()
             elif ch == "g":
                 async with asyncio.timeout(5):
-                    await client.call.graph("graph.txt")
+                    await client.call.graph("graph")
                 await reporter("KEYBOARD", "Workflow graph written to graph.txt.")
             elif ch == "f":
                 await reporter("KEYBOARD", "Discarding hashes and running from scratch.")
                 async with asyncio.timeout(5):
                     await client.call.from_scratch()
             elif ch == "t":
                 await reporter("KEYBOARD", "All steps marked pending and trying to replay.")
```

### Comparing `stepup-1.0.0/stepup/core/utils.py` & `stepup-1.1.0/stepup/core/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,35 +15,31 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Small utilities used throughout."""
 
-import asyncio
 import importlib.util
 import os
 import string
 import re
 from types import ModuleType
-from typing import Any
 
-import attrs
 from path import Path
 
 
 __all__ = (
     # Path manipulation
     "mynormpath",
     "myrelpath",
     "myabsolute",
     "myparent",
     "make_path_out",
-    # Asyncio
-    "MultiEvent",
+    "remove_path",
     # Miscellaneous
     "classproperty",
     "lookupdict",
     "CaseSensitiveTemplate",
     "check_plan",
     "check_inp_path",
     "format_digest",
@@ -141,42 +137,33 @@
     if path_out == path_in:
         raise ValueError(f"The output path cannot equal the input path: {path_out}")
     if not (ext is None or path_out.suffix == ext):
         raise ValueError(f"The output path does not have extension '{ext}': {path_out}.")
     return path_out
 
 
-#
-# Asyncio
-#
-
-
-@attrs.define
-class MultiEvent:
-    """Multiple events of which one at a time can be set."""
-
-    _events: dict[Any, asyncio.Event] = attrs.field()
-
-    @classmethod
-    def from_values(cls, *args):
-        result = cls({arg: asyncio.Event() for arg in args})
-        result.set(args[0])
-        return result
-
-    def set(self, value):
-        self._events[value].set()
-        for other_value, other_event in self._events.items():
-            if other_value != value:
-                other_event.clear()
-
-    def is_set(self, value):
-        return self._events[value].is_set()
-
-    async def wait(self, value):
-        await self._events[value].wait()
+def remove_path(path: Path) -> bool:
+    """Remove a file or directory. Return `True` of the file was removed."""
+    if path.endswith("/"):
+        try:
+            path.rmdir()
+            return True
+        except FileNotFoundError:
+            return False
+        except OSError:
+            return False
+    else:
+        try:
+            path.remove()
+            return True
+        except FileNotFoundError:
+            return False
+        except OSError:
+            return False
+    return False
 
 
 #
 # Miscellaneous
 #
```

### Comparing `stepup-1.0.0/stepup/core/worker.py` & `stepup-1.1.0/stepup/core/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,20 +46,36 @@
 #
 # In the main director process
 #
 
 
 @attrs.define
 class WorkerClient:
+    """Client interface to a worker, used by the director process."""
+
+    # The workflow that the client is interacting with.
     workflow: Workflow = attrs.field()
+
+    # A reporter to send progress and terminal output to.
     reporter: ReporterClient = attrs.field()
+
+    # The path of the directory socket.
+    # A step being executed by a worker needs this socket extend the workflow.
     director_socket_path: str = attrs.field()
+
+    # Flag to enable detailed CPU usage of each step.
     show_perf: bool = attrs.field()
+
+    # Flat to explain why a step could not be skipped.
     explain_rerun: bool = attrs.field()
+
+    # The integer index of the worker (in the list of workers kept by the Runner instance).
     idx: int = attrs.field(converter=int)
+
+    # The RPC client to communicate with the worker process.
     client: AsyncRPCClient | None = attrs.field(init=False, default=None)
 
     #
     # Setup and teardown
     #
 
     async def boot(self):
@@ -236,15 +252,16 @@
 #
 # In the worker process
 #
 
 
 @attrs.define
 class WorkerStep:
-    # Bundle all process related attributes into one WorkerStep object.
+    """Information on the current step that a worker is working on."""
+
     key: str = attrs.field()
     command: str = attrs.field()
     workdir: Path = attrs.field()
     proc: asyncio.subprocess.Process | None = attrs.field(init=False, default=None)
     stdout: bytes = attrs.field(init=False, default=b"")
     stderr: bytes = attrs.field(init=False, default=b"")
     perf_info: str = attrs.field(init=False, default="")
@@ -257,14 +274,16 @@
     @property
     def description(self):
         return self.command if self.workdir == "./" else f"{self.command}  # wd={self.workdir}"
 
 
 @attrs.define
 class WorkerHandler:
+    """RPC Handler in the worker process to respond to requests from the WorkerClient."""
+
     director_socket_path: str
     reporter: ReporterClient = attrs.field()
     show_perf: bool = attrs.field()
     explain_rerun: bool = attrs.field()
     stop_event: asyncio.Event = attrs.field(factory=asyncio.Event)
     step: WorkerStep | None = attrs.field(init=False, default=None)
```

### Comparing `stepup-1.0.0/stepup/core/workflow.py` & `stepup-1.1.0/stepup/core/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,62 +13,62 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""StepUp workflow: cascade with more concrete node implementations."""
+"""The `Workflow` is a `Cascade` subclass with more concrete node implementations."""
 
 import asyncio
+import json
 import os
+import textwrap
 from typing import cast, Collection, Self
 from collections import Counter
 
 import attrs
-from path import Path
 
 from .assoc import Assoc, many_to_one
 from .cascade import Cascade, Node, get_kind
 from .exceptions import GraphError
 from .file import File, FileState
 from .hash import FileHash, ExtendedStepHash
 from .nglob import NGlobMulti
 from .deferred_glob import DeferredGlob
 from .step import Step, StepState, Mandatory
-from .utils import myparent
-
+from .utils import myparent, lookupdict
 
 __all__ = ("Workflow",)
 
 
 @attrs.define
 class Workflow(Cascade):
     # Steps ready for scheduling and execution.
-    queue: asyncio.queues = attrs.field(init=False, factory=asyncio.Queue)
+    job_queue: asyncio.queues = attrs.field(init=False, factory=asyncio.Queue)
+
+    # Directories to be (un)watched
+    dir_queue: asyncio.queues = attrs.field(init=False, factory=asyncio.Queue)
 
-    # This event is set when the scheduler should check the queue again.
-    queue_changed: asyncio.Event = attrs.field(init=False, factory=asyncio.Event)
+    # This event is set when the scheduler should check the job_queue again.
+    job_queue_changed: asyncio.Event = attrs.field(init=False, factory=asyncio.Event)
 
     # The workflow_changed flag is set True in the run phase methods, right before they start
     # changing the graph. Errors raised afterwards result in an inconsistent graph.
     graph_changed: bool = attrs.field(init=False, default=False)
 
     # A list of files and directories that can be deleted.
     # This list contains BUILT files node with file hashes that were removed from the graph.
     to_be_deleted: list[tuple[str, FileHash | None]] = attrs.field(init=False, factory=list)
 
     # Node attributes stored in an Assoc to facilitate reverse lookups:
     file_states: "Assoc[str, FileState]" = attrs.field(init=False, factory=many_to_one)
     step_states: "Assoc[str, StepState]" = attrs.field(init=False, factory=many_to_one)
     step_mandatory: "Assoc[str, Mandatory]" = attrs.field(init=False, factory=many_to_one)
 
-    # A list of used directories, used in watch phase.
-    _used_directories: set = attrs.field(init=False, factory=set)
-
     # All keys using nglobs, used to lookup steps after watch phase that need to be re-executed.
     step_keys_with_nglob: set[str] = attrs.field(init=False, factory=set)
 
     #
     # Initialization and serialization
     #
 
@@ -139,14 +139,52 @@
         # Steps normally have no direct consumers, but better safe than sorry.
         # Note that file suppliers and consumers are kept in place, because parent directories
         # must be suppliers of their contents.
         for step_key in self.kinds.get("step", ()):
             self.suppliers.discard(step_key)
             self.consumers.discard(step_key)
 
+    def _format_dot_generic(self, arrowhead: str, include_dirs: bool, edges: Assoc):
+        lines = [
+            "strict digraph {",
+            "  graph [rankdir=BT bgcolor=transparent]",
+            "  node [penwidth=0 colorscheme=set39 style=filled fillcolor=5]",
+            f"  edge [color=dimgray arrowhead={arrowhead}]",
+        ]
+        lookup = lookupdict()
+        for key, node in self.nodes.items():
+            if key not in edges and key not in edges.inverse:
+                continue
+            if not include_dirs and key.startswith("file:") and key.endswith("/"):
+                continue
+            label = node.key[:-1] if node.key.endswith(":") else node.key[node.key.find(":") + 1 :]
+            label = json.dumps(textwrap.fill(label, 20))
+            if node.kind == "step":
+                props = ""
+            elif node.kind == "file":
+                props = " shape=rect fillcolor=9"
+            elif node.kind == "dg":
+                props = " shape=octagon fillcolor=7"
+            else:
+                props = " shape=hexagon fillcolor=6"
+            lines.append(f"  {lookup[key]} [label={label}{props}]")
+            for other in edges.get(key, ()):
+                if other != key:
+                    lines.append(f"  {lookup[key]} -> {lookup[other]}")
+        lines.append("}")
+        return "\n".join(lines)
+
+    def format_dot_creator(self):
+        """Return the creator-product graph in GraphViz DOT format."""
+        return self._format_dot_generic("empty", True, self.products)
+
+    def format_dot_supplier(self):
+        """Return the supplier-product graph in GraphViz DOT format."""
+        return self._format_dot_generic("normal", False, self.consumers)
+
     #
     # Type-annotated and type-checked node access
     #
 
     def get_file(self, file_key: str) -> File:
         if not file_key.startswith("file:"):
             raise TypeError(f"The key given to get_file is not a file: {file_key}")
@@ -317,29 +355,30 @@
             raise GraphError("A volatile output cannot be a directory.")
         if not (creator_key.startswith("dg:") or self.matching_deferred_glob(path) is None):
             raise GraphError("Cannot manually add a file that matches a deferred glob.")
         if file_state != FileState.STATIC and self.always_static(path):
             raise GraphError(f"Path is created as {file_state} but must be static: {path}")
         file_key = f"file:{path}"
         file = self.get_file(file_key)
-        if file is None or self.is_orphan(file_key):
-            if file_state == FileState.VOLATILE and len(self.consumers.get(file_key, ())) > 0:
-                raise GraphError(f"An input to an existing step cannot be volatile: {path}")
-            file = File(path)
-            self.create(file, creator_key)
-            parent_key, _, _ = self.supply_parent(file)
-            if file_state == FileState.STATIC and not (
-                parent_key is None or self.get_file(parent_key).get_state(self) == FileState.STATIC
-            ):
-                raise GraphError(f"Static path does not have a parent path node: {path}")
-        else:
+        if not (file is None or self.is_orphan(file_key)):
             raise GraphError(f"File was already created: {path}")
+        if file_state == FileState.VOLATILE and len(self.consumers.get(file_key, ())) > 0:
+            raise GraphError(f"An input to an existing step cannot be volatile: {path}")
+        file = File(path)
+        self.create(file, creator_key)
+        parent_key, _, _ = self.supply_parent(file)
         file.set_state(self, file_state)
         if file_state == FileState.STATIC:
+            if not (
+                parent_key is None or self.get_file(parent_key).get_state(self) == FileState.STATIC
+            ):
+                raise GraphError(f"Static path does not have a parent path node: {path}")
             file.release_pending(self)
+        else:
+            self.supply(creator_key, file_key)
         return file_key
 
     def get_parent_key(self, path: str, allow_orphan: bool = False) -> str | None:
         """Get the key of the parent File object, if relevant for consistency checking.
 
         Parameters
         ----------
@@ -374,16 +413,14 @@
 
         Parameters
         ----------
         creator_key
             The node creating this file (or None if not known).
         paths
             The locations of the files or directories (ending with /).
-        deferred
-            This must be set to True when the static file is cre
 
         Returns
         -------
         file_keys
             The keys of the static files.
         """
         if isinstance(paths, str):
@@ -640,20 +677,20 @@
         env_vars = set(env_vars)
         env_vars.difference_update(step.initial_env_vars)
         step.amended_env_vars.update(env_vars)
 
         # Create out_paths
         for out_path in out_paths:
             file_key = self.create_file(step_key, out_path, FileState.PENDING)
-            step.amended_products.add(file_key)
+            step.amended_consumers.add(file_key)
 
         # Create vol_paths
         for vol_path in vol_paths:
             file_key = self.create_file(step_key, vol_path, FileState.VOLATILE)
-            step.amended_products.add(file_key)
+            step.amended_consumers.add(file_key)
 
         if len(inp_paths) > 0:
             step.imply_mandatory_suppliers(self, new_inp_path_keys)
 
         step.reschedule_due_to.update(missing)
 
         return len(missing) == 0
@@ -701,59 +738,64 @@
             dg.ngm.reduce(orphaned_paths)
         super().clean()
 
     #
     # Watch phase
     #
 
-    @property
-    def used_directories(self) -> list[Path]:
-        return sorted(self._used_directories)
-
     def is_relevant(self, path: str):
         file = self.get_file(f"file:{path}")
         if file is not None:
             return file.get_state(self) != FileState.VOLATILE
         for step_key in self.step_keys_with_nglob:
             step = self.get_step(step_key)
             if any(ngm.may_change(set(), {path}) for ngm in step.nglob_multis):
                 return True
         return False
 
-    def process_watcher_changes(self, deleted: Collection[str], added: Collection[str]):
+    def process_watcher_changes(self, deleted: Collection[str], updated: Collection[str]):
+        """Update the workflow given a list of deleted and updated paths observed by the watcher.
+
+        Parameters
+        ----------
+        deleted
+            The deleted files.
+        updated
+            The added / changed files.
+        """
         # Sanity check
-        if not set(deleted).isdisjoint(added):
+        if not set(deleted).isdisjoint(updated):
             raise ValueError("Added and deleted files are not mutually exclusive.")
 
         # Process all deletions
         for path in deleted:
             # Handle deleted files that were used or created by steps.
             file = self.get_file(f"file:{path}")
             if file is None:
                 raise ValueError("Cannot process deletion of file absent from workflow")
             file.watcher_deleted(self)
 
-        # Process all additions (could also be file changes)
-        for path in added:
+        # Process all updates
+        for path in updated:
             file = self.get_file(f"file:{path}")
-            # If added the file is known, it must have changed (or a MISSING file was added).
+            # If updated the file is known, it must have changed (or a MISSING file was added).
             if file is not None:
-                file.watcher_added(self)
+                file.watcher_updated(self)
 
         for step_key in sorted(self.step_keys_with_nglob):
             step = self.get_step(step_key)
             # Check if any of the deleted files matches an nglob. If yes, step becomes pending.
             # Check if added files could result in new nglob matches. If yes, step becomes pending.
             if not self.is_orphan(step_key) and any(
-                ngm.will_change(deleted, added) for ngm in step.nglob_multis
+                ngm.will_change(deleted, updated) for ngm in step.nglob_multis
             ):
                 step.discard_recording()
                 step.make_pending(self, input_changed=True)
             # In case the step gets skipped, we need to make sure the nglob results
             # are up to date.
             for ngm in step.nglob_multis:
                 ngm.reduce(deleted)
-                ngm.extend(added)
+                ngm.extend(updated)
 
         # Queue pending steps that can be executed.
         for step_key in sorted(self.step_states.inverse.get(StepState.PENDING, ())):
             self.get_step(step_key).queue_if_appropriate(self)
```

### Comparing `stepup-1.0.0/stepup.egg-info/PKG-INFO` & `stepup-1.1.0/stepup.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: stepup
-Version: 1.0.0
+Version: 1.1.0
 Summary: StepUp Core provides the basic framework for the StepUp build tool
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
+Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-core/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-core/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-core/
-Project-URL: Changelog, https://github.com/reproducible-reporting/stepup-core/blob/main/CHANGELOG.md
+Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-core/changelog/
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: msgpack
 Requires-Dist: parse
 Requires-Dist: path
 Requires-Dist: rich
-Requires-Dist: watchfiles
+Requires-Dist: watchdog
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-macros-plugin; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 
-[![PyPI Upload](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pypi.yaml)
+[![release](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml)
 [![pytest](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml)
-[![PyPI Version](https://img.shields.io/pypi/v/stepup-core)](https://pypi.org/project/stepup-core/)
+[![PyPI Version](https://img.shields.io/pypi/v/stepup)](https://pypi.org/project/stepup/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-core)
 
 # StepUp Core
 
 StepUp is a simple, powerful and universal build tool.
 StepUp Core provides the basic framework for StepUp, without any domain-specific features.
```

### Comparing `stepup-1.0.0/stepup.egg-info/SOURCES.txt` & `stepup-1.1.0/stepup.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,57 @@
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
 docs/plan.py
+docs/run_example.py
+docs/advanced_topics/amending_static_inputs.md
 docs/advanced_topics/amending_steps.md
 docs/advanced_topics/blocked_steps.md
+docs/advanced_topics/cyclic_dependencies.md
 docs/advanced_topics/environment_variables.md
 docs/advanced_topics/here_and_root.md
 docs/advanced_topics/introduction.md
+docs/advanced_topics/manual_cleaning.md
 docs/advanced_topics/optional_steps.md
 docs/advanced_topics/pools.md
 docs/advanced_topics/static_deferred_glob.md
 docs/advanced_topics/static_named_glob.md
 docs/advanced_topics/variable_substitution.md
 docs/advanced_topics/volatile_outputs.md
+docs/advanced_topics/amending_static_inputs/.gitignore
+docs/advanced_topics/amending_static_inputs/config.txt
+docs/advanced_topics/amending_static_inputs/main.sh
+docs/advanced_topics/amending_static_inputs/plan.py
+docs/advanced_topics/amending_static_inputs/stdout.txt
 docs/advanced_topics/amending_steps/.gitignore
 docs/advanced_topics/amending_steps/main.sh
 docs/advanced_topics/amending_steps/plan.py
 docs/advanced_topics/amending_steps/stdout.txt
 docs/advanced_topics/amending_steps/step.py
 docs/advanced_topics/blocked_steps/.gitignore
 docs/advanced_topics/blocked_steps/main.sh
 docs/advanced_topics/blocked_steps/plan.py
 docs/advanced_topics/blocked_steps/stdout.txt
+docs/advanced_topics/cyclic_dependencies/.gitignore
+docs/advanced_topics/cyclic_dependencies/main.sh
+docs/advanced_topics/cyclic_dependencies/plan.py
+docs/advanced_topics/cyclic_dependencies/stdout.txt
 docs/advanced_topics/environment_variables/.gitignore
 docs/advanced_topics/environment_variables/main.sh
 docs/advanced_topics/environment_variables/plan.py
 docs/advanced_topics/environment_variables/stdout.txt
 docs/advanced_topics/here_and_root/.gitignore
 docs/advanced_topics/here_and_root/main.sh
 docs/advanced_topics/here_and_root/stdout.txt
@@ -54,14 +70,16 @@
 docs/advanced_topics/pools/main.sh
 docs/advanced_topics/pools/plan.py
 docs/advanced_topics/pools/stdout.txt
 docs/advanced_topics/static_deferred_glob/.gitignore
 docs/advanced_topics/static_deferred_glob/bar.txt
 docs/advanced_topics/static_deferred_glob/foo.txt
 docs/advanced_topics/static_deferred_glob/graph.txt
+docs/advanced_topics/static_deferred_glob/graph_creator.svg
+docs/advanced_topics/static_deferred_glob/graph_supplier.svg
 docs/advanced_topics/static_deferred_glob/main.sh
 docs/advanced_topics/static_deferred_glob/plan.py
 docs/advanced_topics/static_deferred_glob/stdout.txt
 docs/advanced_topics/static_named_glob/.gitignore
 docs/advanced_topics/static_named_glob/main.sh
 docs/advanced_topics/static_named_glob/plan.py
 docs/advanced_topics/static_named_glob/stdout.txt
@@ -99,14 +117,16 @@
 docs/getting_started/static_glob.md
 docs/getting_started/static_glob_conditional.md
 docs/getting_started/copy_mkdir/.gitignore
 docs/getting_started/copy_mkdir/main.sh
 docs/getting_started/copy_mkdir/plan.py
 docs/getting_started/copy_mkdir/stdout.txt
 docs/getting_started/dependencies/.gitignore
+docs/getting_started/dependencies/graph_creator.svg
+docs/getting_started/dependencies/graph_supplier.svg
 docs/getting_started/dependencies/main.sh
 docs/getting_started/dependencies/plan.py
 docs/getting_started/dependencies/stdout.txt
 docs/getting_started/distributed_plans/.gitignore
 docs/getting_started/distributed_plans/main.sh
 docs/getting_started/distributed_plans/part1.txt
 docs/getting_started/distributed_plans/plan.py
@@ -135,14 +155,15 @@
 docs/getting_started/script_multiple/plot_ebos.png
 docs/getting_started/script_multiple/stdout.txt
 docs/getting_started/script_single/.gitignore
 docs/getting_started/script_single/config.json
 docs/getting_started/script_single/generate.py
 docs/getting_started/script_single/main.sh
 docs/getting_started/script_single/plan.py
+docs/getting_started/script_single/stdout.txt
 docs/getting_started/static_files/.gitignore
 docs/getting_started/static_files/limerick.txt
 docs/getting_started/static_files/main.sh
 docs/getting_started/static_files/plan.py
 docs/getting_started/static_files/stdout.txt
 docs/getting_started/static_glob/.gitignore
 docs/getting_started/static_glob/main.sh
@@ -166,15 +187,17 @@
 stepup.egg-info/entry_points.txt
 stepup.egg-info/requires.txt
 stepup.egg-info/top_level.txt
 stepup/core/__init__.py
 stepup/core/_version.py
 stepup/core/api.py
 stepup/core/assoc.py
+stepup/core/asyncio.py
 stepup/core/cascade.py
+stepup/core/cleanup.py
 stepup/core/deferred_glob.py
 stepup/core/director.py
 stepup/core/exceptions.py
 stepup/core/file.py
 stepup/core/hash.py
 stepup/core/interact.py
 stepup/core/job.py
@@ -341,29 +364,22 @@
 tests/cases/env_vars_workdir/.gitignore
 tests/cases/env_vars_workdir/README.md
 tests/cases/env_vars_workdir/expected_graph.txt
 tests/cases/env_vars_workdir/expected_stdout.txt
 tests/cases/env_vars_workdir/main.sh
 tests/cases/env_vars_workdir/plan.py
 tests/cases/env_vars_workdir/sub/input.txt
-tests/cases/error_cyclic_early/.gitignore
-tests/cases/error_cyclic_early/README.md
-tests/cases/error_cyclic_early/expected_graph.txt
-tests/cases/error_cyclic_early/expected_stdout.txt
-tests/cases/error_cyclic_early/main.sh
-tests/cases/error_cyclic_early/plan.py
 tests/cases/error_cyclic_late/.gitignore
 tests/cases/error_cyclic_late/README.md
 tests/cases/error_cyclic_late/expected_graph.txt
 tests/cases/error_cyclic_late/expected_stdout.txt
 tests/cases/error_cyclic_late/main.sh
 tests/cases/error_cyclic_late/plan.py
 tests/cases/error_deferred_nonexisting/.gitignore
 tests/cases/error_deferred_nonexisting/README.md
-tests/cases/error_deferred_nonexisting/expected_graph.txt
 tests/cases/error_deferred_nonexisting/expected_stdout.txt
 tests/cases/error_deferred_nonexisting/main.sh
 tests/cases/error_deferred_nonexisting/plan.py
 tests/cases/error_env_var/.gitignore
 tests/cases/error_env_var/README.md
 tests/cases/error_env_var/expected_graph.txt
 tests/cases/error_env_var/expected_stdout.txt
@@ -446,14 +462,22 @@
 tests/cases/noplan/main.sh
 tests/cases/nostatic/.gitignore
 tests/cases/nostatic/README.md
 tests/cases/nostatic/expected_graph.txt
 tests/cases/nostatic/expected_stdout.txt
 tests/cases/nostatic/main.sh
 tests/cases/nostatic/plan.py
+tests/cases/not_cyclic/.gitignore
+tests/cases/not_cyclic/README.md
+tests/cases/not_cyclic/expected_graph_01.txt
+tests/cases/not_cyclic/expected_graph_02.txt
+tests/cases/not_cyclic/expected_graph_03.txt
+tests/cases/not_cyclic/expected_stdout.txt
+tests/cases/not_cyclic/main.sh
+tests/cases/not_cyclic/plan.py
 tests/cases/optional_convert/.gitignore
 tests/cases/optional_convert/README.md
 tests/cases/optional_convert/expected_graph_a.txt
 tests/cases/optional_convert/expected_graph_b.txt
 tests/cases/optional_convert/expected_graph_c.txt
 tests/cases/optional_convert/expected_stdout_a.txt
 tests/cases/optional_convert/expected_stdout_b.txt
```

### Comparing `stepup-1.0.0/tests/cases/README.md` & `stepup-1.1.0/tests/cases/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/amend/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/amend/expected_graph_01.txt`

 * *Files 9% similar despite different names*

```diff
@@ -44,43 +44,49 @@
             supplies   step:./step.py
 
 step:./step.py
              workdir = ./
              command = ./step.py
                state = SUCCEEDED
   consumes (amended) = file:inp2.txt
-   creates (amended) = file:out2.txt
+  supplies (amended) = file:out2.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
             consumes   file:inp2.txt
              creates   file:out1.txt
              creates   file:out2.txt
+            supplies   file:out1.txt
+            supplies   file:out2.txt
 
 file:out1.txt
                 path = out1.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
 
 step:echo word2 > inp2.txt
              workdir = ./
              command = echo word2 > inp2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
              creates   file:inp2.txt
+            supplies   file:inp2.txt
 
 file:inp2.txt
                 path = inp2.txt
                state = BUILT
           created by   step:echo word2 > inp2.txt
             consumes   file:./
+            consumes   step:echo word2 > inp2.txt
             supplies   step:./step.py
 
 file:out2.txt
                 path = out2.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/amend/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/amend/expected_graph_02.txt`

 * *Files 9% similar despite different names*

```diff
@@ -44,43 +44,49 @@
             supplies   step:./step.py
 
 step:./step.py
              workdir = ./
              command = ./step.py
                state = SUCCEEDED
   consumes (amended) = file:inp2.txt
-   creates (amended) = file:out2.txt
+  supplies (amended) = file:out2.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
             consumes   file:inp2.txt
              creates   file:out1.txt
              creates   file:out2.txt
+            supplies   file:out1.txt
+            supplies   file:out2.txt
 
 file:out1.txt
                 path = out1.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
 
 step:echo word2 > inp2.txt
              workdir = ./
              command = echo word2 > inp2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
              creates   file:inp2.txt
+            supplies   file:inp2.txt
 
 file:inp2.txt
                 path = inp2.txt
                state = BUILT
           created by   step:echo word2 > inp2.txt
             consumes   file:./
+            consumes   step:echo word2 > inp2.txt
             supplies   step:./step.py
 
 file:out2.txt
                 path = out2.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/amend/expected_graph_03.txt` & `stepup-1.1.0/tests/cases/amend/expected_graph_03.txt`

 * *Files 9% similar despite different names*

```diff
@@ -44,43 +44,49 @@
             supplies   step:./step.py
 
 step:./step.py
              workdir = ./
              command = ./step.py
                state = SUCCEEDED
   consumes (amended) = file:inp2.txt
-   creates (amended) = file:out2.txt
+  supplies (amended) = file:out2.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
             consumes   file:inp2.txt
              creates   file:out1.txt
              creates   file:out2.txt
+            supplies   file:out1.txt
+            supplies   file:out2.txt
 
 file:out1.txt
                 path = out1.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
 
 step:echo word2 > inp2.txt
              workdir = ./
              command = echo word2 > inp2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
              creates   file:inp2.txt
+            supplies   file:inp2.txt
 
 file:inp2.txt
                 path = inp2.txt
                state = BUILT
           created by   step:echo word2 > inp2.txt
             consumes   file:./
+            consumes   step:echo word2 > inp2.txt
             supplies   step:./step.py
 
 file:out2.txt
                 path = out2.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/amend/expected_graph_04.txt` & `stepup-1.1.0/tests/cases/amend/expected_graph_04.txt`

 * *Files 9% similar despite different names*

```diff
@@ -44,43 +44,49 @@
             supplies   step:./step.py
 
 step:./step.py
              workdir = ./
              command = ./step.py
                state = SUCCEEDED
   consumes (amended) = file:inp2.txt
-   creates (amended) = file:out2.txt
+  supplies (amended) = file:out2.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
             consumes   file:inp2.txt
              creates   file:out1.txt
              creates   file:out2.txt
+            supplies   file:out1.txt
+            supplies   file:out2.txt
 
 file:out1.txt
                 path = out1.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
 
 step:echo word2 > inp2.txt
              workdir = ./
              command = echo word2 > inp2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
              creates   file:inp2.txt
+            supplies   file:inp2.txt
 
 file:inp2.txt
                 path = inp2.txt
                state = BUILT
           created by   step:echo word2 > inp2.txt
             consumes   file:./
+            consumes   step:echo word2 > inp2.txt
             supplies   step:./step.py
 
 file:out2.txt
                 path = out2.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/amend/expected_stdout_01.txt` & `stepup-1.1.0/tests/cases/amend/expected_stdout_01.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./step.py
 RESCHEDULE │ ./step.py
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               ./step.py
 Return code           0
@@ -22,16 +22,15 @@
 Same out hash        out1.txt
 Same out hash        out2.txt
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./step.py
    SUCCESS │ ./step.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ inp2.txt
-     ADDED │ inp2.txt
+   UPDATED │ inp2.txt
      PHASE │ run
  DROPAMEND │ ./step.py
 ────────────────────── Outdated amended step information ───────────────────────
 Modified step hash   extended, digest 3f35ebaa ➜ 54c77a45, inp_digset 4a859afe ➜ 2dfe3ff7
 Modified inp hash    inp2.txt (digest 55af8bcf ➜ b0c92f99, size 6 ➜ 15)
 ──────────────────────── Remained the same (or missing) ────────────────────────
 Same inp hash        ./
```

### Comparing `stepup-1.0.0/tests/cases/amend/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/amend/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest b9ac59ee, inp_digset b9ac59ee
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
       SKIP │ echo word2 > inp2.txt
```

### Comparing `stepup-1.0.0/tests/cases/amend/expected_stdout_03.txt` & `stepup-1.1.0/tests/cases/amend_delay/expected_stdout.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,71 @@
-  WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
-      SKIP │ ./plan.py
+     PHASE │ run
+     START │ ./plan.py
+   SUCCESS │ ./plan.py
+     START │ sleep 0.1; echo Contents of inp2.txt > inp2.txt
+   SUCCESS │ sleep 0.1; echo Contents of inp2.txt > inp2.txt
+     START │ sleep 0.1; cp inp1.txt tmp1.txt
+   SUCCESS │ sleep 0.1; cp inp1.txt tmp1.txt
+     START │ ./step.py > log.txt
+   SUCCESS │ ./step.py > log.txt
+  WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
+     PHASE │ watch
+   DELETED │ inp2.txt
+     PHASE │ run
+    NOSKIP │ sleep 0.1; echo Contents of inp2.txt > inp2.txt
+───────────────────────────── Missing output files ─────────────────────────────
+inp2.txt
+────────────────────────────── Remained the same ───────────────────────────────
+Same step hash       extended, digest db3fc8c7, inp_digset 45a42df1
+Same inp hash        ./
+Same out hash        inp2.txt
+────────────────────────────────────────────────────────────────────────────────
+     START │ sleep 0.1; echo Contents of inp2.txt > inp2.txt
+   SUCCESS │ sleep 0.1; echo Contents of inp2.txt > inp2.txt
+      SKIP │ ./step.py > log.txt
 ───────────────────────────── No changes observed ──────────────────────────────
-Same step hash       extended, digest b9ac59ee, inp_digset b9ac59ee
+Same step hash       extended, digest fc3a16b8, inp_digset d295b71b
 Same inp hash        ./
-Same inp hash        plan.py
+Same inp hash        inp0.txt
+Same inp hash        inp2.txt
+Same inp hash        step.py
+Same inp hash        tmp1.txt
+Same out hash        log.txt
 ────────────────────────────────────────────────────────────────────────────────
- DROPAMEND │ ./step.py
+  WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
+     PHASE │ watch
+   UPDATED │ inp0.txt
+   UPDATED │ inp1.txt
+     PHASE │ run
+ DROPAMEND │ ./step.py > log.txt
 ────────────────────── Outdated amended step information ───────────────────────
-Modified step hash   extended, digest 3f35ebaa ➜ 504fde78, inp_digset 4a859afe ➜ 137fec45
-Modified inp hash    inp2.txt (digest 55af8bcf ➜ 705a962e, size 6 ➜ 16)
+Modified step hash   extended, digest fc3a16b8 ➜ ef517dc9, inp_digset d295b71b ➜ 4f8cf95a
+Modified inp hash    inp0.txt (digest 681fd532 ➜ 2dab5684)
 ──────────────────────── Remained the same (or missing) ────────────────────────
 Same inp hash        ./
-Same inp hash        inp1.txt
-Same out hash        out1.txt
-Same out hash        out2.txt
+Same inp hash        inp2.txt
+Same inp hash        step.py
+Same inp hash        tmp1.txt
+Same out hash        log.txt
 ────────────────────────────────────────────────────────────────────────────────
-    NOSKIP │ echo word2 > inp2.txt
+    NOSKIP │ sleep 0.1; cp inp1.txt tmp1.txt
 ──────────────────────────── Changes causing rerun ─────────────────────────────
-Modified step hash   extended, digest ecd85c33 ➜ b4a74d28, inp_digset 87ee641b
-Modified out hash    inp2.txt (digest 55af8bcf ➜ 705a962e, size 6 ➜ 16)
+Modified step hash   extended, digest 707c670e ➜ 5fe8bdce, inp_digset 69bd8048 ➜ 49269d0c
+Modified inp hash    inp1.txt (digest 6c6e5eb3 ➜ e8869200, size 15 ➜ 16)
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
+Same out hash        tmp1.txt
 ────────────────────────────────────────────────────────────────────────────────
-     START │ ./step.py
-RESCHEDULE │ ./step.py
+     START │ ./step.py > log.txt
+RESCHEDULE │ ./step.py > log.txt
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
-inp2.txt
-────────────────────────────────────────────────────────────────────────────────
-     START │ echo word2 > inp2.txt
-   SUCCESS │ echo word2 > inp2.txt
- DROPAMEND │ ./step.py
-────────────────────── Outdated amended step information ───────────────────────
-Modified step hash   extended, digest 504fde78 ➜ 3f35ebaa, inp_digset 137fec45 ➜ 4a859afe
-Modified inp hash    inp2.txt (digest 705a962e ➜ 55af8bcf, size 16 ➜ 6)
-──────────────────────── Remained the same (or missing) ────────────────────────
-Same inp hash        ./
-Same inp hash        inp1.txt
-Same out hash        out1.txt
-Same out hash        out2.txt
+tmp1.txt
 ────────────────────────────────────────────────────────────────────────────────
-     START │ ./step.py
-   SUCCESS │ ./step.py
+     START │ sleep 0.1; cp inp1.txt tmp1.txt
+   SUCCESS │ sleep 0.1; cp inp1.txt tmp1.txt
+     START │ ./step.py > log.txt
+   SUCCESS │ ./step.py > log.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/amend/main.sh` & `stepup-1.1.0/tests/cases/amend/main.sh`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 # Run the example
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Get graph after normal run.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f step.py ]] || exit -1
 [[ -f inp1.txt ]] || exit -1
 [[ -f inp2.txt ]] || exit -1
 grep word1 out1.txt
 grep word2 out2.txt
 
 # Change an amended input, rerun, and get the graph after completion of the pending steps.
 echo "word2 and some" > inp2.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("inp2.txt")
+watch_update("inp2.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f step.py ]] || exit -1
 [[ -f inp1.txt ]] || exit -1
@@ -46,15 +46,15 @@
 # Restart StepUp without changes
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Get graph after restart without changes.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_03.txt")
+graph("current_graph_03")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f step.py ]] || exit -1
 [[ -f inp1.txt ]] || exit -1
@@ -69,15 +69,15 @@
 echo "word2 and other" > inp2.txt
 stepup -e -w 1 plan.py & # > current_stdout_03.txt &
 
 # Get graph after restart without changes.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_04.txt")
+graph("current_graph_04")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f step.py ]] || exit -1
 [[ -f inp1.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/amend_delay/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/amend_delay/expected_graph_01.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,27 +47,29 @@
              command = sleep 0.1; cp inp1.txt tmp1.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
              creates   file:tmp1.txt
+            supplies   file:tmp1.txt
 
 file:inp1.txt
                 path = inp1.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:sleep 0.1; cp inp1.txt tmp1.txt
 
 file:tmp1.txt
                 path = tmp1.txt
                state = BUILT
           created by   step:sleep 0.1; cp inp1.txt tmp1.txt
             consumes   file:./
+            consumes   step:sleep 0.1; cp inp1.txt tmp1.txt
             supplies   step:./step.py > log.txt
 
 step:./step.py > log.txt
              workdir = ./
              command = ./step.py > log.txt
                state = SUCCEEDED
   consumes (amended) = file:inp0.txt
@@ -77,42 +79,46 @@
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp0.txt
             consumes   file:inp2.txt
             consumes   file:step.py
             consumes   file:tmp1.txt
              creates   file:log.txt
+            supplies   file:log.txt
 
 file:step.py
                 path = step.py
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:./step.py > log.txt
 
 file:log.txt
                 path = log.txt
                state = BUILT
           created by   step:./step.py > log.txt
             consumes   file:./
+            consumes   step:./step.py > log.txt
 
 step:sleep 0.1; echo Contents of inp2.txt > inp2.txt
              workdir = ./
              command = sleep 0.1; echo Contents of inp2.txt > inp2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
              creates   file:inp2.txt
+            supplies   file:inp2.txt
 
 file:inp2.txt
                 path = inp2.txt
                state = BUILT
           created by   step:sleep 0.1; echo Contents of inp2.txt > inp2.txt
             consumes   file:./
+            consumes   step:sleep 0.1; echo Contents of inp2.txt > inp2.txt
             supplies   step:./step.py > log.txt
 
 file:inp0.txt
                 path = inp0.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
```

### Comparing `stepup-1.0.0/tests/cases/amend_delay/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/amend_delay/expected_graph_02.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,27 +47,29 @@
              command = sleep 0.1; cp inp1.txt tmp1.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
              creates   file:tmp1.txt
+            supplies   file:tmp1.txt
 
 file:inp1.txt
                 path = inp1.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:sleep 0.1; cp inp1.txt tmp1.txt
 
 file:tmp1.txt
                 path = tmp1.txt
                state = BUILT
           created by   step:sleep 0.1; cp inp1.txt tmp1.txt
             consumes   file:./
+            consumes   step:sleep 0.1; cp inp1.txt tmp1.txt
             supplies   step:./step.py > log.txt
 
 step:./step.py > log.txt
              workdir = ./
              command = ./step.py > log.txt
                state = SUCCEEDED
   consumes (amended) = file:inp0.txt
@@ -77,42 +79,46 @@
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp0.txt
             consumes   file:inp2.txt
             consumes   file:step.py
             consumes   file:tmp1.txt
              creates   file:log.txt
+            supplies   file:log.txt
 
 file:step.py
                 path = step.py
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:./step.py > log.txt
 
 file:log.txt
                 path = log.txt
                state = BUILT
           created by   step:./step.py > log.txt
             consumes   file:./
+            consumes   step:./step.py > log.txt
 
 step:sleep 0.1; echo Contents of inp2.txt > inp2.txt
              workdir = ./
              command = sleep 0.1; echo Contents of inp2.txt > inp2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
              creates   file:inp2.txt
+            supplies   file:inp2.txt
 
 file:inp2.txt
                 path = inp2.txt
                state = BUILT
           created by   step:sleep 0.1; echo Contents of inp2.txt > inp2.txt
             consumes   file:./
+            consumes   step:sleep 0.1; echo Contents of inp2.txt > inp2.txt
             supplies   step:./step.py > log.txt
 
 file:inp0.txt
                 path = inp0.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
```

### Comparing `stepup-1.0.0/tests/cases/amend_delay/expected_graph_03.txt` & `stepup-1.1.0/tests/cases/amend_delay/expected_graph_03.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,27 +47,29 @@
              command = sleep 0.1; cp inp1.txt tmp1.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
              creates   file:tmp1.txt
+            supplies   file:tmp1.txt
 
 file:inp1.txt
                 path = inp1.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:sleep 0.1; cp inp1.txt tmp1.txt
 
 file:tmp1.txt
                 path = tmp1.txt
                state = BUILT
           created by   step:sleep 0.1; cp inp1.txt tmp1.txt
             consumes   file:./
+            consumes   step:sleep 0.1; cp inp1.txt tmp1.txt
             supplies   step:./step.py > log.txt
 
 step:./step.py > log.txt
              workdir = ./
              command = ./step.py > log.txt
                state = SUCCEEDED
   consumes (amended) = file:inp0.txt
@@ -77,42 +79,46 @@
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp0.txt
             consumes   file:inp2.txt
             consumes   file:step.py
             consumes   file:tmp1.txt
              creates   file:log.txt
+            supplies   file:log.txt
 
 file:step.py
                 path = step.py
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:./step.py > log.txt
 
 file:log.txt
                 path = log.txt
                state = BUILT
           created by   step:./step.py > log.txt
             consumes   file:./
+            consumes   step:./step.py > log.txt
 
 step:sleep 0.1; echo Contents of inp2.txt > inp2.txt
              workdir = ./
              command = sleep 0.1; echo Contents of inp2.txt > inp2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
              creates   file:inp2.txt
+            supplies   file:inp2.txt
 
 file:inp2.txt
                 path = inp2.txt
                state = BUILT
           created by   step:sleep 0.1; echo Contents of inp2.txt > inp2.txt
             consumes   file:./
+            consumes   step:sleep 0.1; echo Contents of inp2.txt > inp2.txt
             supplies   step:./step.py > log.txt
 
 file:inp0.txt
                 path = inp0.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
```

### Comparing `stepup-1.0.0/tests/cases/amend_delay/main.sh` & `stepup-1.1.0/tests/cases/amend_delay/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 echo "First inp1.txt" > inp1.txt
 stepup -e -w 1 plan.py & # > current_stdout.txt &
 
 # Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f inp0.txt ]] || exit -1
 [[ -f inp1.txt ]] || exit -1
 [[ -f tmp1.txt ]] || exit -1
 [[ -f inp2.txt ]] || exit -1
 [[ -f log.txt ]] || exit -1
 
 # Remove input and rerun the plan.
 rm inp2.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_del("inp2.txt")
+watch_delete("inp2.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f inp0.txt ]] || exit -1
 [[ -f inp1.txt ]] || exit -1
 [[ -f tmp1.txt ]] || exit -1
@@ -43,19 +43,19 @@
 [[ -f log.txt ]] || exit -1
 
 # Replace input and rerun the plan.
 echo "Something new" > inp0.txt
 echo "Second inp1.txt" > inp1.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("inp0.txt")
-watch_add("inp1.txt")
+watch_update("inp0.txt")
+watch_update("inp1.txt")
 run()
 wait()
-graph("current_graph_03.txt")
+graph("current_graph_03")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f inp0.txt ]] || exit -1
 [[ -f inp1.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/amend_env_vars/expected_graph.txt` & `stepup-1.1.0/tests/cases/amend_env_vars/expected_graph.txt`

 * *Files 7% similar despite different names*

```diff
@@ -40,28 +40,32 @@
             supplies   step:./step.py
 
 step:./step.py
              workdir = ./
              command = ./step.py
                state = SUCCEEDED
   consumes (amended) = file:foo.txt
-   creates (amended) = file:bar.log
+  supplies (amended) = file:bar.log
                      = file:bar.txt
    env_var (amended) = INP_VAR_TEST_STEPUP_BAR
                      = INP_VAR_TEST_STEPUP_FOO
           created by   step:./plan.py
             consumes   file:./
             consumes   file:foo.txt
              creates   file:bar.log
              creates   file:bar.txt
+            supplies   file:bar.log
+            supplies   file:bar.txt
 
 file:bar.txt
                 path = bar.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
 
 file:bar.log
                 path = bar.log
                state = VOLATILE
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/amend_env_vars/main.sh` & `stepup-1.1.0/tests/cases/amend_env_vars/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 export INP_VAR_TEST_STEPUP_BAR="bar"
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
 [[ -f foo.txt ]] || exit -1
 [[ -f bar.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/amend_missing/expected_graph.txt` & `stepup-1.1.0/tests/cases/amend_missing/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 step:echo Will be deleted by accident > missing.txt
              workdir = ./
              command = echo Will be deleted by accident > missing.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:missing.txt
+            supplies   file:missing.txt
 
 file:missing.txt
                 path = missing.txt
                state = BUILT
           created by   step:echo Will be deleted by accident > missing.txt
             consumes   file:./
+            consumes   step:echo Will be deleted by accident > missing.txt
             supplies   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/amend_missing/expected_stdout.txt` & `stepup-1.1.0/tests/cases/error_deferred_nonexisting/expected_stdout.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
-     START │ ./step.py
-RESCHEDULE │ ./step.py
-──────────────── Rescheduling due to unavailable amended inputs ────────────────
-missing.txt
-────────────────────────────────────────────────────────────────────────────────
-     START │ echo Will be deleted by accident > missing.txt
-   SUCCESS │ echo Will be deleted by accident > missing.txt
-     START │ ./step.py
-      FAIL │ ./step.py
+      FAIL │ cat static/foo/bar/README.md
 ────────────────────────────────── Step info ───────────────────────────────────
-Command               ./step.py
-Return code           1
-──────────────────────────────── Standard error ────────────────────────────────
-Traceback (most recent call last):
-  File "${CASE}/./step.py", line ---, in <module>
-    amend(inp="missing.txt")
-  File "${PWD}/stepup/core/api.py", line ---, in amend
-    check_inp_paths(su_inp_paths)
-  File "${PWD}/stepup/core/api.py", line ---, in check_inp_paths
-    raise ValueError(f"{message}: {inp_path}")
-ValueError: Path does not exist: missing.txt
+Command               cat static/foo/bar/README.md
+──────────────────────────────── Invalid inputs ────────────────────────────────
+STATIC Path does not exist: static/foo/bar/README.md
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step(s) failed, see error messages above
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
-     PHASE │ watch
   DIRECTOR │ Stopping workers.
+     ERROR │ The director raised an exception.
+────────────────────────────────── Traceback ───────────────────────────────────
+Traceback (most recent call last):
+  File "${PWD}/stepup/core/director.py", line ---, in async_main
+    await serve(
+  File "${PWD}/stepup/core/director.py", line ---, in serve
+    await asyncio.gather(watcher_loop, runner_loop, rpc_director)
+  File "${PWD}/stepup/core/watcher.py", line ---, in loop
+    await dir_loop
+  File "${PWD}/stepup/core/watcher.py", line ---, in dir_loop
+    raise FileNotFoundError(f"Cannot watch non-existing directory: {path}")
+FileNotFoundError: Cannot watch non-existing directory: static/
+────────────────────────────────────────────────────────────────────────────────
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/amend_missing/main.sh` & `stepup-1.1.0/tests/cases/amend_missing/main.sh`

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
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f step.py ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/amend_outdir_pending/expected_graph.txt` & `stepup-1.1.0/tests/cases/amend_voldir_pending/expected_graph.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,25 +30,27 @@
              creates   step:./demo.py
 
 step:./demo.py
              workdir = ./
              command = ./demo.py
                state = PENDING
   consumes (amended) = file:nonexisting/
-   creates (amended) = file:nonexisting/foo.out
+  supplies (amended) = file:nonexisting/foo.out
           created by   step:./plan.py
             consumes   file:./
             consumes   (file:nonexisting/)
              creates   file:nonexisting/foo.out
+            supplies   file:nonexisting/foo.out
 
 (file:nonexisting/)
                 path = nonexisting/
                state = PENDING
             consumes   file:./
             supplies   file:nonexisting/foo.out
             supplies   step:./demo.py
 
 file:nonexisting/foo.out
                 path = nonexisting/foo.out
-               state = PENDING
+               state = VOLATILE
           created by   step:./demo.py
             consumes   (file:nonexisting/)
+            consumes   step:./demo.py
```

### Comparing `stepup-1.0.0/tests/cases/amend_outdir_pending/expected_stdout.txt` & `stepup-1.1.0/tests/cases/amend_outdir_pending/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./demo.py
 RESCHEDULE │ ./demo.py
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               ./demo.py
 Return code           0
```

### Comparing `stepup-1.0.0/tests/cases/amend_outdir_pending/main.sh` & `stepup-1.1.0/tests/cases/static/main.sh`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,17 @@
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
+[[ -f original.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/amend_voldir_pending/expected_graph.txt` & `stepup-1.1.0/tests/cases/amend_outdir_pending/expected_graph.txt`

 * *Files 13% similar despite different names*

```diff
@@ -30,25 +30,27 @@
              creates   step:./demo.py
 
 step:./demo.py
              workdir = ./
              command = ./demo.py
                state = PENDING
   consumes (amended) = file:nonexisting/
-   creates (amended) = file:nonexisting/foo.out
+  supplies (amended) = file:nonexisting/foo.out
           created by   step:./plan.py
             consumes   file:./
             consumes   (file:nonexisting/)
              creates   file:nonexisting/foo.out
+            supplies   file:nonexisting/foo.out
 
 (file:nonexisting/)
                 path = nonexisting/
                state = PENDING
             consumes   file:./
             supplies   file:nonexisting/foo.out
             supplies   step:./demo.py
 
 file:nonexisting/foo.out
                 path = nonexisting/foo.out
-               state = VOLATILE
+               state = PENDING
           created by   step:./demo.py
             consumes   (file:nonexisting/)
+            consumes   step:./demo.py
```

### Comparing `stepup-1.0.0/tests/cases/amend_voldir_pending/expected_stdout.txt` & `stepup-1.1.0/tests/cases/amend_voldir_pending/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./demo.py
 RESCHEDULE │ ./demo.py
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
 nonexisting/
 ────────────────────────────────────────────────────────────────────────────────
```

### Comparing `stepup-1.0.0/tests/cases/amend_voldir_pending/main.sh` & `stepup-1.1.0/tests/cases/static_abs/main.sh`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,17 @@
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
+[[ -f original.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/deferred_glob1/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/deferred_glob1/expected_graph_01.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
              workdir = ./
              command = cp -aT static/sub/foo.txt copy.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:static/sub/foo.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:static/sub/foo.txt
                 path = static/sub/foo.txt
                state = STATIC
           created by   dg:'static/**'
             consumes   file:static/sub/
             supplies   step:cp -aT static/sub/foo.txt copy.txt
@@ -63,13 +64,14 @@
             supplies   file:static/sub/
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:cp -aT static/sub/foo.txt copy.txt
             consumes   file:./
+            consumes   step:cp -aT static/sub/foo.txt copy.txt
 
 dg:'static/**'
           created by   step:./plan.py
              creates   file:static/
              creates   file:static/sub/
              creates   file:static/sub/foo.txt
```

### Comparing `stepup-1.0.0/tests/cases/deferred_glob1/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/deferred_glob1/expected_graph_02.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             supplies   file:static/sub/
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:cp -aT static/sub/bar.txt copy.txt
             consumes   file:./
+            consumes   step:cp -aT static/sub/bar.txt copy.txt
 
 dg:'static/**'
           created by   step:./plan.py
              creates   file:static/
              creates   file:static/sub/
              creates   file:static/sub/bar.txt
 
@@ -62,14 +63,15 @@
              workdir = ./
              command = cp -aT static/sub/bar.txt copy.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:static/sub/bar.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:static/sub/bar.txt
                 path = static/sub/bar.txt
                state = STATIC
           created by   dg:'static/**'
             consumes   file:static/sub/
             supplies   step:cp -aT static/sub/bar.txt copy.txt
```

### Comparing `stepup-1.0.0/tests/cases/deferred_glob1/main.sh` & `stepup-1.1.0/tests/cases/deferred_glob1/main.sh`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 export ENV_VAR_TEST_STEPUP_INP="static/sub/foo.txt"
 stepup -w 1 plan.py & # > current_stdout_01.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f static/sub/foo.txt ]] || exit -1
 [[ -f copy.txt ]] || exit -1
@@ -29,15 +29,15 @@
 export ENV_VAR_TEST_STEPUP_INP="static/sub/bar.txt"
 stepup -w 1 plan.py & # > current_stdout_02.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f static/sub/foo.txt ]] || exit -1
 [[ -f copy.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/deferred_glob2/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/deferred_glob2/expected_graph_01.txt`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
              workdir = ./
              command = cp -aT static/sub/foo.txt copy.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:static/sub/foo.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:static/sub/foo.txt
                 path = static/sub/foo.txt
                state = STATIC
           created by   dg:'static/**'
             consumes   file:static/sub/
             supplies   step:cp -aT static/sub/foo.txt copy.txt
@@ -68,7 +69,8 @@
             supplies   file:static/sub/
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:cp -aT static/sub/foo.txt copy.txt
             consumes   file:./
+            consumes   step:cp -aT static/sub/foo.txt copy.txt
```

### Comparing `stepup-1.0.0/tests/cases/deferred_glob2/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/deferred_glob2/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/deferred_glob2/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_output/expected_stdout.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
-     START │ cp -aT static/sub/foo.txt copy.txt
-   SUCCESS │ cp -aT static/sub/foo.txt copy.txt
+     START │ cp -aT input.txt output.txt
+   SUCCESS │ cp -aT input.txt output.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ plan.py
-     ADDED │ plan.py
+   DELETED │ output.txt
      PHASE │ run
-     START │ ./plan.py
-   SUCCESS │ ./plan.py
-     CLEAN │ copy.txt
+     START │ cp -aT input.txt output.txt
+   SUCCESS │ cp -aT input.txt output.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/deferred_glob2/main.sh` & `stepup-1.1.0/tests/cases/deferred_glob2/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 cp plan_01.py plan.py
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f static/sub/foo.txt ]] || exit -1
 [[ -f copy.txt ]] || exit -1
 
 # Remove the file foo.txt and verify the consequences
 cp plan_02.py plan.py
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("plan.py")
+watch_update("plan.py")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f static/sub/foo.txt ]] || exit -1
 [[ ! -f copy.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/deferred_subdir/expected_graph.txt` & `stepup-1.1.0/tests/cases/deferred_subdir/expected_graph.txt`

 * *Files 4% similar despite different names*

```diff
@@ -66,20 +66,22 @@
              workdir = sub/
              command = cp -aT used.txt copy.txt
                state = SUCCEEDED
           created by   step:./plan.py  # wd=sub/
             consumes   file:sub/
             consumes   file:sub/used.txt
              creates   file:sub/copy.txt
+            supplies   file:sub/copy.txt
 
 file:sub/used.txt
                 path = sub/used.txt
                state = STATIC
           created by   dg:'sub/u*.txt'
             consumes   file:sub/
             supplies   step:cp -aT used.txt copy.txt  # wd=sub/
 
 file:sub/copy.txt
                 path = sub/copy.txt
                state = BUILT
           created by   step:cp -aT used.txt copy.txt  # wd=sub/
             consumes   file:sub/
+            consumes   step:cp -aT used.txt copy.txt  # wd=sub/
```

### Comparing `stepup-1.0.0/tests/cases/deferred_subdir/main.sh` & `stepup-1.1.0/tests/cases/deferred_subdir/main.sh`

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

### Comparing `stepup-1.0.0/tests/cases/env_vars/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/env_vars/expected_graph_01.txt`

 * *Files 2% similar despite different names*

```diff
@@ -75,13 +75,15 @@
                state = SUCCEEDED
              env_var = ENV_VAR_TEST_STEPUP_AWDFTD
        extended hash = yes
           created by   step:./demovars.py
             consumes   file:./
             consumes   file:printvars.py
              creates   file:current_variables.txt
+            supplies   file:current_variables.txt
 
 file:current_variables.txt
                 path = current_variables.txt
                state = BUILT
           created by   step:./printvars.py
             consumes   file:./
+            consumes   step:./printvars.py
```

### Comparing `stepup-1.0.0/tests/cases/env_vars/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/env_vars/expected_graph_02.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,13 +76,15 @@
              env_var = ENV_VAR_TEST_STEPUP_AWDFTD
                      = ENV_VAR_TEST_STEPUP_DFTHYH
        extended hash = yes
           created by   step:./demovars.py
             consumes   file:./
             consumes   file:printvars.py
              creates   file:current_variables.txt
+            supplies   file:current_variables.txt
 
 file:current_variables.txt
                 path = current_variables.txt
                state = BUILT
           created by   step:./printvars.py
             consumes   file:./
+            consumes   step:./printvars.py
```

### Comparing `stepup-1.0.0/tests/cases/env_vars/expected_graph_03.txt` & `stepup-1.1.0/tests/cases/env_vars/expected_graph_03.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,13 +76,15 @@
              env_var = ENV_VAR_TEST_STEPUP_AWDFTD
                      = ENV_VAR_TEST_STEPUP_DFTHYH
        extended hash = yes
           created by   step:./demovars.py
             consumes   file:./
             consumes   file:printvars.py
              creates   file:current_variables.txt
+            supplies   file:current_variables.txt
 
 file:current_variables.txt
                 path = current_variables.txt
                state = BUILT
           created by   step:./printvars.py
             consumes   file:./
+            consumes   step:./printvars.py
```

### Comparing `stepup-1.0.0/tests/cases/env_vars/expected_graph_04.txt` & `stepup-1.1.0/tests/cases/env_vars/expected_graph_04.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,13 +76,15 @@
              env_var = ENV_VAR_TEST_STEPUP_AWDFTD
                      = ENV_VAR_TEST_STEPUP_DFTHYH
        extended hash = yes
           created by   step:./demovars.py
             consumes   file:./
             consumes   file:printvars.py
              creates   file:current_variables.txt
+            supplies   file:current_variables.txt
 
 file:current_variables.txt
                 path = current_variables.txt
                state = BUILT
           created by   step:./printvars.py
             consumes   file:./
+            consumes   step:./printvars.py
```

### Comparing `stepup-1.0.0/tests/cases/env_vars/expected_graph_05.txt` & `stepup-1.1.0/tests/cases/env_vars/expected_graph_05.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,13 +76,15 @@
              env_var = ENV_VAR_TEST_STEPUP_AWDFTD
                      = ENV_VAR_TEST_STEPUP_DFTHYH
        extended hash = yes
           created by   step:./demovars.py
             consumes   file:./
             consumes   file:printvars.py
              creates   file:current_variables.txt
+            supplies   file:current_variables.txt
 
 file:current_variables.txt
                 path = current_variables.txt
                state = BUILT
           created by   step:./printvars.py
             consumes   file:./
+            consumes   step:./printvars.py
```

### Comparing `stepup-1.0.0/tests/cases/env_vars/expected_stdout_a.txt` & `stepup-1.1.0/tests/cases/env_vars/expected_stdout_a.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./demovars.py
    SUCCESS │ ./demovars.py
      START │ ./printvars.py
    SUCCESS │ ./printvars.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ variables.json
-     ADDED │ variables.json
+   UPDATED │ variables.json
      PHASE │ run
     NOSKIP │ ./demovars.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
 Modified step hash   extended, digest 85c835c6 ➜ 58d07c3f, inp_digset 85c835c6 ➜ 58d07c3f
 Modified inp hash    variables.json (digest 9fcdaff9 ➜ b38f0cd4, size 35 ➜ 67)
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
@@ -21,16 +20,15 @@
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./demovars.py
    SUCCESS │ ./demovars.py
      START │ ./printvars.py
    SUCCESS │ ./printvars.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ variables.json
-     ADDED │ variables.json
+   UPDATED │ variables.json
      PHASE │ run
       SKIP │ ./demovars.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 58d07c3f, inp_digset 58d07c3f
 Same inp hash        ./
 Same inp hash        demovars.py
 Same inp hash        variables.json
```

### Comparing `stepup-1.0.0/tests/cases/env_vars/expected_stdout_b.txt` & `stepup-1.1.0/tests/cases/env_vars/expected_stdout_b.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest a0d7eeeb, inp_digset a0d7eeeb
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
       SKIP │ ./demovars.py
```

### Comparing `stepup-1.0.0/tests/cases/env_vars/expected_stdout_c.txt` & `stepup-1.1.0/tests/cases/env_vars/expected_stdout_d.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest a0d7eeeb, inp_digset a0d7eeeb
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
       SKIP │ ./demovars.py
@@ -12,16 +12,16 @@
 Same step hash       extended, digest 58d07c3f, inp_digset 58d07c3f
 Same inp hash        ./
 Same inp hash        demovars.py
 Same inp hash        variables.json
 ────────────────────────────────────────────────────────────────────────────────
     NOSKIP │ ./printvars.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
-Modified step hash   extended, digest 4b6ff17e ➜ ec75d2f2, inp_digset b6f74e79 ➜ b3c18f7e
-Modified env var     ENV_VAR_TEST_STEPUP_AWDFTD ='AAAA' ➜ (unset)
+Modified step hash   extended, digest 759b9c26 ➜ cb1aa93f, inp_digset b3c18f7e ➜ a11013a2
+Modified env var     ENV_VAR_TEST_STEPUP_AWDFTD (unset) ➜ ='DDDD'
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
 Same inp hash        printvars.py
 Same env var         ENV_VAR_TEST_STEPUP_DFTHYH ='CCCC'
 Same out hash        current_variables.txt
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./printvars.py
```

### Comparing `stepup-1.0.0/tests/cases/env_vars/expected_stdout_d.txt` & `stepup-1.1.0/tests/cases/env_vars/expected_stdout_c.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest a0d7eeeb, inp_digset a0d7eeeb
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
       SKIP │ ./demovars.py
@@ -12,16 +12,16 @@
 Same step hash       extended, digest 58d07c3f, inp_digset 58d07c3f
 Same inp hash        ./
 Same inp hash        demovars.py
 Same inp hash        variables.json
 ────────────────────────────────────────────────────────────────────────────────
     NOSKIP │ ./printvars.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
-Modified step hash   extended, digest 759b9c26 ➜ cb1aa93f, inp_digset b3c18f7e ➜ a11013a2
-Modified env var     ENV_VAR_TEST_STEPUP_AWDFTD (unset) ➜ ='DDDD'
+Modified step hash   extended, digest 4b6ff17e ➜ ec75d2f2, inp_digset b6f74e79 ➜ b3c18f7e
+Modified env var     ENV_VAR_TEST_STEPUP_AWDFTD ='AAAA' ➜ (unset)
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
 Same inp hash        printvars.py
 Same env var         ENV_VAR_TEST_STEPUP_DFTHYH ='CCCC'
 Same out hash        current_variables.txt
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./printvars.py
```

### Comparing `stepup-1.0.0/tests/cases/env_vars/main.sh` & `stepup-1.1.0/tests/cases/env_vars/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -12,46 +12,46 @@
 cp variables_01.json variables.json
 stepup -e -w 1 plan.py & # > current_stdout_a.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 grep AAAA current_variables.txt
 cp current_variables.txt current_variables_01.txt
 
 # Rerun with changed file variables.json
 cp variables_02.json variables.json
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("variables.json")
+watch_update("variables.json")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 grep AAAA current_variables.txt
 grep BBBB current_variables.txt
 cp current_variables.txt current_variables_02.txt
 
 # Rerun with UNchanged file variables.json
 touch variables.json
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("variables.json")
+watch_update("variables.json")
 run()
 wait()
-graph("current_graph_03.txt")
+graph("current_graph_03")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -64,15 +64,15 @@
 export ENV_VAR_TEST_STEPUP_DFTHYH="CCCC"
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_04.txt")
+graph("current_graph_04")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -85,15 +85,15 @@
 unset ENV_VAR_TEST_STEPUP_AWDFTD
 stepup -e -w 1 plan.py & # > current_stdout_c.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_05.txt")
+graph("current_graph_05")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 grep -v AAAA current_variables.txt
 grep CCCC current_variables.txt
@@ -106,15 +106,15 @@
 export ENV_VAR_TEST_STEPUP_AWDFTD="DDDD"
 stepup -e -w 1 plan.py & # > current_stdout_d.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_06.txt")
+graph("current_graph_06")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 grep DDDD current_variables.txt
 grep CCCC current_variables.txt
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_amend/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/env_vars_amend/expected_graph_01.txt`

 * *Files 10% similar despite different names*

```diff
@@ -45,13 +45,15 @@
                state = SUCCEEDED
    env_var (amended) = ENV_VAR_TEST_STEPUP_SDASFD
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:demovars.py
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
           created by   step:./demovars.py > output.txt
             consumes   file:./
+            consumes   step:./demovars.py > output.txt
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_amend/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/env_vars_amend/expected_graph_02.txt`

 * *Files 10% similar despite different names*

```diff
@@ -45,13 +45,15 @@
                state = SUCCEEDED
    env_var (amended) = ENV_VAR_TEST_STEPUP_SDASFD
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:demovars.py
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
           created by   step:./demovars.py > output.txt
             consumes   file:./
+            consumes   step:./demovars.py > output.txt
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_amend/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/env_vars_amend/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 80ac726d, inp_digset 80ac726d
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
     NOSKIP │ ./demovars.py > output.txt
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_amend/main.sh` & `stepup-1.1.0/tests/cases/env_vars_amend/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Run the example
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 grep AAAA output.txt
 
@@ -27,15 +27,15 @@
 
 # Rerstart with changed variable
 export ENV_VAR_TEST_STEPUP_SDASFD="BBBB"
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 grep BBBB output.txt
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_path/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/env_vars_path/expected_graph_01.txt`

 * *Files 5% similar despite different names*

```diff
@@ -47,19 +47,23 @@
                state = FAILED
              env_var = ENV_VAR_TEST_STEPUP_PREFIX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:README.md
              creates   file:README-stderr.txt
              creates   file:README-stdout.txt
+            supplies   file:README-stderr.txt
+            supplies   file:README-stdout.txt
 
 file:README-stdout.txt
                 path = README-stdout.txt
                state = PENDING
           created by   step:grep variable README.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > README-stdout.txt 2> README-stderr.txt
             consumes   file:./
+            consumes   step:grep variable README.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > README-stdout.txt 2> README-stderr.txt
 
 file:README-stderr.txt
                 path = README-stderr.txt
                state = VOLATILE
           created by   step:grep variable README.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > README-stdout.txt 2> README-stderr.txt
             consumes   file:./
+            consumes   step:grep variable README.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > README-stdout.txt 2> README-stderr.txt
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_path/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/env_vars_path/expected_graph_02.txt`

 * *Files 4% similar despite different names*

```diff
@@ -48,19 +48,23 @@
              env_var = ENV_VAR_TEST_STEPUP_PREFIX
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:FOO.md
              creates   file:FOO-stderr.txt
              creates   file:FOO-stdout.txt
+            supplies   file:FOO-stderr.txt
+            supplies   file:FOO-stdout.txt
 
 file:FOO-stdout.txt
                 path = FOO-stdout.txt
                state = BUILT
           created by   step:grep variable FOO.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > FOO-stdout.txt 2> FOO-stderr.txt
             consumes   file:./
+            consumes   step:grep variable FOO.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > FOO-stdout.txt 2> FOO-stderr.txt
 
 file:FOO-stderr.txt
                 path = FOO-stderr.txt
                state = VOLATILE
           created by   step:grep variable FOO.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > FOO-stdout.txt 2> FOO-stderr.txt
             consumes   file:./
+            consumes   step:grep variable FOO.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > FOO-stdout.txt 2> FOO-stderr.txt
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_path/expected_stdout_01.txt` & `stepup-1.1.0/tests/cases/env_vars_path/expected_stdout_01.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ grep variable README.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > README-stdout.txt 2> README-stderr.txt
       FAIL │ grep variable README.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > README-stdout.txt 2> README-stderr.txt
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               grep variable README.md ${ENV_VAR_TEST_STEPUP_PREFIX}.txt > README-stdout.txt 2> README-stderr.txt
 Return code           2
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_path/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/env_vars_path/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
     NOSKIP │ ./plan.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
 Modified step hash   extended, digest 20bbb647 ➜ c4b2f903, inp_digset 20bbb647 ➜ c4b2f903
 Modified env var     ENV_VAR_TEST_STEPUP_PREFIX ='README' ➜ ='FOO'
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
 Same inp hash        plan.py
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_path/main.sh` & `stepup-1.1.0/tests/cases/env_vars_path/main.sh`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 export ENV_VAR_TEST_STEPUP_PREFIX="README"
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f README-stdout.txt ]] || exit -1
 [[ -f README-stderr.txt ]] || exit -1
@@ -28,15 +28,15 @@
 export ENV_VAR_TEST_STEPUP_PREFIX="FOO"
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ ! -f README-stdout.txt ]] || exit -1
 [[ ! -f README-stderr.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_subs/expected_graph.txt` & `stepup-1.1.0/tests/cases/env_vars_subs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/env_vars_subs/expected_stdout.txt` & `stepup-1.1.0/tests/cases/env_vars_subs/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
 ─────────────────────────────── Standard output ────────────────────────────────
 sub
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./plan.py  # wd=sub/
    SUCCESS │ ./plan.py  # wd=sub/
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_subs/main.sh` & `stepup-1.1.0/tests/cases/env_vars_subs/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 export DELAYED='${HERE}/foo.txt'
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
 [[ -f sub/plan.py ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_workdir/expected_graph.txt` & `stepup-1.1.0/tests/cases/env_vars_workdir/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -51,13 +51,15 @@
              workdir = sub/
              command = cat input.txt > output.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:sub/
             consumes   file:sub/input.txt
              creates   file:sub/output.txt
+            supplies   file:sub/output.txt
 
 file:sub/output.txt
                 path = sub/output.txt
                state = BUILT
           created by   step:cat input.txt > output.txt  # wd=sub/
             consumes   file:sub/
+            consumes   step:cat input.txt > output.txt  # wd=sub/
```

### Comparing `stepup-1.0.0/tests/cases/env_vars_workdir/main.sh` & `stepup-1.1.0/tests/cases/env_vars_workdir/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 export INP_VAR_TEST_STEPUP_WORKDIR="sub"
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
 [[ -f sub/input.txt ]] || exit -1
 [[ -f sub/output.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/error_cyclic_early/expected_graph.txt` & `stepup-1.1.0/tests/cases/error_main_fails/expected_graph_02.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,25 +11,29 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:README.md
+            supplies   (file:output.txt)
             supplies   file:plan.py
             supplies   step:./plan.py
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = FAILED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:README.md
 
-file:README.md
-                path = README.md
-               state = STATIC
-          created by   step:./plan.py
+(step:touch output.txt)
+             workdir = ./
+             command = touch output.txt
+               state = SUCCEEDED
+       extended hash = yes
+
+(file:output.txt)
+                path = output.txt
+               state = BUILT
             consumes   file:./
```

### Comparing `stepup-1.0.0/tests/cases/error_cyclic_early/main.sh` & `stepup-1.1.0/tests/cases/amend_outdir_pending/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,16 @@
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
```

### Comparing `stepup-1.0.0/tests/cases/error_cyclic_late/expected_graph.txt` & `stepup-1.1.0/tests/cases/error_cyclic_late/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/error_cyclic_late/main.sh` & `stepup-1.1.0/tests/cases/error_cyclic_late/main.sh`

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

### Comparing `stepup-1.0.0/tests/cases/error_deferred_nonexisting/expected_graph.txt` & `stepup-1.1.0/tests/cases/restart_deferred_glob/expected_graph_01.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,61 +14,47 @@
 file:./
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:plan.py
             supplies   file:static/
             supplies   step:./plan.py
-            supplies   step:cat static/foo/bar/README.md
+            supplies   step:cat static/foo.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
+       extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
              creates   dg:'static/**'
-             creates   step:cat static/foo/bar/README.md
+             creates   step:cat static/foo.txt
 
 dg:'static/**'
           created by   step:./plan.py
              creates   file:static/
-             creates   file:static/foo/
-             creates   file:static/foo/bar/
-             creates   file:static/foo/bar/README.md
+             creates   file:static/foo.txt
 
-step:cat static/foo/bar/README.md
+step:cat static/foo.txt
              workdir = ./
-             command = cat static/foo/bar/README.md
-               state = FAILED
+             command = cat static/foo.txt
+               state = SUCCEEDED
+       extended hash = yes
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:static/foo/bar/README.md
-
-file:static/foo/bar/README.md
-                path = static/foo/bar/README.md
-               state = STATIC
-          created by   dg:'static/**'
-            consumes   file:static/foo/bar/
-            supplies   step:cat static/foo/bar/README.md
-
-file:static/foo/bar/
-                path = static/foo/bar/
-               state = STATIC
-          created by   dg:'static/**'
-            consumes   file:static/foo/
-            supplies   file:static/foo/bar/README.md
+            consumes   file:static/foo.txt
 
-file:static/foo/
-                path = static/foo/
+file:static/foo.txt
+                path = static/foo.txt
                state = STATIC
           created by   dg:'static/**'
             consumes   file:static/
-            supplies   file:static/foo/bar/
+            supplies   step:cat static/foo.txt
 
 file:static/
                 path = static/
                state = STATIC
           created by   dg:'static/**'
             consumes   file:./
-            supplies   file:static/foo/
+            supplies   file:static/foo.txt
```

### Comparing `stepup-1.0.0/tests/cases/error_deferred_nonexisting/expected_stdout.txt` & `stepup-1.1.0/tests/cases/error_env_var/expected_stdout.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
-   SUCCESS │ ./plan.py
-      FAIL │ cat static/foo/bar/README.md
+      FAIL │ ./plan.py
 ────────────────────────────────── Step info ───────────────────────────────────
-Command               cat static/foo/bar/README.md
-──────────────────────────────── Invalid inputs ────────────────────────────────
-STATIC Path does not exist: static/foo/bar/README.md
+Command               ./plan.py
+Return code           1
+──────────────────────────────── Standard error ────────────────────────────────
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step(s) failed, see error messages above
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/error_deferred_nonexisting/main.sh` & `stepup-1.1.0/tests/cases/amend_voldir_pending/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,16 @@
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
```

### Comparing `stepup-1.0.0/tests/cases/error_env_var/expected_graph.txt` & `stepup-1.1.0/tests/cases/error_env_var/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/error_env_var/expected_stdout.txt` & `stepup-1.1.0/tests/cases/amend_missing/expected_stdout.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
-      FAIL │ ./plan.py
+   SUCCESS │ ./plan.py
+     START │ ./step.py
+RESCHEDULE │ ./step.py
+──────────────── Rescheduling due to unavailable amended inputs ────────────────
+missing.txt
+────────────────────────────────────────────────────────────────────────────────
+     START │ echo Will be deleted by accident > missing.txt
+   SUCCESS │ echo Will be deleted by accident > missing.txt
+     START │ ./step.py
+      FAIL │ ./step.py
 ────────────────────────────────── Step info ───────────────────────────────────
-Command               ./plan.py
+Command               ./step.py
 Return code           1
 ──────────────────────────────── Standard error ────────────────────────────────
-Traceback (most recent call last):
-  File "${CASE}/./plan.py", line ---, in <module>
-    step("echo > foo", out=["${ENV_VAR_TEST_STEPUP_NON_EXISTING}.txt"])
-  File "${PWD}/stepup/core/api.py", line ---, in step
-    out_paths = [translate(subs(out_path)) for out_path in out_paths]
-                           ^^^^^^^^^^^^^^
-  File "${PWD}/stepup/core/api.py", line ---, in subs
-    raise ValueError(f"Undefined shell variable: {name}")
-ValueError: Undefined shell variable: ENV_VAR_TEST_STEPUP_NON_EXISTING
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step(s) failed, see error messages above
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/error_env_var/main.sh` & `stepup-1.1.0/tests/cases/static_dir/main.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
+# Prepare subdir
+mkdir -p subdir
+
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
 
-# Check files that are expected to be present and/or missing.
-[[ -f plan.py ]] || exit -1
-
 # Wait for background processes, if any.
 wait $(jobs -p)
+
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -d subdir ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/error_main_fails/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/nodata/expected_graph_02.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,36 +11,39 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:output.txt
+            supplies   file:analyzed.txt
             supplies   file:plan.py
             supplies   step:./plan.py
-            supplies   step:touch output.txt
+            supplies   step:cat analyzed.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
+                 ngm = ['data.txt'] {}
        extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   step:touch output.txt
+             creates   file:analyzed.txt
+             creates   step:cat analyzed.txt
 
-step:touch output.txt
+file:analyzed.txt
+                path = analyzed.txt
+               state = STATIC
+          created by   step:./plan.py
+            consumes   file:./
+            supplies   step:cat analyzed.txt
+
+step:cat analyzed.txt
              workdir = ./
-             command = touch output.txt
+             command = cat analyzed.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
-             creates   file:output.txt
-
-file:output.txt
-                path = output.txt
-               state = BUILT
-          created by   step:touch output.txt
-            consumes   file:./
+            consumes   file:analyzed.txt
```

### Comparing `stepup-1.0.0/tests/cases/error_main_fails/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_wanted/expected_graph_03.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,25 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   (file:output.txt)
+            supplies   file:input2.txt
             supplies   file:plan.py
             supplies   step:./plan.py
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
-               state = FAILED
+               state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
+             creates   file:input2.txt
 
-(step:touch output.txt)
-             workdir = ./
-             command = touch output.txt
-               state = SUCCEEDED
-       extended hash = yes
-
-(file:output.txt)
-                path = output.txt
-               state = BUILT
+file:input2.txt
+                path = input2.txt
+               state = STATIC
+          created by   step:./plan.py
             consumes   file:./
```

### Comparing `stepup-1.0.0/tests/cases/error_main_fails/main.sh` & `stepup-1.1.0/tests/cases/error_main_fails/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 cp plan_01.py plan.py
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -27,15 +27,15 @@
 cp plan_02.py plan.py
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/error_not_executable/expected_stdout.txt` & `stepup-1.1.0/tests/cases/error_not_executable/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/error_overlap_deferred/expected_stdout.txt` & `stepup-1.1.0/tests/cases/error_main_fails/expected_stdout_02.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,24 @@
-     PHASE │ run
+  WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
   DIRECTOR │ Launched worker 0
+     PHASE │ run
+    NOSKIP │ ./plan.py
+──────────────────────────── Changes causing rerun ─────────────────────────────
+Modified step hash   extended, digest 53ca023c ➜ cc5deac6, inp_digset 53ca023c ➜ cc5deac6
+Modified inp hash    plan.py (digest 98e52b4a ➜ 66b966f4, size 101 ➜ 36)
+────────────────────────────── Remained the same ───────────────────────────────
+Same inp hash        ./
+────────────────────────────────────────────────────────────────────────────────
      START │ ./plan.py
       FAIL │ ./plan.py
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               ./plan.py
 Return code           1
 ──────────────────────────────── Standard error ────────────────────────────────
-Traceback (most recent call last):
-  File "${CASE}/./plan.py", line ---, in <module>
-    step("cat README.md", inp="README.md")
-  File "${PWD}/stepup/core/api.py", line ---, in step
-    return RPC_CLIENT(
-           ^^^^^^^^^^^
-  File "${PWD}/stepup/core/rpc.py", line ---, in __call__
-    _handle_error(body, name, args, kwargs)
-  File "${PWD}/stepup/core/rpc.py", line ---, in _handle_error
-    raise RPCError(f"An exception was raised in the server during the call {fmt_call}: \n\n{body}")
-stepup.core.exceptions.RPCError: An exception was raised in the server during the call step('step:./plan.py', 'cat README.md', [Path('README.md')], (), [], [], Path('./'), False, None, False):
-
-Traceback (most recent call last):
-  File "${PWD}/stepup/core/rpc.py", line ---, in _handle_request
-    result = call(*bound.args, **bound.kwargs)
-             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-  File "${PWD}/stepup/core/director.py", line ---, in step
-    return self._workflow.define_step(
-           ^^^^^^^^^^^^^^^^^^^^^^^^^^^
-  File "${PWD}/stepup/core/workflow.py", line ---, in define_step
-    self.supply_file(step_key, inp_path)
-  File "${PWD}/stepup/core/workflow.py", line ---, in supply_file
-    dg = self.matching_deferred_glob(path)
-         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-  File "${PWD}/stepup/core/workflow.py", line ---, in matching_deferred_glob
-    raise GraphError(f"Multiple deferred globs match: {path}")
-stepup.core.exceptions.GraphError: Multiple deferred globs match: README.md
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step(s) failed, see error messages above
-   WARNING │ Scheduler is put on hold. Not reporting pending steps.
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
-   WARNING │ Dissolving the workflow due to an exceptions while the graph was being changed.
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/error_overlap_deferred/main.sh` & `stepup-1.1.0/tests/cases/error_static_dir/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,16 @@
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
```

### Comparing `stepup-1.0.0/tests/cases/error_static_dir/expected_graph.txt` & `stepup-1.1.0/tests/cases/error_static_dir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/error_static_dir/expected_stdout.txt` & `stepup-1.1.0/tests/cases/permissions_plan_restart/expected_stdout_02.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-     PHASE │ run
+  WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
   DIRECTOR │ Launched worker 0
-     START │ ./plan.py
-      FAIL │ ./plan.py
-────────────────────────────────── Step info ───────────────────────────────────
-Command               ./plan.py
-Return code           1
-──────────────────────────────── Standard error ────────────────────────────────
-Traceback (most recent call last):
-  File "${CASE}/./plan.py", line ---, in <module>
-    static("subdir")
-  File "${PWD}/stepup/core/api.py", line ---, in static
-    check_inp_paths(su_paths)
-  File "${PWD}/stepup/core/api.py", line ---, in check_inp_paths
-    raise ValueError(f"{message}: {inp_path}")
-ValueError: Directory without trailing separator: subdir
+     PHASE │ run
+      SKIP │ ./plan.py
+───────────────────────────── No changes observed ──────────────────────────────
+Same step hash       extended, digest 97a2efee, inp_digset 97a2efee
+Same inp hash        ./
+Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
-   WARNING │ 1 step(s) failed, see error messages above
-   WARNING │ Skipping cleanup due to incomplete build.
+     START │ ./plan.py  # wd=sub/
+   SUCCESS │ ./plan.py  # wd=sub/
+     START │ touch done.txt  # wd=sub/
+   SUCCESS │ touch done.txt  # wd=sub/
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/error_static_dir/main.sh` & `stepup-1.1.0/tests/cases/reqdir_missing/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
+mkdir -p sub/dir/nested
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
+[[ ! -f sub/dir/nested/hello.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/error_step/expected_graph.txt` & `stepup-1.1.0/tests/cases/error_step/expected_graph.txt`

 * *Files 11% similar despite different names*

```diff
@@ -32,13 +32,15 @@
 step:rm .sjdksjdfkjasdfkdjsak
              workdir = ./
              command = rm .sjdksjdfkjasdfkdjsak
                state = FAILED
           created by   step:./plan.py
             consumes   file:./
              creates   file:oops.txt
+            supplies   file:oops.txt
 
 file:oops.txt
                 path = oops.txt
                state = PENDING
           created by   step:rm .sjdksjdfkjasdfkdjsak
             consumes   file:./
+            consumes   step:rm .sjdksjdfkjasdfkdjsak
```

### Comparing `stepup-1.0.0/tests/cases/error_step/expected_stdout.txt` & `stepup-1.1.0/tests/cases/error_step/expected_stdout.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ rm .sjdksjdfkjasdfkdjsak
       FAIL │ rm .sjdksjdfkjasdfkdjsak
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               rm .sjdksjdfkjasdfkdjsak
 Return code           1
 ───────────────────────── Expected outputs not created ─────────────────────────
 oops.txt
 ──────────────────────────────── Standard error ────────────────────────────────
-rm: cannot remove '.sjdksjdfkjasdfkdjsak': No such file or directory
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step(s) failed, see error messages above
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/error_step/main.sh` & `stepup-1.1.0/tests/cases/mkdir/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,18 @@
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
+[[ -f sub/foo.txt ]] || exit -1
+[[ -f exists/.keep ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/here/expected_graph.txt` & `stepup-1.1.0/tests/cases/here/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -59,45 +59,49 @@
              workdir = ./
              command = mkdir -p ../public/
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:../
             consumes   file:./
              creates   file:../public/
+            supplies   file:../public/
 
 file:../
                 path = ../
                state = STATIC
           created by   root:
             consumes   file:./
             supplies   file:../public/
             supplies   step:mkdir -p ../public/
 
 file:../public/
                 path = ../public/
                state = BUILT
           created by   step:mkdir -p ../public/
             consumes   file:../
+            consumes   step:mkdir -p ../public/
             supplies   file:../public/www/
             supplies   step:mkdir -p ../public/www/
 
 step:mkdir -p ../public/www/
              workdir = ./
              command = mkdir -p ../public/www/
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:../public/
             consumes   file:./
              creates   file:../public/www/
+            supplies   file:../public/www/
 
 file:../public/www/
                 path = ../public/www/
                state = BUILT
           created by   step:mkdir -p ../public/www/
             consumes   file:../public/
+            consumes   step:mkdir -p ../public/www/
             supplies   file:../public/www/index.md
             supplies   step:cp -aT index.md ../../public/www/index.md  # wd=www/
 
 step:./plan.py  # wd=www/
              workdir = www/
              command = ./plan.py
                state = SUCCEEDED
@@ -122,13 +126,15 @@
              command = cp -aT index.md ../../public/www/index.md
                state = SUCCEEDED
           created by   step:./plan.py  # wd=www/
             consumes   file:../public/www/
             consumes   file:www/
             consumes   file:www/index.md
              creates   file:../public/www/index.md
+            supplies   file:../public/www/index.md
 
 file:../public/www/index.md
                 path = ../public/www/index.md
                state = BUILT
           created by   step:cp -aT index.md ../../public/www/index.md  # wd=www/
             consumes   file:../public/www/
+            consumes   step:cp -aT index.md ../../public/www/index.md  # wd=www/
```

### Comparing `stepup-1.0.0/tests/cases/here/expected_stdout.txt` & `stepup-1.1.0/tests/cases/here/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Changing to ${CASE}/source
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ mkdir -p ../public/
    SUCCESS │ mkdir -p ../public/
      START │ ./plan.py  # wd=www/
    SUCCESS │ ./plan.py  # wd=www/
      START │ mkdir -p ../public/www/
```

### Comparing `stepup-1.0.0/tests/cases/here/main.sh` & `stepup-1.1.0/tests/cases/here/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 export PUBLIC="../public"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("../current_graph.txt")
+graph("../current_graph")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f source/plan.py ]] || exit -1
 [[ -f source/www/plan.py ]] || exit -1
 [[ -f source/www/index.md ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/makedirs/expected_graph.txt` & `stepup-1.1.0/tests/cases/makedirs/expected_graph.txt`

 * *Files 10% similar despite different names*

```diff
@@ -37,67 +37,81 @@
           created by   step:./plan.py
             consumes   file:./
 
 step:./bunch.py
              workdir = ./
              command = ./bunch.py
                state = SUCCEEDED
-   creates (amended) = file:sub/one/
+  supplies (amended) = file:sub/one/
                      = file:sub/one/bar/
                      = file:sub/one/bar/text
           created by   step:./plan.py
             consumes   file:./
              creates   file:sub/
              creates   file:sub/one/
              creates   file:sub/one/bar/
              creates   file:sub/one/bar/text
              creates   file:sub/other/
              creates   file:sub/other/foo/
              creates   file:sub/other/foo/text
+            supplies   file:sub/
+            supplies   file:sub/one/
+            supplies   file:sub/one/bar/
+            supplies   file:sub/one/bar/text
+            supplies   file:sub/other/
+            supplies   file:sub/other/foo/
+            supplies   file:sub/other/foo/text
 
 file:sub/
                 path = sub/
                state = BUILT
           created by   step:./bunch.py
             consumes   file:./
+            consumes   step:./bunch.py
             supplies   file:sub/one/
             supplies   file:sub/other/
 
 file:sub/other/
                 path = sub/other/
                state = BUILT
           created by   step:./bunch.py
             consumes   file:sub/
+            consumes   step:./bunch.py
             supplies   file:sub/other/foo/
 
 file:sub/other/foo/
                 path = sub/other/foo/
                state = BUILT
           created by   step:./bunch.py
             consumes   file:sub/other/
+            consumes   step:./bunch.py
             supplies   file:sub/other/foo/text
 
 file:sub/other/foo/text
                 path = sub/other/foo/text
                state = BUILT
           created by   step:./bunch.py
             consumes   file:sub/other/foo/
+            consumes   step:./bunch.py
 
 file:sub/one/
                 path = sub/one/
                state = BUILT
           created by   step:./bunch.py
             consumes   file:sub/
+            consumes   step:./bunch.py
             supplies   file:sub/one/bar/
 
 file:sub/one/bar/
                 path = sub/one/bar/
                state = BUILT
           created by   step:./bunch.py
             consumes   file:sub/one/
+            consumes   step:./bunch.py
             supplies   file:sub/one/bar/text
 
 file:sub/one/bar/text
                 path = sub/one/bar/text
                state = BUILT
           created by   step:./bunch.py
             consumes   file:sub/one/bar/
+            consumes   step:./bunch.py
```

### Comparing `stepup-1.0.0/tests/cases/makedirs/main.sh` & `stepup-1.1.0/tests/cases/script_cases/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,20 @@
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
 
-# Check files that are expected to be present and/or missing.
-[[ -f plan.py ]] || exit -1
-[[ -f sub/other/foo/text ]] || exit -1
-[[ -f sub/one/bar/text ]] || exit -1
-
 # Wait for background processes, if any.
 wait $(jobs -p)
+
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f helper.py ]] || exit -1
+[[ -f work.py ]] || exit -1
+[[ -f data-5.0.txt ]] || exit -1
+[[ -f data+7.0.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/mkdir/expected_graph.txt` & `stepup-1.1.0/tests/cases/mkdir/expected_graph.txt`

 * *Files 10% similar despite different names*

```diff
@@ -37,44 +37,50 @@
 step:mkdir -p sub/
              workdir = ./
              command = mkdir -p sub/
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:sub/
+            supplies   file:sub/
 
 file:sub/
                 path = sub/
                state = BUILT
           created by   step:mkdir -p sub/
             consumes   file:./
+            consumes   step:mkdir -p sub/
             supplies   file:sub/foo.txt
             supplies   step:touch sub/foo.txt
 
 step:touch sub/foo.txt
              workdir = ./
              command = touch sub/foo.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:sub/
              creates   file:sub/foo.txt
+            supplies   file:sub/foo.txt
 
 file:sub/foo.txt
                 path = sub/foo.txt
                state = BUILT
           created by   step:touch sub/foo.txt
             consumes   file:sub/
+            consumes   step:touch sub/foo.txt
 
 step:mkdir -p exists/
              workdir = ./
              command = mkdir -p exists/
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:exists/
+            supplies   file:exists/
 
 file:exists/
                 path = exists/
                state = BUILT
           created by   step:mkdir -p exists/
             consumes   file:./
+            consumes   step:mkdir -p exists/
```

### Comparing `stepup-1.0.0/tests/cases/mkdir/main.sh` & `stepup-1.1.0/tests/cases/pool/main.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-stepup -w 1 plan.py & # > current_stdout.txt &
+stepup -w 2 plan.py & # > current_stdout.txt &
 
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
-[[ -f sub/foo.txt ]] || exit -1
-[[ -f exists/.keep ]] || exit -1
+[[ -f r.txt ]] || exit -1
+[[ ! -f u.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/mkdir_error/expected_graph.txt` & `stepup-1.1.0/tests/cases/mkdir_error/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
              workdir = ./
              command = mkdir -p sub/blub/pup/
                state = PENDING
           created by   step:./plan.py
             consumes   file:./
             consumes   (file:sub/blub/)
              creates   file:sub/blub/pup/
+            supplies   file:sub/blub/pup/
 
 (file:sub/blub/)
                 path = sub/blub/
                state = PENDING
             consumes   (file:sub/)
             supplies   file:sub/blub/pup/
             supplies   step:mkdir -p sub/blub/pup/
@@ -52,7 +53,8 @@
             supplies   (file:sub/blub/)
 
 file:sub/blub/pup/
                 path = sub/blub/pup/
                state = PENDING
           created by   step:mkdir -p sub/blub/pup/
             consumes   (file:sub/blub/)
+            consumes   step:mkdir -p sub/blub/pup/
```

### Comparing `stepup-1.0.0/tests/cases/mkdir_error/expected_stdout.txt` & `stepup-1.1.0/tests/cases/mkdir_error/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
    WARNING │ 1 step remains pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
 Command               mkdir -p sub/blub/pup/
 Working directory     ./
 Inputs        STATIC  ./
```

### Comparing `stepup-1.0.0/tests/cases/mkdir_error/main.sh` & `stepup-1.1.0/tests/cases/makedirs/main.sh`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,18 @@
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
 
-# Wait for background processes, if any.
-wait $(jobs -p)
-
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
+[[ -f sub/other/foo/text ]] || exit -1
+[[ -f sub/one/bar/text ]] || exit -1
+
+# Wait for background processes, if any.
+wait $(jobs -p)
```

### Comparing `stepup-1.0.0/tests/cases/nodata/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/nodata/expected_graph_01.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,20 +47,22 @@
              command = grep -i foo data.txt > analyzed.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:data.txt
              creates   file:analyzed.txt
+            supplies   file:analyzed.txt
 
 file:analyzed.txt
                 path = analyzed.txt
                state = BUILT
           created by   step:grep -i foo data.txt > analyzed.txt
             consumes   file:./
+            consumes   step:grep -i foo data.txt > analyzed.txt
             supplies   step:cat analyzed.txt
 
 step:cat analyzed.txt
              workdir = ./
              command = cat analyzed.txt
                state = SUCCEEDED
        extended hash = yes
```

### Comparing `stepup-1.0.0/tests/cases/nodata/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/static/expected_graph.txt`

 * *Files 21% similar despite different names*

```diff
@@ -11,39 +11,25 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:analyzed.txt
+            supplies   file:original.txt
             supplies   file:plan.py
             supplies   step:./plan.py
-            supplies   step:cat analyzed.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
-                 ngm = ['data.txt'] {}
-       extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:analyzed.txt
-             creates   step:cat analyzed.txt
+             creates   file:original.txt
 
-file:analyzed.txt
-                path = analyzed.txt
+file:original.txt
+                path = original.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:cat analyzed.txt
-
-step:cat analyzed.txt
-             workdir = ./
-             command = cat analyzed.txt
-               state = SUCCEEDED
-       extended hash = yes
-          created by   step:./plan.py
-            consumes   file:./
-            consumes   file:analyzed.txt
```

### Comparing `stepup-1.0.0/tests/cases/nodata/expected_graph_03.txt` & `stepup-1.1.0/tests/cases/nodata/expected_graph_03.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
              creates   step:grep -i foo data.txt > analyzed.txt
 
 file:analyzed.txt
                 path = analyzed.txt
                state = BUILT
           created by   step:grep -i foo data.txt > analyzed.txt
             consumes   file:./
+            consumes   step:grep -i foo data.txt > analyzed.txt
             supplies   step:cat analyzed.txt
 
 step:cat analyzed.txt
              workdir = ./
              command = cat analyzed.txt
                state = SUCCEEDED
        extended hash = yes
@@ -63,7 +64,8 @@
              command = grep -i foo data.txt > analyzed.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:data.txt
              creates   file:analyzed.txt
+            supplies   file:analyzed.txt
```

### Comparing `stepup-1.0.0/tests/cases/nodata/expected_stdout_a.txt` & `stepup-1.1.0/tests/cases/nodata/expected_stdout_a.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ grep -i foo data.txt > analyzed.txt
    SUCCESS │ grep -i foo data.txt > analyzed.txt
      START │ cat analyzed.txt
    SUCCESS │ cat analyzed.txt
 ─────────────────────────────── Standard output ────────────────────────────────
```

### Comparing `stepup-1.0.0/tests/cases/nodata/expected_stdout_b.txt` & `stepup-1.1.0/tests/cases/nodata/expected_stdout_b.txt`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ grep -i foo data.txt > analyzed.txt
    SUCCESS │ grep -i foo data.txt > analyzed.txt
       SKIP │ cat analyzed.txt
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 85191f53, inp_digset 85191f53
```

### Comparing `stepup-1.0.0/tests/cases/nodata/main.sh` & `stepup-1.1.0/tests/cases/nodata/main.sh`

 * *Files 9% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 cp original.txt data.txt
 stepup -e -w 1 plan.py & # > current_stdout_a.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f original.txt ]] || exit -1
 [[ -f data.txt ]] || exit -1
 [[ -f analyzed.txt ]] || exit -1
 
 # Remove the data file and run again
 rm data.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_del("data.txt")
+watch_delete("data.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f original.txt ]] || exit -1
 [[ -f analyzed.txt ]] || exit -1
@@ -44,15 +44,15 @@
 cp original.txt data.txt
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_03.txt")
+graph("current_graph_03")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f original.txt ]] || exit -1
 [[ -f data.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/noplan/expected_stdout.txt` & `stepup-1.1.0/tests/cases/noplan/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/nostatic/expected_graph.txt` & `stepup-1.1.0/tests/cases/nostatic/expected_graph.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,33 @@
 step:echo "spam" > first.txt
              workdir = ./
              command = echo "spam" > first.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:first.txt
+            supplies   file:first.txt
 
 file:first.txt
                 path = first.txt
                state = BUILT
           created by   step:echo "spam" > first.txt
             consumes   file:./
+            consumes   step:echo "spam" > first.txt
             supplies   step:cp -v first.txt second.txt
 
 step:cp -v first.txt second.txt
              workdir = ./
              command = cp -v first.txt second.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:first.txt
              creates   file:second.txt
+            supplies   file:second.txt
 
 file:second.txt
                 path = second.txt
                state = BUILT
           created by   step:cp -v first.txt second.txt
             consumes   file:./
+            consumes   step:cp -v first.txt second.txt
```

### Comparing `stepup-1.0.0/tests/cases/nostatic/expected_stdout.txt` & `stepup-1.1.0/tests/cases/nostatic/expected_stdout.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ echo "spam" > first.txt
    SUCCESS │ echo "spam" > first.txt
      START │ cp -v first.txt second.txt
    SUCCESS │ cp -v first.txt second.txt
 ─────────────────────────────── Standard output ────────────────────────────────
 'first.txt' -> 'second.txt'
 ────────────────────────────────────────────────────────────────────────────────
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
+   DELETED │ second.txt
+   DELETED │ first.txt
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/nostatic/main.sh` & `stepup-1.1.0/tests/cases/error_deferred_nonexisting/main.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
-set -e
+# No set -e because this is excepted to error
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
-wait()
-graph("current_graph.txt")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f first.txt ]] || exit -1
-[[ -f second.txt ]] || exit -1
+[[ -f README.md ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/optional_convert/expected_graph_a.txt` & `stepup-1.1.0/tests/cases/optional_convert/expected_graph_a.txt`

 * *Files 7% similar despite different names*

```diff
@@ -74,30 +74,34 @@
                state = SUCCEEDED
            mandatory = IMPLIED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:raw_03.txt
              creates   file:converted_03.txt
+            supplies   file:converted_03.txt
 
 file:converted_03.txt
                 path = converted_03.txt
                state = BUILT
           created by   step:cp -aT raw_03.txt converted_03.txt
             consumes   file:./
+            consumes   step:cp -aT raw_03.txt converted_03.txt
             supplies   step:cp -aT converted_03.txt used.txt
 
 step:cp -aT converted_03.txt used.txt
              workdir = ./
              command = cp -aT converted_03.txt used.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:converted_03.txt
              creates   file:used.txt
+            supplies   file:used.txt
 
 file:used.txt
                 path = used.txt
                state = BUILT
           created by   step:cp -aT converted_03.txt used.txt
             consumes   file:./
+            consumes   step:cp -aT converted_03.txt used.txt
```

### Comparing `stepup-1.0.0/tests/cases/optional_convert/expected_graph_b.txt` & `stepup-1.1.0/tests/cases/optional_convert/expected_graph_b.txt`

 * *Files 7% similar despite different names*

```diff
@@ -74,30 +74,34 @@
                state = SUCCEEDED
            mandatory = IMPLIED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:raw_03.txt
              creates   file:converted_03.txt
+            supplies   file:converted_03.txt
 
 file:converted_03.txt
                 path = converted_03.txt
                state = BUILT
           created by   step:cp -aT raw_03.txt converted_03.txt
             consumes   file:./
+            consumes   step:cp -aT raw_03.txt converted_03.txt
             supplies   step:cp -aT converted_03.txt used.txt
 
 step:cp -aT converted_03.txt used.txt
              workdir = ./
              command = cp -aT converted_03.txt used.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:converted_03.txt
              creates   file:used.txt
+            supplies   file:used.txt
 
 file:used.txt
                 path = used.txt
                state = BUILT
           created by   step:cp -aT converted_03.txt used.txt
             consumes   file:./
+            consumes   step:cp -aT converted_03.txt used.txt
```

### Comparing `stepup-1.0.0/tests/cases/optional_convert/expected_graph_c.txt` & `stepup-1.1.0/tests/cases/optional_convert/expected_graph_c.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,35 +69,39 @@
             consumes   file:./
 
 file:used.txt
                 path = used.txt
                state = BUILT
           created by   step:cp -aT converted_01.txt used.txt
             consumes   file:./
+            consumes   step:cp -aT converted_01.txt used.txt
 
 step:cp -aT raw_01.txt converted_01.txt
              workdir = ./
              command = cp -aT raw_01.txt converted_01.txt
                state = SUCCEEDED
            mandatory = IMPLIED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:raw_01.txt
              creates   file:converted_01.txt
+            supplies   file:converted_01.txt
 
 file:converted_01.txt
                 path = converted_01.txt
                state = BUILT
           created by   step:cp -aT raw_01.txt converted_01.txt
             consumes   file:./
+            consumes   step:cp -aT raw_01.txt converted_01.txt
             supplies   step:cp -aT converted_01.txt used.txt
 
 step:cp -aT converted_01.txt used.txt
              workdir = ./
              command = cp -aT converted_01.txt used.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:converted_01.txt
              creates   file:used.txt
+            supplies   file:used.txt
```

### Comparing `stepup-1.0.0/tests/cases/optional_convert/expected_stdout_a.txt` & `stepup-1.1.0/tests/cases/optional_convert/expected_stdout_a.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp -aT raw_03.txt converted_03.txt
    SUCCESS │ cp -aT raw_03.txt converted_03.txt
      START │ cp -aT converted_03.txt used.txt
    SUCCESS │ cp -aT converted_03.txt used.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
```

### Comparing `stepup-1.0.0/tests/cases/optional_convert/main.sh` & `stepup-1.1.0/tests/cases/optional_convert/main.sh`

 * *Files 15% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 export ENV_VAR_TEST_STEPUP_IDX="3"
 stepup -e -w 1 plan.py & # > current_stdout_a.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_a.txt")
+graph("current_graph_a")
 EOD
 
 # Rerun without changes
 python3 - << EOD
 from stepup.core.interact import *
 run()
 wait()
-graph("current_graph_b.txt")
+graph("current_graph_b")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -40,15 +40,15 @@
 export ENV_VAR_TEST_STEPUP_IDX="1"
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_c.txt")
+graph("current_graph_c")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/output_not_created/expected_graph.txt` & `stepup-1.1.0/tests/cases/output_not_created/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -35,29 +35,33 @@
 step:touch input.txt
              workdir = ./
              command = touch input.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:input.txt
+            supplies   file:input.txt
 
 file:input.txt
                 path = input.txt
                state = BUILT
           created by   step:touch input.txt
             consumes   file:./
+            consumes   step:touch input.txt
             supplies   step:cp input.txt wrong.txt
 
 step:cp input.txt wrong.txt
              workdir = ./
              command = cp input.txt wrong.txt
                state = FAILED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = PENDING
           created by   step:cp input.txt wrong.txt
             consumes   file:./
+            consumes   step:cp input.txt wrong.txt
```

### Comparing `stepup-1.0.0/tests/cases/output_not_created/expected_stdout.txt` & `stepup-1.1.0/tests/cases/output_not_created/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ touch input.txt
    SUCCESS │ touch input.txt
      START │ cp input.txt wrong.txt
       FAIL │ cp input.txt wrong.txt
 ────────────────────────────────── Step info ───────────────────────────────────
```

### Comparing `stepup-1.0.0/tests/cases/output_not_created/main.sh` & `stepup-1.1.0/tests/cases/output_not_created/main.sh`

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

### Comparing `stepup-1.0.0/tests/cases/pending/expected_graph.txt` & `stepup-1.1.0/tests/cases/pending/expected_graph.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,29 @@
              command = cp -v first.txt second.txt
                state = PENDING
           created by   step:./plan.py
             consumes   file:./
             consumes   (file:first.txt)
              creates   file:second.txt
              creates   file:third.txt
+            supplies   file:second.txt
+            supplies   file:third.txt
 
 (file:first.txt)
                 path = first.txt
                state = PENDING
             consumes   file:./
             supplies   step:cp -v first.txt second.txt
 
 file:second.txt
                 path = second.txt
                state = PENDING
           created by   step:cp -v first.txt second.txt
             consumes   file:./
+            consumes   step:cp -v first.txt second.txt
 
 file:third.txt
                 path = third.txt
                state = VOLATILE
           created by   step:cp -v first.txt second.txt
             consumes   file:./
+            consumes   step:cp -v first.txt second.txt
```

### Comparing `stepup-1.0.0/tests/cases/pending/expected_stdout.txt` & `stepup-1.1.0/tests/cases/pending/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
    WARNING │ 1 step remains pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
 Command               cp -v first.txt second.txt
 Working directory     ./
 Inputs        STATIC  ./
```

### Comparing `stepup-1.0.0/tests/cases/pending/main.sh` & `stepup-1.1.0/tests/cases/error_env_var/main.sh`

 * *Files 15% similar despite different names*

```diff
@@ -7,16 +7,16 @@
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
 
-# Wait for background processes, if any.
-wait $(jobs -p)
-
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
+
+# Wait for background processes, if any.
+wait $(jobs -p)
```

### Comparing `stepup-1.0.0/tests/cases/permissions_file_rerun/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/permissions_file_rerun/expected_graph_01.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,13 +42,15 @@
              workdir = ./
              command = cp -aT input.txt output.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
           created by   step:cp -aT input.txt output.txt
             consumes   file:./
+            consumes   step:cp -aT input.txt output.txt
```

### Comparing `stepup-1.0.0/tests/cases/permissions_file_rerun/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/permissions_file_rerun/expected_graph_02.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,13 +42,15 @@
              workdir = ./
              command = cp -aT input.txt output.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
           created by   step:cp -aT input.txt output.txt
             consumes   file:./
+            consumes   step:cp -aT input.txt output.txt
```

### Comparing `stepup-1.0.0/tests/cases/permissions_file_rerun/expected_stdout.txt` & `stepup-1.1.0/tests/cases/permissions_file_rerun/expected_stdout.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp -aT input.txt output.txt
    SUCCESS │ cp -aT input.txt output.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ input.txt
-     ADDED │ input.txt
+   UPDATED │ input.txt
      PHASE │ run
      START │ cp -aT input.txt output.txt
    SUCCESS │ cp -aT input.txt output.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/permissions_file_rerun/main.sh` & `stepup-1.1.0/tests/cases/permissions_file_rerun/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 chmod +x input.txt
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f input.txt ]] || exit -1
 [[ -f output.txt ]] || exit -1
 stat input.txt | grep 'Access: (0755/-rwxr-xr-x)'
@@ -24,18 +24,18 @@
 
 # Rerun the plan with different permissions for the input.
 chmod -x input.txt
 
 # Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("input.txt")
+watch_update("input.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/permissions_plan_rerun/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/permissions_plan_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/permissions_plan_rerun/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/permissions_plan_rerun/expected_graph_02.txt`

 * *Files 4% similar despite different names*

```diff
@@ -59,13 +59,15 @@
 step:touch done.txt  # wd=sub/
              workdir = sub/
              command = touch done.txt
                state = SUCCEEDED
           created by   step:./plan.py  # wd=sub/
             consumes   file:sub/
              creates   file:sub/done.txt
+            supplies   file:sub/done.txt
 
 file:sub/done.txt
                 path = sub/done.txt
                state = BUILT
           created by   step:touch done.txt  # wd=sub/
             consumes   file:sub/
+            consumes   step:touch done.txt  # wd=sub/
```

### Comparing `stepup-1.0.0/tests/cases/permissions_plan_rerun/expected_stdout.txt` & `stepup-1.1.0/tests/cases/permissions_plan_rerun/expected_stdout.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./plan.py  # wd=sub/
       FAIL │ ./plan.py  # wd=sub/
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               ./plan.py
 Working directory     sub/
 Return code           126
 ──────────────────────────────── Standard error ────────────────────────────────
-/bin/sh: line 1: ./plan.py: Permission denied
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step(s) failed, see error messages above
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ sub/plan.py
-     ADDED │ sub/plan.py
+   UPDATED │ sub/plan.py
      PHASE │ run
      START │ ./plan.py  # wd=sub/
    SUCCESS │ ./plan.py  # wd=sub/
      START │ touch done.txt  # wd=sub/
    SUCCESS │ touch done.txt  # wd=sub/
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
```

### Comparing `stepup-1.0.0/tests/cases/permissions_plan_rerun/main.sh` & `stepup-1.1.0/tests/cases/permissions_step_rerun/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the plan with non-executable step.py.
-chmod -x sub/plan.py
+chmod -x step.py
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f sub/plan.py ]] || exit -1
-[[ ! -f sub/done.txt ]] || exit -1
+[[ -f step.py ]] || exit -1
+[[ ! -f message.txt ]] || exit -1
 
 # Rerun the plan with executable step.py.
-chmod +x sub/plan.py
+chmod +x step.py
 
 # Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("sub/plan.py")
+watch_update("step.py")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f sub/plan.py ]] || exit -1
-[[ -f sub/done.txt ]] || exit -1
+[[ -f step.py ]] || exit -1
+[[ -f message.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/permissions_plan_restart/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/permissions_plan_restart/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/permissions_plan_restart/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/permissions_plan_restart/expected_graph_02.txt`

 * *Files 4% similar despite different names*

```diff
@@ -62,13 +62,15 @@
              workdir = sub/
              command = touch done.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py  # wd=sub/
             consumes   file:sub/
              creates   file:sub/done.txt
+            supplies   file:sub/done.txt
 
 file:sub/done.txt
                 path = sub/done.txt
                state = BUILT
           created by   step:touch done.txt  # wd=sub/
             consumes   file:sub/
+            consumes   step:touch done.txt  # wd=sub/
```

### Comparing `stepup-1.0.0/tests/cases/permissions_plan_restart/expected_stdout_01.txt` & `stepup-1.1.0/tests/cases/permissions_plan_restart/expected_stdout_01.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./plan.py  # wd=sub/
       FAIL │ ./plan.py  # wd=sub/
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               ./plan.py
 Working directory     sub/
 Return code           126
 ──────────────────────────────── Standard error ────────────────────────────────
-/bin/sh: line 1: ./plan.py: Permission denied
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step(s) failed, see error messages above
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/permissions_plan_restart/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/restart_deferred_glob/expected_stdout_01.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-  WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
-      SKIP │ ./plan.py
-───────────────────────────── No changes observed ──────────────────────────────
-Same step hash       extended, digest 97a2efee, inp_digset 97a2efee
-Same inp hash        ./
-Same inp hash        plan.py
+     PHASE │ run
+     START │ ./plan.py
+   SUCCESS │ ./plan.py
+     START │ cat static/foo.txt
+   SUCCESS │ cat static/foo.txt
+─────────────────────────────── Standard output ────────────────────────────────
+This is a deferred static file.
 ────────────────────────────────────────────────────────────────────────────────
-     START │ ./plan.py  # wd=sub/
-   SUCCESS │ ./plan.py  # wd=sub/
-     START │ touch done.txt  # wd=sub/
-   SUCCESS │ touch done.txt  # wd=sub/
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/permissions_plan_restart/main.sh` & `stepup-1.1.0/tests/cases/permissions_plan_restart/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 chmod -x sub/plan.py
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -29,15 +29,15 @@
 chmod +x sub/plan.py
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/permissions_step_rerun/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/permissions_step_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/permissions_step_rerun/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/permissions_step_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/permissions_step_rerun/expected_stdout.txt` & `stepup-1.1.0/tests/cases/permissions_step_rerun/expected_stdout.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./step.py
       FAIL │ ./step.py
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               ./step.py
 Return code           126
 ──────────────────────────────── Standard error ────────────────────────────────
-/bin/sh: line 1: ./step.py: Permission denied
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step(s) failed, see error messages above
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ step.py
-     ADDED │ step.py
+   UPDATED │ step.py
      PHASE │ run
      START │ ./step.py
    SUCCESS │ ./step.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/permissions_step_rerun/main.sh` & `stepup-1.1.0/tests/cases/watch_nochanges/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
-# Run the plan with non-executable step.py.
-chmod -x step.py
+# Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
-# Wait and get graph.
+# Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f step.py ]] || exit -1
-[[ ! -f message.txt ]] || exit -1
+[[ -f input.txt ]] || exit -1
+[[ -f output.txt ]] || exit -1
 
-# Rerun the plan with executable step.py.
-chmod +x step.py
-
-# Wait and get graph.
+# Rerun, no changes expected.
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("step.py")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f step.py ]] || exit -1
-[[ -f message.txt ]] || exit -1
+[[ -f input.txt ]] || exit -1
+[[ -f output.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/permissions_step_restart/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/permissions_step_restart/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/permissions_step_restart/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/permissions_step_restart/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/permissions_step_restart/expected_stdout_01.txt` & `stepup-1.1.0/tests/cases/error_static_dir/expected_stdout.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
-   SUCCESS │ ./plan.py
-     START │ ./step.py
-      FAIL │ ./step.py
+      FAIL │ ./plan.py
 ────────────────────────────────── Step info ───────────────────────────────────
-Command               ./step.py
-Return code           126
+Command               ./plan.py
+Return code           1
 ──────────────────────────────── Standard error ────────────────────────────────
-/bin/sh: line 1: ./step.py: Permission denied
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step(s) failed, see error messages above
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/permissions_step_restart/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/permissions_step_restart/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 5e1badbc, inp_digset 5e1badbc
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./step.py
```

### Comparing `stepup-1.0.0/tests/cases/permissions_step_restart/main.sh` & `stepup-1.1.0/tests/cases/permissions_step_restart/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 chmod -x step.py
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -28,15 +28,15 @@
 chmod +x step.py
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/pool/expected_graph.txt` & `stepup-1.1.0/tests/cases/pool/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/pool/expected_stdout.txt` & `stepup-1.1.0/tests/cases/pool/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
   DIRECTOR │ Launched worker 1
+     PHASE │ run
      START │ ./plan.py
      START │ echo 1; mv r.txt u.txt; sleep 0.1; mv u.txt r.txt
    SUCCESS │ ./plan.py
    SUCCESS │ echo 1; mv r.txt u.txt; sleep 0.1; mv u.txt r.txt
 ─────────────────────────────── Standard output ────────────────────────────────
 1
 ────────────────────────────────────────────────────────────────────────────────
```

### Comparing `stepup-1.0.0/tests/cases/pool/main.sh` & `stepup-1.1.0/tests/cases/script_single/main.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-stepup -w 2 plan.py & # > current_stdout.txt &
+stepup -w 1 plan.py & # > current_stdout.txt &
 
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
-[[ -f r.txt ]] || exit -1
-[[ ! -f u.txt ]] || exit -1
+[[ -f work/generate.py ]] || exit -1
+[[ -f work/test.csv ]] || exit -1
+[[ -f work/copy.csv ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/reqdir_missing/expected_graph.txt` & `stepup-1.1.0/tests/cases/reqdir_missing/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
              workdir = ./
              command = echo hello > sub/dir/nested/hello.txt
                state = PENDING
           created by   step:./plan.py
             consumes   file:./
             consumes   (file:sub/dir/nested/)
              creates   file:sub/dir/nested/hello.txt
+            supplies   file:sub/dir/nested/hello.txt
 
 (file:sub/dir/nested/)
                 path = sub/dir/nested/
                state = PENDING
             consumes   (file:sub/dir/)
             supplies   file:sub/dir/nested/hello.txt
             supplies   step:echo hello > sub/dir/nested/hello.txt
@@ -58,7 +59,8 @@
             supplies   (file:sub/dir/)
 
 file:sub/dir/nested/hello.txt
                 path = sub/dir/nested/hello.txt
                state = PENDING
           created by   step:echo hello > sub/dir/nested/hello.txt
             consumes   (file:sub/dir/nested/)
+            consumes   step:echo hello > sub/dir/nested/hello.txt
```

### Comparing `stepup-1.0.0/tests/cases/reqdir_missing/expected_stdout.txt` & `stepup-1.1.0/tests/cases/reqdir_missing/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
    WARNING │ 1 step remains pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
 Command               echo hello > sub/dir/nested/hello.txt
 Working directory     ./
 Inputs        STATIC  ./
```

### Comparing `stepup-1.0.0/tests/cases/reqdir_missing/main.sh` & `stepup-1.1.0/tests/cases/script_cases_settings/main.sh`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-mkdir -p sub/dir/nested
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
-[[ ! -f sub/dir/nested/hello.txt ]] || exit -1
+[[ -f helper.py ]] || exit -1
+[[ -f work.py ]] || exit -1
+[[ -f data+0.3.txt ]] || exit -1
+[[ -f data-1.2.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/restart_blocked/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/restart_blocked/expected_graph_02.txt`

 * *Files 3% similar despite different names*

```diff
@@ -57,47 +57,52 @@
              workdir = ./
              command = cp -aT initial.txt input.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:initial.txt
              creates   file:input.txt
+            supplies   file:input.txt
 
 file:input.txt
                 path = input.txt
                state = BUILT
           created by   step:cp -aT initial.txt input.txt
             consumes   file:./
+            consumes   step:cp -aT initial.txt input.txt
             supplies   step:./expensive.py
 
 step:./expensive.py
              workdir = ./
              command = ./expensive.py
-               state = PENDING
-               block = True
+               state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:expensive.py
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
-               state = PENDING
+               state = BUILT
           created by   step:./expensive.py
             consumes   file:./
+            consumes   step:./expensive.py
             supplies   step:cp -aT output.txt final.txt
 
 step:cp -aT output.txt final.txt
              workdir = ./
              command = cp -aT output.txt final.txt
-               state = PENDING
+               state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:output.txt
              creates   file:final.txt
+            supplies   file:final.txt
 
 file:final.txt
                 path = final.txt
-               state = PENDING
+               state = BUILT
           created by   step:cp -aT output.txt final.txt
             consumes   file:./
+            consumes   step:cp -aT output.txt final.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_blocked/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/restart_blocked/expected_graph_01.txt`

 * *Files 3% similar despite different names*

```diff
@@ -57,46 +57,53 @@
              workdir = ./
              command = cp -aT initial.txt input.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:initial.txt
              creates   file:input.txt
+            supplies   file:input.txt
 
 file:input.txt
                 path = input.txt
                state = BUILT
           created by   step:cp -aT initial.txt input.txt
             consumes   file:./
+            consumes   step:cp -aT initial.txt input.txt
             supplies   step:./expensive.py
 
 step:./expensive.py
              workdir = ./
              command = ./expensive.py
-               state = SUCCEEDED
+               state = PENDING
+               block = True
           created by   step:./plan.py
             consumes   file:./
             consumes   file:expensive.py
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
-               state = BUILT
+               state = PENDING
           created by   step:./expensive.py
             consumes   file:./
+            consumes   step:./expensive.py
             supplies   step:cp -aT output.txt final.txt
 
 step:cp -aT output.txt final.txt
              workdir = ./
              command = cp -aT output.txt final.txt
-               state = SUCCEEDED
+               state = PENDING
           created by   step:./plan.py
             consumes   file:./
             consumes   file:output.txt
              creates   file:final.txt
+            supplies   file:final.txt
 
 file:final.txt
                 path = final.txt
-               state = BUILT
+               state = PENDING
           created by   step:cp -aT output.txt final.txt
             consumes   file:./
+            consumes   step:cp -aT output.txt final.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_blocked/expected_stdout_01.txt` & `stepup-1.1.0/tests/cases/restart_blocked/expected_stdout_01.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp -aT initial.txt input.txt
    SUCCESS │ cp -aT initial.txt input.txt
    WARNING │ 2 steps remain pending due to blocked steps
 ──────────────────────────────── Blocked steps ─────────────────────────────────
 step:./expensive.py
```

### Comparing `stepup-1.0.0/tests/cases/restart_blocked/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/restart_blocked/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
       SKIP │ cp -aT initial.txt input.txt
      START │ ./expensive.py
    SUCCESS │ ./expensive.py
 ─────────────────────────────── Standard output ────────────────────────────────
 The initial file.
```

### Comparing `stepup-1.0.0/tests/cases/restart_blocked/main.sh` & `stepup-1.1.0/tests/cases/restart_blocked/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 cp plan_blocked.py plan.py
 stepup -w 1 plan.py & # > current_stdout_01.txt &
 
 # First graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 [[ -f initial.txt ]] || exit -1
@@ -27,15 +27,15 @@
 # Modify a few things and restart
 cp plan_unblocked.py plan.py
 stepup -w 1 plan.py & # > current_stdout_02.txt &
 
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/restart_changes/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/restart_changes/expected_graph_01.txt`

 * *Files 6% similar despite different names*

```diff
@@ -49,36 +49,40 @@
              command = cp source_both.txt copy_both1.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan_01.py
             consumes   file:./
             consumes   file:source_both.txt
              creates   file:copy_both1.txt
+            supplies   file:copy_both1.txt
 
 file:copy_both1.txt
                 path = copy_both1.txt
                state = BUILT
           created by   step:cp source_both.txt copy_both1.txt
             consumes   file:./
+            consumes   step:cp source_both.txt copy_both1.txt
 
 step:cp source_01.txt copy_01.txt
              workdir = ./
              command = cp source_01.txt copy_01.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan_01.py
             consumes   file:./
             consumes   file:source_01.txt
              creates   file:copy_01.txt
+            supplies   file:copy_01.txt
 
 file:source_01.txt
                 path = source_01.txt
                state = STATIC
           created by   step:./plan_01.py
             consumes   file:./
             supplies   step:cp source_01.txt copy_01.txt
 
 file:copy_01.txt
                 path = copy_01.txt
                state = BUILT
           created by   step:cp source_01.txt copy_01.txt
             consumes   file:./
+            consumes   step:cp source_01.txt copy_01.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_changes/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/restart_changes/expected_graph_02.txt`

 * *Files 6% similar despite different names*

```diff
@@ -49,20 +49,22 @@
              command = cp source_both.txt copy_both2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan_02.py
             consumes   file:./
             consumes   file:source_both.txt
              creates   file:copy_both2.txt
+            supplies   file:copy_both2.txt
 
 file:copy_both2.txt
                 path = copy_both2.txt
                state = BUILT
           created by   step:cp source_both.txt copy_both2.txt
             consumes   file:./
+            consumes   step:cp source_both.txt copy_both2.txt
 
 file:source_02.txt
                 path = source_02.txt
                state = STATIC
           created by   step:./plan_02.py
             consumes   file:./
             supplies   step:cp source_02.txt copy_02.txt
@@ -72,13 +74,15 @@
              command = cp source_02.txt copy_02.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan_02.py
             consumes   file:./
             consumes   file:source_02.txt
              creates   file:copy_02.txt
+            supplies   file:copy_02.txt
 
 file:copy_02.txt
                 path = copy_02.txt
                state = BUILT
           created by   step:cp source_02.txt copy_02.txt
             consumes   file:./
+            consumes   step:cp source_02.txt copy_02.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_changes/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/restart_changes/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan_02.py
    SUCCESS │ ./plan_02.py
      START │ cp source_both.txt copy_both2.txt
    SUCCESS │ cp source_both.txt copy_both2.txt
      START │ cp source_02.txt copy_02.txt
    SUCCESS │ cp source_02.txt copy_02.txt
      CLEAN │ copy_both1.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_changes/main.sh` & `stepup-1.1.0/tests/cases/restart_changes/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Run the first plan.
 stepup -e -w 1 plan_01.py & # > current_stdout_01.txt &
 
 # Run StepUp for a first time.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -29,15 +29,15 @@
 echo
 stepup -e -w 1 plan_02.py & # > current_stdout_02.txt &
 
 # Restart StepUp.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/restart_deferred_glob/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/restart_deferred_glob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/restart_deferred_glob/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_input/expected_graph_01.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,50 +11,46 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
+            supplies   file:input.txt
+            supplies   file:output.txt
             supplies   file:plan.py
-            supplies   file:static/
             supplies   step:./plan.py
-            supplies   step:cat static/foo.txt
+            supplies   step:cp input.txt output.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
-       extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   dg:'static/**'
-             creates   step:cat static/foo.txt
+             creates   file:input.txt
+             creates   step:cp input.txt output.txt
 
-dg:'static/**'
+file:input.txt
+                path = input.txt
+               state = STATIC
           created by   step:./plan.py
-             creates   file:static/
-             creates   file:static/foo.txt
+            consumes   file:./
+            supplies   step:cp input.txt output.txt
 
-step:cat static/foo.txt
+step:cp input.txt output.txt
              workdir = ./
-             command = cat static/foo.txt
+             command = cp input.txt output.txt
                state = SUCCEEDED
-       extended hash = yes
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:static/foo.txt
-
-file:static/foo.txt
-                path = static/foo.txt
-               state = STATIC
-          created by   dg:'static/**'
-            consumes   file:static/
-            supplies   step:cat static/foo.txt
-
-file:static/
-                path = static/
-               state = STATIC
-          created by   dg:'static/**'
+            consumes   file:input.txt
+             creates   file:output.txt
+            supplies   file:output.txt
+
+file:output.txt
+                path = output.txt
+               state = BUILT
+          created by   step:cp input.txt output.txt
             consumes   file:./
-            supplies   file:static/foo.txt
+            consumes   step:cp input.txt output.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_deferred_glob/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/restart_deferred_glob/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 9bc2d092, inp_digset 9bc2d092
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
       SKIP │ cat static/foo.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_deferred_glob/main.sh` & `stepup-1.1.0/tests/cases/restart_deferred_glob/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Run the plan.
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Run StepUp for a first time.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -25,15 +25,15 @@
 # Run the plan.
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Restart StepUp without making changes.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/restart_nochanges/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/restart_nochanges/expected_graph_01.txt`

 * *Files 6% similar despite different names*

```diff
@@ -40,47 +40,53 @@
              workdir = ./
              command = echo something > single.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
              creates   file:single.txt
+            supplies   file:single.txt
 
 file:single.txt
                 path = single.txt
                state = BUILT
           created by   step:echo something > single.txt
             consumes   file:./
+            consumes   step:echo something > single.txt
             supplies   step:cat single.txt single.txt > double.txt
 
 step:cat single.txt single.txt > double.txt
              workdir = ./
              command = cat single.txt single.txt > double.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:single.txt
              creates   file:double.txt
+            supplies   file:double.txt
 
 file:double.txt
                 path = double.txt
                state = BUILT
           created by   step:cat single.txt single.txt > double.txt
             consumes   file:./
+            consumes   step:cat single.txt single.txt > double.txt
             supplies   step:cat double.txt double.txt > quadruple.txt
 
 step:cat double.txt double.txt > quadruple.txt
              workdir = ./
              command = cat double.txt double.txt > quadruple.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:double.txt
              creates   file:quadruple.txt
+            supplies   file:quadruple.txt
 
 file:quadruple.txt
                 path = quadruple.txt
                state = BUILT
           created by   step:cat double.txt double.txt > quadruple.txt
             consumes   file:./
+            consumes   step:cat double.txt double.txt > quadruple.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_nochanges/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/restart_nochanges/expected_graph_02.txt`

 * *Files 6% similar despite different names*

```diff
@@ -40,47 +40,53 @@
              workdir = ./
              command = echo something > single.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
              creates   file:single.txt
+            supplies   file:single.txt
 
 file:single.txt
                 path = single.txt
                state = BUILT
           created by   step:echo something > single.txt
             consumes   file:./
+            consumes   step:echo something > single.txt
             supplies   step:cat single.txt single.txt > double.txt
 
 step:cat single.txt single.txt > double.txt
              workdir = ./
              command = cat single.txt single.txt > double.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:single.txt
              creates   file:double.txt
+            supplies   file:double.txt
 
 file:double.txt
                 path = double.txt
                state = BUILT
           created by   step:cat single.txt single.txt > double.txt
             consumes   file:./
+            consumes   step:cat single.txt single.txt > double.txt
             supplies   step:cat double.txt double.txt > quadruple.txt
 
 step:cat double.txt double.txt > quadruple.txt
              workdir = ./
              command = cat double.txt double.txt > quadruple.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:double.txt
              creates   file:quadruple.txt
+            supplies   file:quadruple.txt
 
 file:quadruple.txt
                 path = quadruple.txt
                state = BUILT
           created by   step:cat double.txt double.txt > quadruple.txt
             consumes   file:./
+            consumes   step:cat double.txt double.txt > quadruple.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_nochanges/expected_stdout_01.txt` & `stepup-1.1.0/tests/cases/restart_nochanges/expected_stdout_01.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ echo something > single.txt
    SUCCESS │ echo something > single.txt
      START │ cat single.txt single.txt > double.txt
    SUCCESS │ cat single.txt single.txt > double.txt
      START │ cat double.txt double.txt > quadruple.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_nochanges/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/restart_nochanges/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 76df2380, inp_digset 76df2380
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
       SKIP │ echo something > single.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_nochanges/main.sh` & `stepup-1.1.0/tests/cases/restart_nochanges/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Run the plan.
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Run StepUp for a first time.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -27,15 +27,15 @@
 # Run the plan.
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Restart StepUp without making changes.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/restart_orphan/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_mixed/expected_graph_01.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,56 +11,67 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:bar.txt
-            supplies   file:foo.txt
+            supplies   file:copy1.txt
+            supplies   file:copy2.txt
+            supplies   file:orig.txt
             supplies   file:plan.py
             supplies   step:./plan.py
-            supplies   step:cp -aT foo.txt bar.txt
-            supplies   step:echo test > foo.txt
+            supplies   step:cp copy1.txt copy2.txt
+            supplies   step:cp orig.txt copy1.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
-       extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   step:cp -aT foo.txt bar.txt
-             creates   step:echo test > foo.txt
+             creates   file:orig.txt
+             creates   step:cp copy1.txt copy2.txt
+             creates   step:cp orig.txt copy1.txt
 
-step:cp -aT foo.txt bar.txt
-             workdir = ./
-             command = cp -aT foo.txt bar.txt
-               state = SUCCEEDED
-       extended hash = yes
+file:orig.txt
+                path = orig.txt
+               state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:foo.txt
-             creates   file:bar.txt
+            supplies   step:cp orig.txt copy1.txt
 
-file:foo.txt
-                path = foo.txt
-               state = BUILT
-          created by   step:echo test > foo.txt
+step:cp orig.txt copy1.txt
+             workdir = ./
+             command = cp orig.txt copy1.txt
+               state = SUCCEEDED
+          created by   step:./plan.py
             consumes   file:./
-            supplies   step:cp -aT foo.txt bar.txt
+            consumes   file:orig.txt
+             creates   file:copy1.txt
+            supplies   file:copy1.txt
 
-file:bar.txt
-                path = bar.txt
+file:copy1.txt
+                path = copy1.txt
                state = BUILT
-          created by   step:cp -aT foo.txt bar.txt
+          created by   step:cp orig.txt copy1.txt
             consumes   file:./
+            consumes   step:cp orig.txt copy1.txt
+            supplies   step:cp copy1.txt copy2.txt
 
-step:echo test > foo.txt
+step:cp copy1.txt copy2.txt
              workdir = ./
-             command = echo test > foo.txt
+             command = cp copy1.txt copy2.txt
                state = SUCCEEDED
-       extended hash = yes
           created by   step:./plan.py
             consumes   file:./
-             creates   file:foo.txt
+            consumes   file:copy1.txt
+             creates   file:copy2.txt
+            supplies   file:copy2.txt
+
+file:copy2.txt
+                path = copy2.txt
+               state = BUILT
+          created by   step:cp copy1.txt copy2.txt
+            consumes   file:./
+            consumes   step:cp copy1.txt copy2.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_orphan/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_boot/expected_graph_01.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,56 +11,57 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:bar.txt
-            supplies   file:foo.txt
+            supplies   file:final.txt
+            supplies   file:first.txt
             supplies   file:plan.py
             supplies   step:./plan.py
-            supplies   step:cp -aT foo.txt bar.txt
-            supplies   step:echo test > foo.txt
+            supplies   step:cp first.txt final.txt
+            supplies   step:echo "test 1" > first.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
-       extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   step:cp -aT foo.txt bar.txt
-             creates   step:echo test > foo.txt
+             creates   step:cp first.txt final.txt
+             creates   step:echo "test 1" > first.txt
 
-step:cp -aT foo.txt bar.txt
+step:echo "test 1" > first.txt
              workdir = ./
-             command = cp -aT foo.txt bar.txt
+             command = echo "test 1" > first.txt
                state = SUCCEEDED
-       extended hash = yes
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:foo.txt
-             creates   file:bar.txt
+             creates   file:first.txt
+            supplies   file:first.txt
 
-file:foo.txt
-                path = foo.txt
+file:first.txt
+                path = first.txt
                state = BUILT
-          created by   step:echo test > foo.txt
+          created by   step:echo "test 1" > first.txt
             consumes   file:./
-            supplies   step:cp -aT foo.txt bar.txt
+            consumes   step:echo "test 1" > first.txt
+            supplies   step:cp first.txt final.txt
 
-file:bar.txt
-                path = bar.txt
-               state = BUILT
-          created by   step:cp -aT foo.txt bar.txt
-            consumes   file:./
-
-step:echo test > foo.txt
+step:cp first.txt final.txt
              workdir = ./
-             command = echo test > foo.txt
+             command = cp first.txt final.txt
                state = SUCCEEDED
-       extended hash = yes
           created by   step:./plan.py
             consumes   file:./
-             creates   file:foo.txt
+            consumes   file:first.txt
+             creates   file:final.txt
+            supplies   file:final.txt
+
+file:final.txt
+                path = final.txt
+               state = BUILT
+          created by   step:cp first.txt final.txt
+            consumes   file:./
+            consumes   step:cp first.txt final.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_orphan/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/restart_orphan/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 45f26b3e, inp_digset 45f26b3e
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
       SKIP │ echo test > foo.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_orphan/main.sh` & `stepup-1.1.0/tests/cases/restart_orphan/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Run the plan.
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Run StepUp for a first time.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -26,15 +26,15 @@
 # Run the plan.
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Restart StepUp without making changes.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/restart_outdated_amend/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/restart_outdated_amend/expected_graph_01.txt`

 * *Files 8% similar despite different names*

```diff
@@ -54,27 +54,29 @@
              creates   file:inp1.txt
 
 step:./step.py
              workdir = ./
              command = ./step.py
                state = SUCCEEDED
   consumes (amended) = file:inp1.txt
-   creates (amended) = file:copy.txt
+  supplies (amended) = file:copy.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
             consumes   file:subs.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:inp1.txt
                 path = inp1.txt
                state = STATIC
           created by   dg:'inp*.txt'
             consumes   file:./
             supplies   step:./step.py
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/restart_outdated_amend/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/restart_outdated_amend/expected_graph_02.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,27 +54,29 @@
              creates   file:inp2.txt
 
 step:./step.py
              workdir = ./
              command = ./step.py
                state = SUCCEEDED
   consumes (amended) = file:inp2.txt
-   creates (amended) = file:copy.txt
+  supplies (amended) = file:copy.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp2.txt
             consumes   file:subs.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
 
 file:inp2.txt
                 path = inp2.txt
                state = STATIC
           created by   dg:'inp*.txt'
             consumes   file:./
             supplies   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/restart_outdated_amend/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/restart_outdated_amend/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 03904dae, inp_digset 03904dae
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
  DROPAMEND │ ./step.py
```

### Comparing `stepup-1.0.0/tests/cases/restart_outdated_amend/main.sh` & `stepup-1.1.0/tests/cases/restart_outdated_amend/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 echo inp1.txt > subs.txt
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -30,15 +30,15 @@
 rm inp1.txt
 echo inp2 > inp2.txt
 echo inp2.txt > subs.txt
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/restart_output/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/restart_output/expected_graph_01.txt`

 * *Files 0% similar despite different names*

```diff
@@ -44,13 +44,15 @@
              command = cp -aT original.txt copy.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:original.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:cp -aT original.txt copy.txt
             consumes   file:./
+            consumes   step:cp -aT original.txt copy.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_output/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/restart_output/expected_graph_02.txt`

 * *Files 0% similar despite different names*

```diff
@@ -44,13 +44,15 @@
              command = cp -aT original.txt copy.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:original.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:cp -aT original.txt copy.txt
             consumes   file:./
+            consumes   step:cp -aT original.txt copy.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_output/expected_stdout_02.txt` & `stepup-1.1.0/tests/cases/restart_output/expected_stdout_02.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 8d0cad40, inp_digset 8d0cad40
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
     NOSKIP │ cp -aT original.txt copy.txt
```

### Comparing `stepup-1.0.0/tests/cases/restart_output/main.sh` & `stepup-1.1.0/tests/cases/restart_output/main.sh`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 xargs rm -rvf < .gitignore
 
 # Run the plan.
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
@@ -23,15 +23,15 @@
 
 # Restart StepUp after removing the output.
 rm copy.txt
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/script_cases/expected_graph.txt` & `stepup-1.1.0/tests/cases/script_cases/expected_graph.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,29 +71,33 @@
              command = ./work.py run -- '-5.0'
                state = SUCCEEDED
           created by   step:./work.py plan
             consumes   file:./
             consumes   file:helper.py
             consumes   file:work.py
              creates   file:data-5.0.txt
+            supplies   file:data-5.0.txt
 
 file:data-5.0.txt
                 path = data-5.0.txt
                state = BUILT
           created by   step:./work.py run -- '-5.0'
             consumes   file:./
+            consumes   step:./work.py run -- '-5.0'
 
 step:./work.py run -- '+7.0'
              workdir = ./
              command = ./work.py run -- '+7.0'
                state = SUCCEEDED
           created by   step:./work.py plan
             consumes   file:./
             consumes   file:helper.py
             consumes   file:work.py
              creates   file:data+7.0.txt
+            supplies   file:data+7.0.txt
 
 file:data+7.0.txt
                 path = data+7.0.txt
                state = BUILT
           created by   step:./work.py run -- '+7.0'
             consumes   file:./
+            consumes   step:./work.py run -- '+7.0'
```

### Comparing `stepup-1.0.0/tests/cases/script_cases/main.sh` & `stepup-1.1.0/tests/cases/watch_output/main.sh`

 * *Files 19% similar despite different names*

```diff
@@ -7,20 +7,33 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph_01")
+EOD
+
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f input.txt ]] || exit -1
+[[ -f output.txt ]] || exit -1
+
+# Remove a built file and rerun.
+rm output.txt
+python3 - << EOD
+from stepup.core.interact import *
+watch_delete("output.txt")
+run()
+wait()
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f helper.py ]] || exit -1
-[[ -f work.py ]] || exit -1
-[[ -f data-5.0.txt ]] || exit -1
-[[ -f data+7.0.txt ]] || exit -1
+[[ -f input.txt ]] || exit -1
+[[ -f output.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/script_cases_settings/README.md` & `stepup-1.1.0/tests/cases/script_cases_settings/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/script_cases_settings/expected_graph.txt` & `stepup-1.1.0/tests/cases/script_cases_settings/expected_graph.txt`

 * *Files 4% similar despite different names*

```diff
@@ -82,29 +82,33 @@
              command = ./work.py run -- '+0.3'
                state = SUCCEEDED
           created by   step:./work.py plan
             consumes   file:./
             consumes   file:helper.py
             consumes   file:work.py
              creates   file:data+0.3.txt
+            supplies   file:data+0.3.txt
 
 file:data+0.3.txt
                 path = data+0.3.txt
                state = BUILT
           created by   step:./work.py run -- '+0.3'
             consumes   file:./
+            consumes   step:./work.py run -- '+0.3'
 
 step:./work.py run -- '-1.2'
              workdir = ./
              command = ./work.py run -- '-1.2'
                state = SUCCEEDED
           created by   step:./work.py plan
             consumes   file:./
             consumes   file:helper.py
             consumes   file:work.py
              creates   file:data-1.2.txt
+            supplies   file:data-1.2.txt
 
 file:data-1.2.txt
                 path = data-1.2.txt
                state = BUILT
           created by   step:./work.py run -- '-1.2'
             consumes   file:./
+            consumes   step:./work.py run -- '-1.2'
```

### Comparing `stepup-1.0.0/tests/cases/script_cases_settings/main.sh` & `stepup-1.1.0/tests/cases/watch_outdated_amend1/main.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
-# Run the example
-stepup -w 1 plan.py & # > current_stdout.txt &
+# Run with the initial subs.txt.
+echo inp1 > inp1.txt
+echo inp1.txt > subs.txt
+stepup -e -w 1 plan.py & # > current_stdout.txt &
 
-# Get the graph after completion of the pending steps.
+# Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph_01")
+EOD
+
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f inp1.txt ]] || exit -1
+[[ -f copy.txt ]] || exit -1
+grep inp1 copy.txt
+
+# Change subs.txt and rerun.
+rm inp1.txt
+echo inp2 > inp2.txt
+echo inp2.txt > subs.txt
+python3 - << EOD
+from stepup.core.interact import *
+watch_update("subs.txt")
+watch_delete("inp1.txt")
+run()
+wait()
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f helper.py ]] || exit -1
-[[ -f work.py ]] || exit -1
-[[ -f data+0.3.txt ]] || exit -1
-[[ -f data-1.2.txt ]] || exit -1
+[[ ! -f inp1.txt ]] || exit -1
+[[ -f inp2.txt ]] || exit -1
+[[ -f copy.txt ]] || exit -1
+grep inp2 copy.txt
```

### Comparing `stepup-1.0.0/tests/cases/script_single/expected_graph.txt` & `stepup-1.1.0/tests/cases/script_single/expected_graph.txt`

 * *Files 7% similar despite different names*

```diff
@@ -68,27 +68,30 @@
              command = cp -aT work/test.csv work/copy.csv
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:work/
             consumes   file:work/test.csv
              creates   file:work/copy.csv
+            supplies   file:work/copy.csv
 
 file:work/test.csv
                 path = work/test.csv
                state = BUILT
           created by   step:./generate.py run  # wd=work/
             consumes   file:work/
+            consumes   step:./generate.py run  # wd=work/
             supplies   step:cp -aT work/test.csv work/copy.csv
 
 file:work/copy.csv
                 path = work/copy.csv
                state = BUILT
           created by   step:cp -aT work/test.csv work/copy.csv
             consumes   file:work/
+            consumes   step:cp -aT work/test.csv work/copy.csv
 
 file:work/config.json
                 path = work/config.json
                state = STATIC
           created by   step:./generate.py plan --optional  # wd=work/
             consumes   file:work/
             supplies   step:./generate.py run  # wd=work/
@@ -99,7 +102,8 @@
                state = SUCCEEDED
            mandatory = IMPLIED
           created by   step:./generate.py plan --optional  # wd=work/
             consumes   file:work/
             consumes   file:work/config.json
             consumes   file:work/generate.py
              creates   file:work/test.csv
+            supplies   file:work/test.csv
```

### Comparing `stepup-1.0.0/tests/cases/script_single/expected_stdout.txt` & `stepup-1.1.0/tests/cases/script_single/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./generate.py plan --optional  # wd=work/
    SUCCESS │ ./generate.py plan --optional  # wd=work/
      START │ ./generate.py run  # wd=work/
    SUCCESS │ ./generate.py run  # wd=work/
      START │ cp -aT work/test.csv work/copy.csv
```

### Comparing `stepup-1.0.0/tests/cases/script_single/main.sh` & `stepup-1.1.0/tests/cases/error_step/main.sh`

 * *Files 20% similar despite different names*

```diff
@@ -7,19 +7,16 @@
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
-[[ -f work/generate.py ]] || exit -1
-[[ -f work/test.csv ]] || exit -1
-[[ -f work/copy.csv ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/script_single/work/generate.py` & `stepup-1.1.0/tests/cases/script_single/work/generate.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/static/expected_graph.txt` & `stepup-1.1.0/tests/cases/static_dir/expected_graph.txt`

 * *Files 27% similar despite different names*

```diff
@@ -11,25 +11,25 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:original.txt
             supplies   file:plan.py
+            supplies   file:subdir/
             supplies   step:./plan.py
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:original.txt
+             creates   file:subdir/
 
-file:original.txt
-                path = original.txt
+file:subdir/
+                path = subdir/
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
```

### Comparing `stepup-1.0.0/tests/cases/static/main.sh` & `stepup-1.1.0/tests/cases/mkdir_error/main.sh`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,16 @@
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
-[[ -f original.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/static_abs/expected_graph.txt` & `stepup-1.1.0/tests/cases/static_abs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/static_abs/main.sh` & `stepup-1.1.0/tests/cases/pending/main.sh`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,16 @@
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
-[[ -f original.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/static_dir/main.sh` & `stepup-1.1.0/tests/cases/subdir/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
-# Prepare subdir
-mkdir -p subdir
-
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
-[[ -d subdir ]] || exit -1
+[[ -f example.txt ]] || exit -1
+[[ -f sub/example.txt ]] || exit -1
+[[ -f sub/upper.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/static_glob/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/static_glob/expected_graph_01.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,29 +57,33 @@
              command = cp -aT inp1.txt out1.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
              creates   file:out1.txt
+            supplies   file:out1.txt
 
 file:out1.txt
                 path = out1.txt
                state = BUILT
           created by   step:cp -aT inp1.txt out1.txt
             consumes   file:./
+            consumes   step:cp -aT inp1.txt out1.txt
 
 step:cp -aT inp2.txt out2.txt
              workdir = ./
              command = cp -aT inp2.txt out2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp2.txt
              creates   file:out2.txt
+            supplies   file:out2.txt
 
 file:out2.txt
                 path = out2.txt
                state = BUILT
           created by   step:cp -aT inp2.txt out2.txt
             consumes   file:./
+            consumes   step:cp -aT inp2.txt out2.txt
```

### Comparing `stepup-1.0.0/tests/cases/static_glob/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/static_glob/expected_graph_02.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,22 @@
              command = cp -aT inp2.txt out2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp2.txt
              creates   file:out2.txt
+            supplies   file:out2.txt
 
 file:out2.txt
                 path = out2.txt
                state = BUILT
           created by   step:cp -aT inp2.txt out2.txt
             consumes   file:./
+            consumes   step:cp -aT inp2.txt out2.txt
 
 file:inp3.txt
                 path = inp3.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:cp -aT inp3.txt out3.txt
@@ -73,13 +75,15 @@
              command = cp -aT inp3.txt out3.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp3.txt
              creates   file:out3.txt
+            supplies   file:out3.txt
 
 file:out3.txt
                 path = out3.txt
                state = BUILT
           created by   step:cp -aT inp3.txt out3.txt
             consumes   file:./
+            consumes   step:cp -aT inp3.txt out3.txt
```

### Comparing `stepup-1.0.0/tests/cases/static_glob/expected_graph_03.txt` & `stepup-1.1.0/tests/cases/static_glob/expected_graph_03.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,20 +50,22 @@
              command = cp -aT inp3.txt out3.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp3.txt
              creates   file:out3.txt
+            supplies   file:out3.txt
 
 file:out3.txt
                 path = out3.txt
                state = BUILT
           created by   step:cp -aT inp3.txt out3.txt
             consumes   file:./
+            consumes   step:cp -aT inp3.txt out3.txt
 
 file:inp4.txt
                 path = inp4.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:cp -aT inp4.txt out4.txt
@@ -73,13 +75,15 @@
              command = cp -aT inp4.txt out4.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp4.txt
              creates   file:out4.txt
+            supplies   file:out4.txt
 
 file:out4.txt
                 path = out4.txt
                state = BUILT
           created by   step:cp -aT inp4.txt out4.txt
             consumes   file:./
+            consumes   step:cp -aT inp4.txt out4.txt
```

### Comparing `stepup-1.0.0/tests/cases/static_glob/expected_stdout_a.txt` & `stepup-1.1.0/tests/cases/static_glob/expected_stdout_a.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp -aT inp1.txt out1.txt
    SUCCESS │ cp -aT inp1.txt out1.txt
      START │ cp -aT inp2.txt out2.txt
    SUCCESS │ cp -aT inp2.txt out2.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-     ADDED │ inp3.txt
+   UPDATED │ inp3.txt
    DELETED │ inp1.txt
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
       SKIP │ cp -aT inp2.txt out2.txt
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 6e3e1fd1, inp_digset 304ea15f
```

### Comparing `stepup-1.0.0/tests/cases/static_glob/expected_stdout_b.txt` & `stepup-1.1.0/tests/cases/static_glob/expected_stdout_b.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
       SKIP │ cp -aT inp3.txt out3.txt
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 67412ddd, inp_digset 2d040ea7
 Same inp hash        ./
 Same inp hash        inp3.txt
```

### Comparing `stepup-1.0.0/tests/cases/static_glob/main.sh` & `stepup-1.1.0/tests/cases/static_glob/main.sh`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Run the example
 stepup -e -w 1 plan.py & # > current_stdout_a.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 grep First inp1.txt
 grep Second inp2.txt
 grep First out1.txt
@@ -27,19 +27,19 @@
 [[ ! -f out3.txt ]] || exit -1
 
 # Modify nglob results and rerun
 echo "Third input" > inp3.txt
 rm inp1.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("inp3.txt")
-watch_del("inp1.txt")
+watch_update("inp3.txt")
+watch_delete("inp1.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ ! -f out1.txt ]] || exit -1
 grep Second inp2.txt
@@ -53,15 +53,15 @@
 # Modify nglob results and restart
 echo "Fourth input" > inp4.txt
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 rm inp2.txt
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_03.txt")
+graph("current_graph_03")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ ! -f out1.txt ]] || exit -1
 [[ ! -f out2.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/static_nglob/expected_graph_01.txt`

 * *Files 2% similar despite different names*

```diff
@@ -124,55 +124,61 @@
              command = cp -aT ch-1-intro/sec-1-1-blabla.txt ch-1-intro/sec-1-1-blabla.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-1-intro/
             consumes   file:ch-1-intro/sec-1-1-blabla.txt
              creates   file:ch-1-intro/sec-1-1-blabla.md
+            supplies   file:ch-1-intro/sec-1-1-blabla.md
 
 file:ch-1-intro/sec-1-1-blabla.md
                 path = ch-1-intro/sec-1-1-blabla.md
                state = BUILT
           created by   step:cp -aT ch-1-intro/sec-1-1-blabla.txt ch-1-intro/sec-1-1-blabla.md
             consumes   file:ch-1-intro/
+            consumes   step:cp -aT ch-1-intro/sec-1-1-blabla.txt ch-1-intro/sec-1-1-blabla.md
             supplies   step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
 
 step:cp -aT ch-1-intro/sec-1-2-some-more.txt ch-1-intro/sec-1-2-some-more.md
              workdir = ./
              command = cp -aT ch-1-intro/sec-1-2-some-more.txt ch-1-intro/sec-1-2-some-more.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-1-intro/
             consumes   file:ch-1-intro/sec-1-2-some-more.txt
              creates   file:ch-1-intro/sec-1-2-some-more.md
+            supplies   file:ch-1-intro/sec-1-2-some-more.md
 
 file:ch-1-intro/sec-1-2-some-more.md
                 path = ch-1-intro/sec-1-2-some-more.md
                state = BUILT
           created by   step:cp -aT ch-1-intro/sec-1-2-some-more.txt ch-1-intro/sec-1-2-some-more.md
             consumes   file:ch-1-intro/
+            consumes   step:cp -aT ch-1-intro/sec-1-2-some-more.txt ch-1-intro/sec-1-2-some-more.md
             supplies   step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
 
 step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
              workdir = ./
              command = cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-1-intro/
             consumes   file:ch-1-intro/sec-1-1-blabla.md
             consumes   file:ch-1-intro/sec-1-2-some-more.md
              creates   file:ch-1-intro/ch-1-compiled.md
+            supplies   file:ch-1-intro/ch-1-compiled.md
 
 file:ch-1-intro/ch-1-compiled.md
                 path = ch-1-intro/ch-1-compiled.md
                state = BUILT
           created by   step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
             consumes   file:ch-1-intro/
+            consumes   step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
             supplies   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
 
 file:ch-2-theory/sec-2-1-basics.txt
                 path = ch-2-theory/sec-2-1-basics.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:ch-2-theory/
@@ -190,55 +196,61 @@
              command = cp -aT ch-2-theory/sec-2-2-advanced.txt ch-2-theory/sec-2-2-advanced.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-2-theory/
             consumes   file:ch-2-theory/sec-2-2-advanced.txt
              creates   file:ch-2-theory/sec-2-2-advanced.md
+            supplies   file:ch-2-theory/sec-2-2-advanced.md
 
 file:ch-2-theory/sec-2-2-advanced.md
                 path = ch-2-theory/sec-2-2-advanced.md
                state = BUILT
           created by   step:cp -aT ch-2-theory/sec-2-2-advanced.txt ch-2-theory/sec-2-2-advanced.md
             consumes   file:ch-2-theory/
+            consumes   step:cp -aT ch-2-theory/sec-2-2-advanced.txt ch-2-theory/sec-2-2-advanced.md
             supplies   step:cat ch-2-theory/sec-2-2-advanced.md ch-2-theory/sec-2-1-basics.md > ch-2-theory/ch-2-compiled.md
 
 step:cp -aT ch-2-theory/sec-2-1-basics.txt ch-2-theory/sec-2-1-basics.md
              workdir = ./
              command = cp -aT ch-2-theory/sec-2-1-basics.txt ch-2-theory/sec-2-1-basics.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-2-theory/
             consumes   file:ch-2-theory/sec-2-1-basics.txt
              creates   file:ch-2-theory/sec-2-1-basics.md
+            supplies   file:ch-2-theory/sec-2-1-basics.md
 
 file:ch-2-theory/sec-2-1-basics.md
                 path = ch-2-theory/sec-2-1-basics.md
                state = BUILT
           created by   step:cp -aT ch-2-theory/sec-2-1-basics.txt ch-2-theory/sec-2-1-basics.md
             consumes   file:ch-2-theory/
+            consumes   step:cp -aT ch-2-theory/sec-2-1-basics.txt ch-2-theory/sec-2-1-basics.md
             supplies   step:cat ch-2-theory/sec-2-2-advanced.md ch-2-theory/sec-2-1-basics.md > ch-2-theory/ch-2-compiled.md
 
 step:cat ch-2-theory/sec-2-2-advanced.md ch-2-theory/sec-2-1-basics.md > ch-2-theory/ch-2-compiled.md
              workdir = ./
              command = cat ch-2-theory/sec-2-2-advanced.md ch-2-theory/sec-2-1-basics.md > ch-2-theory/ch-2-compiled.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-2-theory/
             consumes   file:ch-2-theory/sec-2-1-basics.md
             consumes   file:ch-2-theory/sec-2-2-advanced.md
              creates   file:ch-2-theory/ch-2-compiled.md
+            supplies   file:ch-2-theory/ch-2-compiled.md
 
 file:ch-2-theory/ch-2-compiled.md
                 path = ch-2-theory/ch-2-compiled.md
                state = BUILT
           created by   step:cat ch-2-theory/sec-2-2-advanced.md ch-2-theory/sec-2-1-basics.md > ch-2-theory/ch-2-compiled.md
             consumes   file:ch-2-theory/
+            consumes   step:cat ch-2-theory/sec-2-2-advanced.md ch-2-theory/sec-2-1-basics.md > ch-2-theory/ch-2-compiled.md
             supplies   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
 
 file:ch-3-conclusions/sec-3-1-summary.txt
                 path = ch-3-conclusions/sec-3-1-summary.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:ch-3-conclusions/
@@ -256,66 +268,74 @@
              command = cp -aT ch-3-conclusions/sec-3-2-outlook.txt ch-3-conclusions/sec-3-2-outlook.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-3-conclusions/
             consumes   file:ch-3-conclusions/sec-3-2-outlook.txt
              creates   file:ch-3-conclusions/sec-3-2-outlook.md
+            supplies   file:ch-3-conclusions/sec-3-2-outlook.md
 
 file:ch-3-conclusions/sec-3-2-outlook.md
                 path = ch-3-conclusions/sec-3-2-outlook.md
                state = BUILT
           created by   step:cp -aT ch-3-conclusions/sec-3-2-outlook.txt ch-3-conclusions/sec-3-2-outlook.md
             consumes   file:ch-3-conclusions/
+            consumes   step:cp -aT ch-3-conclusions/sec-3-2-outlook.txt ch-3-conclusions/sec-3-2-outlook.md
             supplies   step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
 
 step:cp -aT ch-3-conclusions/sec-3-1-summary.txt ch-3-conclusions/sec-3-1-summary.md
              workdir = ./
              command = cp -aT ch-3-conclusions/sec-3-1-summary.txt ch-3-conclusions/sec-3-1-summary.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-3-conclusions/
             consumes   file:ch-3-conclusions/sec-3-1-summary.txt
              creates   file:ch-3-conclusions/sec-3-1-summary.md
+            supplies   file:ch-3-conclusions/sec-3-1-summary.md
 
 file:ch-3-conclusions/sec-3-1-summary.md
                 path = ch-3-conclusions/sec-3-1-summary.md
                state = BUILT
           created by   step:cp -aT ch-3-conclusions/sec-3-1-summary.txt ch-3-conclusions/sec-3-1-summary.md
             consumes   file:ch-3-conclusions/
+            consumes   step:cp -aT ch-3-conclusions/sec-3-1-summary.txt ch-3-conclusions/sec-3-1-summary.md
             supplies   step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
 
 step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
              workdir = ./
              command = cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-3-conclusions/
             consumes   file:ch-3-conclusions/sec-3-1-summary.md
             consumes   file:ch-3-conclusions/sec-3-2-outlook.md
              creates   file:ch-3-conclusions/ch-3-compiled.md
+            supplies   file:ch-3-conclusions/ch-3-compiled.md
 
 file:ch-3-conclusions/ch-3-compiled.md
                 path = ch-3-conclusions/ch-3-compiled.md
                state = BUILT
           created by   step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
             consumes   file:ch-3-conclusions/
+            consumes   step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
             supplies   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
 
 step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
              workdir = ./
              command = cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-1-intro/ch-1-compiled.md
             consumes   file:ch-2-theory/ch-2-compiled.md
             consumes   file:ch-3-conclusions/ch-3-compiled.md
              creates   file:book.md
+            supplies   file:book.md
 
 file:book.md
                 path = book.md
                state = BUILT
           created by   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
             consumes   file:./
+            consumes   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/static_nglob/expected_graph_02.txt`

 * *Files 2% similar despite different names*

```diff
@@ -124,55 +124,61 @@
              command = cp -aT ch-1-intro/sec-1-1-blabla.txt ch-1-intro/sec-1-1-blabla.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-1-intro/
             consumes   file:ch-1-intro/sec-1-1-blabla.txt
              creates   file:ch-1-intro/sec-1-1-blabla.md
+            supplies   file:ch-1-intro/sec-1-1-blabla.md
 
 file:ch-1-intro/sec-1-1-blabla.md
                 path = ch-1-intro/sec-1-1-blabla.md
                state = BUILT
           created by   step:cp -aT ch-1-intro/sec-1-1-blabla.txt ch-1-intro/sec-1-1-blabla.md
             consumes   file:ch-1-intro/
+            consumes   step:cp -aT ch-1-intro/sec-1-1-blabla.txt ch-1-intro/sec-1-1-blabla.md
             supplies   step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
 
 step:cp -aT ch-1-intro/sec-1-2-some-more.txt ch-1-intro/sec-1-2-some-more.md
              workdir = ./
              command = cp -aT ch-1-intro/sec-1-2-some-more.txt ch-1-intro/sec-1-2-some-more.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-1-intro/
             consumes   file:ch-1-intro/sec-1-2-some-more.txt
              creates   file:ch-1-intro/sec-1-2-some-more.md
+            supplies   file:ch-1-intro/sec-1-2-some-more.md
 
 file:ch-1-intro/sec-1-2-some-more.md
                 path = ch-1-intro/sec-1-2-some-more.md
                state = BUILT
           created by   step:cp -aT ch-1-intro/sec-1-2-some-more.txt ch-1-intro/sec-1-2-some-more.md
             consumes   file:ch-1-intro/
+            consumes   step:cp -aT ch-1-intro/sec-1-2-some-more.txt ch-1-intro/sec-1-2-some-more.md
             supplies   step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
 
 step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
              workdir = ./
              command = cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-1-intro/
             consumes   file:ch-1-intro/sec-1-1-blabla.md
             consumes   file:ch-1-intro/sec-1-2-some-more.md
              creates   file:ch-1-intro/ch-1-compiled.md
+            supplies   file:ch-1-intro/ch-1-compiled.md
 
 file:ch-1-intro/ch-1-compiled.md
                 path = ch-1-intro/ch-1-compiled.md
                state = BUILT
           created by   step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
             consumes   file:ch-1-intro/
+            consumes   step:cat ch-1-intro/sec-1-1-blabla.md ch-1-intro/sec-1-2-some-more.md > ch-1-intro/ch-1-compiled.md
             supplies   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
 
 file:ch-2-theory/sec-2-1-basics.txt
                 path = ch-2-theory/sec-2-1-basics.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:ch-2-theory/
@@ -183,27 +189,30 @@
              command = cp -aT ch-2-theory/sec-2-1-basics.txt ch-2-theory/sec-2-1-basics.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-2-theory/
             consumes   file:ch-2-theory/sec-2-1-basics.txt
              creates   file:ch-2-theory/sec-2-1-basics.md
+            supplies   file:ch-2-theory/sec-2-1-basics.md
 
 file:ch-2-theory/sec-2-1-basics.md
                 path = ch-2-theory/sec-2-1-basics.md
                state = BUILT
           created by   step:cp -aT ch-2-theory/sec-2-1-basics.txt ch-2-theory/sec-2-1-basics.md
             consumes   file:ch-2-theory/
+            consumes   step:cp -aT ch-2-theory/sec-2-1-basics.txt ch-2-theory/sec-2-1-basics.md
             supplies   step:cat ch-2-theory/sec-2-1-basics.md ch-2-theory/sec-2-2-original.md > ch-2-theory/ch-2-compiled.md
 
 file:ch-2-theory/ch-2-compiled.md
                 path = ch-2-theory/ch-2-compiled.md
                state = BUILT
           created by   step:cat ch-2-theory/sec-2-1-basics.md ch-2-theory/sec-2-2-original.md > ch-2-theory/ch-2-compiled.md
             consumes   file:ch-2-theory/
+            consumes   step:cat ch-2-theory/sec-2-1-basics.md ch-2-theory/sec-2-2-original.md > ch-2-theory/ch-2-compiled.md
             supplies   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
 
 file:ch-3-conclusions/sec-3-1-summary.txt
                 path = ch-3-conclusions/sec-3-1-summary.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:ch-3-conclusions/
@@ -221,73 +230,81 @@
              command = cp -aT ch-3-conclusions/sec-3-2-outlook.txt ch-3-conclusions/sec-3-2-outlook.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-3-conclusions/
             consumes   file:ch-3-conclusions/sec-3-2-outlook.txt
              creates   file:ch-3-conclusions/sec-3-2-outlook.md
+            supplies   file:ch-3-conclusions/sec-3-2-outlook.md
 
 file:ch-3-conclusions/sec-3-2-outlook.md
                 path = ch-3-conclusions/sec-3-2-outlook.md
                state = BUILT
           created by   step:cp -aT ch-3-conclusions/sec-3-2-outlook.txt ch-3-conclusions/sec-3-2-outlook.md
             consumes   file:ch-3-conclusions/
+            consumes   step:cp -aT ch-3-conclusions/sec-3-2-outlook.txt ch-3-conclusions/sec-3-2-outlook.md
             supplies   step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
 
 step:cp -aT ch-3-conclusions/sec-3-1-summary.txt ch-3-conclusions/sec-3-1-summary.md
              workdir = ./
              command = cp -aT ch-3-conclusions/sec-3-1-summary.txt ch-3-conclusions/sec-3-1-summary.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-3-conclusions/
             consumes   file:ch-3-conclusions/sec-3-1-summary.txt
              creates   file:ch-3-conclusions/sec-3-1-summary.md
+            supplies   file:ch-3-conclusions/sec-3-1-summary.md
 
 file:ch-3-conclusions/sec-3-1-summary.md
                 path = ch-3-conclusions/sec-3-1-summary.md
                state = BUILT
           created by   step:cp -aT ch-3-conclusions/sec-3-1-summary.txt ch-3-conclusions/sec-3-1-summary.md
             consumes   file:ch-3-conclusions/
+            consumes   step:cp -aT ch-3-conclusions/sec-3-1-summary.txt ch-3-conclusions/sec-3-1-summary.md
             supplies   step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
 
 step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
              workdir = ./
              command = cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-3-conclusions/
             consumes   file:ch-3-conclusions/sec-3-1-summary.md
             consumes   file:ch-3-conclusions/sec-3-2-outlook.md
              creates   file:ch-3-conclusions/ch-3-compiled.md
+            supplies   file:ch-3-conclusions/ch-3-compiled.md
 
 file:ch-3-conclusions/ch-3-compiled.md
                 path = ch-3-conclusions/ch-3-compiled.md
                state = BUILT
           created by   step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
             consumes   file:ch-3-conclusions/
+            consumes   step:cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
             supplies   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
 
 step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
              workdir = ./
              command = cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-1-intro/ch-1-compiled.md
             consumes   file:ch-2-theory/ch-2-compiled.md
             consumes   file:ch-3-conclusions/ch-3-compiled.md
              creates   file:book.md
+            supplies   file:book.md
 
 file:book.md
                 path = book.md
                state = BUILT
           created by   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
             consumes   file:./
+            consumes   step:cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
 
 file:ch-2-theory/sec-2-2-original.txt
                 path = ch-2-theory/sec-2-2-original.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:ch-2-theory/
             supplies   step:cp -aT ch-2-theory/sec-2-2-original.txt ch-2-theory/sec-2-2-original.md
@@ -297,25 +314,28 @@
              command = cp -aT ch-2-theory/sec-2-2-original.txt ch-2-theory/sec-2-2-original.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-2-theory/
             consumes   file:ch-2-theory/sec-2-2-original.txt
              creates   file:ch-2-theory/sec-2-2-original.md
+            supplies   file:ch-2-theory/sec-2-2-original.md
 
 file:ch-2-theory/sec-2-2-original.md
                 path = ch-2-theory/sec-2-2-original.md
                state = BUILT
           created by   step:cp -aT ch-2-theory/sec-2-2-original.txt ch-2-theory/sec-2-2-original.md
             consumes   file:ch-2-theory/
+            consumes   step:cp -aT ch-2-theory/sec-2-2-original.txt ch-2-theory/sec-2-2-original.md
             supplies   step:cat ch-2-theory/sec-2-1-basics.md ch-2-theory/sec-2-2-original.md > ch-2-theory/ch-2-compiled.md
 
 step:cat ch-2-theory/sec-2-1-basics.md ch-2-theory/sec-2-2-original.md > ch-2-theory/ch-2-compiled.md
              workdir = ./
              command = cat ch-2-theory/sec-2-1-basics.md ch-2-theory/sec-2-2-original.md > ch-2-theory/ch-2-compiled.md
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:ch-2-theory/
             consumes   file:ch-2-theory/sec-2-1-basics.md
             consumes   file:ch-2-theory/sec-2-2-original.md
              creates   file:ch-2-theory/ch-2-compiled.md
+            supplies   file:ch-2-theory/ch-2-compiled.md
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob/expected_stdout.txt` & `stepup-1.1.0/tests/cases/static_nglob/expected_stdout.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
 ─────────────────────────────── Standard output ────────────────────────────────
 Planning ch 1 intro
 Planning sec 1 blabla
 Planning sec 2 some-more
 Planning ch 2 theory
@@ -31,16 +31,16 @@
    SUCCESS │ cat ch-2-theory/sec-2-2-advanced.md ch-2-theory/sec-2-1-basics.md > ch-2-theory/ch-2-compiled.md
      START │ cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
    SUCCESS │ cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
      START │ cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
    SUCCESS │ cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-     ADDED │ ch-2-theory/sec-2-2-original.txt
    DELETED │ ch-2-theory/sec-2-2-advanced.txt
+   UPDATED │ ch-2-theory/sec-2-2-original.txt
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
 ─────────────────────────────── Standard output ────────────────────────────────
 Planning ch 1 intro
 Planning sec 1 blabla
 Planning sec 2 some-more
@@ -63,9 +63,12 @@
    SUCCESS │ cat ch-2-theory/sec-2-1-basics.md ch-2-theory/sec-2-2-original.md > ch-2-theory/ch-2-compiled.md
       SKIP │ cat ch-3-conclusions/sec-3-2-outlook.md ch-3-conclusions/sec-3-1-summary.md > ch-3-conclusions/ch-3-compiled.md
      START │ cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
    SUCCESS │ cat ch-1-intro/ch-1-compiled.md ch-2-theory/ch-2-compiled.md ch-3-conclusions/ch-3-compiled.md > book.md
      CLEAN │ ch-2-theory/sec-2-2-advanced.md
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
+   DELETED │ ch-3-conclusions/sec-3-1-summary.md
+   DELETED │ ch-3-conclusions/ch-3-compiled.md
+   DELETED │ book.md
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob/main.sh` & `stepup-1.1.0/tests/cases/static_nglob/main.sh`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f ch-1-intro/sec-1-1-blabla.md ]] || exit -1
 [[ -f ch-1-intro/sec-1-2-some-more.md ]] || exit -1
 [[ -f ch-1-intro/ch-1-compiled.md ]] || exit -1
@@ -30,24 +30,20 @@
 [[ -f ch-3-conclusions/ch-3-compiled.md ]] || exit -1
 [[ -f book.md ]] || exit -1
 
 # Rename file and run again
 mv ch-2-theory/sec-2-2-advanced.txt ch-2-theory/sec-2-2-original.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("ch-2-theory/sec-2-2-original.txt")
+watch_update("ch-2-theory/sec-2-2-original.txt")
 run()
 wait()
-graph("current_graph_02.txt")
-join()
+graph("current_graph_02")
 EOD
 
-# Wait for background processes, if any.
-wait $(jobs -p)
-
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f ch-1-intro/sec-1-1-blabla.txt ]] || exit -1
 [[ -f ch-1-intro/sec-1-2-some-more.txt ]] || exit -1
 [[ -f ch-2-theory/sec-2-1-basics.txt ]] || exit -1
 [[ ! -f ch-2-theory/sec-2-1-advanced.txt ]] || exit -1
 [[ -f ch-2-theory/sec-2-2-original.txt ]] || exit -1
@@ -60,7 +56,23 @@
 [[ ! -f ch-2-theory/sec-2-2-advanced.md ]] || exit -1
 [[ -f ch-2-theory/sec-2-2-original.md ]] || exit -1
 [[ -f ch-2-theory/ch-2-compiled.md ]] || exit -1
 [[ -f ch-3-conclusions/sec-3-1-summary.md ]] || exit -1
 [[ -f ch-3-conclusions/sec-3-2-outlook.md ]] || exit -1
 [[ -f ch-3-conclusions/ch-3-compiled.md ]] || exit -1
 [[ -f book.md ]] || exit -1
+
+# Test cleanup
+cleanup ch-3-conclusions/sec-3-1-summary.txt
+[[ -f ch-3-conclusions/sec-3-1-summary.txt ]] || exit -1
+[[ ! -f ch-3-conclusions/sec-3-1-summary.md ]] || exit -1
+[[ -f ch-3-conclusions/sec-3-2-outlook.md ]] || exit -1
+[[ ! -f ch-3-conclusions/ch-3-compiled.md ]] || exit -1
+[[ ! -f book.md ]] || exit -1
+
+python3 - << EOD
+from stepup.core.interact import *
+join()
+EOD
+
+# Wait for background processes, if any.
+wait $(jobs -p)
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob/plan.py` & `stepup-1.1.0/tests/cases/static_nglob/plan.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/static_nglob_partial/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/static_nglob_partial/expected_graph_03.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:head_x.txt
             supplies   file:head_y.txt
+            supplies   file:head_z.txt
             supplies   file:paste_x.txt
             supplies   file:plan.py
             supplies   file:tail_x.txt
             supplies   step:./plan.py
             supplies   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 
 step:./plan.py
@@ -30,14 +31,15 @@
                  ngm = ['head_${*char}.txt', 'tail_${*char}.txt'] {'char': '?'}
        extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
              creates   file:head_x.txt
              creates   file:head_y.txt
+             creates   file:head_z.txt
              creates   file:tail_x.txt
              creates   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 
 file:head_x.txt
                 path = head_x.txt
                state = STATIC
           created by   step:./plan.py
@@ -63,13 +65,21 @@
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:head_x.txt
             consumes   file:tail_x.txt
              creates   file:paste_x.txt
+            supplies   file:paste_x.txt
 
 file:paste_x.txt
                 path = paste_x.txt
                state = BUILT
           created by   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
             consumes   file:./
+            consumes   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
+
+file:head_z.txt
+                path = head_z.txt
+               state = STATIC
+          created by   step:./plan.py
+            consumes   file:./
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob_partial/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/static_nglob_partial/expected_graph_02.txt`

 * *Files 7% similar despite different names*

```diff
@@ -71,20 +71,22 @@
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:head_x.txt
             consumes   file:tail_x.txt
              creates   file:paste_x.txt
+            supplies   file:paste_x.txt
 
 file:paste_x.txt
                 path = paste_x.txt
                state = BUILT
           created by   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
             consumes   file:./
+            consumes   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 
 file:head_z.txt
                 path = head_z.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
 
@@ -101,13 +103,15 @@
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:head_y.txt
             consumes   file:tail_y.txt
              creates   file:paste_y.txt
+            supplies   file:paste_y.txt
 
 file:paste_y.txt
                 path = paste_y.txt
                state = BUILT
           created by   step:paste -d ' ' head_y.txt tail_y.txt > paste_y.txt
             consumes   file:./
+            consumes   step:paste -d ' ' head_y.txt tail_y.txt > paste_y.txt
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob_partial/expected_graph_03.txt` & `stepup-1.1.0/tests/cases/watch_outdated_amend1/expected_graph_01.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,73 +11,72 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:head_x.txt
-            supplies   file:head_y.txt
-            supplies   file:head_z.txt
-            supplies   file:paste_x.txt
+            supplies   file:copy.txt
+            supplies   file:inp1.txt
             supplies   file:plan.py
-            supplies   file:tail_x.txt
+            supplies   file:step.py
+            supplies   file:subs.txt
             supplies   step:./plan.py
-            supplies   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
+            supplies   step:./step.py
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
-                 ngm = ['head_${*char}.txt', 'tail_${*char}.txt'] {'char': '?'}
        extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:head_x.txt
-             creates   file:head_y.txt
-             creates   file:head_z.txt
-             creates   file:tail_x.txt
-             creates   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
+             creates   dg:'inp*.txt'
+             creates   file:step.py
+             creates   file:subs.txt
+             creates   step:./step.py
 
-file:head_x.txt
-                path = head_x.txt
+file:step.py
+                path = step.py
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 
-file:head_y.txt
-                path = head_y.txt
+file:subs.txt
+                path = subs.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:./step.py
 
-file:tail_x.txt
-                path = tail_x.txt
-               state = STATIC
+dg:'inp*.txt'
           created by   step:./plan.py
-            consumes   file:./
-            supplies   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
+             creates   file:inp1.txt
 
-step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
+step:./step.py
              workdir = ./
-             command = paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
+             command = ./step.py
                state = SUCCEEDED
+  consumes (amended) = file:inp1.txt
+  supplies (amended) = file:copy.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:head_x.txt
-            consumes   file:tail_x.txt
-             creates   file:paste_x.txt
+            consumes   file:inp1.txt
+            consumes   file:subs.txt
+             creates   file:copy.txt
+            supplies   file:copy.txt
 
-file:paste_x.txt
-                path = paste_x.txt
-               state = BUILT
-          created by   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
+file:inp1.txt
+                path = inp1.txt
+               state = STATIC
+          created by   dg:'inp*.txt'
             consumes   file:./
+            supplies   step:./step.py
 
-file:head_z.txt
-                path = head_z.txt
-               state = STATIC
-          created by   step:./plan.py
+file:copy.txt
+                path = copy.txt
+               state = BUILT
+          created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob_partial/expected_graph_04.txt` & `stepup-1.1.0/tests/cases/static_nglob_partial/expected_graph_04.txt`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,22 @@
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:head_x.txt
             consumes   file:tail_x.txt
              creates   file:paste_x.txt
+            supplies   file:paste_x.txt
 
 file:paste_x.txt
                 path = paste_x.txt
                state = BUILT
           created by   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
             consumes   file:./
+            consumes   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 
 file:head_z.txt
                 path = head_z.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:paste -d ' ' head_z.txt tail_z.txt > paste_z.txt
@@ -114,30 +116,34 @@
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:head_y.txt
             consumes   file:tail_y.txt
              creates   file:paste_y.txt
+            supplies   file:paste_y.txt
 
 file:paste_y.txt
                 path = paste_y.txt
                state = BUILT
           created by   step:paste -d ' ' head_y.txt tail_y.txt > paste_y.txt
             consumes   file:./
+            consumes   step:paste -d ' ' head_y.txt tail_y.txt > paste_y.txt
 
 step:paste -d ' ' head_z.txt tail_z.txt > paste_z.txt
              workdir = ./
              command = paste -d ' ' head_z.txt tail_z.txt > paste_z.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:head_z.txt
             consumes   file:tail_z.txt
              creates   file:paste_z.txt
+            supplies   file:paste_z.txt
 
 file:paste_z.txt
                 path = paste_z.txt
                state = BUILT
           created by   step:paste -d ' ' head_z.txt tail_z.txt > paste_z.txt
             consumes   file:./
+            consumes   step:paste -d ' ' head_z.txt tail_z.txt > paste_z.txt
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob_partial/expected_stdout_a.txt` & `stepup-1.1.0/tests/cases/static_nglob_partial/expected_stdout_a.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
    SUCCESS │ paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-     ADDED │ head_z.txt
-     ADDED │ tail_y.txt
+   UPDATED │ tail_y.txt
+   UPDATED │ head_z.txt
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
       SKIP │ paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 8fc79cdb, inp_digset e3db54b9
 Same inp hash        ./
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob_partial/expected_stdout_b.txt` & `stepup-1.1.0/tests/cases/static_nglob_partial/expected_stdout_b.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
       SKIP │ paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 8fc79cdb, inp_digset e3db54b9
 Same inp hash        ./
 Same inp hash        head_x.txt
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob_partial/main.sh` & `stepup-1.1.0/tests/cases/static_nglob_partial/main.sh`

 * *Files 10% similar despite different names*

```diff
@@ -14,50 +14,50 @@
 # Run the example
 stepup -e -w 1 plan.py & # > current_stdout_a.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ ! -f paste_ignored.txt ]] || exit -1
 grep 'hx tx' paste_x.txt
 [[ ! -f paste_y.txt ]] || exit -1
 
 # Modify nglob results and rerun
 echo "ty" > tail_y.txt
 echo "hz" > head_z.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("tail_y.txt")
-watch_add("head_z.txt")
+watch_update("tail_y.txt")
+watch_update("head_z.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ ! -f paste_ignored.txt ]] || exit -1
 grep 'hx tx' paste_x.txt
 grep 'hy ty' paste_y.txt
 [[ ! -f paste_z.txt ]] || exit -1
 
 # Modify nglob results and rerun
 rm tail_y.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_del("tail_y.txt")
+watch_delete("tail_y.txt")
 run()
 wait()
-graph("current_graph_03.txt")
+graph("current_graph_03")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ ! -f paste_ignored.txt ]] || exit -1
 grep 'hx tx' paste_x.txt
@@ -70,15 +70,15 @@
 # Modify nglob results and restart
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 echo "ty" > tail_y.txt
 echo "tz" > tail_z.txt
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_04.txt")
+graph("current_graph_04")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ ! -f paste_ignored.txt ]] || exit -1
 grep 'hx tx' paste_x.txt
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob_subdir/expected_graph.txt` & `stepup-1.1.0/tests/cases/static_nglob_subdir/expected_graph.txt`

 * *Files 2% similar despite different names*

```diff
@@ -82,28 +82,32 @@
              workdir = sub/
              command = cp -aT inp1.txt out1.txt
                state = SUCCEEDED
           created by   step:./plan.py  # wd=sub/
             consumes   file:sub/
             consumes   file:sub/inp1.txt
              creates   file:sub/out1.txt
+            supplies   file:sub/out1.txt
 
 file:sub/out1.txt
                 path = sub/out1.txt
                state = BUILT
           created by   step:cp -aT inp1.txt out1.txt  # wd=sub/
             consumes   file:sub/
+            consumes   step:cp -aT inp1.txt out1.txt  # wd=sub/
 
 step:cp -aT inp2.txt out2.txt  # wd=sub/
              workdir = sub/
              command = cp -aT inp2.txt out2.txt
                state = SUCCEEDED
           created by   step:./plan.py  # wd=sub/
             consumes   file:sub/
             consumes   file:sub/inp2.txt
              creates   file:sub/out2.txt
+            supplies   file:sub/out2.txt
 
 file:sub/out2.txt
                 path = sub/out2.txt
                state = BUILT
           created by   step:cp -aT inp2.txt out2.txt  # wd=sub/
             consumes   file:sub/
+            consumes   step:cp -aT inp2.txt out2.txt  # wd=sub/
```

### Comparing `stepup-1.0.0/tests/cases/static_nglob_subdir/main.sh` & `stepup-1.1.0/tests/cases/static_nglob_subdir/main.sh`

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
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f sub/plan.py ]] || exit -1
 [[ -f sub/inp1.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/subdir/expected_graph.txt` & `stepup-1.1.0/tests/cases/subdir/expected_graph.txt`

 * *Files 6% similar despite different names*

```diff
@@ -67,20 +67,22 @@
              command = cp -aT example.txt sub/example.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:example.txt
             consumes   file:sub/
              creates   file:sub/example.txt
+            supplies   file:sub/example.txt
 
 file:sub/example.txt
                 path = sub/example.txt
                state = BUILT
           created by   step:cp -aT example.txt sub/example.txt
             consumes   file:sub/
+            consumes   step:cp -aT example.txt sub/example.txt
             supplies   step:tr '[:lower:]' '[:upper:]' < example.txt > upper.txt  # wd=sub/
 
 step:./plan.py  # wd=sub/
              workdir = sub/
              command = ./plan.py
                state = SUCCEEDED
           created by   step:./plan.py
@@ -93,20 +95,22 @@
              workdir = sub/
              command = tr '[:lower:]' '[:upper:]' < example.txt > upper.txt
                state = SUCCEEDED
           created by   step:./plan.py  # wd=sub/
             consumes   file:sub/
             consumes   file:sub/example.txt
              creates   file:sub/upper.txt
+            supplies   file:sub/upper.txt
 
 file:sub/upper.txt
                 path = sub/upper.txt
                state = BUILT
           created by   step:tr '[:lower:]' '[:upper:]' < example.txt > upper.txt  # wd=sub/
             consumes   file:sub/
+            consumes   step:tr '[:lower:]' '[:upper:]' < example.txt > upper.txt  # wd=sub/
 
 step:cat ../plan.py  # wd=sub/
              workdir = sub/
              command = cat ../plan.py
                state = SUCCEEDED
           created by   step:./plan.py  # wd=sub/
             consumes   file:plan.py
```

### Comparing `stepup-1.0.0/tests/cases/subdir/expected_stdout.txt` & `stepup-1.1.0/tests/cases/subdir/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp -aT example.txt sub/example.txt
    SUCCESS │ cp -aT example.txt sub/example.txt
      START │ ./plan.py  # wd=sub/
    SUCCESS │ ./plan.py  # wd=sub/
      START │ tr '[:lower:]' '[:upper:]' < example.txt > upper.txt  # wd=sub/
```

### Comparing `stepup-1.0.0/tests/cases/subdir/main.sh` & `stepup-1.1.0/tests/cases/error_overlap_deferred/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,17 @@
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
-[[ -f example.txt ]] || exit -1
-[[ -f sub/example.txt ]] || exit -1
-[[ -f sub/upper.txt ]] || exit -1
+[[ -f README.md ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/watch_blocked/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_blocked/expected_graph_02.txt`

 * *Files 3% similar despite different names*

```diff
@@ -57,47 +57,52 @@
              workdir = ./
              command = cp -aT initial.txt input.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:initial.txt
              creates   file:input.txt
+            supplies   file:input.txt
 
 file:input.txt
                 path = input.txt
                state = BUILT
           created by   step:cp -aT initial.txt input.txt
             consumes   file:./
+            consumes   step:cp -aT initial.txt input.txt
             supplies   step:./expensive.py
 
 step:./expensive.py
              workdir = ./
              command = ./expensive.py
-               state = PENDING
-               block = True
+               state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:expensive.py
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
-               state = PENDING
+               state = BUILT
           created by   step:./expensive.py
             consumes   file:./
+            consumes   step:./expensive.py
             supplies   step:cp -aT output.txt final.txt
 
 step:cp -aT output.txt final.txt
              workdir = ./
              command = cp -aT output.txt final.txt
-               state = PENDING
+               state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:output.txt
              creates   file:final.txt
+            supplies   file:final.txt
 
 file:final.txt
                 path = final.txt
-               state = PENDING
+               state = BUILT
           created by   step:cp -aT output.txt final.txt
             consumes   file:./
+            consumes   step:cp -aT output.txt final.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_blocked/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_blocked/expected_graph_01.txt`

 * *Files 3% similar despite different names*

```diff
@@ -57,46 +57,53 @@
              workdir = ./
              command = cp -aT initial.txt input.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:initial.txt
              creates   file:input.txt
+            supplies   file:input.txt
 
 file:input.txt
                 path = input.txt
                state = BUILT
           created by   step:cp -aT initial.txt input.txt
             consumes   file:./
+            consumes   step:cp -aT initial.txt input.txt
             supplies   step:./expensive.py
 
 step:./expensive.py
              workdir = ./
              command = ./expensive.py
-               state = SUCCEEDED
+               state = PENDING
+               block = True
           created by   step:./plan.py
             consumes   file:./
             consumes   file:expensive.py
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
-               state = BUILT
+               state = PENDING
           created by   step:./expensive.py
             consumes   file:./
+            consumes   step:./expensive.py
             supplies   step:cp -aT output.txt final.txt
 
 step:cp -aT output.txt final.txt
              workdir = ./
              command = cp -aT output.txt final.txt
-               state = SUCCEEDED
+               state = PENDING
           created by   step:./plan.py
             consumes   file:./
             consumes   file:output.txt
              creates   file:final.txt
+            supplies   file:final.txt
 
 file:final.txt
                 path = final.txt
-               state = BUILT
+               state = PENDING
           created by   step:cp -aT output.txt final.txt
             consumes   file:./
+            consumes   step:cp -aT output.txt final.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_blocked/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_blocked/expected_stdout.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp -aT initial.txt input.txt
    SUCCESS │ cp -aT initial.txt input.txt
    WARNING │ 2 steps remain pending due to blocked steps
 ──────────────────────────────── Blocked steps ─────────────────────────────────
 step:./expensive.py
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ plan.py
-     ADDED │ plan.py
+   UPDATED │ plan.py
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
       SKIP │ cp -aT initial.txt input.txt
      START │ ./expensive.py
    SUCCESS │ ./expensive.py
 ─────────────────────────────── Standard output ────────────────────────────────
```

### Comparing `stepup-1.0.0/tests/cases/watch_blocked/main.sh` & `stepup-1.1.0/tests/cases/watch_blocked/main.sh`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 cp plan_blocked.py plan.py
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # First graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 [[ -f initial.txt ]] || exit -1
 [[ -f input.txt ]] || exit -1
 [[ ! -f output.txt ]] || exit -1
 [[ ! -f final.txt ]] || exit -1
 
 # Modify a few things and rerun
 cp plan_unblocked.py plan.py
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("plan.py")
+watch_update("plan.py")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/watch_boot/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_input/expected_graph_02.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,53 +11,46 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:final.txt
-            supplies   file:first.txt
+            supplies   file:input.txt
+            supplies   file:output.txt
             supplies   file:plan.py
             supplies   step:./plan.py
-            supplies   step:cp first.txt final.txt
-            supplies   step:echo "test 1" > first.txt
+            supplies   step:cp input.txt output.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   step:cp first.txt final.txt
-             creates   step:echo "test 1" > first.txt
+             creates   file:input.txt
+             creates   step:cp input.txt output.txt
 
-step:echo "test 1" > first.txt
-             workdir = ./
-             command = echo "test 1" > first.txt
-               state = SUCCEEDED
+file:input.txt
+                path = input.txt
+               state = MISSING
           created by   step:./plan.py
             consumes   file:./
-             creates   file:first.txt
-
-file:first.txt
-                path = first.txt
-               state = BUILT
-          created by   step:echo "test 1" > first.txt
-            consumes   file:./
-            supplies   step:cp first.txt final.txt
+            supplies   step:cp input.txt output.txt
 
-step:cp first.txt final.txt
+step:cp input.txt output.txt
              workdir = ./
-             command = cp first.txt final.txt
-               state = SUCCEEDED
+             command = cp input.txt output.txt
+               state = PENDING
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:first.txt
-             creates   file:final.txt
-
-file:final.txt
-                path = final.txt
-               state = BUILT
-          created by   step:cp first.txt final.txt
+            consumes   file:input.txt
+             creates   file:output.txt
+            supplies   file:output.txt
+
+file:output.txt
+                path = output.txt
+               state = PENDING
+          created by   step:cp input.txt output.txt
             consumes   file:./
+            consumes   step:cp input.txt output.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_boot/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_boot/expected_graph_02.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,31 +33,35 @@
              creates   step:echo "test 2" > second.txt
 
 file:final.txt
                 path = final.txt
                state = BUILT
           created by   step:cp second.txt final.txt
             consumes   file:./
+            consumes   step:cp second.txt final.txt
 
 step:echo "test 2" > second.txt
              workdir = ./
              command = echo "test 2" > second.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:second.txt
+            supplies   file:second.txt
 
 file:second.txt
                 path = second.txt
                state = BUILT
           created by   step:echo "test 2" > second.txt
             consumes   file:./
+            consumes   step:echo "test 2" > second.txt
             supplies   step:cp second.txt final.txt
 
 step:cp second.txt final.txt
              workdir = ./
              command = cp second.txt final.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:second.txt
              creates   file:final.txt
+            supplies   file:final.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_boot/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_boot/expected_stdout.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ echo "test 1" > first.txt
    SUCCESS │ echo "test 1" > first.txt
      START │ cp first.txt final.txt
    SUCCESS │ cp first.txt final.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ plan.py
-     ADDED │ plan.py
+   UPDATED │ plan.py
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ echo "test 2" > second.txt
    SUCCESS │ echo "test 2" > second.txt
      START │ cp second.txt final.txt
    SUCCESS │ cp second.txt final.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_boot/main.sh` & `stepup-1.1.0/tests/cases/watch_boot/main.sh`

 * *Files 22% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 cp -a plan_01.py plan.py
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f first.txt ]] || exit -1
 [[ -f final.txt ]] || exit -1
 
 # Modify the plan.py script and rerun with the modified plan.py.
 cp -a plan_02.py plan.py
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("plan.py")
+watch_update("plan.py")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/watch_chain/README.md` & `stepup-1.1.0/tests/cases/watch_chain/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/watch_chain/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_chain/expected_graph_01.txt`

 * *Files 5% similar despite different names*

```diff
@@ -61,57 +61,65 @@
           created by   step:./plan.py
             consumes   file:./
             consumes   file:config.json
             consumes   file:use_config.py
              creates   file:output.txt
              creates   step:echo All is fine. > script.log
              creates   step:echo log written to script.log. > report.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
           created by   step:./use_config.py
             consumes   file:./
+            consumes   step:./use_config.py
 
 step:cp -aT report.txt copy.txt
              workdir = ./
              command = cp -aT report.txt copy.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:report.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:report.txt
                 path = report.txt
                state = BUILT
           created by   step:echo log written to script.log. > report.txt
             consumes   file:./
+            consumes   step:echo log written to script.log. > report.txt
             supplies   step:cp -aT report.txt copy.txt
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:cp -aT report.txt copy.txt
             consumes   file:./
+            consumes   step:cp -aT report.txt copy.txt
 
 step:echo All is fine. > script.log
              workdir = ./
              command = echo All is fine. > script.log
                state = SUCCEEDED
           created by   step:./use_config.py
             consumes   file:./
              creates   file:script.log
+            supplies   file:script.log
 
 file:script.log
                 path = script.log
                state = BUILT
           created by   step:echo All is fine. > script.log
             consumes   file:./
+            consumes   step:echo All is fine. > script.log
 
 step:echo log written to script.log. > report.txt
              workdir = ./
              command = echo log written to script.log. > report.txt
                state = SUCCEEDED
           created by   step:./use_config.py
             consumes   file:./
              creates   file:report.txt
+            supplies   file:report.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_chain/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_chain/expected_graph_02.txt`

 * *Files 6% similar despite different names*

```diff
@@ -61,57 +61,65 @@
           created by   step:./plan.py
             consumes   file:./
             consumes   file:config.json
             consumes   file:use_config.py
              creates   file:output.txt
              creates   step:echo All is fine. > other.log
              creates   step:echo log written to other.log. > report.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
           created by   step:./use_config.py
             consumes   file:./
+            consumes   step:./use_config.py
 
 step:cp -aT report.txt copy.txt
              workdir = ./
              command = cp -aT report.txt copy.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:report.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:report.txt
                 path = report.txt
                state = BUILT
           created by   step:echo log written to other.log. > report.txt
             consumes   file:./
+            consumes   step:echo log written to other.log. > report.txt
             supplies   step:cp -aT report.txt copy.txt
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:cp -aT report.txt copy.txt
             consumes   file:./
+            consumes   step:cp -aT report.txt copy.txt
 
 step:echo All is fine. > other.log
              workdir = ./
              command = echo All is fine. > other.log
                state = SUCCEEDED
           created by   step:./use_config.py
             consumes   file:./
              creates   file:other.log
+            supplies   file:other.log
 
 file:other.log
                 path = other.log
                state = BUILT
           created by   step:echo All is fine. > other.log
             consumes   file:./
+            consumes   step:echo All is fine. > other.log
 
 step:echo log written to other.log. > report.txt
              workdir = ./
              command = echo log written to other.log. > report.txt
                state = SUCCEEDED
           created by   step:./use_config.py
             consumes   file:./
              creates   file:report.txt
+            supplies   file:report.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_chain/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_chain/expected_stdout.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./use_config.py
    SUCCESS │ ./use_config.py
      START │ echo All is fine. > script.log
    SUCCESS │ echo All is fine. > script.log
      START │ echo log written to script.log. > report.txt
    SUCCESS │ echo log written to script.log. > report.txt
      START │ cp -aT report.txt copy.txt
    SUCCESS │ cp -aT report.txt copy.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ config.json
-     ADDED │ config.json
+   UPDATED │ config.json
      PHASE │ run
      START │ ./use_config.py
    SUCCESS │ ./use_config.py
      START │ echo All is fine. > other.log
    SUCCESS │ echo All is fine. > other.log
      START │ echo log written to other.log. > report.txt
    SUCCESS │ echo log written to other.log. > report.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_chain/main.sh` & `stepup-1.1.0/tests/cases/watch_chain/main.sh`

 * *Files 16% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 cp config_01.json config.json
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f script.log ]] || exit -1
 grep script.log report.txt
 grep script.log copy.txt
 [[ -f output.txt ]] || exit -1
 
 # Modify config.json and rerun.
 cp config_02.json config.json
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("config.json")
+watch_update("config.json")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/watch_chain/use_config.py` & `stepup-1.1.0/tests/cases/watch_chain/use_config.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/cases/watch_input/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_input/expected_graph_03.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,13 +42,15 @@
              workdir = ./
              command = cp input.txt output.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
           created by   step:cp input.txt output.txt
             consumes   file:./
+            consumes   step:cp input.txt output.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_input/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_nochanges/expected_graph_01.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,26 +29,28 @@
             consumes   file:./
             consumes   file:plan.py
              creates   file:input.txt
              creates   step:cp input.txt output.txt
 
 file:input.txt
                 path = input.txt
-               state = MISSING
+               state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:cp input.txt output.txt
 
 step:cp input.txt output.txt
              workdir = ./
              command = cp input.txt output.txt
-               state = PENDING
+               state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
-               state = PENDING
+               state = BUILT
           created by   step:cp input.txt output.txt
             consumes   file:./
+            consumes   step:cp input.txt output.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_input/expected_graph_03.txt` & `stepup-1.1.0/tests/cases/watch_nochanges/expected_graph_02.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,13 +42,15 @@
              workdir = ./
              command = cp input.txt output.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
           created by   step:cp input.txt output.txt
             consumes   file:./
+            consumes   step:cp input.txt output.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_input/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_input/expected_stdout.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp input.txt output.txt
    SUCCESS │ cp input.txt output.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ input.txt
@@ -15,15 +15,15 @@
 Inputs        STATIC  ./
              MISSING  input.txt
 Outputs      PENDING  output.txt
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-     ADDED │ input.txt
+   UPDATED │ input.txt
      PHASE │ run
      START │ cp input.txt output.txt
    SUCCESS │ cp input.txt output.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/watch_input/main.sh` & `stepup-1.1.0/tests/cases/watch_input/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 cp first.txt input.txt
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Remove input and rerun the plan.
 rm input.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_del("input.txt")
+watch_delete("input.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 EOD
 
 # Replace input and rerun the plan.
 cp second.txt input.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("input.txt")
+watch_update("input.txt")
 run()
 wait()
-graph("current_graph_03.txt")
+graph("current_graph_03")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/watch_middle/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_middle/expected_graph_01.txt`

 * *Files 8% similar despite different names*

```diff
@@ -38,36 +38,40 @@
              workdir = ./
              command = cp copy.txt another.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:copy.txt
              creates   file:another.txt
+            supplies   file:another.txt
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:cp original.txt copy.txt
             consumes   file:./
+            consumes   step:cp original.txt copy.txt
             supplies   step:cp copy.txt another.txt
 
 file:another.txt
                 path = another.txt
                state = BUILT
           created by   step:cp copy.txt another.txt
             consumes   file:./
+            consumes   step:cp copy.txt another.txt
 
 step:cp original.txt copy.txt
              workdir = ./
              command = cp original.txt copy.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:original.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:original.txt
                 path = original.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:cp original.txt copy.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_middle/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_middle/expected_graph_02.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,31 +33,35 @@
 
 (step:cp copy.txt another.txt)
              workdir = ./
              command = cp copy.txt another.txt
                state = PENDING
             consumes   file:./
             consumes   (file:copy.txt)
+            supplies   (file:another.txt)
 
 (file:copy.txt)
                 path = copy.txt
                state = PENDING
             consumes   file:./
+            consumes   (step:cp original.txt copy.txt)
             supplies   (step:cp copy.txt another.txt)
 
 (file:another.txt)
                 path = another.txt
                state = PENDING
             consumes   file:./
+            consumes   (step:cp copy.txt another.txt)
 
 (step:cp original.txt copy.txt)
              workdir = ./
              command = cp original.txt copy.txt
                state = PENDING
             consumes   file:./
             consumes   (file:original.txt)
+            supplies   (file:copy.txt)
 
 (file:original.txt)
                 path = original.txt
                state = STATIC
             consumes   file:./
             supplies   (step:cp original.txt copy.txt)
```

### Comparing `stepup-1.0.0/tests/cases/watch_middle/expected_graph_03.txt` & `stepup-1.1.0/tests/cases/watch_middle/expected_graph_03.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
              creates   step:cp original.txt between.txt
 
 file:another.txt
                 path = another.txt
                state = BUILT
           created by   step:cp between.txt another.txt
             consumes   file:./
+            consumes   step:cp between.txt another.txt
 
 file:original.txt
                 path = original.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:cp original.txt between.txt
@@ -51,23 +52,26 @@
              workdir = ./
              command = cp between.txt another.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:between.txt
              creates   file:another.txt
+            supplies   file:another.txt
 
 file:between.txt
                 path = between.txt
                state = BUILT
           created by   step:cp original.txt between.txt
             consumes   file:./
+            consumes   step:cp original.txt between.txt
             supplies   step:cp between.txt another.txt
 
 step:cp original.txt between.txt
              workdir = ./
              command = cp original.txt between.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:original.txt
              creates   file:between.txt
+            supplies   file:between.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_middle/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_middle/expected_stdout.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp original.txt copy.txt
    SUCCESS │ cp original.txt copy.txt
      START │ cp copy.txt another.txt
    SUCCESS │ cp copy.txt another.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
@@ -16,15 +16,15 @@
 Working directory     ./
 Inputs        STATIC  ./
              MISSING  plan.py
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-     ADDED │ plan.py
+   UPDATED │ plan.py
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp original.txt between.txt
    SUCCESS │ cp original.txt between.txt
      START │ cp between.txt another.txt
    SUCCESS │ cp between.txt another.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_middle/main.sh` & `stepup-1.1.0/tests/cases/watch_middle/main.sh`

 * *Files 17% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 cp plan_01.py plan.py
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Remove plan and rerun.
 rm plan.py
 python3 - << EOD
 from stepup.core.interact import *
-watch_del("plan.py")
+watch_delete("plan.py")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 EOD
 
 # Check files that are expected to be present and/or missing.
 # Files should not be removed because of pending steps:
 [[ -f copy.txt ]] || exit -1
 [[ -f another.txt ]] || exit -1
 
 # Replace plan and rerun.
 cp plan_02.py plan.py
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("plan.py")
+watch_update("plan.py")
 run()
 wait()
-graph("current_graph_03.txt")
+graph("current_graph_03")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/watch_mixed/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_mixed/expected_graph_02.txt`

 * *Files 21% similar despite different names*

```diff
@@ -11,63 +11,59 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:copy1.txt
+            supplies   (file:copy1.txt)
             supplies   file:copy2.txt
-            supplies   file:orig.txt
+            supplies   (file:orig.txt)
             supplies   file:plan.py
             supplies   step:./plan.py
             supplies   step:cp copy1.txt copy2.txt
-            supplies   step:cp orig.txt copy1.txt
+            supplies   (step:cp orig.txt copy1.txt)
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:orig.txt
              creates   step:cp copy1.txt copy2.txt
-             creates   step:cp orig.txt copy1.txt
 
-file:orig.txt
+(file:orig.txt)
                 path = orig.txt
-               state = STATIC
-          created by   step:./plan.py
+               state = MISSING
             consumes   file:./
-            supplies   step:cp orig.txt copy1.txt
+            supplies   (step:cp orig.txt copy1.txt)
 
-step:cp orig.txt copy1.txt
+(step:cp orig.txt copy1.txt)
              workdir = ./
              command = cp orig.txt copy1.txt
-               state = SUCCEEDED
-          created by   step:./plan.py
+               state = PENDING
             consumes   file:./
-            consumes   file:orig.txt
-             creates   file:copy1.txt
+            consumes   (file:orig.txt)
 
-file:copy1.txt
+(file:copy1.txt)
                 path = copy1.txt
-               state = BUILT
-          created by   step:cp orig.txt copy1.txt
+               state = PENDING
             consumes   file:./
             supplies   step:cp copy1.txt copy2.txt
 
 step:cp copy1.txt copy2.txt
              workdir = ./
              command = cp copy1.txt copy2.txt
-               state = SUCCEEDED
+               state = PENDING
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:copy1.txt
+            consumes   (file:copy1.txt)
              creates   file:copy2.txt
+            supplies   file:copy2.txt
 
 file:copy2.txt
                 path = copy2.txt
-               state = BUILT
+               state = PENDING
           created by   step:cp copy1.txt copy2.txt
             consumes   file:./
+            consumes   step:cp copy1.txt copy2.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_mixed/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_mixed/expected_stdout.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp orig.txt copy1.txt
    SUCCESS │ cp orig.txt copy1.txt
      START │ cp copy1.txt copy2.txt
    SUCCESS │ cp copy1.txt copy2.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ plan.py
-     ADDED │ plan.py
+   UPDATED │ plan.py
    DELETED │ orig.txt
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
    WARNING │ 1 step remains pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
 Command               cp copy1.txt copy2.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_mixed/main.sh` & `stepup-1.1.0/tests/cases/watch_mixed/main.sh`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 cp backup.txt orig.txt
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # First graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Modify a few things and rerun
 cp plan_trimmed.py plan.py
 rm orig.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("plan.py")
-watch_del("orig.txt")
+watch_update("plan.py")
+watch_delete("orig.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup-1.0.0/tests/cases/watch_nochanges/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_output/expected_graph_01.txt`

 * *Files 13% similar despite different names*

```diff
@@ -15,40 +15,42 @@
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:input.txt
             supplies   file:output.txt
             supplies   file:plan.py
             supplies   step:./plan.py
-            supplies   step:cp input.txt output.txt
+            supplies   step:cp -aT input.txt output.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
              creates   file:input.txt
-             creates   step:cp input.txt output.txt
+             creates   step:cp -aT input.txt output.txt
 
 file:input.txt
                 path = input.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:cp input.txt output.txt
+            supplies   step:cp -aT input.txt output.txt
 
-step:cp input.txt output.txt
+step:cp -aT input.txt output.txt
              workdir = ./
-             command = cp input.txt output.txt
+             command = cp -aT input.txt output.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
-          created by   step:cp input.txt output.txt
+          created by   step:cp -aT input.txt output.txt
             consumes   file:./
+            consumes   step:cp -aT input.txt output.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_nochanges/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_output/expected_graph_02.txt`

 * *Files 13% similar despite different names*

```diff
@@ -15,40 +15,42 @@
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:input.txt
             supplies   file:output.txt
             supplies   file:plan.py
             supplies   step:./plan.py
-            supplies   step:cp input.txt output.txt
+            supplies   step:cp -aT input.txt output.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
              creates   file:input.txt
-             creates   step:cp input.txt output.txt
+             creates   step:cp -aT input.txt output.txt
 
 file:input.txt
                 path = input.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:cp input.txt output.txt
+            supplies   step:cp -aT input.txt output.txt
 
-step:cp input.txt output.txt
+step:cp -aT input.txt output.txt
              workdir = ./
-             command = cp input.txt output.txt
+             command = cp -aT input.txt output.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:input.txt
              creates   file:output.txt
+            supplies   file:output.txt
 
 file:output.txt
                 path = output.txt
                state = BUILT
-          created by   step:cp input.txt output.txt
+          created by   step:cp -aT input.txt output.txt
             consumes   file:./
+            consumes   step:cp -aT input.txt output.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_nochanges/main.sh` & `stepup-1.1.0/tests/cases/permissions_plan_rerun/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
-# Run the example
+# Run the plan with non-executable step.py.
+chmod -x sub/plan.py
 stepup -w 1 plan.py & # > current_stdout.txt &
 
-# Get the graph after completion of the pending steps.
+# Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f input.txt ]] || exit -1
-[[ -f output.txt ]] || exit -1
+[[ -f sub/plan.py ]] || exit -1
+[[ ! -f sub/done.txt ]] || exit -1
 
-# Rerun, no changes expected.
+# Rerun the plan with executable step.py.
+chmod +x sub/plan.py
+
+# Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
+watch_update("sub/plan.py")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f input.txt ]] || exit -1
-[[ -f output.txt ]] || exit -1
+[[ -f sub/plan.py ]] || exit -1
+[[ -f sub/done.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/watch_outdated_amend1/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_outdated_amend1/expected_graph_02.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:copy.txt
-            supplies   file:inp1.txt
+            supplies   file:inp2.txt
             supplies   file:plan.py
             supplies   file:step.py
             supplies   file:subs.txt
             supplies   step:./plan.py
             supplies   step:./step.py
 
 step:./plan.py
@@ -47,34 +47,36 @@
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:./step.py
 
 dg:'inp*.txt'
           created by   step:./plan.py
-             creates   file:inp1.txt
+             creates   file:inp2.txt
 
 step:./step.py
              workdir = ./
              command = ./step.py
                state = SUCCEEDED
-  consumes (amended) = file:inp1.txt
-   creates (amended) = file:copy.txt
+  consumes (amended) = file:inp2.txt
+  supplies (amended) = file:copy.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:inp1.txt
+            consumes   file:inp2.txt
             consumes   file:subs.txt
              creates   file:copy.txt
-
-file:inp1.txt
-                path = inp1.txt
-               state = STATIC
-          created by   dg:'inp*.txt'
-            consumes   file:./
-            supplies   step:./step.py
+            supplies   file:copy.txt
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:./step.py
             consumes   file:./
+            consumes   step:./step.py
+
+file:inp2.txt
+                path = inp2.txt
+               state = STATIC
+          created by   dg:'inp*.txt'
+            consumes   file:./
+            supplies   step:./step.py
```

### Comparing `stepup-1.0.0/tests/cases/watch_outdated_amend1/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_wanted/expected_graph_01.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,70 +11,79 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:copy.txt
-            supplies   file:inp2.txt
+            supplies   (file:input1.txt)
+            supplies   (file:input2.txt)
+            supplies   file:output1.txt
+            supplies   file:output2.txt
             supplies   file:plan.py
-            supplies   file:step.py
-            supplies   file:subs.txt
+            supplies   file:static.txt
             supplies   step:./plan.py
-            supplies   step:./step.py
+            supplies   step:cp input1.txt output1.txt
+            supplies   step:cp input2.txt output2.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
-       extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   dg:'inp*.txt'
-             creates   file:step.py
-             creates   file:subs.txt
-             creates   step:./step.py
+             creates   file:static.txt
+             creates   step:cp input1.txt output1.txt
+             creates   step:cp input2.txt output2.txt
 
-file:step.py
-                path = step.py
+file:static.txt
+                path = static.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
 
-file:subs.txt
-                path = subs.txt
-               state = STATIC
+step:cp input1.txt output1.txt
+             workdir = ./
+             command = cp input1.txt output1.txt
+               state = PENDING
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:./step.py
+            consumes   (file:input1.txt)
+             creates   file:output1.txt
+            supplies   file:output1.txt
 
-dg:'inp*.txt'
-          created by   step:./plan.py
-             creates   file:inp2.txt
+(file:input1.txt)
+                path = input1.txt
+               state = PENDING
+            consumes   file:./
+            supplies   step:cp input1.txt output1.txt
+
+file:output1.txt
+                path = output1.txt
+               state = PENDING
+          created by   step:cp input1.txt output1.txt
+            consumes   file:./
+            consumes   step:cp input1.txt output1.txt
 
-step:./step.py
+step:cp input2.txt output2.txt
              workdir = ./
-             command = ./step.py
-               state = SUCCEEDED
-  consumes (amended) = file:inp2.txt
-   creates (amended) = file:copy.txt
-       extended hash = yes
+             command = cp input2.txt output2.txt
+               state = PENDING
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:inp2.txt
-            consumes   file:subs.txt
-             creates   file:copy.txt
-
-file:copy.txt
-                path = copy.txt
-               state = BUILT
-          created by   step:./step.py
-            consumes   file:./
-
-file:inp2.txt
-                path = inp2.txt
-               state = STATIC
-          created by   dg:'inp*.txt'
+            consumes   (file:input2.txt)
+             creates   file:output2.txt
+            supplies   file:output2.txt
+
+(file:input2.txt)
+                path = input2.txt
+               state = PENDING
+            consumes   file:./
+            supplies   step:cp input2.txt output2.txt
+
+file:output2.txt
+                path = output2.txt
+               state = PENDING
+          created by   step:cp input2.txt output2.txt
             consumes   file:./
-            supplies   step:./step.py
+            consumes   step:cp input2.txt output2.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_outdated_amend1/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_outdated_amend1/expected_stdout.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ ./step.py
    SUCCESS │ ./step.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ subs.txt
-     ADDED │ subs.txt
    DELETED │ inp1.txt
+   UPDATED │ subs.txt
      PHASE │ run
  DROPAMEND │ ./step.py
 ────────────────────── Outdated amended step information ───────────────────────
 Modified step hash   extended, digest 764de23c ➜ ccae7573, inp_digset d7b8a410 ➜ 7eb5fb40
 Modified inp hash    subs.txt (digest 30d31453 ➜ c273a7ee)
 ──────────────────────── Remained the same (or missing) ────────────────────────
 Same inp hash        ./
```

### Comparing `stepup-1.0.0/tests/cases/watch_outdated_amend1/main.sh` & `stepup-1.1.0/tests/cases/watch_outdated_amend2/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -2,46 +2,52 @@
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run with the initial subs.txt.
 echo inp1 > inp1.txt
-echo inp1.txt > subs.txt
+echo conv1.txt > subs1.txt
 stepup -e -w 1 plan.py & # > current_stdout.txt &
 
 # Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f inp1.txt ]] || exit -1
-[[ -f copy.txt ]] || exit -1
-grep inp1 copy.txt
+[[ -f subs1.txt ]] || exit -1
+[[ -f subs2.txt ]] || exit -1
+grep conv1.txt subs2.txt
+[[ -f subs3.txt ]] || exit -1
+grep conv1.txt subs3.txt
 
 # Change subs.txt and rerun.
 rm inp1.txt
 echo inp2 > inp2.txt
-echo inp2.txt > subs.txt
+echo conv2.txt > subs1.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("subs.txt")
-watch_del("inp1.txt")
+watch_update("subs1.txt")
+watch_delete("inp1.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ ! -f inp1.txt ]] || exit -1
 [[ -f inp2.txt ]] || exit -1
-[[ -f copy.txt ]] || exit -1
-grep inp2 copy.txt
+[[ -f subs1.txt ]] || exit -1
+[[ -f subs2.txt ]] || exit -1
+grep conv2.txt subs2.txt
+[[ -f subs3.txt ]] || exit -1
+grep conv2.txt subs3.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_outdated_amend2/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_outdated_amend2/expected_graph_01.txt`

 * *Files 8% similar despite different names*

```diff
@@ -68,52 +68,58 @@
              command = cp -aT inp1.txt conv1.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp1.txt
              creates   file:conv1.txt
+            supplies   file:conv1.txt
 
 file:conv1.txt
                 path = conv1.txt
                state = BUILT
           created by   step:cp -aT inp1.txt conv1.txt
             consumes   file:./
+            consumes   step:cp -aT inp1.txt conv1.txt
             supplies   step:./step.py subs1.txt > subs2.txt
             supplies   step:./step.py subs2.txt > subs3.txt
 
 step:./step.py subs1.txt > subs2.txt
              workdir = ./
              command = ./step.py subs1.txt > subs2.txt
                state = SUCCEEDED
   consumes (amended) = file:conv1.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:conv1.txt
             consumes   file:subs1.txt
              creates   file:subs2.txt
+            supplies   file:subs2.txt
 
 file:subs2.txt
                 path = subs2.txt
                state = BUILT
           created by   step:./step.py subs1.txt > subs2.txt
             consumes   file:./
+            consumes   step:./step.py subs1.txt > subs2.txt
             supplies   step:./step.py subs2.txt > subs3.txt
 
 step:./step.py subs2.txt > subs3.txt
              workdir = ./
              command = ./step.py subs2.txt > subs3.txt
                state = SUCCEEDED
   consumes (amended) = file:conv1.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:conv1.txt
             consumes   file:subs2.txt
              creates   file:subs3.txt
+            supplies   file:subs3.txt
 
 file:subs3.txt
                 path = subs3.txt
                state = BUILT
           created by   step:./step.py subs2.txt > subs3.txt
             consumes   file:./
+            consumes   step:./step.py subs2.txt > subs3.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_outdated_amend2/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/watch_outdated_amend2/expected_graph_02.txt`

 * *Files 5% similar despite different names*

```diff
@@ -63,39 +63,43 @@
   consumes (amended) = file:conv2.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:conv2.txt
             consumes   file:subs1.txt
              creates   file:subs2.txt
+            supplies   file:subs2.txt
 
 file:subs2.txt
                 path = subs2.txt
                state = BUILT
           created by   step:./step.py subs1.txt > subs2.txt
             consumes   file:./
+            consumes   step:./step.py subs1.txt > subs2.txt
             supplies   step:./step.py subs2.txt > subs3.txt
 
 step:./step.py subs2.txt > subs3.txt
              workdir = ./
              command = ./step.py subs2.txt > subs3.txt
                state = SUCCEEDED
   consumes (amended) = file:conv2.txt
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:conv2.txt
             consumes   file:subs2.txt
              creates   file:subs3.txt
+            supplies   file:subs3.txt
 
 file:subs3.txt
                 path = subs3.txt
                state = BUILT
           created by   step:./step.py subs2.txt > subs3.txt
             consumes   file:./
+            consumes   step:./step.py subs2.txt > subs3.txt
 
 file:inp2.txt
                 path = inp2.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:cp -aT inp2.txt conv2.txt
@@ -105,15 +109,17 @@
              command = cp -aT inp2.txt conv2.txt
                state = SUCCEEDED
        extended hash = yes
           created by   step:./plan.py
             consumes   file:./
             consumes   file:inp2.txt
              creates   file:conv2.txt
+            supplies   file:conv2.txt
 
 file:conv2.txt
                 path = conv2.txt
                state = BUILT
           created by   step:cp -aT inp2.txt conv2.txt
             consumes   file:./
+            consumes   step:cp -aT inp2.txt conv2.txt
             supplies   step:./step.py subs1.txt > subs2.txt
             supplies   step:./step.py subs2.txt > subs3.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_outdated_amend2/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_outdated_amend2/expected_stdout.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp -aT inp1.txt conv1.txt
    SUCCESS │ cp -aT inp1.txt conv1.txt
      START │ ./step.py subs1.txt > subs2.txt
    SUCCESS │ ./step.py subs1.txt > subs2.txt
      START │ ./step.py subs2.txt > subs3.txt
    SUCCESS │ ./step.py subs2.txt > subs3.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-     ADDED │ inp2.txt
-   DELETED │ subs1.txt
-     ADDED │ subs1.txt
    DELETED │ inp1.txt
+   UPDATED │ inp2.txt
+   UPDATED │ subs1.txt
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ cp -aT inp2.txt conv2.txt
    SUCCESS │ cp -aT inp2.txt conv2.txt
  DROPAMEND │ ./step.py subs1.txt > subs2.txt
 ────────────────────── Outdated amended step information ───────────────────────
```

### Comparing `stepup-1.0.0/tests/cases/watch_outdated_amend2/main.sh` & `stepup-1.1.0/tests/cases/watch_wanted/main.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,66 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
-# Run with the initial subs.txt.
-echo inp1 > inp1.txt
-echo conv1.txt > subs1.txt
-stepup -e -w 1 plan.py & # > current_stdout.txt &
+# Run the initial plan.
+touch static.txt
+touch input1.txt
+touch input2.txt
+cp plan_01.py plan.py
+stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f inp1.txt ]] || exit -1
-[[ -f subs1.txt ]] || exit -1
-[[ -f subs2.txt ]] || exit -1
-grep conv1.txt subs2.txt
-[[ -f subs3.txt ]] || exit -1
-grep conv1.txt subs3.txt
-
-# Change subs.txt and rerun.
-rm inp1.txt
-echo inp2 > inp2.txt
-echo conv2.txt > subs1.txt
+[[ -f static.txt ]] || exit -1
+[[ -f input1.txt ]] || exit -1
+[[ -f input2.txt ]] || exit -1
+[[ ! -f output1.txt ]] || exit -1
+[[ ! -f output2.txt ]] || exit -1
+
+# Remove plan and rerun.
+rm plan.py
+python3 - << EOD
+from stepup.core.interact import *
+watch_delete("plan.py")
+run()
+wait()
+graph("current_graph_02")
+EOD
+
+# Check files that are expected to be present and/or missing.
+[[ -f static.txt ]] || exit -1
+[[ -f input1.txt ]] || exit -1
+[[ -f input2.txt ]] || exit -1
+[[ ! -f output1.txt ]] || exit -1
+[[ ! -f output2.txt ]] || exit -1
+
+# Replace plan and rerun.
+cp plan_02.py plan.py
 python3 - << EOD
 from stepup.core.interact import *
-watch_add("subs1.txt")
-watch_del("inp1.txt")
+watch_update("plan.py")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_03")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ ! -f inp1.txt ]] || exit -1
-[[ -f inp2.txt ]] || exit -1
-[[ -f subs1.txt ]] || exit -1
-[[ -f subs2.txt ]] || exit -1
-grep conv2.txt subs2.txt
-[[ -f subs3.txt ]] || exit -1
-grep conv2.txt subs3.txt
+[[ -f static.txt ]] || exit -1
+[[ -f input1.txt ]] || exit -1
+[[ -f input2.txt ]] || exit -1
+[[ ! -f output1.txt ]] || exit -1
+[[ ! -f output2.txt ]] || exit -1
```

### Comparing `stepup-1.0.0/tests/cases/watch_output/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/not_cyclic/expected_graph_01.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,40 +15,35 @@
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:input.txt
             supplies   file:output.txt
             supplies   file:plan.py
             supplies   step:./plan.py
-            supplies   step:cp -aT input.txt output.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
+  consumes (amended) = file:input.txt
+  supplies (amended) = file:output.txt
           created by   root:
             consumes   file:./
+            consumes   file:input.txt
             consumes   file:plan.py
              creates   file:input.txt
-             creates   step:cp -aT input.txt output.txt
+             creates   file:output.txt
+            supplies   file:output.txt
 
 file:input.txt
                 path = input.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:cp -aT input.txt output.txt
-
-step:cp -aT input.txt output.txt
-             workdir = ./
-             command = cp -aT input.txt output.txt
-               state = SUCCEEDED
-          created by   step:./plan.py
-            consumes   file:./
-            consumes   file:input.txt
-             creates   file:output.txt
+            supplies   step:./plan.py
 
 file:output.txt
                 path = output.txt
                state = BUILT
-          created by   step:cp -aT input.txt output.txt
+          created by   step:./plan.py
             consumes   file:./
+            consumes   step:./plan.py
```

### Comparing `stepup-1.0.0/tests/cases/watch_output/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/not_cyclic/expected_graph_02.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,40 +15,35 @@
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:input.txt
             supplies   file:output.txt
             supplies   file:plan.py
             supplies   step:./plan.py
-            supplies   step:cp -aT input.txt output.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
+  consumes (amended) = file:input.txt
+  supplies (amended) = file:output.txt
           created by   root:
             consumes   file:./
+            consumes   file:input.txt
             consumes   file:plan.py
              creates   file:input.txt
-             creates   step:cp -aT input.txt output.txt
+             creates   file:output.txt
+            supplies   file:output.txt
 
 file:input.txt
                 path = input.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:cp -aT input.txt output.txt
-
-step:cp -aT input.txt output.txt
-             workdir = ./
-             command = cp -aT input.txt output.txt
-               state = SUCCEEDED
-          created by   step:./plan.py
-            consumes   file:./
-            consumes   file:input.txt
-             creates   file:output.txt
+            supplies   step:./plan.py
 
 file:output.txt
                 path = output.txt
                state = BUILT
-          created by   step:cp -aT input.txt output.txt
+          created by   step:./plan.py
             consumes   file:./
+            consumes   step:./plan.py
```

### Comparing `stepup-1.0.0/tests/cases/watch_output/expected_stdout.txt` & `stepup-1.1.0/tests/cases/not_cyclic/expected_stdout.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
-     START │ cp -aT input.txt output.txt
-   SUCCESS │ cp -aT input.txt output.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
+   UPDATED │ input.txt
+     PHASE │ run
+     START │ ./plan.py
+   SUCCESS │ ./plan.py
+  WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
+     PHASE │ watch
+   UPDATED │ input.txt
    DELETED │ output.txt
      PHASE │ run
-     START │ cp -aT input.txt output.txt
-   SUCCESS │ cp -aT input.txt output.txt
+     START │ ./plan.py
+   SUCCESS │ ./plan.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/cases/watch_output/main.sh` & `stepup-1.1.0/tests/cases/not_cyclic/main.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,57 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
+echo "hello" > input.txt
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f input.txt ]] || exit -1
-[[ -f output.txt ]] || exit -1
+grep hello output.txt
 
-# Remove a built file and rerun.
+# Change the input and check that the step reruns without pending dependencies
+echo "bye" > input.txt
+python3 - << EOD
+from stepup.core.interact import *
+watch_update("input.txt")
+run()
+wait()
+graph("current_graph_02")
+EOD
+
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f input.txt ]] || exit -1
+grep bye output.txt
+
+# Touch input (no changes) and check that the step reruns without pending dependencies
+touch input.txt
 rm output.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_del("output.txt")
+watch_update("input.txt")
+watch_delete("output.txt")
 run()
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_03")
 join()
 EOD
 
-# Wait for background processes, if any.
-wait $(jobs -p)
-
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f input.txt ]] || exit -1
-[[ -f output.txt ]] || exit -1
+grep bye output.txt
+
+# Wait for background processes, if any.
+wait $(jobs -p)
```

### Comparing `stepup-1.0.0/tests/cases/watch_wanted/expected_graph_01.txt` & `stepup-1.1.0/tests/cases/watch_wanted/expected_graph_02.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,84 +2,78 @@
              version = v1
              creates   file:./
              creates   file:plan.py
              creates   step:./plan.py
 
 file:plan.py
                 path = plan.py
-               state = STATIC
+               state = MISSING
           created by   root:
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
             supplies   (file:input1.txt)
             supplies   (file:input2.txt)
-            supplies   file:output1.txt
-            supplies   file:output2.txt
+            supplies   (file:output1.txt)
+            supplies   (file:output2.txt)
             supplies   file:plan.py
-            supplies   file:static.txt
+            supplies   (file:static.txt)
             supplies   step:./plan.py
-            supplies   step:cp input1.txt output1.txt
-            supplies   step:cp input2.txt output2.txt
+            supplies   (step:cp input1.txt output1.txt)
+            supplies   (step:cp input2.txt output2.txt)
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
-               state = SUCCEEDED
+               state = PENDING
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:static.txt
-             creates   step:cp input1.txt output1.txt
-             creates   step:cp input2.txt output2.txt
 
-file:static.txt
+(file:static.txt)
                 path = static.txt
                state = STATIC
-          created by   step:./plan.py
             consumes   file:./
 
-step:cp input1.txt output1.txt
+(step:cp input1.txt output1.txt)
              workdir = ./
              command = cp input1.txt output1.txt
                state = PENDING
-          created by   step:./plan.py
             consumes   file:./
             consumes   (file:input1.txt)
-             creates   file:output1.txt
+            supplies   (file:output1.txt)
 
 (file:input1.txt)
                 path = input1.txt
                state = PENDING
             consumes   file:./
-            supplies   step:cp input1.txt output1.txt
+            supplies   (step:cp input1.txt output1.txt)
 
-file:output1.txt
+(file:output1.txt)
                 path = output1.txt
                state = PENDING
-          created by   step:cp input1.txt output1.txt
             consumes   file:./
+            consumes   (step:cp input1.txt output1.txt)
 
-step:cp input2.txt output2.txt
+(step:cp input2.txt output2.txt)
              workdir = ./
              command = cp input2.txt output2.txt
                state = PENDING
-          created by   step:./plan.py
             consumes   file:./
             consumes   (file:input2.txt)
-             creates   file:output2.txt
+            supplies   (file:output2.txt)
 
 (file:input2.txt)
                 path = input2.txt
                state = PENDING
             consumes   file:./
-            supplies   step:cp input2.txt output2.txt
+            supplies   (step:cp input2.txt output2.txt)
 
-file:output2.txt
+(file:output2.txt)
                 path = output2.txt
                state = PENDING
-          created by   step:cp input2.txt output2.txt
             consumes   file:./
+            consumes   (step:cp input2.txt output2.txt)
```

### Comparing `stepup-1.0.0/tests/cases/watch_wanted/expected_graph_02.txt` & `stepup-1.1.0/tests/cases/static_nglob_partial/expected_graph_01.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,74 +2,76 @@
              version = v1
              creates   file:./
              creates   file:plan.py
              creates   step:./plan.py
 
 file:plan.py
                 path = plan.py
-               state = MISSING
+               state = STATIC
           created by   root:
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   (file:input1.txt)
-            supplies   (file:input2.txt)
-            supplies   (file:output1.txt)
-            supplies   (file:output2.txt)
+            supplies   file:head_x.txt
+            supplies   file:head_y.txt
+            supplies   file:paste_x.txt
             supplies   file:plan.py
-            supplies   (file:static.txt)
+            supplies   file:tail_x.txt
             supplies   step:./plan.py
-            supplies   (step:cp input1.txt output1.txt)
-            supplies   (step:cp input2.txt output2.txt)
+            supplies   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
-               state = PENDING
+               state = SUCCEEDED
+                 ngm = ['head_${*char}.txt', 'tail_${*char}.txt'] {'char': '?'}
+       extended hash = yes
           created by   root:
             consumes   file:./
             consumes   file:plan.py
+             creates   file:head_x.txt
+             creates   file:head_y.txt
+             creates   file:tail_x.txt
+             creates   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 
-(file:static.txt)
-                path = static.txt
+file:head_x.txt
+                path = head_x.txt
                state = STATIC
+          created by   step:./plan.py
             consumes   file:./
+            supplies   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 
-(step:cp input1.txt output1.txt)
-             workdir = ./
-             command = cp input1.txt output1.txt
-               state = PENDING
-            consumes   file:./
-            consumes   (file:input1.txt)
-
-(file:input1.txt)
-                path = input1.txt
-               state = PENDING
+file:head_y.txt
+                path = head_y.txt
+               state = STATIC
+          created by   step:./plan.py
             consumes   file:./
-            supplies   (step:cp input1.txt output1.txt)
 
-(file:output1.txt)
-                path = output1.txt
-               state = PENDING
+file:tail_x.txt
+                path = tail_x.txt
+               state = STATIC
+          created by   step:./plan.py
             consumes   file:./
+            supplies   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
 
-(step:cp input2.txt output2.txt)
+step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
              workdir = ./
-             command = cp input2.txt output2.txt
-               state = PENDING
-            consumes   file:./
-            consumes   (file:input2.txt)
-
-(file:input2.txt)
-                path = input2.txt
-               state = PENDING
-            consumes   file:./
-            supplies   (step:cp input2.txt output2.txt)
-
-(file:output2.txt)
-                path = output2.txt
-               state = PENDING
+             command = paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
+               state = SUCCEEDED
+       extended hash = yes
+          created by   step:./plan.py
+            consumes   file:./
+            consumes   file:head_x.txt
+            consumes   file:tail_x.txt
+             creates   file:paste_x.txt
+            supplies   file:paste_x.txt
+
+file:paste_x.txt
+                path = paste_x.txt
+               state = BUILT
+          created by   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
             consumes   file:./
+            consumes   step:paste -d ' ' head_x.txt tail_x.txt > paste_x.txt
```

### Comparing `stepup-1.0.0/tests/cases/watch_wanted/expected_stdout.txt` & `stepup-1.1.0/tests/cases/watch_wanted/expected_stdout.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
    WARNING │ 2 steps remain pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
 Command               cp input1.txt output1.txt
 Working directory     ./
 Inputs        STATIC  ./
@@ -27,15 +27,15 @@
 Working directory     ./
 Inputs        STATIC  ./
              MISSING  plan.py
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ Skipping cleanup due to incomplete build.
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-     ADDED │ plan.py
+   UPDATED │ plan.py
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.0.0/tests/conftest.py` & `stepup-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/core_common.py` & `stepup-1.1.0/tests/core_common.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/echo_server_socket.py` & `stepup-1.1.0/tests/echo_server_socket.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/echo_server_stdio.py` & `stepup-1.1.0/tests/echo_server_stdio.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/test_assoc.py` & `stepup-1.1.0/tests/test_assoc.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/test_basics.py` & `stepup-1.1.0/tests/test_basics.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,17 +92,17 @@
 
 
 @pytest.mark.asyncio
 async def test_from_scratch(client: AsyncRPCClient, tmpdir: str):
     with open("DONE.txt", "w") as fh:
         fh.write("done")
     await client("wait")
-    path_graph = Path(tmpdir) / "graph.txt"
-    await client("graph", path_graph)
-    _check_graph(path_graph, FROM_SCRATCH_GRAPH)
+    prefix_graph = Path(tmpdir) / "graph"
+    await client("graph", prefix_graph)
+    _check_graph(prefix_graph + ".txt", FROM_SCRATCH_GRAPH)
 
 
 STATIC_GRAPH = """\
 root:
              version = v1
              creates   file:./
              creates   file:plan.py
@@ -148,17 +148,17 @@
             fh.write("bar")
         step_key_plan = "step:./plan.py"
         await client("static", step_key_plan, ["foo"])
     finally:
         with open("DONE.txt", "w") as fh:
             fh.write("done")
     await client("wait")
-    path_graph = Path(tmpdir) / "graph.txt"
-    await client("graph", path_graph)
-    _check_graph(path_graph, STATIC_GRAPH)
+    prefix_graph = Path(tmpdir) / "graph"
+    await client("graph", prefix_graph)
+    _check_graph(prefix_graph + ".txt", STATIC_GRAPH)
 
 
 COPY_GRAPH = """\
 root:
              version = v1
              creates   file:./
              creates   file:plan.py
@@ -195,27 +195,29 @@
              workdir = ./
              command = cp -v original.txt copy.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:original.txt
              creates   file:copy.txt
+            supplies   file:copy.txt
 
 file:original.txt
                 path = original.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:cp -v original.txt copy.txt
 
 file:copy.txt
                 path = copy.txt
                state = BUILT
           created by   step:cp -v original.txt copy.txt
             consumes   file:./
+            consumes   step:cp -v original.txt copy.txt
 
 """
 
 
 @pytest.mark.asyncio
 async def test_copy(client: AsyncRPCClient, tmpdir: str):
     try:
@@ -237,10 +239,10 @@
         )
         assert step_key_copy == "step:cp -v original.txt copy.txt"
         await client("static", step_key_plan, ["original.txt"])
     finally:
         with open("DONE.txt", "w") as fh:
             fh.write("done")
     await client("wait")
-    path_graph = Path(tmpdir) / "graph.txt"
-    await client("graph", path_graph)
-    _check_graph(path_graph, COPY_GRAPH)
+    prefix_graph = Path(tmpdir) / "graph"
+    await client("graph", prefix_graph)
+    _check_graph(prefix_graph + ".txt", COPY_GRAPH)
```

### Comparing `stepup-1.0.0/tests/test_cascade.py` & `stepup-1.1.0/tests/test_cascade.py`

 * *Files 19% similar despite different names*

```diff
@@ -184,15 +184,14 @@
     assert cascade.get_products(key) == []
     assert cascade.format_str() == SINGLETON1_FORMAT_STR
     cascade.orphan("foo:one")
     check_cascade_unstructure(cascade)
     cascade.clean()
     check_cascade_unstructure(cascade)
     assert cascade.log == ["new foo:one", "act foo:one hello", "orphan foo:one", "clean foo:one"]
-    print(cascade.format_str())
     assert cascade.format_str() == SINGLETON2_FORMAT_STR
 
     # Validate sanity checking
     foo = Foo("one")
     with pytest.raises(TypeError):
         cascade.create(foo, None)
     cascade.create(foo, "root:")
@@ -423,15 +422,14 @@
     assert cascade.format_str() == CLEAN_CONSUMER2_FORMAT_STR
     cascade.orphan("foo:3")
     cascade.clean()
     assert "foo:0" not in cascade.nodes
     assert "foo:3" not in cascade.nodes
     assert "foo:1" not in cascade.nodes
     assert "foo:2" not in cascade.nodes
-    print(cascade.format_str())
     assert cascade.format_str() == FROM_SCRATCH_FORMAT_STR
 
 
 def test_recycle_consumers():
     """When an orphan node with consumers is recycled, the consumer relations remain."""
     cascade = LogCascade.from_scratch()
     cascade.create(Foo("0", other=10), "root:")
@@ -465,18 +463,58 @@
     assert "foo:0" not in cascade.nodes
 
 
 def test_cyclic1():
     cascade = LogCascade.from_scratch()
     cascade.create(Foo("0"), "vacuum:")
     cascade.create(Foo("1"), "foo:0")
-    with pytest.raises(GraphError):
-        cascade.supply("foo:1", "foo:0")
+    cascade.supply("foo:1", "foo:0")
+    assert "foo:1" in cascade.suppliers["foo:0"]
 
 
 def test_cyclic2():
     cascade = LogCascade.from_scratch()
     cascade.create(Foo("0"), "root:")
     cascade.create(Foo("1"), "root:")
     cascade.supply("foo:0", "foo:1")
     with pytest.raises(GraphError):
         cascade.supply("foo:1", "foo:0")
+
+
+def test_walk_consumers():
+    cascade = LogCascade.from_scratch()
+    cascade.create(Foo("0"), "root:")
+    cascade.create(Foo("1"), "root:")
+    cascade.create(Foo("2"), "root:")
+    cascade.create(Foo("3"), "root:")
+    cascade.supply("foo:0", "foo:1")
+    cascade.supply("foo:1", "foo:2")
+    cascade.supply("foo:1", "foo:3")
+    visited = set()
+    cascade.walk_consumers("foo:0", visited)
+    assert visited == {"foo:0", "foo:1", "foo:2", "foo:3"}
+    visited = set()
+    cascade.walk_consumers("foo:1", visited)
+    assert visited == {"foo:1", "foo:2", "foo:3"}
+    visited = set()
+    cascade.walk_consumers("foo:3", visited)
+    assert visited == {"foo:3"}
+
+
+def test_walk_suppliers():
+    cascade = LogCascade.from_scratch()
+    cascade.create(Foo("0"), "root:")
+    cascade.create(Foo("1"), "root:")
+    cascade.create(Foo("2"), "root:")
+    cascade.create(Foo("3"), "root:")
+    cascade.supply("foo:0", "foo:1")
+    cascade.supply("foo:1", "foo:2")
+    cascade.supply("foo:1", "foo:3")
+    visited = set()
+    cascade.walk_suppliers("foo:0", visited)
+    assert visited == {"foo:0"}
+    visited = set()
+    cascade.walk_suppliers("foo:1", visited)
+    assert visited == {"foo:0", "foo:1"}
+    visited = set()
+    cascade.walk_suppliers("foo:3", visited)
+    assert visited == {"foo:0", "foo:1", "foo:3"}
```

### Comparing `stepup-1.0.0/tests/test_cases.py` & `stepup-1.1.0/tests/test_cases.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         "deferred_glob2",
         "deferred_subdir",
         "env_vars",
         "env_vars_amend",
         "env_vars_path",
         "env_vars_subs",
         "env_vars_workdir",
-        "error_cyclic_early",
         "error_cyclic_late",
         "error_deferred_nonexisting",
         "error_env_var",
         "error_main_fails",
         "error_not_executable",
         "error_overlap_deferred",
         "error_static_dir",
@@ -59,14 +58,15 @@
         "here",
         "makedirs",
         "mkdir",
         "mkdir_error",
         "nodata",
         "noplan",
         "nostatic",
+        "not_cyclic",
         "optional_convert",
         "output_not_created",
         "pending",
         "permissions_file_rerun",
         "permissions_plan_rerun",
         "permissions_plan_restart",
         "permissions_step_rerun",
```

### Comparing `stepup-1.0.0/tests/test_hash.py` & `stepup-1.1.0/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/test_nglob.py` & `stepup-1.1.0/tests/test_nglob.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/test_rpc.py` & `stepup-1.1.0/tests/test_rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 import asyncio
 import sys
 
 import pytest
 import pytest_asyncio
 from path import Path
 
+from stepup.core.asyncio import pipe
 from stepup.core.exceptions import RPCError
-from stepup.core.rpc import pipe, serve_rpc, fmt_rpc_call, AsyncRPCClient, SocketSyncRPCClient
+from stepup.core.rpc import serve_rpc, fmt_rpc_call, AsyncRPCClient, SocketSyncRPCClient
 
 from core_common import EchoHandler
 
 
 @pytest_asyncio.fixture()
 async def pc():
     async with asyncio.timeout(5):
```

### Comparing `stepup-1.0.0/tests/test_scheduler.py` & `stepup-1.1.0/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/test_utils.py` & `stepup-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `stepup-1.0.0/tests/test_workflow.py` & `stepup-1.1.0/tests/test_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,26 +128,26 @@
             },
             {"c": "file", "p": 7, "s": FileState.STATIC.value},
             {"c": "file", "p": 8, "s": FileState.PENDING.value},
             {"c": "file", "p": 9, "s": FileState.PENDING.value},
             {"c": "file", "p": 10, "s": FileState.PENDING.value},
         ],
         "products": [[0, 0], [0, 1], [0, 2], [0, 3], [1, 4], [1, 5], [2, 6]],
-        "consumers": [[3, 2], [3, 4], [3, 5], [4, 2], [4, 6], [5, 2]],
+        "consumers": [[2, 6], [3, 2], [3, 4], [3, 5], [4, 2], [4, 6], [5, 2]],
         "strings": ["./", "sub/", "foo.txt", "sub/bar.txt"],
     }
     assert remove_hashes(wfs.unstructure()) == expected
     check_workflow_unstructure(wfs)
     assert wfs.get_step(step_key) == wfs.nodes[step_key]
     assert wfs.get_steps() == [wfs.nodes[step_key]]
-    assert wfs.used_directories == ["./", "sub/"]
+    assert wfs.dir_queue.get_nowait() == (False, "./")
     with pytest.raises(TypeError):
         wfs.get_step("file:./")
 
-    # Redefining the boot script is not allows
+    # Redefining the boot script is not allowed.
     with pytest.raises(GraphError):
         wfs.define_step(
             "root:", "cp foo.txt sub/bar.txt", inp_paths=["foo.txt"], out_paths=["sub/bar.txt"]
         )
     assert remove_hashes(wfs.unstructure()) == expected
 
     # Make the step RUNNING and test amending stuff.
@@ -206,20 +206,20 @@
             },
         ],
         "products": [[0, 0], [0, 1], [0, 2], [0, 3], [0, 4], [0, 5], [1, 6], [2, 7]],
         "consumers": [[3, 2], [3, 4], [3, 5], [4, 6], [5, 7]],
         "strings": ["./", "blub/", "sub/", "blub/foo.txt", "sub/bar.txt"],
     }
     workflow = Workflow.structure(state)
-    assert workflow.used_directories == ["./", "blub/", "sub/"]
+    check_workflow_unstructure(workflow)
 
 
 def test_simple_example(wfs: Workflow):
     # Create a runnable step and check the queue
-    assert wfs.queue.qsize() == 0
+    assert wfs.job_queue.qsize() == 0
     step_key = wfs.define_step(
         "root:", "cp foo.txt bar.txt", inp_paths=["foo.txt"], out_paths=["bar.txt"]
     )
     assert remove_hashes(wfs.unstructure()) == {
         "nodes": [
             {"c": "root", "v": "v1"},
             {"c": "vacuum"},
@@ -230,15 +230,15 @@
                 "s": StepState.PENDING.value,
             },
             {"c": "file", "p": 6, "s": FileState.STATIC.value},
             {"c": "file", "p": 7, "s": FileState.PENDING.value},
             {"c": "file", "p": 8, "s": FileState.PENDING.value},
         ],
         "products": [[0, 0], [0, 1], [0, 2], [0, 3], [1, 4], [2, 5]],
-        "consumers": [[3, 2], [3, 4], [3, 5], [4, 2]],
+        "consumers": [[2, 5], [3, 2], [3, 4], [3, 5], [4, 2]],
         "strings": ["./", "foo.txt", "bar.txt"],
     }
     wfs.declare_static("root:", ["foo.txt"])
     assert remove_hashes(wfs.unstructure()) == {
         "nodes": [
             {"c": "root", "v": "v1"},
             {"c": "vacuum"},
@@ -249,26 +249,26 @@
                 "s": StepState.QUEUED.value,
             },
             {"c": "file", "p": 6, "s": FileState.STATIC.value},
             {"c": "file", "p": 7, "s": FileState.STATIC.value},
             {"c": "file", "p": 8, "s": FileState.PENDING.value},
         ],
         "products": [[0, 0], [0, 1], [0, 2], [0, 3], [0, 4], [2, 5]],
-        "consumers": [[3, 2], [3, 4], [3, 5], [4, 2]],
+        "consumers": [[2, 5], [3, 2], [3, 4], [3, 5], [4, 2]],
         "strings": ["./", "foo.txt", "bar.txt"],
     }
     assert wfs.get_file_counters() == Counter({FileState.STATIC: 2, FileState.PENDING: 1})
     assert wfs.get_step_counters() == Counter({StepState.QUEUED: 1})
 
     # Verify things that should not be allowed
     with pytest.raises(GraphError):
         wfs.declare_static("root:", ["bar.txt"])
 
     # Mimic the runner, pretending to execute the step
-    assert wfs.queue.get_nowait() == RunJob(step_key, None)
+    assert wfs.job_queue.get_nowait() == RunJob(step_key, None)
     wfs.get_step(step_key).completed(wfs, True, StepHash(b"mockhash", b"zzz"))
     assert remove_hashes(wfs.unstructure()) == {
         "nodes": [
             {"c": "root", "v": "v1"},
             {"c": "vacuum"},
             {
                 "c": "step",
@@ -277,15 +277,15 @@
                 "s": StepState.SUCCEEDED.value,
             },
             {"c": "file", "p": 6, "s": FileState.STATIC.value},
             {"c": "file", "p": 7, "s": FileState.STATIC.value},
             {"c": "file", "p": 8, "s": FileState.BUILT.value},
         ],
         "products": [[0, 0], [0, 1], [0, 2], [0, 3], [0, 4], [2, 5]],
-        "consumers": [[3, 2], [3, 4], [3, 5], [4, 2]],
+        "consumers": [[2, 5], [3, 2], [3, 4], [3, 5], [4, 2]],
         "strings": ["./", "foo.txt", "bar.txt"],
     }
     assert wfs.get_file_counters() == Counter({FileState.STATIC: 2, FileState.BUILT: 1})
     assert wfs.get_step_counters() == Counter({StepState.SUCCEEDED: 1})
 
     # Verify things that should not be allowed
     with pytest.raises(GraphError):
@@ -307,15 +307,15 @@
                 "s": StepState.PENDING.value,
             },
             {"c": "file", "p": 6, "s": FileState.STATIC.value},
             {"c": "file", "p": 7, "s": FileState.STATIC.value},
             {"c": "file", "p": 8, "s": FileState.PENDING.value},
         ],
         "products": [[0, 0], [0, 1], [0, 2], [1, 3], [1, 4], [2, 5]],
-        "consumers": [[3, 2], [3, 4], [3, 5], [4, 2]],
+        "consumers": [[2, 5], [3, 2], [3, 4], [3, 5], [4, 2]],
         "strings": ["./", "foo.txt", "bar.txt"],
     }
     wfs.declare_static("root:", ["./"])
     assert remove_hashes(wfs.unstructure()) == {
         "nodes": [
             {"c": "root", "v": "v1"},
             {"c": "vacuum"},
@@ -326,15 +326,15 @@
                 "s": StepState.PENDING.value,
             },
             {"c": "file", "p": 6, "s": FileState.STATIC.value},
             {"c": "file", "p": 7, "s": FileState.STATIC.value},
             {"c": "file", "p": 8, "s": FileState.PENDING.value},
         ],
         "products": [[0, 0], [0, 1], [0, 2], [0, 3], [1, 4], [2, 5]],
-        "consumers": [[3, 2], [3, 4], [3, 5], [4, 2]],
+        "consumers": [[2, 5], [3, 2], [3, 4], [3, 5], [4, 2]],
         "strings": ["./", "foo.txt", "bar.txt"],
     }
     wfs.declare_static("root:", ["foo.txt"])
     assert remove_hashes(wfs.unstructure()) == {
         "nodes": [
             {"c": "root", "v": "v1"},
             {"c": "vacuum"},
@@ -345,15 +345,15 @@
                 "s": StepState.QUEUED.value,
             },
             {"c": "file", "p": 6, "s": FileState.STATIC.value},
             {"c": "file", "p": 7, "s": FileState.STATIC.value},
             {"c": "file", "p": 8, "s": FileState.PENDING.value},
         ],
         "products": [[0, 0], [0, 1], [0, 2], [0, 3], [0, 4], [2, 5]],
-        "consumers": [[3, 2], [3, 4], [3, 5], [4, 2]],
+        "consumers": [[2, 5], [3, 2], [3, 4], [3, 5], [4, 2]],
         "strings": ["./", "foo.txt", "bar.txt"],
     }
 
 
 def test_define_boot_input_static(wfs: Workflow):
     echo_key = wfs.define_step("root:", "echo", ["foo.txt"])
     (foo_key,) = wfs.declare_static("root:", ["foo.txt"])
@@ -543,25 +543,25 @@
 
 
 def test_define_queued_step_no_pool(wfp: Workflow):
     plan_key = "step:./plan.py"
     step_key = wfp.define_step(plan_key, "touch given", vol_paths=["given"])
     step = wfp.get_step(step_key)
     assert step.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
-    assert wfp.queue.get_nowait() == RunJob(step_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step_key, None)
 
 
 def test_define_queued_step_pool(wfp: Workflow):
     plan_key = "step:./plan.py"
     step_key = wfp.define_step(plan_key, "touch given", out_paths=["given"], pool="aa")
     step = wfp.get_step(step_key)
     assert step.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
-    assert wfp.queue.get_nowait() == RunJob(step_key, "aa")
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step_key, "aa")
 
 
 def test_define_queued_step_replay():
     state = {
         "nodes": [
             {"c": "root", "v": "v1"},
             {"c": "vacuum"},
@@ -574,184 +574,189 @@
                 "p": "bb",
                 "h": [b"mock", b"aaa"],
             },
             {"c": "file", "p": 7, "s": FileState.STATIC.value, "h": [b"foo", 0, 0.0, 0, 0]},
             {"c": "file", "p": 8, "s": FileState.BUILT.value, "h": [b"bar", 0, 0.0, 0, 0]},
         ],
         "products": [[0, 0], [0, 1], [0, 2], [0, 3], [0, 4], [3, 5]],
-        "consumers": [[2, 3], [2, 4], [2, 5], [4, 3]],
+        "consumers": [[2, 3], [2, 4], [2, 5], [3, 5], [4, 3]],
         "strings": ["./", "inp", "out"],
     }
     workflow = Workflow.structure(state)
     step_key = "step:cat < inp > out"
     step = workflow.get_step(step_key)
     assert step.get_state(workflow) == StepState.SUCCEEDED
     assert step.hash.digest == b"mock"
     assert step.hash.inp_digest == b"aaa"
     assert isinstance(step.recording, StepRecording)
     workflow.process_watcher_changes(set(), {Path("inp")})
     assert step.get_state(workflow) == StepState.QUEUED
     out = workflow.get_file("file:out")
     assert out.get_state(workflow) == FileState.PENDING
-    assert workflow.queue.get_nowait() == TryReplayJob(step_key, "bb")
+    assert workflow.job_queue.get_nowait() == TryReplayJob(step_key, "bb")
     step.replay_rest(workflow)
     assert workflow.unstructure() == state
     workflow.discard_recordings()
     assert step.hash is None
     assert step.recording is None
 
 
 def test_define_queued_step_replay_extra(wfp):
     # Prepare jobs for normal run
     plan_key = "step:./plan.py"
     plan = wfp.get_step(plan_key)
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
     wfp.declare_static(plan_key, ["ainp", "ainp2"])
-    wfp.queue_changed.clear()
+    wfp.job_queue_changed.clear()
     foo_key = wfp.define_step(plan_key, "foo > log", env_vars={"VAR": "VALUE"}, out_paths=["log"])
     foo = wfp.get_step(foo_key)
     assert foo.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue_changed.is_set()
+    assert wfp.job_queue_changed.is_set()
     bar_key = wfp.define_step(
         foo_key, "bar > spam", inp_paths=["log"], env_vars={"X": "Y"}, vol_paths=["spam"]
     )
     bar = wfp.get_step(bar_key)
     assert bar.get_state(wfp) == StepState.PENDING
     plan.completed(wfp, True, StepHash(b"plan_ok", b"zzz"))
 
     # Simulate run
     # foo
-    assert wfp.queue.get_nowait() == RunJob(foo_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(foo_key, None)
     wfp.amend_step(foo_key, inp_paths=["ainp"], out_paths=["aout"], vol_paths=["avol"])
     foo.completed(wfp, True, StepHash(b"foo_ok", b"zzz"))
     assert foo.get_state(wfp) == StepState.SUCCEEDED
-    print(foo.recording.steps_args)
     assert bar.get_state(wfp) == StepState.QUEUED
     # bar
-    assert wfp.queue.get_nowait() == RunJob(bar_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(bar_key, None)
     wfp.amend_step(bar_key, inp_paths=["ainp2"], out_paths=["aout2"], vol_paths=["avol2"])
     assert "file:ainp2" in wfp.suppliers[bar_key]
     bar.completed(wfp, True, StepHash(b"bar_ok", b"zzz"))
     assert bar.get_state(wfp) == StepState.SUCCEEDED
     check_workflow_unstructure(wfp)
     state1 = wfp.unstructure()
 
     # Make foo pending and check state
-    wfp.queue_changed.clear()
+    wfp.job_queue_changed.clear()
     foo.make_pending(wfp)
-    assert not wfp.queue_changed.is_set()
+    assert not wfp.job_queue_changed.is_set()
     assert foo.hash is not None
     assert isinstance(foo.recording, StepRecording)
     assert foo.get_state(wfp) == StepState.PENDING
     assert not foo.validate_amended
     assert wfp.get_file("file:log").get_state(wfp) == FileState.PENDING
     assert wfp.is_orphan(bar_key)
     assert bar.hash is not None
     assert isinstance(bar.recording, StepRecording)
     assert bar.get_state(wfp) == StepState.PENDING
     assert bar.validate_amended
     check_workflow_unstructure(wfp)
 
     # Simulate rerun
     foo.queue_if_appropriate(wfp)
-    assert wfp.queue_changed.is_set()
+    assert wfp.job_queue_changed.is_set()
     assert foo.get_state(wfp) == StepState.QUEUED
     assert bar.get_state(wfp) == StepState.PENDING
-    assert wfp.queue.get_nowait() == TryReplayJob(foo_key, None)
+    assert wfp.job_queue.get_nowait() == TryReplayJob(foo_key, None)
     foo.clean_before_run(wfp)
     foo.replay_amend(wfp)
     foo.replay_rest(wfp)
     assert foo.get_state(wfp) == StepState.SUCCEEDED
     assert bar.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == TryReplayJob(bar_key, None)
+    assert wfp.job_queue.get_nowait() == TryReplayJob(bar_key, None)
     bar.clean_before_run(wfp)
     bar.replay_amend(wfp)
     bar.replay_rest(wfp)
     assert bar.get_state(wfp) == StepState.SUCCEEDED
     check_workflow_unstructure(wfp)
     assert wfp.unstructure() == state1
 
 
 def test_replay_step_amended_orphaned_input(wfp):
     # Prepare jobs for normal run
     plan_key = "step:./plan.py"
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
     (ainp_key,) = wfp.declare_static(plan_key, ["ainp"])
-    wfp.queue_changed.clear()
+    wfp.job_queue_changed.clear()
     foo_key = wfp.define_step(plan_key, "foo > log", out_paths=["log"])
     foo = wfp.get_step(foo_key)
     assert foo.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue_changed.is_set()
+    assert foo.get_out_paths(wfp) == ["log"]
+    assert wfp.job_queue_changed.is_set()
 
     # Simulate run
-    assert wfp.queue.get_nowait() == RunJob(foo_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(foo_key, None)
     wfp.amend_step(foo_key, inp_paths=["ainp"], out_paths=["aout"], vol_paths=["avol"])
     foo.completed(wfp, True, StepHash(b"foo_ok", b"zzz"))
     assert foo.get_state(wfp) == StepState.SUCCEEDED
     check_workflow_unstructure(wfp)
     state1 = wfp.unstructure()
 
     # Make ainp orphan and check state
-    wfp.queue_changed.clear()
+    wfp.job_queue_changed.clear()
+    assert foo.get_out_paths(wfp) == ["aout", "log"]
     wfp.orphan(ainp_key)
-    assert not wfp.queue_changed.is_set()
+    assert foo.get_out_paths(wfp) == ["log"]
+    assert not wfp.job_queue_changed.is_set()
     assert foo.hash is not None
     assert isinstance(foo.recording, StepRecording)
     assert foo.get_state(wfp) == StepState.PENDING
     assert wfp.get_file("file:log").get_state(wfp) == FileState.PENDING
     check_workflow_unstructure(wfp)
 
     # Replay
     wfp.declare_static(plan_key, ["ainp"])
     foo.queue_if_appropriate(wfp)
-    assert wfp.queue_changed.is_set()
+    assert wfp.job_queue_changed.is_set()
     assert foo.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == TryReplayJob(foo_key, None)
+    assert wfp.job_queue.get_nowait() == TryReplayJob(foo_key, None)
     foo.clean_before_run(wfp)
     foo.replay_amend(wfp)
+    assert isinstance(foo.recording, StepRecording)
     foo.replay_rest(wfp)
     assert foo.get_state(wfp) == StepState.SUCCEEDED
+    assert not wfp.is_orphan("file:log")
+    assert wfp.get_file("file:log").get_state(wfp) == FileState.BUILT
     check_workflow_unstructure(wfp)
     assert wfp.unstructure() == state1
 
 
 def test_replay_ngm(wfp: Workflow):
     # Prepare jobs for normal run
     plan_key = "step:./plan.py"
     plan = wfp.get_step(plan_key)
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
-    wfp.queue_changed.clear()
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
+    wfp.job_queue_changed.clear()
     foo_key = wfp.define_step(plan_key, "foo")
     foo = wfp.get_step(foo_key)
     assert foo.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue_changed.is_set()
+    assert wfp.job_queue_changed.is_set()
     plan.completed(wfp, True, StepHash(b"plan_ok", b"ee"))
     assert plan.get_state(wfp) == StepState.SUCCEEDED
 
     # Simulate run
-    assert wfp.queue.get_nowait() == RunJob(foo_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(foo_key, None)
     ngm = NGlobMulti.from_patterns(["${*prefix}_data.txt"], subs={"prefix": "n???"})
     wfp.register_nglob(foo_key, ngm)
     foo.completed(wfp, True, StepHash(b"foo_ok", b"zzz"))
     assert foo.get_state(wfp) == StepState.SUCCEEDED
     check_workflow_unstructure(wfp)
 
     # Make foo pending and check state
-    wfp.queue_changed.clear()
+    wfp.job_queue_changed.clear()
     foo.make_pending(wfp)
-    assert not wfp.queue_changed.is_set()
+    assert not wfp.job_queue_changed.is_set()
     assert foo.hash is not None
     assert isinstance(foo.recording, StepRecording)
     assert foo.get_state(wfp) == StepState.PENDING
 
     # Replay
     foo.queue_if_appropriate(wfp)
-    assert wfp.queue_changed.is_set()
+    assert wfp.job_queue_changed.is_set()
     assert foo.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == TryReplayJob(foo_key, None)
+    assert wfp.job_queue.get_nowait() == TryReplayJob(foo_key, None)
     foo.clean_before_run(wfp)
     foo.replay_amend(wfp)
     foo.replay_rest(wfp)
     assert foo.get_state(wfp) == StepState.SUCCEEDED
     check_workflow_unstructure(wfp)
     assert len(foo.nglob_multis) == 1
     assert len(foo.nglob_multis[0].nglob_singles) == 1
@@ -762,30 +767,30 @@
 
 
 def test_amend_step(wfp: Workflow):
     plan_key = "step:./plan.py"
     step_key = wfp.define_step(plan_key, "blub > log", vol_paths=["log"])
     step = wfp.get_step(step_key)
     assert step.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
-    assert wfp.queue.get_nowait() == RunJob(step_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step_key, None)
     assert wfp.amend_step(step_key)
     assert not wfp.amend_step(
         step_key, inp_paths=["inp1", "inp2"], out_paths=["out3"], vol_paths=["vol4"]
     )
     assert step.amended_suppliers == {"file:inp1", "file:inp2"}
-    assert step.amended_products == {"file:out3", "file:vol4"}
+    assert step.amended_consumers == {"file:out3", "file:vol4"}
     step.completed(wfp, False, StepHash(b"fail", b"inp_fail"))
     step.set_state(wfp, StepState.PENDING)
     wfp.declare_static("step:./plan.py", ["inp1"])
     step.set_state(wfp, StepState.PENDING)
     wfp.declare_static("step:./plan.py", ["inp2"])
     step.set_state(wfp, StepState.QUEUED)
     assert wfp.get_products(step_key) == ["file:log", "file:out3", "file:vol4"]
-    assert wfp.queue.get_nowait() == ValidateAmendedJob(step_key, None)
+    assert wfp.job_queue.get_nowait() == ValidateAmendedJob(step_key, None)
 
 
 def test_define_queued_step_replay_amended():
     state = {
         "nodes": [
             {"c": "root", "v": "v1"},
             {"c": "vacuum"},
@@ -794,15 +799,15 @@
                 "c": "step",
                 "w": 10,
                 "m": "foo < inp > out 2> vol",
                 "s": StepState.SUCCEEDED.value,
                 "p": "bb",
                 "h": [b"boo", b"www"],
                 "as": [7],
-                "ao": [8, 9],
+                "ac": [8, 9],
             },
             {"c": "file", "p": 11, "s": FileState.STATIC.value, "h": [b"foo", 0, 0.0, 0, 0]},
             {"c": "file", "p": 12, "s": FileState.BUILT.value, "h": [b"bar", 0, 0.0, 0, 0]},
             {"c": "file", "p": 13, "s": FileState.BUILT.value, "h": [b"bar", 0, 0.0, 0, 0]},
             {"c": "file", "p": 14, "s": FileState.STATIC.value, "h": [b"foo", 0, 0.0, 0, 0]},
             {"c": "file", "p": 15, "s": FileState.BUILT.value, "h": [b"bar", 0, 0.0, 0, 0]},
             {"c": "file", "p": 16, "s": FileState.BUILT.value, "h": [b"bar", 0, 0.0, 0, 0]},
@@ -815,29 +820,43 @@
             [0, 4],
             [0, 7],
             [3, 5],
             [3, 6],
             [3, 8],
             [3, 9],
         ],
-        "consumers": [[2, 3], [2, 4], [2, 5], [2, 6], [2, 7], [2, 8], [2, 9], [4, 3], [7, 3]],
+        "consumers": [
+            [2, 3],
+            [2, 4],
+            [2, 5],
+            [2, 6],
+            [2, 7],
+            [2, 8],
+            [2, 9],
+            [3, 5],
+            [3, 6],
+            [3, 8],
+            [3, 9],
+            [4, 3],
+            [7, 3],
+        ],
         "strings": ["./", "inp", "out", "vol", "ainp", "aout", "avol"],
     }
     workflow = Workflow.structure(state)
     step_key = "step:foo < inp > out 2> vol"
     step = workflow.get_step(step_key)
     assert step.get_state(workflow) == StepState.SUCCEEDED
     assert step.hash.digest == b"boo"
     assert step.hash.inp_digest == b"www"
     assert isinstance(step.recording, StepRecording)
     workflow.process_watcher_changes(set(), {Path("ainp")})
     assert step.get_state(workflow) == StepState.QUEUED
     out = workflow.get_file("file:out")
     assert out.get_state(workflow) == FileState.PENDING
-    assert workflow.queue.get_nowait() == TryReplayJob(step_key, "bb")
+    assert workflow.job_queue.get_nowait() == TryReplayJob(step_key, "bb")
     step.clean_before_run(workflow)
     assert "file:ainp" not in workflow.get_suppliers(step_key, include_orphans=True)
     assert workflow.is_orphan("file:aout")
     assert workflow.is_orphan("file:avol")
     step.replay_amend(workflow)
     assert "file:ainp" in workflow.get_suppliers(step_key, include_orphans=True)
     assert not workflow.is_orphan("file:aout")
@@ -907,54 +926,54 @@
     assert wfp.get_file("file:cc5_foo.txt").get_state(wfp) == FileState.MISSING
     assert "file:bb7_bar.txt" not in wfp.nodes
     assert ngm.files() == ("aa1_bar.txt", "aa1_foo.txt", "bb7_bar.txt", "bb7_foo.txt")
     assert ngm.nglob_singles[0].results == {("aa1",): {"aa1_foo.txt"}, ("bb7",): {"bb7_foo.txt"}}
     assert ngm.nglob_singles[1].results == {("aa1",): {"aa1_bar.txt"}, ("bb7",): {"bb7_bar.txt"}}
 
 
-def test_watcher_added_static_orphan(wfp):
+def test_watcher_updated_static_orphan(wfp):
     plan_key = "step:./plan.py"
     wfp.declare_static(plan_key, ["foo.txt"])
     wfp.orphan("file:foo.txt")
     wfp.process_watcher_changes({}, {"foo.txt"})
 
 
 def test_watcher_deleted_static_orphan(wfp):
     plan_key = "step:./plan.py"
     wfp.declare_static(plan_key, ["foo.txt"])
     wfp.orphan("file:foo.txt")
     wfp.process_watcher_changes({"foo.txt"}, {})
 
 
-def test_watcher_added_built_orphan(wfp):
+def test_watcher_updated_built_orphan(wfp):
     plan_key = "step:./plan.py"
     step_key = wfp.define_step(plan_key, "touch foo.txt", out_paths=["foo.txt"])
     wfp.orphan(step_key)
     wfp.process_watcher_changes({}, {"foo.txt"})
 
 
 def test_watcher_deleted_built_orphan(wfp):
     plan_key = "step:./plan.py"
     step_key = wfp.define_step(plan_key, "touch foo.txt", out_paths=["foo.txt"])
     wfp.orphan(step_key)
     wfp.process_watcher_changes({"foo.txt"}, {})
 
 
 def test_directory_usage(wfs: Workflow):
-    assert len(wfs._used_directories) == 0
+    assert wfs.dir_queue.empty()
     wfs.declare_static("root:", ["./"])
-    assert wfs.used_directories == ["./"]
+    assert wfs.dir_queue.get_nowait() == (False, "./")
     wfs.declare_static("root:", ["foo.txt"])
-    assert wfs.used_directories == ["./"]
+    assert wfs.dir_queue.empty()
     wfs.orphan("file:foo.txt")
-    assert wfs.used_directories == ["./"]
+    assert wfs.dir_queue.empty()
     wfs.orphan("file:./")
-    assert wfs.used_directories == ["./"]
+    assert wfs.dir_queue.empty()
     wfs.clean()
-    assert len(wfs._used_directories) == 0
+    assert wfs.dir_queue.get_nowait() == (True, "./")
 
 
 def test_parent_must_exist():
     # Load workflow from graph with files lacking parents. This should raise an error
     state = {
         "nodes": [
             {"c": "root", "v": "v1"},
@@ -994,27 +1013,28 @@
 def test_to_be_deleted(wfp: Workflow):
     plan_key = "step:./plan.py"
     wfp.declare_static(plan_key, ["static"])
     wfp.define_step(plan_key, "blub1", out_paths=["built", "gone"])
     wfp.define_step(plan_key, "blub2", vol_paths=["volatile"])
     wfp.define_step(plan_key, "blub3", out_paths=["pending"])
     wfp.define_step(plan_key, "mkdir sub", out_paths=["sub/"])
-    gone_file_hash = FileHash(b"m", 0, 0.0, 0, 0)
+    gone_file_hash = FileHash(b"mockg", 0, 0.0, 0, 0)
     wfp.set_file_hash("gone", gone_file_hash)
     built_file_hash = FileHash(b"mockb", 0, 0.0, 0, 0)
     wfp.set_file_hash("built", built_file_hash)
     sub_file_hash = FileHash(b"d", 0, 0.0, 0, 0)
     wfp.set_file_hash("sub/", sub_file_hash)
     wfp.get_step("step:blub1").completed(wfp, True, StepHash(b"aaa", b"zzz"))
     wfp.orphan(plan_key)
     assert wfp.to_be_deleted == []
     assert "step:./plan.py" in wfp.step_states
     wfp.clean()
     assert wfp.to_be_deleted == [
         ("built", built_file_hash),
+        ("gone", gone_file_hash),
         ("sub/", sub_file_hash),
         ("volatile", None),
     ]
     assert "step:./plan.py" not in wfp.step_states
 
 
 def test_watcher_deleted(wfp):
@@ -1043,44 +1063,44 @@
     assert prr_file.get_state(wfp) == FileState.BUILT
     prr_file.watcher_deleted(wfp)
     assert prr_file.get_state(wfp) == FileState.PENDING
     assert step1.get_state(wfp) == StepState.PENDING
     assert step2.get_state(wfp) == StepState.PENDING
 
 
-def test_watcher_added(wfp):
+def test_watcher_updated(wfp):
     plan_key = "step:./plan.py"
     (tst_key,) = wfp.declare_static("root:", ["tst"])
     cat_key = wfp.define_step(plan_key, "cat tst", ["tst"])
     step1_key = wfp.define_step(plan_key, "bla1", out_paths=["prr"])
     step2_key = wfp.define_step(plan_key, "bla2", ["prr"])
 
     # Static
     cat = wfp.get_step(cat_key)
     cat.completed(wfp, True, StepHash(b"sfdsafds", b"zzz"))
     tst_file = wfp.get_file(tst_key)
     tst_file.watcher_deleted(wfp)
     assert tst_file.get_state(wfp) == FileState.MISSING
     assert cat.get_state(wfp) == StepState.PENDING
-    tst_file.watcher_added(wfp)
+    tst_file.watcher_updated(wfp)
     assert tst_file.get_state(wfp) == FileState.STATIC
     assert cat.get_state(wfp) == StepState.PENDING
 
     # Built
     prr_key = "file:prr"
     prr_file = wfp.get_file(prr_key)
     assert prr_file.get_state(wfp) == FileState.PENDING
-    prr_file.watcher_added(wfp)
+    prr_file.watcher_updated(wfp)
     assert prr_file.get_state(wfp) == FileState.PENDING
     step1 = wfp.get_step(step1_key)
     step1.completed(wfp, True, StepHash(b"11", b"zzz"))
     step2 = wfp.get_step(step2_key)
     step2.completed(wfp, False, StepHash(b"fail", b"inp_fail"))
     assert prr_file.get_state(wfp) == FileState.BUILT
-    prr_file.watcher_added(wfp)
+    prr_file.watcher_updated(wfp)
     assert prr_file.get_state(wfp) == FileState.PENDING
     assert step1.get_state(wfp) == StepState.PENDING
     assert step2.get_state(wfp) == StepState.PENDING
 
 
 def test_step_recycle(wfp):
     plan_key = "step:./plan.py"
@@ -1100,16 +1120,16 @@
 
 def test_dissolve(wfp):
     # Simulate use of pattern in and successful execution of plan.py.
     plan_key = "step:./plan.py"
     wfp.declare_static(plan_key, ["sub/"])
     wfp.declare_static(plan_key, ["sub/static.txt"])
     wfp.register_nglob(plan_key, NGlobMulti.from_patterns(["*.txt"]))
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
-    assert wfp.queue.qsize() == 0
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.qsize() == 0
     plan = wfp.get_step(plan_key)
     plan.completed(wfp, True, StepHash(b"sth", b"zzz"))
     assert plan.get_state(wfp) == StepState.SUCCEEDED
     assert plan.hash.digest == b"sth"
     assert isinstance(plan.recording, StepRecording)
 
     # Check effect of anticipate_everthing_changed
@@ -1184,31 +1204,32 @@
 
 
 def test_amended_env_vars(wfp):
     plan_key = "step:./plan.py"
     step_key = wfp.define_step(plan_key, "prog1", env_vars=["egg"])
     step = wfp.get_step(step_key)
     assert step.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
-    assert wfp.queue.get_nowait() == RunJob(step_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step_key, None)
     wfp.amend_step(step_key, env_vars=["foo", "egg"])
     wfp.amend_step(step_key, env_vars=["foo", "bar"])
     assert step.initial_env_vars == {"egg"}
     assert step.amended_env_vars == {"foo", "bar"}
     check_workflow_unstructure(wfp)
 
 
-def test_cyclic_amend_static(wfp):
+def test_acyclic_amend_static(wfp):
     plan_key = "step:./plan.py"
     plan = wfp.get_step(plan_key)
     assert plan.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
     wfp.declare_static(plan_key, ["static.txt"])
-    with pytest.raises(GraphError):
-        wfp.amend_step(plan_key, inp_paths=["static.txt"])
+    wfp.amend_step(plan_key, inp_paths=["static.txt"])
+    assert plan.get_inp_paths(wfp) == ["./", "plan.py", "static.txt"]
+    assert plan.get_static_paths(wfp) == ["static.txt"]
 
 
 def test_cyclic_two_steps(wfp):
     plan_key = "step:./plan.py"
     wfp.define_step(plan_key, "cat first > second", inp_paths=["first"], out_paths=["second"])
     with pytest.raises(GraphError):
         wfp.define_step(plan_key, "cat second > first", inp_paths=["second"], out_paths=["first"])
@@ -1226,20 +1247,20 @@
     step2 = wfp.get_step(step2_key)
     assert step2.get_mandatory(wfp) == Mandatory.YES
     assert step2.get_state(wfp) == StepState.PENDING
     assert step1.get_mandatory(wfp) == Mandatory.IMPLIED
     assert step1.get_state(wfp) == StepState.QUEUED
 
     # Simulate scheduler
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
-    assert wfp.queue.get_nowait() == RunJob(step1_key, None)
-    assert wfp.queue.qsize() == 0
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step1_key, None)
+    assert wfp.job_queue.qsize() == 0
     step1.completed(wfp, True, StepHash(b"sth", b"zzz"))
     assert step2.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == RunJob(step2_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step2_key, None)
 
     # Simulate watcher: orphan mandatory step
     wfp.orphan(step2_key)
     assert step1.get_mandatory(wfp) == Mandatory.NO
     assert step1.get_state(wfp) == StepState.SUCCEEDED
 
     # Run clean
@@ -1267,23 +1288,23 @@
     assert step3.get_state(wfp) == StepState.PENDING
     assert step2.get_mandatory(wfp) == Mandatory.IMPLIED
     assert step2.get_state(wfp) == StepState.PENDING
     assert step1.get_mandatory(wfp) == Mandatory.IMPLIED
     assert step1.get_state(wfp) == StepState.QUEUED
 
     # Simulate scheduler
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
-    assert wfp.queue.get_nowait() == RunJob(step1_key, None)
-    assert wfp.queue.qsize() == 0
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step1_key, None)
+    assert wfp.job_queue.qsize() == 0
     step1.completed(wfp, True, StepHash(b"sth", b"zzz"))
     assert step2.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == RunJob(step2_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step2_key, None)
     step2.completed(wfp, True, StepHash(b"sth", b"zzz"))
     assert step3.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.get_nowait() == RunJob(step3_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step3_key, None)
     step3.completed(wfp, True, StepHash(b"sth", b"zzz"))
 
     # Simulate watcher: orphan middle step
     wfp.orphan(step2_key)
     assert step1.get_mandatory(wfp) == Mandatory.NO
     assert step1.get_state(wfp) == StepState.SUCCEEDED
     assert step2.get_mandatory(wfp) == Mandatory.IMPLIED
@@ -1371,19 +1392,19 @@
     assert wfp.get_file("file:static/foo/").get_state(wfp) == FileState.STATIC
     assert wfp.get_file("file:static/foo/bar.txt").get_state(wfp) == FileState.STATIC
     assert "static/" in dg.ngm.files()
     assert "static/foo/" in dg.ngm.files()
     assert "static/foo/bar.txt" in dg.ngm.files()
 
     # Simulate the execution of the steps
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
     plan = wfp.get_step(plan_key)
     plan.completed(wfp, True, StepHash(b"sth", b"zzz"))
-    assert wfp.queue.get_nowait() == RunJob(step_key, None)
-    assert wfp.queue.qsize() == 0
+    assert wfp.job_queue.get_nowait() == RunJob(step_key, None)
+    assert wfp.job_queue.qsize() == 0
     step = wfp.get_step(step_key)
     step.completed(wfp, True, StepHash(b"sth", b"zzz"))
     check_workflow_unstructure(wfp)
 
     # Check the recording
     assert plan.recording.deferred_glob_args == [["static/**"]]
     assert step.recording.deferred_glob_args == []
@@ -1401,15 +1422,15 @@
     assert "static/foo/bar.txt" not in dg.ngm.files()
 
     # make the plan pending and check recording
     plan.make_pending(wfp)
     assert wfp.is_orphan(dg_key)
     plan.queue_if_appropriate(wfp)
     assert plan.get_state(wfp) == StepState.QUEUED
-    assert wfp.queue.qsize() == 1
+    assert wfp.job_queue.qsize() == 1
     assert dg_key in wfp.nodes
 
 
 def test_deferred_glob_two_matches(wfp):
     plan_key = "step:./plan.py"
     wfp.defer_glob(plan_key, ["*.md"])
     wfp.defer_glob(plan_key, ["README.*"])
@@ -1550,16 +1571,16 @@
 
 def test_replay_amend_orphan_inputs(wfp):
     plan_key = "step:./plan.py"
     step_key = wfp.define_step(plan_key, "echo foo > bar", inp_paths=["foo"], out_paths=["bar"])
     (foo_key,) = wfp.declare_static(plan_key, ["foo"])
 
     # Simulate running the step
-    assert wfp.queue.get_nowait() == RunJob(plan_key, None)
-    assert wfp.queue.get_nowait() == RunJob(step_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(plan_key, None)
+    assert wfp.job_queue.get_nowait() == RunJob(step_key, None)
     step = wfp.get_step(step_key)
     wfp.amend_step(step_key, env_vars=["AAA"], vol_paths=["bbb"])
     step.completed(wfp, True, StepHash(b"step_ok", b"zzz"))
     assert step.get_state(wfp) == StepState.SUCCEEDED
 
     # Make the static input orphan and redefine the step
     wfp.orphan(foo_key)
```

