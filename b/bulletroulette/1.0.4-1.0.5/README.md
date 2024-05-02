# Comparing `tmp/bulletroulette-1.0.4.tar.gz` & `tmp/bulletroulette-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulletroulette-1.0.4.tar", last modified: Mon Apr 15 12:17:48 2024, max compression
+gzip compressed data, was "bulletroulette-1.0.5.tar", last modified: Thu May  2 11:11:30 2024, max compression
```

## Comparing `bulletroulette-1.0.4.tar` & `bulletroulette-1.0.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-13 02:31:44.000000 bulletroulette-1.0.4/LICENSE
--rw-rw-r--   0 gqx       (1000) gqx       (1000)      183 2024-04-14 03:20:19.000000 bulletroulette-1.0.4/MANIFEST.in
--rw-r--r--   0 gqx       (1000) gqx       (1000)     4173 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/PKG-INFO
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     3163 2024-04-14 10:02:38.000000 bulletroulette-1.0.4/README.md
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-15 12:17:48.604539 bulletroulette-1.0.4/bulletroulette/
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       98 2024-04-14 00:21:35.000000 bulletroulette-1.0.4/bulletroulette/__init__.py
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/bulletroulette/assets/
--rw-------   0 gqx       (1000) gqx       (1000)     4216 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/A.png
--rw-------   0 gqx       (1000) gqx       (1000)     4273 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/B.png
--rw-------   0 gqx       (1000) gqx       (1000)     4252 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/C.png
--rw-------   0 gqx       (1000) gqx       (1000)     4138 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/D.png
--rw-------   0 gqx       (1000) gqx       (1000)     2114 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/DELETE.png
--rw-------   0 gqx       (1000) gqx       (1000)     3620 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/E.png
--rw-------   0 gqx       (1000) gqx       (1000)     2702 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/ENTER.png
--rw-------   0 gqx       (1000) gqx       (1000)     3576 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/F.png
--rw-------   0 gqx       (1000) gqx       (1000)     4297 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/G.png
--rw-------   0 gqx       (1000) gqx       (1000)     3598 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/H.png
--rw-------   0 gqx       (1000) gqx       (1000)     3592 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/I.png
--rw-------   0 gqx       (1000) gqx       (1000)     3790 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/J.png
--rw-------   0 gqx       (1000) gqx       (1000)     4139 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/K.png
--rw-------   0 gqx       (1000) gqx       (1000)     3505 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/L.png
--rw-------   0 gqx       (1000) gqx       (1000)     3964 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/M.png
--rw-------   0 gqx       (1000) gqx       (1000)     4052 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/N.png
--rw-------   0 gqx       (1000) gqx       (1000)     4271 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/O.png
--rw-------   0 gqx       (1000) gqx       (1000)     3931 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/P.png
--rw-------   0 gqx       (1000) gqx       (1000)     4456 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/Q.png
--rw-------   0 gqx       (1000) gqx       (1000)     4171 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/R.png
--rw-------   0 gqx       (1000) gqx       (1000)     4263 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/S.png
--rwx------   0 gqx       (1000) gqx       (1000) 10050868 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/Simhei.ttf
--rw-------   0 gqx       (1000) gqx       (1000)     3701 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/T.png
--rw-------   0 gqx       (1000) gqx       (1000)     3887 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/U.png
--rw-------   0 gqx       (1000) gqx       (1000)     4313 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/V.png
--rw-------   0 gqx       (1000) gqx       (1000)     4535 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/W.png
--rw-------   0 gqx       (1000) gqx       (1000)     4286 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/X.png
--rw-------   0 gqx       (1000) gqx       (1000)     3987 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/Y.png
--rw-------   0 gqx       (1000) gqx       (1000)     3920 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/Z.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    25284 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/beer.png
--rwx------   0 gqx       (1000) gqx       (1000)  1526669 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/bg.png
--rwx------   0 gqx       (1000) gqx       (1000)  1107220 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/bgmsc.ogg
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     6692 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/blank.png
--rwx------   0 gqx       (1000) gqx       (1000)   192078 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/blank.wav
--rwx------   0 gqx       (1000) gqx       (1000)     5494 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/charge.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)   117887 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/dealershootplayer.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    43271 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/dealershootself.png
--rw-------   0 gqx       (1000) gqx       (1000)    97047 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/gun.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    61801 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/handcuff.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    64423 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/knife.png
--rwx------   0 gqx       (1000) gqx       (1000)    96078 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/livedealer.wav
--rwx------   0 gqx       (1000) gqx       (1000)   432078 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/liveplayer.wav
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    12620 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/liveround.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    15499 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/magnifier.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    34020 2024-04-13 01:14:24.000000 bulletroulette-1.0.4/bulletroulette/assets/noneprop.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)   130200 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/pill.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    43256 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/propbox.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    33816 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/smoke.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)   432984 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/super.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1143 2024-04-14 02:40:49.000000 bulletroulette-1.0.4/bulletroulette/data.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     3187 2024-04-14 02:40:51.000000 bulletroulette-1.0.4/bulletroulette/roles.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    13690 2024-04-14 10:45:40.000000 bulletroulette-1.0.4/bulletroulette/run.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1009 2024-04-14 02:41:24.000000 bulletroulette-1.0.4/bulletroulette/sprites.py
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/bulletroulette.egg-info/
--rw-r--r--   0 gqx       (1000) gqx       (1000)     4173 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/PKG-INFO
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1857 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/SOURCES.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/dependency_links.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       14 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/requires.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       15 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/top_level.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/setup.cfg
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1621 2024-04-15 12:17:41.000000 bulletroulette-1.0.4/setup.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-05-02 11:11:30.530979 bulletroulette-1.0.5/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-13 02:31:44.000000 bulletroulette-1.0.5/LICENSE
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)      183 2024-04-14 03:20:19.000000 bulletroulette-1.0.5/MANIFEST.in
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     4119 2024-05-02 11:11:30.530979 bulletroulette-1.0.5/PKG-INFO
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     3163 2024-04-14 10:02:38.000000 bulletroulette-1.0.5/README.md
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-05-02 11:11:30.506979 bulletroulette-1.0.5/bulletroulette/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       98 2024-04-14 00:21:35.000000 bulletroulette-1.0.5/bulletroulette/__init__.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-05-02 11:11:30.530979 bulletroulette-1.0.5/bulletroulette/assets/
+-rw-------   0 gqx       (1000) gqx       (1000)     4216 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/A.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4273 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/B.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4252 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/C.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4138 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/D.png
+-rw-------   0 gqx       (1000) gqx       (1000)     2114 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/DELETE.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3620 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/E.png
+-rw-------   0 gqx       (1000) gqx       (1000)     2702 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/ENTER.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3576 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/F.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4297 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/G.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3598 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/H.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3592 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/I.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3790 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/J.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4139 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/K.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3505 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/L.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3964 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/M.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4052 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/N.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4271 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/O.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3931 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/P.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4456 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/Q.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4171 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/R.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4263 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/S.png
+-rwx------   0 gqx       (1000) gqx       (1000) 10050868 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/Simhei.ttf
+-rw-------   0 gqx       (1000) gqx       (1000)     3701 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/T.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3887 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/U.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4313 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/V.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4535 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/W.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4286 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/X.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3987 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/Y.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3920 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/Z.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    25284 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/beer.png
+-rwx------   0 gqx       (1000) gqx       (1000)  1526669 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/bg.png
+-rwx------   0 gqx       (1000) gqx       (1000)  1107220 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/bgmsc.ogg
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     6692 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/blank.png
+-rwx------   0 gqx       (1000) gqx       (1000)   192078 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/blank.wav
+-rwx------   0 gqx       (1000) gqx       (1000)     5494 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/charge.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)   117887 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/dealershootplayer.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    43271 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/dealershootself.png
+-rw-------   0 gqx       (1000) gqx       (1000)    97047 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/gun.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    61801 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/handcuff.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    64423 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/knife.png
+-rwx------   0 gqx       (1000) gqx       (1000)    96078 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/livedealer.wav
+-rwx------   0 gqx       (1000) gqx       (1000)   432078 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/liveplayer.wav
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    12620 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/liveround.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    15499 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/magnifier.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    34020 2024-04-13 01:14:24.000000 bulletroulette-1.0.5/bulletroulette/assets/noneprop.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)   130200 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/pill.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    43256 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/propbox.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    33816 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/smoke.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)   432984 2024-04-09 13:27:21.000000 bulletroulette-1.0.5/bulletroulette/assets/super.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1143 2024-04-14 02:40:49.000000 bulletroulette-1.0.5/bulletroulette/data.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     3187 2024-04-14 02:40:51.000000 bulletroulette-1.0.5/bulletroulette/roles.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    13591 2024-05-02 11:09:39.000000 bulletroulette-1.0.5/bulletroulette/run.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1009 2024-04-14 02:41:24.000000 bulletroulette-1.0.5/bulletroulette/sprites.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-05-02 11:11:30.530979 bulletroulette-1.0.5/bulletroulette.egg-info/
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     4119 2024-05-02 11:11:30.000000 bulletroulette-1.0.5/bulletroulette.egg-info/PKG-INFO
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1867 2024-05-02 11:11:30.000000 bulletroulette-1.0.5/bulletroulette.egg-info/SOURCES.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-05-02 11:11:30.000000 bulletroulette-1.0.5/bulletroulette.egg-info/dependency_links.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       14 2024-05-02 11:11:30.000000 bulletroulette-1.0.5/bulletroulette.egg-info/requires.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       15 2024-05-02 11:11:30.000000 bulletroulette-1.0.5/bulletroulette.egg-info/top_level.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-05-02 11:11:30.534979 bulletroulette-1.0.5/setup.cfg
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1568 2024-05-02 11:11:24.000000 bulletroulette-1.0.5/setup.py
```

### Comparing `bulletroulette-1.0.4/LICENSE` & `bulletroulette-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/PKG-INFO` & `bulletroulette-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bulletroulette
-Version: 1.0.4
-Summary: 模仿steam游戏“恶魔轮盘”，目前没有提供开发接口（只能单纯玩）
+Version: 1.0.5
+Summary: 模仿steam游戏“恶魔轮盘”
 Home-page: https://github.com/BinaryGuo/Buckshot_Roulette
 Author: GQX
 Author-email: kill114514251@outlook.com
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `bulletroulette-1.0.4/README.md` & `bulletroulette-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/A.png` & `bulletroulette-1.0.5/bulletroulette/assets/A.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/B.png` & `bulletroulette-1.0.5/bulletroulette/assets/B.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/C.png` & `bulletroulette-1.0.5/bulletroulette/assets/C.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/D.png` & `bulletroulette-1.0.5/bulletroulette/assets/D.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/DELETE.png` & `bulletroulette-1.0.5/bulletroulette/assets/DELETE.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/E.png` & `bulletroulette-1.0.5/bulletroulette/assets/E.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/ENTER.png` & `bulletroulette-1.0.5/bulletroulette/assets/ENTER.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/F.png` & `bulletroulette-1.0.5/bulletroulette/assets/F.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/G.png` & `bulletroulette-1.0.5/bulletroulette/assets/G.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/H.png` & `bulletroulette-1.0.5/bulletroulette/assets/H.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/I.png` & `bulletroulette-1.0.5/bulletroulette/assets/I.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/J.png` & `bulletroulette-1.0.5/bulletroulette/assets/J.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/K.png` & `bulletroulette-1.0.5/bulletroulette/assets/K.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/L.png` & `bulletroulette-1.0.5/bulletroulette/assets/L.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/M.png` & `bulletroulette-1.0.5/bulletroulette/assets/M.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/N.png` & `bulletroulette-1.0.5/bulletroulette/assets/N.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/O.png` & `bulletroulette-1.0.5/bulletroulette/assets/O.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/P.png` & `bulletroulette-1.0.5/bulletroulette/assets/P.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/Q.png` & `bulletroulette-1.0.5/bulletroulette/assets/Q.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/R.png` & `bulletroulette-1.0.5/bulletroulette/assets/R.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/S.png` & `bulletroulette-1.0.5/bulletroulette/assets/S.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/Simhei.ttf` & `bulletroulette-1.0.5/bulletroulette/assets/Simhei.ttf`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/T.png` & `bulletroulette-1.0.5/bulletroulette/assets/T.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/U.png` & `bulletroulette-1.0.5/bulletroulette/assets/U.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/V.png` & `bulletroulette-1.0.5/bulletroulette/assets/V.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/W.png` & `bulletroulette-1.0.5/bulletroulette/assets/W.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/X.png` & `bulletroulette-1.0.5/bulletroulette/assets/X.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/Y.png` & `bulletroulette-1.0.5/bulletroulette/assets/Y.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/Z.png` & `bulletroulette-1.0.5/bulletroulette/assets/Z.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/beer.png` & `bulletroulette-1.0.5/bulletroulette/assets/beer.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/bg.png` & `bulletroulette-1.0.5/bulletroulette/assets/bg.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/bgmsc.ogg` & `bulletroulette-1.0.5/bulletroulette/assets/bgmsc.ogg`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/blank.png` & `bulletroulette-1.0.5/bulletroulette/assets/blank.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/blank.wav` & `bulletroulette-1.0.5/bulletroulette/assets/blank.wav`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/charge.png` & `bulletroulette-1.0.5/bulletroulette/assets/charge.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/dealershootplayer.png` & `bulletroulette-1.0.5/bulletroulette/assets/dealershootplayer.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/dealershootself.png` & `bulletroulette-1.0.5/bulletroulette/assets/dealershootself.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/gun.png` & `bulletroulette-1.0.5/bulletroulette/assets/gun.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/handcuff.png` & `bulletroulette-1.0.5/bulletroulette/assets/handcuff.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/knife.png` & `bulletroulette-1.0.5/bulletroulette/assets/knife.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/livedealer.wav` & `bulletroulette-1.0.5/bulletroulette/assets/livedealer.wav`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/liveplayer.wav` & `bulletroulette-1.0.5/bulletroulette/assets/liveplayer.wav`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/liveround.png` & `bulletroulette-1.0.5/bulletroulette/assets/liveround.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/magnifier.png` & `bulletroulette-1.0.5/bulletroulette/assets/magnifier.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/noneprop.png` & `bulletroulette-1.0.5/bulletroulette/assets/noneprop.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/pill.png` & `bulletroulette-1.0.5/bulletroulette/assets/pill.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/propbox.png` & `bulletroulette-1.0.5/bulletroulette/assets/propbox.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/smoke.png` & `bulletroulette-1.0.5/bulletroulette/assets/smoke.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/assets/super.png` & `bulletroulette-1.0.5/bulletroulette/assets/super.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/data.py` & `bulletroulette-1.0.5/bulletroulette/data.py`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/roles.py` & `bulletroulette-1.0.5/bulletroulette/roles.py`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette/run.py` & `bulletroulette-1.0.5/bulletroulette/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# 主程序（没错，运行它！）
-__version__ = "1.0" # 版本说明（没什么用）
-
 # 外部导入
 cannotuseGUI = False
 from random import shuffle
 from time import sleep
 import pygame
 from os import chdir,path
 from traceback import print_exc
