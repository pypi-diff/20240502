# Comparing `tmp/keri-1.2.0.dev1.tar.gz` & `tmp/keri-1.2.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keri-1.2.0.dev1.tar", last modified: Sat Apr 13 22:53:57 2024, max compression
+gzip compressed data, was "keri-1.2.0.dev2.tar", last modified: Thu May  2 02:06:53 2024, max compression
```

## Comparing `keri-1.2.0.dev1.tar` & `keri-1.2.0.dev2.tar`

### file list

```diff
@@ -1,210 +1,214 @@
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.087839 keri-1.2.0.dev1/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/LICENSE
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-04-13 22:53:57.087558 keri-1.2.0.dev1/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2457 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/README.md
--rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-04-13 22:53:57.087881 keri-1.2.0.dev1/setup.cfg
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4061 2024-04-13 22:43:05.000000 keri-1.2.0.dev1/setup.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.058806 keri-1.2.0.dev1/src/
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.061585 keri-1.2.0.dev1/src/keri/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       83 2024-04-13 22:43:05.000000 keri-1.2.0.dev1/src/keri/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.067066 keri-1.2.0.dev1/src/keri/app/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    37921 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/agenting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/apping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/challenging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.067447 keri-1.2.0.dev1/src/keri/app/cli/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.070708 keri-1.2.0.dev1/src/keri/app/cli/commands/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.071277 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/respond.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1847 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/clean.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.071517 keri-1.2.0.dev1/src/keri/app/cli/commands/contacts/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/contacts/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2662 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/contacts/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2074 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/decrypt.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.071877 keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9425 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/confirm.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4076 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/request.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.072085 keri-1.2.0.dev1/src/keri/app/cli/commands/did/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/did/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/did/generate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.072536 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/add.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ends/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/escrow.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3744 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7156 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5479 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/init.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4897 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/interact.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.073878 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/admit.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      529 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/agree.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      470 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/apply.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/grant.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9870 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      564 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/offer.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/spurn.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/kevers.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.074169 keri-1.2.0.dev1/src/keri/app/cli/commands/local/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/local/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/local/watch.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.074531 keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/debug.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/update.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.074988 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1938 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1785 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/run.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1806 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/show.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6153 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/migrate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.076326 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3045 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/continue.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6698 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/interact.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30790 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/notice.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10190 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/shell.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4891 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/update.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      440 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/nonce.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.076781 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/clean.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/resolve.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.077356 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/remove.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2549 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/set.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/query.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2161 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/rename.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/rollback.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8964 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/saidify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      519 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/salt.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/sign.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.077559 keri-1.2.0.dev1/src/keri/app/cli/commands/ssh/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ssh/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/ssh/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-04-05 21:44:00.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/time.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.078118 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10874 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/create.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.078575 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/vc/revoke.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2940 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1251 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/version.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.079117 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4073 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/authenticate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3047 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4836 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/start.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4655 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/cli/commands/witness/submit.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.080134 keri-1.2.0.dev1/src/keri/app/cli/common/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/common/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/common/config.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3887 2024-04-12 20:57:42.000000 keri-1.2.0.dev1/src/keri/app/cli/common/displaying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3357 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/cli/common/existing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/common/incepting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/common/rotating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/cli/common/terming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/cli/kli.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8151 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/configing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/connecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10242 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/delegating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24676 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/directing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    18769 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/app/forwarding.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26643 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/grouping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   124687 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/habbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8702 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/httping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    41665 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/app/indirecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    73656 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/app/keeping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/notifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    23097 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/oobiing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/querying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/signaling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-04-05 21:44:00.000000 keri-1.2.0.dev1/src/keri/app/signing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/app/specing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/app/storing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.081882 keri-1.2.0.dev1/src/keri/core/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      566 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/core/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   202289 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/coring.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    37818 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/core/counting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   306732 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34157 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/core/indexing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    58295 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/parsing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26820 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/routing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/core/scheming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    82877 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/serdering.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    35338 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/core/signing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    25640 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/core/structing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.083045 keri-1.2.0.dev1/src/keri/db/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/db/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   127663 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/db/basing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    77257 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/db/dbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9359 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/db/escrowing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/db/koming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.083284 keri-1.2.0.dev1/src/keri/db/migrations/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/db/migrations/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2861 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/db/migrations/rekey_habs.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    59458 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/db/subing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.084187 keri-1.2.0.dev1/src/keri/demo/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/demo/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2790 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/demo/demo_bob.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2806 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/demo/demo_eve.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/demo/demo_kev.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2831 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/demo/demo_sam.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/demo/demoing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.084778 keri-1.2.0.dev1/src/keri/end/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/end/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24903 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/end/ending.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/end/priming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.085027 keri-1.2.0.dev1/src/keri/help/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      619 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/help/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12483 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/help/helping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    27047 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/kering.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.085241 keri-1.2.0.dev1/src/keri/peer/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/peer/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    19698 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/peer/exchanging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.085875 keri-1.2.0.dev1/src/keri/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-04-05 21:44:00.000000 keri-1.2.0.dev1/src/keri/vc/protocoling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2528 2024-04-12 21:26:40.000000 keri-1.2.0.dev1/src/keri/vc/proving.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.2.0.dev1/src/keri/vc/walleting.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.086749 keri-1.2.0.dev1/src/keri/vdr/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.2.0.dev1/src/keri/vdr/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34327 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/vdr/credentialing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    84668 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/vdr/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    14424 2024-04-13 22:22:16.000000 keri-1.2.0.dev1/src/keri/vdr/verifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    35856 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/src/keri/vdr/viring.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.087292 keri-1.2.0.dev1/src/keri.egg-info/
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5932 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/SOURCES.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/dependency_links.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/entry_points.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.2.0.dev1/src/keri.egg-info/not-zip-safe
--rw-r--r--   0 pfeairheller   (501) staff       (20)      314 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/requires.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-04-13 22:53:57.000000 keri-1.2.0.dev1/src/keri.egg-info/top_level.txt
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-13 22:53:57.086879 keri-1.2.0.dev1/tests/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    28418 2024-04-10 20:11:23.000000 keri-1.2.0.dev1/tests/test_kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.908031 keri-1.2.0.dev2/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/LICENSE
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-02 02:06:53.907755 keri-1.2.0.dev2/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2457 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/README.md
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-05-02 02:06:53.908078 keri-1.2.0.dev2/setup.cfg
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4061 2024-05-02 01:55:35.000000 keri-1.2.0.dev2/setup.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.880052 keri-1.2.0.dev2/src/
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.882593 keri-1.2.0.dev2/src/keri/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       83 2024-05-02 01:55:35.000000 keri-1.2.0.dev2/src/keri/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.887565 keri-1.2.0.dev2/src/keri/app/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    37921 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/agenting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/apping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/challenging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.887977 keri-1.2.0.dev2/src/keri/app/cli/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.890932 keri-1.2.0.dev2/src/keri/app/cli/commands/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.891427 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/respond.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1847 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/clean.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.891660 keri-1.2.0.dev2/src/keri/app/cli/commands/contacts/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/contacts/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2662 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/contacts/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2074 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/decrypt.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.892008 keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9425 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/confirm.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4076 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/request.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.892196 keri-1.2.0.dev2/src/keri/app/cli/commands/did/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/did/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/did/generate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.892638 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/add.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/escrow.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3744 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7156 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5479 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/init.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4897 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/interact.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.893724 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/admit.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      531 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/agree.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      472 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/apply.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/grant.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10073 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      566 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/offer.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/spurn.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/kevers.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.893945 keri-1.2.0.dev2/src/keri/app/cli/commands/local/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/local/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/local/watch.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.894337 keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/debug.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/update.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.894865 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1938 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1785 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/run.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1806 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/show.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6153 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.896336 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3045 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/continue.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6698 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/interact.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30790 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/notice.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10190 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/shell.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4891 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/update.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      442 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/nonce.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.896772 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/clean.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/resolve.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.897186 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/remove.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2549 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/set.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-05-02 01:19:02.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/query.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2161 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/rename.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/rollback.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8964 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/saidify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      519 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/salt.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/sign.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.897379 keri-1.2.0.dev2/src/keri/app/cli/commands/ssh/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ssh/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ssh/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-04-05 21:44:00.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/time.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.898001 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10874 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/create.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.898488 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/revoke.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2940 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1251 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/version.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.898763 keri-1.2.0.dev2/src/keri/app/cli/commands/watcher/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       78 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/watcher/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4507 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/watcher/add.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.899448 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4187 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/authenticate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3047 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4836 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/start.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4655 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/submit.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.900487 keri-1.2.0.dev2/src/keri/app/cli/common/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/common/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/common/config.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3887 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/common/displaying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3357 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/common/existing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/cli/common/incepting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/common/rotating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/common/terming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-04-22 16:39:31.000000 keri-1.2.0.dev2/src/keri/app/cli/kli.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8151 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/configing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/connecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10242 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/delegating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    24676 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/directing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    18769 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/forwarding.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26643 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/grouping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   124689 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/habbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8702 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/httping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    41828 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/indirecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    73656 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/keeping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/notifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26860 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/oobiing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/querying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/signaling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-04-05 21:44:00.000000 keri-1.2.0.dev2/src/keri/app/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/specing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/storing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.902315 keri-1.2.0.dev2/src/keri/core/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      507 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/core/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   201749 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/coring.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    38577 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/counting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   306428 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/core/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34501 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/indexing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    58321 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/core/parsing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26820 2024-04-29 23:03:37.000000 keri-1.2.0.dev2/src/keri/core/routing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/core/scheming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    82877 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/core/serdering.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    35338 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/core/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    15364 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/streaming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    25641 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/structing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.903615 keri-1.2.0.dev2/src/keri/db/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/db/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   127858 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/db/basing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    77257 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/db/dbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9246 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/db/escrowing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/db/koming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.903848 keri-1.2.0.dev2/src/keri/db/migrations/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/db/migrations/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2861 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/db/migrations/rekey_habs.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    59458 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/db/subing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.904643 keri-1.2.0.dev2/src/keri/demo/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/demo/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2790 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/demo/demo_bob.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2806 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/demo/demo_eve.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/demo/demo_kev.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2831 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/demo/demo_sam.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/demo/demoing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.905087 keri-1.2.0.dev2/src/keri/end/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/end/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    25038 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/end/ending.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/end/priming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.905329 keri-1.2.0.dev2/src/keri/help/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      619 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/help/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12484 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/help/helping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    27254 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.905527 keri-1.2.0.dev2/src/keri/peer/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/peer/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    19698 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/peer/exchanging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.906195 keri-1.2.0.dev2/src/keri/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-04-05 21:44:00.000000 keri-1.2.0.dev2/src/keri/vc/protocoling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2528 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/vc/proving.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/vc/walleting.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.906953 keri-1.2.0.dev2/src/keri/vdr/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/vdr/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34327 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/vdr/credentialing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    84698 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/vdr/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    14424 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/vdr/verifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    35856 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/vdr/viring.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.907459 keri-1.2.0.dev2/src/keri.egg-info/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6046 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/SOURCES.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/dependency_links.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/entry_points.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.2.0.dev2/src/keri.egg-info/not-zip-safe
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      314 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/requires.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/top_level.txt
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.907088 keri-1.2.0.dev2/tests/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    28418 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/tests/test_kering.py
```

### Comparing `keri-1.2.0.dev1/LICENSE` & `keri-1.2.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/PKG-INFO` & `keri-1.2.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.2.0.dev1
+Version: 1.2.0.dev2
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
```

### Comparing `keri-1.2.0.dev1/README.md` & `keri-1.2.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/setup.py` & `keri-1.2.0.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from glob import glob
 from os.path import basename
 from os.path import splitext
 
 from setuptools import find_packages, setup
 setup(
     name='keri',
-    version='1.2.0-dev1',  # also change in src/keri/__init__.py
+    version='1.2.0-dev2',  # also change in src/keri/__init__.py
     license='Apache Software License 2.0',
     description='Key Event Receipt Infrastructure',
     long_description="KERI Decentralized Key Management Infrastructure",
     author='Samuel M. Smith',
     author_email='smith.samuel.m@gmail.com',
     url='https://github.com/WebOfTrust/keripy',
     packages=find_packages('src'),
```

### Comparing `keri-1.2.0.dev1/src/keri/app/agenting.py` & `keri-1.2.0.dev2/src/keri/app/agenting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/apping.py` & `keri-1.2.0.dev2/src/keri/app/apping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/challenging.py` & `keri-1.2.0.dev2/src/keri/app/challenging.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/generate.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/respond.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/respond.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/challenge/verify.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/verify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/clean.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/contacts/list.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/contacts/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/decrypt.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/decrypt.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/confirm.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/confirm.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/delegate/request.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/request.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/did/generate.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/did/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ends/add.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ends/add.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ends/export.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ends/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ends/list.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ends/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/escrow.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/escrow.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/export.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/incept.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/init.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/interact.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/admit.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/admit.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/agree.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/offer.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 keri.app.cli.commands module
 
 """
 import argparse
 
 from hio.base import doing
 
-from keri.core import coring
+from keri.core import signing
 
-parser = argparse.ArgumentParser(description='Reply to IPEX offer message acknowledged willingness to accept offered '
-                                             'credential')
+parser = argparse.ArgumentParser(description='Reply to IPEX apply message or initiate an IPEX exchange with an offer'
+                                             ' for a credential with certain characteristics')
 parser.set_defaults(handler=lambda args: handler(args))
 
 
 def handler(_):
     return [doing.doify(nonce)]
 
 
 def nonce(tymth, tock=0.0):
     """ nonce
     """
     _ = (yield tock)
 
-    print(coring.randomNonce())
+    print(signing.Salter().qb64)
```

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/grant.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/grant.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/join.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/join.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/list.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 keri.kli.commands module
 
 """
 
 import argparse
 import datetime
 import os
+import json
 import sys
 
 from hio import help
 from hio.base import doing
 
 from keri import kering
 from keri.app import indirecting, notifying, connecting
@@ -195,14 +196,20 @@
             f"    Status: Issued {terming.Colors.OKGREEN}{terming.Symbols.CHECKMARK}{terming.Colors.ENDC}")
         print(f"    Issued by {sad['i']}")
         print(f"    Issued on {iss['dt']}")
         print(f"    Already responded? {accepted}")
         if response is not None:
             print(f"    Response: {responseType} ({response.qb64})")
 
+        if self.verbose:
+            bsad = json.dumps(sad, indent=2)
+            print("    Full Credential:")
+            for line in bsad.splitlines():
+                print(f"\t{line}")
+
     def apply(self, note, exn, pathed):
         pass
 
     def offer(self, note, exn, pathed):
         pass
 
     def agree(self, note, exn, pathed):
```

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/offer.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/salt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- encoding: utf-8 -*-
 """
 keri.app.cli.commands module
 
 """
 import argparse
 
+import pysodium
 from hio.base import doing
 
-from keri.core import coring
+from keri import core
 
-parser = argparse.ArgumentParser(description='Reply to IPEX apply message or initiate an IPEX exchange with an offer'
-                                             ' for a credential with certain characteristics')
+parser = argparse.ArgumentParser(description='Print a new random passcode')
 parser.set_defaults(handler=lambda args: handler(args))
 
 
 def handler(_):
-    return [doing.doify(nonce)]
+    return [doing.doify(passcode)]
 
 
-def nonce(tymth, tock=0.0):
-    """ nonce
+def passcode(tymth, tock=0.0):
+    """ Command line version handler
     """
     _ = (yield tock)
 
-    print(coring.randomNonce())
+    print(core.Salter(raw=pysodium.randombytes(pysodium.crypto_sign_SEEDBYTES)).qb64)
```

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ipex/spurn.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/spurn.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/kevers.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/kevers.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/list.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/local/watch.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/local/watch.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/debug.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/debug.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/mailbox/update.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/list.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/run.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/run.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/migrate/show.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/show.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/migrate.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/continue.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/continue.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/demo.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/incept.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/interact.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/join.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/join.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/notice.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/notice.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/rotate.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/rotate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/shell.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/shell.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/multisig/update.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/clean.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/clean.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/generate.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/oobi/resolve.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/resolve.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/generate.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/remove.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/remove.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/passcode/set.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/set.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/query.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/rename.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/rename.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/rollback.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/rollback.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/rotate.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/rotate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/saidify.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/saidify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/sign.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/sign.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/ssh/export.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/ssh/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/status.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/create.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/create.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/export.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/list.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/incept.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/list.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/registry/status.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/vc/revoke.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/revoke.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/verify.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/verify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/version.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/witness/authenticate.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/witness/authenticate.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,18 @@
                     required=False, default="")
 parser.add_argument('--passcode', '-p', help='22 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--witness", '-w', help="the witness AID or alias to authenticate against", required=True)
 
 
 def auth(args):
-    """ Command line list credential registries handler
+    """ Command line handler for authenticating  against a witness by retrieving the secret or a TOTP
+
+    Parameters:
+        args(Namespace): parsed command line arguments
 
     """
 
     ed = AuthDoer(name=args.name,
                   alias=args.alias,
                   base=args.base,
                   bran=args.bran,
@@ -61,15 +64,15 @@
             if len(wit) != 1:
                 raise ValueError(f"invalid recipient {witness}")
             wit = wit[0]['id']
 
         if not wit:
             raise ValueError(f"unknown witness {witness}")
 
-        self.witness = witness
+        self.witness = wit
         self.clienter = httping.Clienter()
         doers = [doing.doify(self.authDo), self.clienter]
 
         super(AuthDoer, self).__init__(doers=doers)
 
     def authDo(self, tymth, tock=0.0):
         """ Export credential from store and any related material
```

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/witness/demo.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/witness/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/witness/start.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/witness/start.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/commands/witness/submit.py` & `keri-1.2.0.dev2/src/keri/app/cli/commands/witness/submit.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/common/config.py` & `keri-1.2.0.dev2/src/keri/app/cli/common/config.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/common/displaying.py` & `keri-1.2.0.dev2/src/keri/app/cli/common/displaying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/common/existing.py` & `keri-1.2.0.dev2/src/keri/app/cli/common/existing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/common/incepting.py` & `keri-1.2.0.dev2/src/keri/app/cli/common/incepting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/common/rotating.py` & `keri-1.2.0.dev2/src/keri/app/cli/common/rotating.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/cli/kli.py` & `keri-1.2.0.dev2/src/keri/app/cli/kli.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/configing.py` & `keri-1.2.0.dev2/src/keri/app/configing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/connecting.py` & `keri-1.2.0.dev2/src/keri/app/connecting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/delegating.py` & `keri-1.2.0.dev2/src/keri/app/delegating.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/directing.py` & `keri-1.2.0.dev2/src/keri/app/directing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/forwarding.py` & `keri-1.2.0.dev2/src/keri/app/forwarding.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/grouping.py` & `keri-1.2.0.dev2/src/keri/app/grouping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/habbing.py` & `keri-1.2.0.dev2/src/keri/app/habbing.py`

 * *Files 0% similar despite different names*

```diff
@@ -2073,15 +2073,15 @@
 
         Parameters:
             cues is deque of cues
 
         """
         while cues:  # iteratively process each cue in cues
             msgs = bytearray()
-            cue = cues.pull() #cues.popleft()
+            cue = cues.pull()  # cues.popleft()
             cueKin = cue["kin"]  # type or kind of cue
 
             if cueKin in ("receipt",):  # cue to receipt a received event from other pre
                 cuedSerder = cue["serder"]  # Serder of received event for other pre
                 cuedKed = cuedSerder.ked
                 cuedPrefixer = coring.Prefixer(qb64=cuedKed["i"])
                 logger.info("%s got cue: kin=%s%s", self.pre, cueKin,
```

### Comparing `keri-1.2.0.dev1/src/keri/app/httping.py` & `keri-1.2.0.dev2/src/keri/app/httping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/indirecting.py` & `keri-1.2.0.dev2/src/keri/app/indirecting.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 def setupWitness(hby, alias="witness", mbx=None, aids=None, tcpPort=5631, httpPort=5632,
                  keypath=None, certpath=None, cafilepath=None):
     """
     Setup witness controller and doers
 
     """