@@ -274,20 +271,19 @@
                                     next = 0
                                 else:
                                     print("咔......")
                         if dealer.gethealth() == 0 or player.gethealth() == 0:exit()
                         sleep(1.5)
                 del dealer
                 del player
-    except KeyboardInterrupt:
-        print("\n检测到^C")
-        exit()
+    except KeyboardInterrupt:print("\n检测到^C")
     except SystemExit:pass
     except:
         print("抱歉，我们检测到了一个错误，这可能不是您造成的，但您无法继续进行游戏了")
         print("错误信息：")
         print_exc()
     print("游戏结束!")
     print("感谢您的游玩!")
     print("名称:Buckshot Roulette（恶魔轮盘赌）")
     print("版本：1.0")
-    print("LevoLet Inc.")
+    print("LevoLet Inc.")
+    pygame.quit()
```

### Comparing `bulletroulette-1.0.4/bulletroulette/sprites.py` & `bulletroulette-1.0.5/bulletroulette/sprites.py`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.4/bulletroulette.egg-info/PKG-INFO` & `bulletroulette-1.0.5/bulletroulette.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bulletroulette
-Version: 1.0.4
-Summary: 模仿steam游戏“恶魔轮盘”，目前没有提供开发接口（只能单纯玩）
+Version: 1.0.5
+Summary: 模仿steam游戏“恶魔轮盘”
 Home-page: https://github.com/BinaryGuo/Buckshot_Roulette
 Author: GQX
 Author-email: kill114514251@outlook.com
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `bulletroulette-1.0.4/bulletroulette.egg-info/SOURCES.txt` & `bulletroulette-1.0.5/bulletroulette.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 bulletroulette/__init__.py
 bulletroulette/data.py
 bulletroulette/roles.py
 bulletroulette/run.py
 bulletroulette/sprites.py
 bulletroulette.egg-info/PKG-INFO
```

### Comparing `bulletroulette-1.0.4/setup.py` & `bulletroulette-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="bulletroulette",  # 模块名称
-    version="1.0.4",  # 当前版本
+    version="1.0.5",  # 当前版本
     author="GQX",  # 作者
     author_email="kill114514251@outlook.com",  # 作者邮箱
-    description="模仿steam游戏“恶魔轮盘”，目前没有提供开发接口（只能单纯玩）",  # 模块简介
+    description="模仿steam游戏“恶魔轮盘”",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     url="https://github.com/BinaryGuo/Buckshot_Roulette",  # 模块github地址
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     include_package_data=True,
     package_data={
         "bulletroulette" : ["assets/*.png","assets/*.ogg","assets/*.ttf","assets/*.wav"]
@@ -31,8 +31,8 @@
         "Programming Language :: Python :: 3.8",
     ],
     # 依赖模块
     install_requires=[
         "pygame>=2.0.1",
     ],
     python_requires=">=3.8",
-)
+)
```