+    host = "0.0.0.0"
     cues = decking.Deck()
     doers = []
 
     # make hab
     hab = hby.habByName(name=alias)
     if hab is None:
         hab = hby.makeHab(name=alias, transferable=False)
@@ -83,15 +84,15 @@
                             rvy=rvy)
 
     httpEnd = HttpEnd(rxbs=parser.ims, mbx=mbx)
     app.add_route("/", httpEnd)
     receiptEnd = ReceiptEnd(hab=hab, inbound=cues, aids=aids)
     app.add_route("/receipts", receiptEnd)
 
-    server = createHttpServer(httpPort, app, keypath, certpath, cafilepath)
+    server = createHttpServer(host, httpPort, app, keypath, certpath, cafilepath)
     if not server.reopen():
         raise RuntimeError(f"cannot create http server on port {httpPort}")
     httpServerDoer = http.ServerDoer(server=server)
 
     # setup doers
     regDoer = basing.BaserDoer(baser=verfer.reger)
 
@@ -108,35 +109,36 @@
                             kvy=kvy, tvy=tvy, rvy=rvy, exc=exchanger, replies=rep.reps,
                             responses=rep.cues, queries=httpEnd.qrycues)
 
     doers.extend([regDoer, httpServerDoer, rep, witStart, receiptEnd, *oobiery.doers])
     return doers
 
 
-def createHttpServer(port, app, keypath=None, certpath=None, cafilepath=None):
+def createHttpServer(host, port, app, keypath=None, certpath=None, cafilepath=None):
     """
     Create an HTTP or HTTPS server depending on whether TLS key material is present
     Parameters:
+        host(str)          : host to bind to for this server, or None for default of '0.0.0.0', all ifaces
         port (int)         : port to listen on for all HTTP(s) server instances
         app (falcon.App)   : application instance to pass to the http.Server instance
         keypath (string)   : the file path to the TLS private key
         certpath (string)  : the file path to the TLS signed certificate (public key)
         cafilepath (string): the file path to the TLS CA certificate chain file
     Returns:
         hio.core.http.Server
     """
     if keypath is not None and certpath is not None and cafilepath is not None:
         servant = tcp.ServerTls(certify=False,
                                 keypath=keypath,
                                 certpath=certpath,
                                 cafilepath=cafilepath,
                                 port=port)
-        server = http.Server(port=port, app=app, servant=servant)
+        server = http.Server(host=host, port=port, app=app, servant=servant)
     else:
-        server = http.Server(port=port, app=app)
+        server = http.Server(host=host, port=port, app=app)
     return server
 
 
 class WitnessStart(doing.DoDoer):
     """ Doer to print witness prefix after initialization
 
     """
@@ -242,15 +244,15 @@
         """
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
 
         while True:
             while self.cues:
-                cue = self.cues.pull() # self.cues.popleft()
+                cue = self.cues.pull()  # self.cues.popleft()
                 cueKin = cue["kin"]
                 if cueKin == "stream":
                     self.queries.append(cue)
                 else:
                     self.responses.append(cue)
                 yield self.tock
             yield self.tock
```

### Comparing `keri-1.2.0.dev1/src/keri/app/keeping.py` & `keri-1.2.0.dev2/src/keri/app/keeping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/notifying.py` & `keri-1.2.0.dev2/src/keri/app/notifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/oobiing.py` & `keri-1.2.0.dev2/src/keri/app/oobiing.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 from collections import namedtuple
 from urllib import parse
 from urllib.parse import urlparse
 
 import falcon
 from hio.base import doing
 from hio.help import decking
-from keri.core import coring
 
+from keri.core import coring
 from . import httping
-from .habbing import GroupHab
 from .. import help
 from .. import kering
-from ..app import forwarding, connecting
+from ..app import connecting
 from ..core import routing, eventing, parsing, scheming, serdering
 from ..db import basing
 from ..end import ending
 from ..end.ending import OOBI_RE, DOOBI_RE
 from ..help import helping
+from ..kering import Ilks, ValidationError, UnverifiedReplyError, ConfigurationError
 from ..peer import exchanging
 
 logger = help.ogler.getLogger()
 
 Resultage = namedtuple("Resultage", 'resolved failed')  # stream cold start status
 Result = Resultage(resolved='resolved', failed='failed')
 
@@ -272,36 +272,125 @@
 class Oobiery:
     """ Resolver for OOBIs
 
     """
 
     RetryDelay = 30
 
-    def __init__(self, hby, clienter=None, cues=None):
+    def __init__(self, hby, rvy=None, clienter=None, cues=None):
         """  DoDoer to handle the request and parsing of OOBIs
 
         Parameters:
             hby (Habery): database environment
             clienter (Clienter): DoDoer client provider responsible for managing HTTP client requests
             cues (decking.Deck): outbound cues from processing oobis
         """
 
         self.hby = hby
+        self.rvy = rvy
+        if self.rvy is not None:
+            self.registerReplyRoutes(self.rvy.rtr)
+
         self.clienter = clienter or httping.Clienter()
         self.org = connecting.Organizer(hby=self.hby)
+
+        # Set up a local parser for returned events from OOBI queries.
         rtr = routing.Router()
         rvy = routing.Revery(db=self.hby.db, rtr=rtr)
         kvy = eventing.Kevery(db=self.hby.db, lax=True, local=False, rvy=rvy)
         kvy.registerReplyRoutes(router=rtr)
         self.parser = parsing.Parser(framed=True, kvy=kvy, rvy=rvy)
 
         self.cues = cues if cues is not None else decking.Deck()
         self.clients = dict()
         self.doers = [self.clienter, doing.doify(self.scoobiDo)]
 
+    def registerReplyRoutes(self, router):
+        """ Register the routes for processing messages embedded in `rpy` event messages
+
+        The Oobiery handles rpy messages with the /introduce route by processing the contained oobi
+
+        Parameters:
+            router(Router): reply message router
+
+        """
+        router.addRoute("/introduce", self)
+
+    def processReply(self, *, serder, saider, route, cigars=None, tsgs=None, **kwargs):
+        """
+        Process one reply message for route = /introduce
+        with either attached nontrans receipt couples in cigars or attached trans
+        indexed sig groups in tsgs.
+        Assumes already validated saider, dater, and route from serder.ked
+
+        Parameters:
+            serder (SerderKERI): instance of reply msg (SAD)
+            saider (Saider): instance  from said in serder (SAD)
+            route (str): reply route
+            cigars (list): of Cigar instances that contain nontrans signing couple
+                          signature in .raw and public key in .verfer
+            tsgs (list): tuples (quadruples) of form
+                (prefixer, seqner, diger, [sigers]) where:
+                prefixer is pre of trans endorser
+                seqner is sequence number of trans endorser's est evt for keys for sigs
+                diger is digest of trans endorser's est evt for keys for sigs
+                [sigers] is list of indexed sigs from trans endorser's keys from est evt
+
+        OobiRecord:
+            date: str = date time of reply message of the introduction
+
+        Reply Message:
+        {
+          "v" : "KERI10JSON00011c_",
+          "t" : "rpy",
+          "d": "EZ-i0d8JZAoTNZH3ULaU6JR2nmwyvYAfSVPzhzS6b5CM",
+          "dt": "2020-08-22T17:50:12.988921+00:00",
+          "r" : "/introduce",
+          "a" :
+          {
+             "cid": "ENcOes8_t2C7tck4X4j61fSm0sWkLbZrEZffq7mSn8On",
+             "oobi":  "http://localhost:5632/oobi/ENcOes8_t2C7tck4X4j61fSm0sWkLbZrEZffq7mSn8On/witness",
+          }
+        }
+
+        """
+        if route != "/introduce":
+            raise ValidationError(f"Usupported route={route} in {Ilks.rpy} "
+                                  f"msg={serder.ked}.")
+
+        data = serder.ked['a']
+        dt = serder.ked["dt"]
+
+        for k in ("cid", "oobi"):
+            if k not in data:
+                raise ValidationError(f"Missing element={k} from attributes in"
+                                      f" {Ilks.rpy} msg={serder.ked}.")
+
+        cider = coring.Prefixer(qb64=data["cid"])  # raises error if unsupported code
+        cid = cider.qb64  # controller authorizing eid at role
+        aid = cid  # authorizing attribution id
+
+        oobi = data["oobi"]
+        url = urlparse(oobi)
+        if url.scheme not in ("http", "https"):
+            raise ValidationError(f"Invalid url scheme for introduced OOBI scheme={url.scheme}")
+
+        if self.rvy is None:
+            raise ConfigurationError("this oobiery is not configured to handle rpy introductions")
+
+        # Process BADA RUN but with no previous reply message, always process introductions
+        accepted = self.rvy.acceptReply(serder=serder, saider=saider, route=route,
+                                        aid=aid, osaider=None, cigars=cigars,
+                                        tsgs=tsgs)
+        if not accepted:
+            raise UnverifiedReplyError(f"Unverified introduciton reply. {serder.ked}")
+
+        obr = basing.OobiRecord(cid=cid, date=dt)
+        self.hby.db.oobis.put(keys=(oobi,), val=obr)
+
     def scoobiDo(self, tymth=None, tock=0.0):
         """
         Returns doifiable Doist compatibile generator method (doer dog) to process
             .exc responses and pass them on to the HTTPRespondant
 
         Parameters:
             tymth (function): injected function wrapper closure returned by .tymen() of
```

### Comparing `keri-1.2.0.dev1/src/keri/app/querying.py` & `keri-1.2.0.dev2/src/keri/app/querying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/signaling.py` & `keri-1.2.0.dev2/src/keri/app/signaling.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/signing.py` & `keri-1.2.0.dev2/src/keri/app/signing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/specing.py` & `keri-1.2.0.dev2/src/keri/app/specing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/app/storing.py` & `keri-1.2.0.dev2/src/keri/app/storing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/core/coring.py` & `keri-1.2.0.dev2/src/keri/core/coring.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 import re
 import json
 from typing import Union
 from collections import namedtuple, deque
 from collections.abc import Sequence, Mapping
-from dataclasses import dataclass, astuple
+from dataclasses import dataclass, astuple, asdict
 from base64 import urlsafe_b64encode as encodeB64
 from base64 import urlsafe_b64decode as decodeB64
 from fractions import Fraction
 
 import cbor2 as cbor
 import msgpack
 import pysodium
@@ -180,32 +180,29 @@
     else:
         raise DeserializeError("Invalid deserialization kind: {}"
                                    "".format(kind))
 
     return ked
 
 
-# ToDo: nonces only need 128 bits of entropy. a Salt is enough
-# Just use Salter().qb64.
 # Deprecated
+# randomNonce() refactored to match Salter().qb64 and only used in coring to avoid circular dependencies
+# use Salter().qb64 in other places
 
 def randomNonce():
-    """ Generate a random ed25519 seed and encode as qb64
+    """ Generate a random 128 bits salt and encode as qb64
 
     Returns:
-        str: qb64 encoded ed25519 random seed
+        str: qb64 encoded 128 bits random salt
     """
-    preseed = pysodium.randombytes(pysodium.crypto_sign_SEEDBYTES)
-    seedqb64 = Matter(raw=preseed, code=MtrDex.Ed25519_Seed).qb64
+    preseed = pysodium.randombytes(pysodium.crypto_pwhash_SALTBYTES)
+    seedqb64 = Matter(raw=preseed, code=MtrDex.Salt_128).qb64
     return seedqb64
 
 
-
-
-
 # secret derivation security tier
 Tierage = namedtuple("Tierage", 'low med high')
 
 Tiers = Tierage(low='low', med='med', high='high')
 
 
 
@@ -902,14 +899,17 @@
         '5E': Sizage(hs=2, ss=2, fs=None, ls=1),
         '6E': Sizage(hs=2, ss=2, fs=None, ls=2),
         '7AAE': Sizage(hs=4, ss=4, fs=None, ls=0),
         '8AAE': Sizage(hs=4, ss=4, fs=None, ls=1),
         '9AAE': Sizage(hs=4, ss=4, fs=None, ls=2),
     }
 
+    Codes = asdict(MtrDex)  # map code name to code
+    Names = {val : key for key, val in Codes.items()} # invert map code to code name
+
 
 
     def __init__(self, raw=None, code=MtrDex.Ed25519N, soft='', rize=None,
                  qb64b=None, qb64=None, qb2=None, strip=False):
         """
         Validate as fully qualified
         Parameters:
@@ -1113,14 +1113,25 @@
         Some codes only have a hard part. Soft part may be for variable sized
         matter or for special codes that are code only (raw is empty)
         """
         return self._code
 
 
     @property
+    def name(self):
+        """
+        Returns:
+            name (str): code name for self.code. Used for annotation for
+            primitives like Matter
+
+        """
+        return self.Names[self.code]
+
+
+    @property
     def hard(self):
         """
         Returns:
             hard (str): hard part only of full text code. Alias for .code.
 
         """
         return self.code
@@ -1696,14 +1707,18 @@
         _infil (types.MethodType): creates qb64b from .raw and .code
                                    (fully qualified Base64)
         _exfil (types.MethodType): extracts .code and .raw from qb64b
                                    (fully qualified Base64)
 
     Methods:
     """
+    Codes = asdict(NumDex)  # map code name to code
+    Names = {val : key for key, val in Codes.items()} # invert map code to code name
+
+
 
     def __init__(self, raw=None, qb64b=None, qb64=None, qb2=None,
                  code=None, num=None, numh=None, **kwa):
         """
         Inherited Parameters:  (see Matter)
             raw (bytes): unqualified crypto material usable for crypto operations
             code (str | None): stable (hard) part of derivation code.
@@ -4793,81 +4808,14 @@
         except Exception as ex:
             return False
 
         return False
 
 
 
-class Streamer:
-    """
-    Streamer is CESR sniffable stream class
-
-
-    Has the following public properties:
-
-    Properties:
-
-
-    Methods:
-
-
-    Hidden:
-
-
-
-    """
-
-    def __init__(self, stream):
-        """Initialize instance
-
-
-        Parameters:
-            stream (bytes | bytearray): sniffable CESR stream
-
-
-        """
-        self._stream = bytes(stream)
-
-
-    @property
-    def stream(self):
-        """stream property getter
-        """
-        return self._stream
-
-    @property
-    def text(self):
-        """expanded stream as qb64 text
-        Returns:
-           stream (bytes): expanded text qb64 version of stream
-
-        """
-        return self._stream
-
-    @property
-    def binary(self):
-        """compacted stream as qb2 binary
-        Returns:
-           stream (bytes): compacted binary qb2 version of stream
-
-        """
-        return self._stream
-
-    @property
-    def texter(self):
-        """expanded stream as Texter instance
-        Returns:
-           texter (Texter): Texter primitive of stream suitable wrapping
-
-        """
-        return self._stream
-
-
-
-
 class Sadder:
     """
     Sadder is self addressed data (SAD) serializer-deserializer class
 
     Instance creation of a Sadder does not verifiy it .said property it merely
     extracts it. In order to ensure Sadder instance has a verified .said then
     must call .saider.verify(sad=self.ked)
```

### Comparing `keri-1.2.0.dev1/src/keri/core/counting.py` & `keri-1.2.0.dev2/src/keri/core/counting.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
     BigESSRWrapperGroup: str = '-0E'  # Big ESSR Wrapper Group (Universal).
     FixedMessageBodyGroup: str = '-F'  # Fixed Field Message Body Group (Universal).
     BigFixedMessageBodyGroup: str = '-0F'  # Big Fixed Field Message Body Group (Universal).
     MapMessageBodyGroup: str = '-G'  # Field Map Message Body Group (Universal).
     BigMapMessageBodyGroup: str = '-0G'  # Big Field Map Message Body Group (Universal).
     GenericMapGroup: str = '-H'  # Generic Field Map Group (Universal).
     BigGenericMapGroup: str = '-0H'  # Big Generic Field Map Group (Universal).
-    GenericListGroup: str = '-L'  # Generic List Group (Universal).
-    BigGenericListGroup: str = '-0L'  # Big Generic List Group (Universal).
+    GenericListGroup: str = '-I'  # Generic List Group (Universal).
+    BigGenericListGroup: str = '-0I'  # Big Generic List Group (Universal).
     ControllerIdxSigs: str = '-J'  # Controller Indexed Signature(s) of qb64.
     BigControllerIdxSigs: str = '-0J'  # Big Controller Indexed Signature(s) of qb64.
     WitnessIdxSigs: str = '-K'  # Witness Indexed Signature(s) of qb64.
     BigWitnessIdxSigs: str = '-0K'  # Big Witness Indexed Signature(s) of qb64.
     NonTransReceiptCouples: str = '-L'  # NonTrans Receipt Couple(s), pre+cig.
     BigNonTransReceiptCouples: str = '-0L'  # Big NonTrans Receipt Couple(s), pre+cig.
     TransReceiptQuadruples: str = '-M'  # Trans Receipt Quadruple(s), pre+snu+dig+sig.
@@ -415,18 +415,18 @@
     def __init__(self, tag=None, *, code = None, count=None, countB64=None,
                  qb64b=None, qb64=None, qb2=None, strip=False, gvrsn=Vrsn_2_0):
         """
         Validate as fully qualified
         Parameters:
             tag (str | None):  label of stable (hard) part of derivation code
                                to lookup in codex so it can depend on version.
-                               takes precedence over tag
+                               takes precedence over code.
             code (str | None):  stable (hard) part of derivation code
                             if tag provided lookup code from tag
-                            else if tag is None and code provided use code
+                            else if tag is None and code provided use code.
             count (int | None): count of framed material in quadlets/triplets
                                for composition. Count does not include code.
                                When both count and countB64 are None then count
                                defaults to 1
             countB64 (str | None): count of framed material in quadlets/triplets
                                 for composition as Base64 representation of int.
             qb64b (bytes | bytearray | None): fully qualified crypto material text domain
@@ -513,37 +513,48 @@
                 del qb2[:self._sizes[self.code].fs * 3 // 4]
 
         else:
             raise kering.EmptyMaterialError("Improper initialization need either "
                                      "(code and count) or qb64b or "
                                      "qb64 or qb2.")
 
+        codenames = { val: key for key, val in asdict(self.codes).items()} # map codes to code names
+        self._tag = codenames[self.code]
+
     @property
     def version(self):
         """
         Returns ._version
         Makes .version read only
         """
         return self._version
 
     @property
+    def gvrsn(self):
+        """
+        Returns .version alias for .version
+
+        """
+        return self.version
+
+    @property
     def codes(self):
         """
         Returns ._codes
         Makes .codes read only
         """
         return self._codes
 
     @property
     def tags(self):
         """
-        Returns ._tags
+        Returns tags for current .version
         Makes .tags read only
         """
-        return self._tags
+        return self.Tags[self.version]  # use own version
 
     @property
     def sizes(self):
         """
         Returns ._sizes
         Makes .sizes read only
         """
@@ -556,14 +567,34 @@
             code (str): hard part only of full text code.
                 Getter for ._code. Makes .code read only
 
         Soft part is count
         """
         return self._code
 
+    @property
+    def tag(self):
+        """
+        Returns:
+            tag (str): code name for self.code
+
+        Getter for ._tag. Makes .tag read only
+        """
+        return self._tag
+
+    @property
+    def name(self):
+        """
+        Returns:
+            name (str): code name for self.code alias of .tag. Match interface
+            for annotation for primitives like Matter
+
+        """
+        return self.tag
+
 
     @property
     def hard(self):
         """
         Returns:
             hard (str): hard part only of full text code. Alias for .code.
```

### Comparing `keri-1.2.0.dev1/src/keri/core/eventing.py` & `keri-1.2.0.dev2/src/keri/core/eventing.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,15 @@
     """
     Returns serder of delegated inception event message.
     Utility function to automate creation of delegated inception events.
     Syntactic suger that calls incept but with delpre so ilk is dip.
 
     Parameters:
         keys  (list): current signing keys qb64
-        sith (int | str | list | None): current signing threshold input to Tholder
+        isith (int | str | list | None): current signing threshold input to Tholder
         ndigs (list | None): current signing key digests qb64
         nsith int | str | list | None): next signing threshold input to Tholder
         toad (int | str | None): witness threshold number if str then hex str
         wits (list | None): witness identifier prefixes qb64
         cnfg (list | None): configuration traits from TraitDex
         data (list | None): seal dicts
         version (Version): KERI protocol version string
@@ -944,15 +944,15 @@
 
     Parameters:
         pre (str): identifier prefix qb64
         keys  (list): current signing keys qb64
         dig (str): said of previous event qb64
         ilk (str): ilk of event. Must be in (Ilks.rot, Ilks.drt)
         sn (int | str): sequence number int or hex str
-        sith (int | str | list): current signing threshold input to Tholder
+        isith (int | str | list): current signing threshold input to Tholder
         ndigs (list): current signing key digests qb64
         nsith int | str | list): next signing threshold input to Tholder
         toad (int | str ): witness threshold number if str then hex str
         wits (list): prior witness identifier prefixes qb64
         cuts (list): witness prefixes to cut qb64
         adds (list): witness prefixes to add qb64
         data (list): seal dicts
@@ -1158,23 +1158,14 @@
                a=data if data else {},  # attributes
                )
 
     serder = serdering.SerderKERI(sad=sad, makify=True)
     serder._verify()  # raises error if fails verifications
     return serder
 
-    #_, sad = coring.Saider.saidify(sad=sad, kind=kind, label=label)
-
-    #saider = coring.Saider(qb64=sad[label])
-    #if not saider.verify(sad=sad, kind=kind, label=label, prefixed=True):
-        #raise ValidationError("Invalid said = {} for reply msg={}."
-                              #"".format(saider.qb64, sad))
-
-    #return Serder(ked=sad)  # return serialized Self-Addressed Data (SAD)
-
 
 def prod(route="",
           replyRoute="",
           query=None,
           stamp=None,
           version=Version,
           kind=Serials.json):
@@ -4111,29 +4102,26 @@
 
     def removeStaleReplyLocScheme(self, saider):
         """
         Process reply escrow at saider for route "/loc/scheme"
         """
         pass
 
-
     def registerReplyRoutes(self, router):
         """ Register the routes for processing messages embedded in `rpy` event messages
 
         Parameters:
             router(Router): reply message router
 
         """
         router.addRoute("/end/role/{action}", self, suffix="EndRole")
         router.addRoute("/loc/scheme", self, suffix="LocScheme")
         router.addRoute("/ksn/{aid}", self, suffix="KeyStateNotice")
 
-
-    def processReplyEndRole(self, *, serder, saider, route,
-                            cigars=None, tsgs=None, **kwargs):
+    def processReplyEndRole(self, *, serder, saider, route, cigars=None, tsgs=None, **kwargs):
         """
         Process one reply message for route = /end/role/add or /end/role/cut
         with either attached nontrans receipt couples in cigars or attached trans
         indexed sig groups in tsgs.
         Assumes already validated saider, dater, and route from serder.ked
 
         Parameters:
@@ -4528,14 +4516,19 @@
         ilk = ked["t"]
         route = ked["r"]
         qry = ked["q"]
 
         # do signature validation and replay attack prevention logic here
         # src, dt, route
 
+        if source is None and cigars:
+            dest = cigars[0].verfer.qb64
+        else:
+            dest = source.qb64
+
         if route == "logs":
             pre = qry["i"]
             src = qry["src"]
             anchor = qry["a"] if "a" in qry else None
             sn = int(qry["s"], 16) if "s" in qry else None
 
             if pre not in self.kevers:
@@ -4559,15 +4552,15 @@
 
             if kever.delpre:
                 cloner = self.db.clonePreIter(pre=kever.delpre, fn=0)  # create iterator at 0
                 for msg in cloner:
                     msgs.append(msg)
 
             if msgs:
-                self.cues.push(dict(kin="replay", src=src, msgs=msgs, dest=source.qb64))
+                self.cues.push(dict(kin="replay", pre=pre, src=src, msgs=msgs, dest=dest))
 
         elif route == "ksn":
             pre = qry["i"]
             src = qry["src"]
 
             if pre not in self.kevers:
                 self.escrowQueryNotFoundEvent(serder=serder, prefixer=source, sigers=sigers, cigars=cigars)
@@ -4581,15 +4574,15 @@
 
             if len(wigers) < kever.toader.num:
                 self.escrowQueryNotFoundEvent(serder=serder, prefixer=source, sigers=sigers, cigars=cigars)
                 raise QueryNotFoundError("Query not found error={}.".format(ked))
 
             rserder = reply(route=f"/ksn/{src}", data=kever.state()._asdict())
             self.cues.push(dict(kin="reply", src=src, route="/ksn", serder=rserder,
-                                dest=source.qb64))
+                                dest=dest))
 
         elif route == "mbx":
             pre = qry["i"]
             src = qry["src"]
             topics = qry["topics"]
 
             if pre not in self.kevers:
```

### Comparing `keri-1.2.0.dev1/src/keri/core/indexing.py` & `keri-1.2.0.dev2/src/keri/core/indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,14 @@
         ._ondex (int): value for .ondex property
         ._infil is method to compute fully qualified Base64 from .raw and .code
         ._binfil is method to compute fully qualified Base2 from .raw and .code
         ._exfil is method to extract .code and .raw from fully qualified Base64
         ._bexfil is method to extract .code and .raw from fully qualified Base2
 
     """
-    Codex = IdrDex
     # Hards table maps from bytes Base64 first code char to int of hard size, hs,
     # (stable) of code. The soft size, ss, (unstable) is always > 0 for Indexer.
     Hards = ({chr(c): 1 for c in range(65, 65 + 26)})
     Hards.update({chr(c): 1 for c in range(97, 97 + 26)})
     Hards.update([('0', 2), ('1', 2), ('2', 2), ('3', 2), ('4', 2)])
     # Sizes table maps hs chars of code to Xizage namedtuple of (hs, ss, os, fs, ls)
     # where hs is hard size, ss is soft size, os is other index size,
@@ -224,14 +223,19 @@
         '1z': Xizage(hs=2, ss=2, os=1, fs=76, ls=1),
         '4z': Xizage(hs=2, ss=6, os=3, fs=80, ls=1),
     }
     # Bards table maps to hard size, hs, of code from bytes holding sextets
     # converted from first code char. Used for ._bexfil.
     Bards = ({codeB64ToB2(c): hs for c, hs in Hards.items()})
 
+    Codes = asdict(IdrDex)  # map code name to code
+    Names = {val : key for key, val in Codes.items()} # invert map code to code name
+
+
+
     def __init__(self, raw=None, code=IdrDex.Ed25519_Sig, index=0, ondex=None,
                  qb64b=None, qb64=None, qb2=None, strip=False):
         """
         Validate as fully qualified
         Parameters:
             raw (bytes): unqualified crypto material usable for crypto operations
             code is str of stable (hard) part of derivation code
@@ -337,14 +341,25 @@
     def code(self):
         """
         Returns ._code
         Makes .code read only
         """
         return self._code
 
+
+    @property
+    def name(self):
+        """
+        Returns:
+            name (str): code name for self.code. Used for annotation for
+            primitives like Matter
+
+        """
+        return self.Names[self.code]
+
     @property
     def raw(self):
         """
         Returns ._raw
         Makes .raw read only
         """
         return self._raw
```

### Comparing `keri-1.2.0.dev1/src/keri/core/parsing.py` & `keri-1.2.0.dev2/src/keri/core/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1034,16 +1034,16 @@
                     if cigars:  # process separately so do not clash on errors
                         rvy.processReply(serder, cigars=cigars)  # nontrans
 
                     if tsgs:  # process separately so do not clash on errors
                         rvy.processReply(serder, tsgs=tsgs)  # trans
 
                 except AttributeError as e:
-                    raise kering.ValidationError("No kevery to process so dropped msg"
-                                                 "= {}.".format(serder.pretty()))
+                    raise kering.ValidationError("No revery to process so dropped msg"
+                                                 "= {}.".format(serder.pretty())) from e
 
             elif ilk in (Ilks.qry,):  # query message
                 args = dict(serder=serder)
                 if ssgs:
                     pre, sigers = ssgs[-1] if ssgs else (None, None)  # use last one if more than one
                     args["source"] = pre
                     args["sigers"] = sigers
@@ -1055,17 +1055,17 @@
                     raise kering.ValidationError("Missing attached requester signature(s) "
                                                  "to key log query msg = {}.".format(serder.pretty()))
 
                 route = serder.ked["r"]
                 if route in ["logs", "ksn", "mbx"]:
                     try:
                         kvy.processQuery(**args)
-                    except AttributeError:
+                    except AttributeError as e:
                         raise kering.ValidationError("No kevery to process so dropped msg"
-                                                     "= {}.".format(serder.pretty()))
+                                                     "= {} from e = {}".format(serder.pretty(), e))
 
                 elif route in ["tels", "tsn"]:
                     try:
                         tvy.processQuery(**args)
                     except AttributeError as e:
                         raise kering.ValidationError("No tevery to process so dropped msg"
                                                      "= {} from {}.".format(serder.pretty(), e))
```

### Comparing `keri-1.2.0.dev1/src/keri/core/routing.py` & `keri-1.2.0.dev2/src/keri/core/routing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/core/scheming.py` & `keri-1.2.0.dev2/src/keri/core/scheming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/core/serdering.py` & `keri-1.2.0.dev2/src/keri/core/serdering.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/core/signing.py` & `keri-1.2.0.dev2/src/keri/core/signing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/core/structing.py` & `keri-1.2.0.dev2/src/keri/core/structing.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .. import help
 from ..help import nonStringSequence
 
 from . import coring
 from .coring import (MapDom, Matter, Diger, Prefixer, Number)
 
 
+
 # ToDo Change seal namedtuple definitions to NamedTuple subclasses so can
 # use typehints on field values which type hints are the primitive types. Use
 # union | on type hints to allow qb64, qb2, primitive instance, primitive class
 # as acceptable values  This provides more clarity in documentation. Actually
 # enforcing types is harder with union | but can still be accomplished.
 
 #  for the following Seal namedtuples use the ._asdict() method to convert to dict
```

### Comparing `keri-1.2.0.dev1/src/keri/db/basing.py` & `keri-1.2.0.dev2/src/keri/db/basing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1496,14 +1496,17 @@
 
         # add authorizer (delegator/issuer) source seal event couple to attachments
         couple = self.getAes(dgkey)
         if couple is not None:
             atc.extend(coring.Counter(code=coring.CtrDex.SealSourceCouples,
                                       count=1).qb64b)
             atc.extend(couple)
+        elif self.kevers[pre].delegated:
+            if coring.SerderKERI(raw=raw).estive:
+                raise kering.MissingEntryError("Missing delegator anchor seal for dig={}.".format(dig))
 
         # add trans endorsement quadruples to attachments not controller
         # may have been originally key event attachments or receipted endorsements
         if quads := self.getVrcs(key=dgkey):
             atc.extend(coring.Counter(code=coring.CtrDex.TransReceiptQuadruples,
                                       count=len(quads)).qb64b)
             for quad in quads:
```

### Comparing `keri-1.2.0.dev1/src/keri/db/dbing.py` & `keri-1.2.0.dev2/src/keri/db/dbing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/db/escrowing.py` & `keri-1.2.0.dev2/src/keri/db/escrowing.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,14 @@
                     processReply(serder=serder, saider=saider, route=serder.ked["r"],
                                  cigars=cigars, tsgs=tsgs, aid=aid)
 
                 except extype as ex:
                     # still waiting on missing prior event to validate
                     if logger.isEnabledFor(logging.DEBUG):
                         logger.exception("Kevery unescrow attempt failed: %s", ex.args[0])
-                    else:
-                        logger.error("Kevery unescrow attempt failed: %s", ex.args[0])
 
                 except Exception as ex:  # other error so remove from reply escrow
                     self.escrowdb.remIokey(iokeys=(typ, pre, aid, ion))  # remove escrow
                     if logger.isEnabledFor(logging.DEBUG):
                         logger.exception("Kevery unescrowed due to error: %s", ex.args[0])
                     else:
                         logger.error("Kevery unescrowed due to error: %s", ex.args[0])
```

### Comparing `keri-1.2.0.dev1/src/keri/db/koming.py` & `keri-1.2.0.dev2/src/keri/db/koming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/db/migrations/rekey_habs.py` & `keri-1.2.0.dev2/src/keri/db/migrations/rekey_habs.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/db/subing.py` & `keri-1.2.0.dev2/src/keri/db/subing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/demo/demo_bob.py` & `keri-1.2.0.dev2/src/keri/demo/demo_bob.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/demo/demo_eve.py` & `keri-1.2.0.dev2/src/keri/demo/demo_eve.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/demo/demo_kev.py` & `keri-1.2.0.dev2/src/keri/demo/demo_kev.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/demo/demo_sam.py` & `keri-1.2.0.dev2/src/keri/demo/demo_sam.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/demo/demoing.py` & `keri-1.2.0.dev2/src/keri/demo/demoing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/end/ending.py` & `keri-1.2.0.dev2/src/keri/end/ending.py`

 * *Files 1% similar despite different names*

```diff
@@ -573,14 +573,18 @@
             return
 
         kever = self.hby.kevers[aid]
         if not self.hby.db.fullyWitnessed(kever.serder):
             rep.status = falcon.HTTP_NOT_FOUND
             return
 
+        if kever.delegated and kever.delpre not in self.hby.kevers:
+            rep.status = falcon.HTTP_NOT_FOUND
+            return
+
         owits = oset(kever.wits)
         if kever.prefixer.qb64 in self.hby.prefixes:  # One of our identifiers
             hab = self.hby.habs[kever.prefixer.qb64]
         elif match := owits.intersection(self.hby.prefixes):  # We are a witness for identifier
             pre = match.pop()
             hab = self.hby.habs[pre]
         else:  # Not allowed to respond
```

### Comparing `keri-1.2.0.dev1/src/keri/end/priming.py` & `keri-1.2.0.dev2/src/keri/end/priming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/help/__init__.py` & `keri-1.2.0.dev2/src/keri/help/__init__.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/help/helping.py` & `keri-1.2.0.dev2/src/keri/help/helping.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 B64ChrByIdx[63] = '_'
 # Map char to Base64 index
 B64IdxByChr = {char: index for index, char in B64ChrByIdx.items()}
 # tuple
 B64_CHARS = tuple(B64ChrByIdx.values())  # tuple of characters in Base64
 
 
-B64REX = b'^[0-9A-Za-z_-]*\Z'   # [A-Za-z0-9\-\_]
+B64REX = rb'^[0-9A-Za-z_-]*\Z'   # [A-Za-z0-9\-\_]
 Reb64 = re.compile(B64REX)  # compile is faster
 # to use if Reb64.match(bext):
 
 
 def intToB64(i, l=1):
     """
     Returns conversion of int i to Base64 str
```

### Comparing `keri-1.2.0.dev1/src/keri/kering.py` & `keri-1.2.0.dev2/src/keri/kering.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
     def __iter__(self):
         return iter(astuple(self))
 
 
 ColdDex = ColdCodex()  # Make instance
 
 Coldage = namedtuple("Coldage", 'msg txt bny')  # stream cold start status
-Colds = Coldage(msg='msg', txt='txt', bny='bny')
+Colds = Coldage(msg='msg', txt='txt', bny='bny') # add 'ant' for annotated
 
 
 def sniff(ims):
     """
     Returns status string of cold start of stream ims bytearray by looking
     at first triplet of first byte to determin if message or counter code
     and if counter code whether Base64 or Base2 representation
@@ -286,14 +286,16 @@
     tritet = ims[0] >> 5
     if tritet in (ColdDex.JSON, ColdDex.MGPK1, ColdDex.CBOR, ColdDex.MGPK2):
         return Colds.msg
     if tritet in (ColdDex.CtB64, ColdDex.OpB64):
         return Colds.txt
     if tritet in (ColdDex.CtOpB2,):
         return Colds.bny
+    #if tritet in (ColdDex.AnB64, ):
+
 
     raise ColdStartError("Unexpected tritet={} at stream start.".format(tritet))
 
 
 """
 ilk is short for packet or message type for a given protocol
     icp = incept, inception
@@ -827,14 +829,21 @@
     """
     Bad or Unsupported Serialization Kind
 
     Usage:
         raise KindError("error message")
     """
 
+class IlkError(ExtractionError):
+    """
+    Bad or Unsupported Message Type (Ilk)
+
+    Usage:
+        raise IlkError("error message")
+    """
 
 class ConversionError(ExtractionError):
     """
     Problem with Base64 to Binary conversion
 
     Usage:
         raise ConversionError("error message")
```

### Comparing `keri-1.2.0.dev1/src/keri/peer/exchanging.py` & `keri-1.2.0.dev2/src/keri/peer/exchanging.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/vc/protocoling.py` & `keri-1.2.0.dev2/src/keri/vc/protocoling.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/vc/proving.py` & `keri-1.2.0.dev2/src/keri/vc/proving.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/vc/walleting.py` & `keri-1.2.0.dev2/src/keri/vc/walleting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/vdr/credentialing.py` & `keri-1.2.0.dev2/src/keri/vdr/credentialing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/vdr/eventing.py` & `keri-1.2.0.dev2/src/keri/vdr/eventing.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from keri import kering
 from .. import core
 from .. import help
 from ..core import serdering, coring, indexing
 from ..core.coring import (MtrDex, Serials, versify, Prefixer,
                            Ilks, Seqner, Verfer, Number)
+from ..core.signing import (Salter,)
 from ..core.eventing import SealEvent, ample, TraitDex, verifySigs
 from ..db import basing, dbing
 from ..db.dbing import dgKey, snKey
 from ..help import helping
 from ..kering import (MissingWitnessSignatureError, Version,
                       MissingAnchorError, ValidationError, OutOfOrderError, LikelyDuplicitousError)
 from ..vdr import viring
@@ -86,15 +87,15 @@
     if baks:
         if toad < 1 or toad > len(baks):  # out of bounds toad
             raise ValueError("Invalid toad = {} for baks = {}".format(toad, baks))
     else:
         if toad != 0:  # invalid toad
             raise ValueError("Invalid toad = {} for baks = {}".format(toad, baks))
 
-    nonce = nonce if nonce is not None else coring.randomNonce()
+    nonce = nonce if nonce is not None else Salter().qb64
     ked = dict(v=vs,  # version string
                t=ilk,
                d="",
                i="",  # qb64 prefix
                ii=pre,
                s="{:x}".format(isn),  # hex string no leading zeros lowercase
                c=cnfg,
```

### Comparing `keri-1.2.0.dev1/src/keri/vdr/verifying.py` & `keri-1.2.0.dev2/src/keri/vdr/verifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri/vdr/viring.py` & `keri-1.2.0.dev2/src/keri/vdr/viring.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev1/src/keri.egg-info/PKG-INFO` & `keri-1.2.0.dev2/src/keri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.2.0.dev1
+Version: 1.2.0.dev2
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
```

### Comparing `keri-1.2.0.dev1/src/keri.egg-info/SOURCES.txt` & `keri-1.2.0.dev2/src/keri.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,16 @@
 src/keri/app/cli/commands/vc/export.py
 src/keri/app/cli/commands/vc/list.py
 src/keri/app/cli/commands/vc/revoke.py
 src/keri/app/cli/commands/vc/registry/__init__.py
 src/keri/app/cli/commands/vc/registry/incept.py
 src/keri/app/cli/commands/vc/registry/list.py
 src/keri/app/cli/commands/vc/registry/status.py
+src/keri/app/cli/commands/watcher/__init__.py
+src/keri/app/cli/commands/watcher/add.py
 src/keri/app/cli/commands/witness/__init__.py
 src/keri/app/cli/commands/witness/authenticate.py
 src/keri/app/cli/commands/witness/demo.py
 src/keri/app/cli/commands/witness/start.py
 src/keri/app/cli/commands/witness/submit.py
 src/keri/app/cli/common/__init__.py
 src/keri/app/cli/common/config.py
@@ -136,14 +138,15 @@
 src/keri/core/eventing.py
 src/keri/core/indexing.py
 src/keri/core/parsing.py
 src/keri/core/routing.py
 src/keri/core/scheming.py
 src/keri/core/serdering.py
 src/keri/core/signing.py
+src/keri/core/streaming.py
 src/keri/core/structing.py
 src/keri/db/__init__.py
 src/keri/db/basing.py
 src/keri/db/dbing.py
 src/keri/db/escrowing.py
 src/keri/db/koming.py
 src/keri/db/subing.py
```

### Comparing `keri-1.2.0.dev1/tests/test_kering.py` & `keri-1.2.0.dev2/tests/test_kering.py`

 * *Files identical despite different names*

