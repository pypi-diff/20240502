# Comparing `tmp/musicntwrk-2.3.3.tar.gz` & `tmp/musicntwrk-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicntwrk-2.3.3.tar", last modified: Thu Apr 25 20:52:17 2024, max compression
+gzip compressed data, was "musicntwrk-2.3.4.tar", last modified: Wed May  1 22:15:44 2024, max compression
```

## Comparing `musicntwrk-2.3.3.tar` & `musicntwrk-2.3.4.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.102902 musicntwrk-2.3.3/
--rw-r--r--   0 marco      (502) staff       (20)     7568 2024-04-25 20:52:17.102331 musicntwrk-2.3.3/PKG-INFO
--rw-r--r--   0 marco      (502) staff       (20)     6849 2022-07-24 12:39:52.000000 musicntwrk-2.3.3/README.md
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.101362 musicntwrk-2.3.3/musicntwrk.egg-info/
--rw-r--r--   0 marco      (502) staff       (20)     7568 2024-04-25 20:52:16.000000 musicntwrk-2.3.3/musicntwrk.egg-info/PKG-INFO
--rw-r--r--   0 marco      (502) staff       (20)     4795 2024-04-25 20:52:16.000000 musicntwrk-2.3.3/musicntwrk.egg-info/SOURCES.txt
--rw-r--r--   0 marco      (502) staff       (20)        1 2024-04-25 20:52:16.000000 musicntwrk-2.3.3/musicntwrk.egg-info/dependency_links.txt
--rw-r--r--   0 marco      (502) staff       (20)      159 2024-04-25 20:52:16.000000 musicntwrk-2.3.3/musicntwrk.egg-info/requires.txt
--rw-r--r--   0 marco      (502) staff       (20)       11 2024-04-25 20:52:16.000000 musicntwrk-2.3.3/musicntwrk.egg-info/top_level.txt
--rw-r--r--   0 marco      (502) staff       (20)       97 2023-06-23 22:57:58.000000 musicntwrk-2.3.3/pyproject.toml
--rw-r--r--   0 marco      (502) staff       (20)       38 2024-04-25 20:52:17.103032 musicntwrk-2.3.3/setup.cfg
--rw-r--r--   0 marco      (502) staff       (20)     1508 2024-04-25 20:51:55.000000 musicntwrk-2.3.3/setup.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:16.998073 musicntwrk-2.3.3/src/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/__init__.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.000553 musicntwrk-2.3.3/src/comptools/
--rw-r--r--   0 marco      (502) staff       (20)    39621 2021-05-31 23:27:25.000000 musicntwrk-2.3.3/src/comptools/MidiFile.py
--rw-r--r--   0 marco      (502) staff       (20)     1762 2024-03-14 00:36:27.000000 musicntwrk-2.3.3/src/comptools/displayNotes.py
--rw-r--r--   0 marco      (502) staff       (20)     2786 2021-09-23 16:53:48.000000 musicntwrk-2.3.3/src/comptools/genmidi.py
--rw-r--r--   0 marco      (502) staff       (20)     7771 2023-05-25 20:48:36.000000 musicntwrk-2.3.3/src/comptools/music.py
--rw-r--r--   0 marco      (502) staff       (20)     1888 2021-05-31 23:27:25.000000 musicntwrk-2.3.3/src/comptools/notation.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.010514 musicntwrk-2.3.3/src/data/
--rw-r--r--   0 marco      (502) staff       (20)      828 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/MIDImap.py
--rw-r--r--   0 marco      (502) staff       (20)     2559 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/MIDImidi.py
--rw-r--r--   0 marco      (502) staff       (20)      988 2023-05-25 21:55:41.000000 musicntwrk-2.3.3/src/data/MIDIscore.py
--rw-r--r--   0 marco      (502) staff       (20)     1275 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/WRITEscore.py
--rw-r--r--   0 marco      (502) staff       (20)     1013 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/WRITEscoreNoTime.py
--rw-r--r--   0 marco      (502) staff       (20)     2086 2023-01-08 21:25:29.000000 musicntwrk-2.3.3/src/data/WRITEscoreOps.py
--rw-r--r--   0 marco      (502) staff       (20)     3272 2021-10-26 23:20:31.000000 musicntwrk-2.3.3/src/data/WRITEscoreOpsMIDI.py
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2926 2024-04-24 14:50:20.000000 musicntwrk-2.3.3/src/data/analyzeSound.py
--rw-r--r--   0 marco      (502) staff       (20)     3956 2024-04-24 14:50:18.000000 musicntwrk-2.3.3/src/data/analyzeTimbre.py
--rw-r--r--   0 marco      (502) staff       (20)   114667 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/ctcsound.py
--rw-r--r--   0 marco      (502) staff       (20)     3993 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/i_spectral.py
--rw-r--r--   0 marco      (502) staff       (20)     3275 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/i_spectral2.py
--rw-r--r--   0 marco      (502) staff       (20)     1921 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/i_spectral_pure.py
--rw-r--r--   0 marco      (502) staff       (20)     2597 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/i_spectral_pyo.py
--rw-r--r--   0 marco      (502) staff       (20)     6358 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/i_time_series.py
--rw-r--r--   0 marco      (502) staff       (20)     1270 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/r_1Ddata.py
--rw-r--r--   0 marco      (502) staff       (20)    10624 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/data/scaleMapping.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.024520 musicntwrk-2.3.3/src/harmony/
--rw-r--r--   0 marco      (502) staff       (20)       66 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2035 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/applyOps.py
--rw-r--r--   0 marco      (502) staff       (20)     1256 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/changePoint.py
--rw-r--r--   0 marco      (502) staff       (20)     2640 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/chinese_postman.py
--rw-r--r--   0 marco      (502) staff       (20)     1703 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/enharmonicDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     1309 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/getRN.py
--rw-r--r--   0 marco      (502) staff       (20)     4084 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/harmonicDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     3055 2024-04-24 15:25:04.000000 musicntwrk-2.3.3/src/harmony/keySections.py
--rw-r--r--   0 marco      (502) staff       (20)     3022 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/lookupOps.py
--rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/lookupProgr.py
--rw-r--r--   0 marco      (502) staff       (20)     1265 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/lookupWrapper.py
--rw-r--r--   0 marco      (502) staff       (20)     2416 2023-08-02 08:26:29.000000 musicntwrk-2.3.3/src/harmony/networkHarmonyGen.py
--rw-r--r--   0 marco      (502) staff       (20)     2769 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/plotHarmonicTable.py
--rw-r--r--   0 marco      (502) staff       (20)     2784 2023-12-28 02:44:32.000000 musicntwrk-2.3.3/src/harmony/rhythmicDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     4765 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/scoreAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     1257 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/scoreDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     2307 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/scoreFilter.py
--rw-r--r--   0 marco      (502) staff       (20)     2492 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/shortHands.py
--rw-r--r--   0 marco      (502) staff       (20)     2002 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/showAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     4473 2023-08-02 08:24:19.000000 musicntwrk-2.3.3/src/harmony/spiralChordSpace.py
--rw-r--r--   0 marco      (502) staff       (20)     2921 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/tonalAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     7685 2023-01-27 02:25:22.000000 musicntwrk-2.3.3/src/harmony/tonalHarmonyCalculator.py
--rw-r--r--   0 marco      (502) staff       (20)     4652 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/tonalHarmonyModels.py
--rw-r--r--   0 marco      (502) staff       (20)     1899 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/harmony/tonalPartition.py
--rw-r--r--   0 marco      (502) staff       (20)     2647 2024-04-24 21:17:23.000000 musicntwrk-2.3.3/src/harmony/tonnentz.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.029037 musicntwrk-2.3.3/src/ml_utils/
--rw-r--r--   0 marco      (502) staff       (20)       88 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/ml_utils/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2695 2024-04-14 21:34:16.000000 musicntwrk-2.3.3/src/ml_utils/checkRun.py
--rw-r--r--   0 marco      (502) staff       (20)     1407 2024-04-14 21:35:54.000000 musicntwrk-2.3.3/src/ml_utils/modelDump.py
--rw-r--r--   0 marco      (502) staff       (20)     1479 2024-04-14 22:54:15.000000 musicntwrk-2.3.3/src/ml_utils/modelLoad.py
--rw-r--r--   0 marco      (502) staff       (20)     1513 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/ml_utils/multiModelPredictor.py
--rw-r--r--   0 marco      (502) staff       (20)     1432 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/ml_utils/prepareDataSet.py
--rw-r--r--   0 marco      (502) staff       (20)     2024 2024-04-15 02:03:11.000000 musicntwrk-2.3.3/src/ml_utils/readModels.py
--rw-r--r--   0 marco      (502) staff       (20)      814 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/ml_utils/scaleDataSet.py
--rw-r--r--   0 marco      (502) staff       (20)     3299 2024-04-14 22:01:21.000000 musicntwrk-2.3.3/src/ml_utils/trainCNNmodel.py
--rw-r--r--   0 marco      (502) staff       (20)     2260 2024-04-14 21:50:15.000000 musicntwrk-2.3.3/src/ml_utils/trainNNmodel.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.038905 musicntwrk-2.3.3/src/msctools/
--rw-r--r--   0 marco      (502) staff       (20)     8840 2023-01-15 21:28:01.000000 musicntwrk-2.3.3/src/msctools/base.py
--rw-r--r--   0 marco      (502) staff       (20)      597 2024-04-20 12:53:06.000000 musicntwrk-2.3.3/src/msctools/cfg.py
--rw-r--r--   0 marco      (502) staff       (20)     2248 2023-09-08 07:15:36.000000 musicntwrk-2.3.3/src/msctools/converters.py
--rw-r--r--   0 marco      (502) staff       (20)      336 2024-01-30 00:27:07.000000 musicntwrk-2.3.3/src/msctools/decorators.py
--rw-r--r--   0 marco      (502) staff       (20)     7069 2022-12-03 20:17:50.000000 musicntwrk-2.3.3/src/msctools/devices.py
--rw-r--r--   0 marco      (502) staff       (20)    78504 2024-01-20 15:29:09.000000 musicntwrk-2.3.3/src/msctools/dictionaries.py
--rw-r--r--   0 marco      (502) staff       (20)    48647 2023-11-09 23:14:46.000000 musicntwrk-2.3.3/src/msctools/dsp.py
--rw-r--r--   0 marco      (502) staff       (20)     5940 2024-04-17 17:59:59.000000 musicntwrk-2.3.3/src/msctools/envelopes.py
--rw-r--r--   0 marco      (502) staff       (20)     6152 2024-04-24 14:23:33.000000 musicntwrk-2.3.3/src/msctools/envelopes_thread.py
--rw-r--r--   0 marco      (502) staff       (20)    19624 2024-04-20 12:45:11.000000 musicntwrk-2.3.3/src/msctools/networks.py
--rw-r--r--   0 marco      (502) staff       (20)      865 2023-04-13 16:06:16.000000 musicntwrk-2.3.3/src/msctools/oscserver.py
--rw-r--r--   0 marco      (502) staff       (20)     1285 2022-12-20 16:04:25.000000 musicntwrk-2.3.3/src/msctools/osctools.py
--rw-r--r--   0 marco      (502) staff       (20)      472 2022-11-22 00:46:09.000000 musicntwrk-2.3.3/src/msctools/pan.py
--rw-r--r--   0 marco      (502) staff       (20)     4807 2024-04-20 12:31:37.000000 musicntwrk-2.3.3/src/msctools/players.py
--rw-r--r--   0 marco      (502) staff       (20)     4914 2024-04-24 14:23:35.000000 musicntwrk-2.3.3/src/msctools/players_thread.py
--rw-r--r--   0 marco      (502) staff       (20)     1637 2024-02-13 23:17:01.000000 musicntwrk-2.3.3/src/msctools/pyoPlayer.py
--rw-r--r--   0 marco      (502) staff       (20)    17002 2024-04-20 13:03:26.000000 musicntwrk-2.3.3/src/msctools/pyotools.py
--rw-r--r--   0 marco      (502) staff       (20)     1355 2024-04-20 12:31:32.000000 musicntwrk-2.3.3/src/msctools/session.py
--rw-r--r--   0 marco      (502) staff       (20)      434 2023-01-02 23:35:19.000000 musicntwrk-2.3.3/src/msctools/utils.py
--rw-r--r--   0 marco      (502) staff       (20)     5386 2023-04-13 16:05:54.000000 musicntwrk-2.3.3/src/msctools/videocapture.py
--rw-r--r--   0 marco      (502) staff       (20)    68822 2024-01-26 02:18:22.000000 musicntwrk-2.3.3/src/musicntwrk.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.049177 musicntwrk-2.3.3/src/networks/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/networks/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2580 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/analysisNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2646 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/orchestralNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2388 2023-04-04 23:24:43.000000 musicntwrk-2.3.3/src/networks/orchestralVector.py
--rw-r--r--   0 marco      (502) staff       (20)     1695 2024-04-24 21:12:18.000000 musicntwrk-2.3.3/src/networks/orchestralVectorColor.py
--rw-r--r--   0 marco      (502) staff       (20)     4853 2024-04-24 15:27:50.000000 musicntwrk-2.3.3/src/networks/pcsDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     5852 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/pcsEgoNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4914 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/pcsNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2966 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/rLeadNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2470 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/networks/readScore.py
--rw-r--r--   0 marco      (502) staff       (20)     3085 2022-01-09 00:40:38.000000 musicntwrk-2.3.3/src/networks/rhythmDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     4322 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/rhythmNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4053 2023-12-28 02:35:13.000000 musicntwrk-2.3.3/src/networks/rhythmPDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     2456 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/networks/scoreDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     1592 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/networks/scoreMIDIDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     5809 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/scoreNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     5791 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/scoreSubNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     3697 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/timbralNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4102 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/vLeadNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4789 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/vLeadNetworkByName.py
--rw-r--r--   0 marco      (502) staff       (20)     2936 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/vLeadNetworkByNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)     2634 2023-08-02 08:22:01.000000 musicntwrk-2.3.3/src/networks/vLeadNetworkVec.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.054851 musicntwrk-2.3.3/src/plotting/
--rw-r--r--   0 marco      (502) staff       (20)     1066 2024-04-24 14:50:17.000000 musicntwrk-2.3.3/src/plotting/barplot.py
--rw-r--r--   0 marco      (502) staff       (20)    24919 2023-12-21 02:30:18.000000 musicntwrk-2.3.3/src/plotting/chordspace.py
--rw-r--r--   0 marco      (502) staff       (20)     7250 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/plotting/drawMultiLayerNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2888 2023-07-05 22:49:56.000000 musicntwrk-2.3.3/src/plotting/drawNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     6340 2023-08-02 09:17:49.000000 musicntwrk-2.3.3/src/plotting/drawNetwork3D.py
--rw-r--r--   0 marco      (502) staff       (20)     2256 2021-11-23 20:31:22.000000 musicntwrk-2.3.3/src/plotting/drawNetworkViz.py
--rw-r--r--   0 marco      (502) staff       (20)     1246 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/plotting/drawNetworkX.py
--rw-r--r--   0 marco      (502) staff       (20)      895 2024-04-24 14:50:15.000000 musicntwrk-2.3.3/src/plotting/plotCC.py
--rw-r--r--   0 marco      (502) staff       (20)      716 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/plotting/plotCurveXY.py
--rw-r--r--   0 marco      (502) staff       (20)      711 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/plotting/plotCurveY.py
--rw-r--r--   0 marco      (502) staff       (20)     1680 2023-08-02 14:25:53.000000 musicntwrk-2.3.3/src/plotting/plotDegreeAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     1869 2024-04-24 14:50:13.000000 musicntwrk-2.3.3/src/plotting/plotOpsHistogram.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.084419 musicntwrk-2.3.3/src/timbre/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/timbre/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     1743 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/timbre/computeASCBW.py
--rw-r--r--   0 marco      (502) staff       (20)     1552 2023-04-04 23:13:40.000000 musicntwrk-2.3.3/src/timbre/computeCompMPS.py
--rw-r--r--   0 marco      (502) staff       (20)     1663 2023-04-04 23:14:32.000000 musicntwrk-2.3.3/src/timbre/computeMFCC.py
--rw-r--r--   0 marco      (502) staff       (20)     2653 2024-04-24 14:50:11.000000 musicntwrk-2.3.3/src/timbre/computeModifiedASCBW.py
--rw-r--r--   0 marco      (502) staff       (20)     1475 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/timbre/computePSCC.py
--rw-r--r--   0 marco      (502) staff       (20)     2263 2023-06-23 21:10:40.000000 musicntwrk-2.3.3/src/timbre/computeStandardizedMFCC.py
--rw-r--r--   0 marco      (502) staff       (20)     1769 2022-10-29 00:31:52.000000 musicntwrk-2.3.3/src/timbre/computeStandardizedMFPS.py
--rw-r--r--   0 marco      (502) staff       (20)     1926 2022-10-29 00:31:50.000000 musicntwrk-2.3.3/src/timbre/computeStandardizedPSCC.py
--rw-r--r--   0 marco      (502) staff       (20)     1194 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/timbre/mfccSoundDecay.py
--rw-r--r--   0 marco      (502) staff       (20)      848 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/timbre/mfccSoundDecayOptimal.py
--rw-r--r--   0 marco      (502) staff       (20)     1395 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/timbre/mfccSoundDecayPiecewise.py
--rw-r--r--   0 marco      (502) staff       (20)     2092 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/timbre/minimizeBKPT.py
--rw-r--r--   0 marco      (502) staff       (20)      974 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/timbre/normSoundDecay.py
--rw-r--r--   0 marco      (502) staff       (20)     1342 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/timbre/normSoundDecay2.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-25 20:52:17.100818 musicntwrk-2.3.3/src/utils/
--rw-r--r--   0 marco      (502) staff       (20)     1142 2023-05-25 21:57:17.000000 musicntwrk-2.3.3/src/utils/Remove.py
--rw-r--r--   0 marco      (502) staff       (20)     1962 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/SegmentedLinearReg.py
--rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/Sublists.py
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     3121 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/communications.py
--rw-r--r--   0 marco      (502) staff       (20)     9768 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/diffusionEntropyAnalyis.py
--rw-r--r--   0 marco      (502) staff       (20)     5511 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/diffusionEntropyAnalyisNew.py
--rw-r--r--   0 marco      (502) staff       (20)     1758 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/entropyKLdiv.py
--rw-r--r--   0 marco      (502) staff       (20)     1005 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/extractByString.py
--rw-r--r--   0 marco      (502) staff       (20)      830 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/fetchWaves.py
--rw-r--r--   0 marco      (502) staff       (20)     1086 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/findLengthMax.py
--rw-r--r--   0 marco      (502) staff       (20)      883 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/flatten.py
--rw-r--r--   0 marco      (502) staff       (20)      591 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/floatize.py
--rw-r--r--   0 marco      (502) staff       (20)     1669 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/generalizedOpsHistogram.py
--rw-r--r--   0 marco      (502) staff       (20)     1541 2022-06-24 15:34:43.000000 musicntwrk-2.3.3/src/utils/generalizedOpsName.py
--rw-r--r--   0 marco      (502) staff       (20)      760 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/init_list_of_objects.py
--rw-r--r--   0 marco      (502) staff       (20)     1700 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/load_balancing.py
--rw-r--r--   0 marco      (502) staff       (20)     1398 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/minimalDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1297 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/minimalDistanceVec.py
--rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/minimalNoBijDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1053 2021-11-19 16:54:18.000000 musicntwrk-2.3.3/src/utils/opsCheckByName.py
--rw-r--r--   0 marco      (502) staff       (20)      827 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/opsCheckByNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)      878 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/opsDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1653 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/opsHistogram.py
--rw-r--r--   0 marco      (502) staff       (20)     1537 2021-11-12 22:37:47.000000 musicntwrk-2.3.3/src/utils/opsName.py
--rw-r--r--   0 marco      (502) staff       (20)     2413 2021-11-19 01:35:52.000000 musicntwrk-2.3.3/src/utils/opsNameFull.py
--rw-r--r--   0 marco      (502) staff       (20)     1638 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/opsNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)      721 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/play_with_simpleaudio.py
--rw-r--r--   0 marco      (502) staff       (20)     4681 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/powerFit.py
--rw-r--r--   0 marco      (502) staff       (20)     1384 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/rhythmDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     2605 2021-08-06 01:36:29.000000 musicntwrk-2.3.3/src/utils/scaleFreeFit.py
--rw-r--r--   0 marco      (502) staff       (20)     1130 2021-11-22 17:37:40.000000 musicntwrk-2.3.3/src/utils/score2vLead.py
--rw-r--r--   0 marco      (502) staff       (20)      730 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/str2float.py
--rw-r--r--   0 marco      (502) staff       (20)      702 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/str2frac.py
--rw-r--r--   0 marco      (502) staff       (20)      963 2021-06-25 20:55:30.000000 musicntwrk-2.3.3/src/utils/vectorDistance.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.335737 musicntwrk-2.3.4/
+-rw-r--r--   0 marco      (502) staff       (20)     7568 2024-05-01 22:15:44.335084 musicntwrk-2.3.4/PKG-INFO
+-rw-r--r--   0 marco      (502) staff       (20)     6849 2022-07-24 12:39:52.000000 musicntwrk-2.3.4/README.md
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.334071 musicntwrk-2.3.4/musicntwrk.egg-info/
+-rw-r--r--   0 marco      (502) staff       (20)     7568 2024-05-01 22:15:44.000000 musicntwrk-2.3.4/musicntwrk.egg-info/PKG-INFO
+-rw-r--r--   0 marco      (502) staff       (20)     4795 2024-05-01 22:15:44.000000 musicntwrk-2.3.4/musicntwrk.egg-info/SOURCES.txt
+-rw-r--r--   0 marco      (502) staff       (20)        1 2024-05-01 22:15:44.000000 musicntwrk-2.3.4/musicntwrk.egg-info/dependency_links.txt
+-rw-r--r--   0 marco      (502) staff       (20)      159 2024-05-01 22:15:44.000000 musicntwrk-2.3.4/musicntwrk.egg-info/requires.txt
+-rw-r--r--   0 marco      (502) staff       (20)       11 2024-05-01 22:15:44.000000 musicntwrk-2.3.4/musicntwrk.egg-info/top_level.txt
+-rw-r--r--   0 marco      (502) staff       (20)       97 2023-06-23 22:57:58.000000 musicntwrk-2.3.4/pyproject.toml
+-rw-r--r--   0 marco      (502) staff       (20)       38 2024-05-01 22:15:44.335864 musicntwrk-2.3.4/setup.cfg
+-rw-r--r--   0 marco      (502) staff       (20)     1508 2024-05-01 16:13:22.000000 musicntwrk-2.3.4/setup.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.227079 musicntwrk-2.3.4/src/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/__init__.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.230245 musicntwrk-2.3.4/src/comptools/
+-rw-r--r--   0 marco      (502) staff       (20)    39621 2021-05-31 23:27:25.000000 musicntwrk-2.3.4/src/comptools/MidiFile.py
+-rw-r--r--   0 marco      (502) staff       (20)     1762 2024-03-14 00:36:27.000000 musicntwrk-2.3.4/src/comptools/displayNotes.py
+-rw-r--r--   0 marco      (502) staff       (20)     2786 2021-09-23 16:53:48.000000 musicntwrk-2.3.4/src/comptools/genmidi.py
+-rw-r--r--   0 marco      (502) staff       (20)     7771 2023-05-25 20:48:36.000000 musicntwrk-2.3.4/src/comptools/music.py
+-rw-r--r--   0 marco      (502) staff       (20)     1888 2021-05-31 23:27:25.000000 musicntwrk-2.3.4/src/comptools/notation.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.240026 musicntwrk-2.3.4/src/data/
+-rw-r--r--   0 marco      (502) staff       (20)      828 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/MIDImap.py
+-rw-r--r--   0 marco      (502) staff       (20)     2559 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/MIDImidi.py
+-rw-r--r--   0 marco      (502) staff       (20)      988 2023-05-25 21:55:41.000000 musicntwrk-2.3.4/src/data/MIDIscore.py
+-rw-r--r--   0 marco      (502) staff       (20)     1275 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/WRITEscore.py
+-rw-r--r--   0 marco      (502) staff       (20)     1013 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/WRITEscoreNoTime.py
+-rw-r--r--   0 marco      (502) staff       (20)     2086 2023-01-08 21:25:29.000000 musicntwrk-2.3.4/src/data/WRITEscoreOps.py
+-rw-r--r--   0 marco      (502) staff       (20)     3272 2021-10-26 23:20:31.000000 musicntwrk-2.3.4/src/data/WRITEscoreOpsMIDI.py
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2926 2024-04-24 14:50:20.000000 musicntwrk-2.3.4/src/data/analyzeSound.py
+-rw-r--r--   0 marco      (502) staff       (20)     3956 2024-04-24 14:50:18.000000 musicntwrk-2.3.4/src/data/analyzeTimbre.py
+-rw-r--r--   0 marco      (502) staff       (20)   114667 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/ctcsound.py
+-rw-r--r--   0 marco      (502) staff       (20)     3993 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/i_spectral.py
+-rw-r--r--   0 marco      (502) staff       (20)     3275 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/i_spectral2.py
+-rw-r--r--   0 marco      (502) staff       (20)     1921 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/i_spectral_pure.py
+-rw-r--r--   0 marco      (502) staff       (20)     2597 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/i_spectral_pyo.py
+-rw-r--r--   0 marco      (502) staff       (20)     6358 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/i_time_series.py
+-rw-r--r--   0 marco      (502) staff       (20)     1270 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/r_1Ddata.py
+-rw-r--r--   0 marco      (502) staff       (20)    10624 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/data/scaleMapping.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.252531 musicntwrk-2.3.4/src/harmony/
+-rw-r--r--   0 marco      (502) staff       (20)       66 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2035 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/applyOps.py
+-rw-r--r--   0 marco      (502) staff       (20)     1256 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/changePoint.py
+-rw-r--r--   0 marco      (502) staff       (20)     2640 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/chinese_postman.py
+-rw-r--r--   0 marco      (502) staff       (20)     1703 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/enharmonicDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     1309 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/getRN.py
+-rw-r--r--   0 marco      (502) staff       (20)     4137 2024-04-30 22:40:21.000000 musicntwrk-2.3.4/src/harmony/harmonicDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     3055 2024-04-24 15:25:04.000000 musicntwrk-2.3.4/src/harmony/keySections.py
+-rw-r--r--   0 marco      (502) staff       (20)     3022 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/lookupOps.py
+-rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/lookupProgr.py
+-rw-r--r--   0 marco      (502) staff       (20)     1265 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/lookupWrapper.py
+-rw-r--r--   0 marco      (502) staff       (20)     2416 2023-08-02 08:26:29.000000 musicntwrk-2.3.4/src/harmony/networkHarmonyGen.py
+-rw-r--r--   0 marco      (502) staff       (20)     2769 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/plotHarmonicTable.py
+-rw-r--r--   0 marco      (502) staff       (20)     2784 2023-12-28 02:44:32.000000 musicntwrk-2.3.4/src/harmony/rhythmicDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     4765 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/scoreAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     1257 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/scoreDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     2307 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/scoreFilter.py
+-rw-r--r--   0 marco      (502) staff       (20)     2492 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/shortHands.py
+-rw-r--r--   0 marco      (502) staff       (20)     2002 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/showAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     4473 2023-08-02 08:24:19.000000 musicntwrk-2.3.4/src/harmony/spiralChordSpace.py
+-rw-r--r--   0 marco      (502) staff       (20)     2921 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/tonalAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     7685 2023-01-27 02:25:22.000000 musicntwrk-2.3.4/src/harmony/tonalHarmonyCalculator.py
+-rw-r--r--   0 marco      (502) staff       (20)     4652 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/tonalHarmonyModels.py
+-rw-r--r--   0 marco      (502) staff       (20)     1899 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/harmony/tonalPartition.py
+-rw-r--r--   0 marco      (502) staff       (20)     2647 2024-04-24 21:17:23.000000 musicntwrk-2.3.4/src/harmony/tonnentz.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.257493 musicntwrk-2.3.4/src/ml_utils/
+-rw-r--r--   0 marco      (502) staff       (20)       88 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/ml_utils/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2695 2024-04-14 21:34:16.000000 musicntwrk-2.3.4/src/ml_utils/checkRun.py
+-rw-r--r--   0 marco      (502) staff       (20)     1407 2024-04-14 21:35:54.000000 musicntwrk-2.3.4/src/ml_utils/modelDump.py
+-rw-r--r--   0 marco      (502) staff       (20)     1479 2024-04-14 22:54:15.000000 musicntwrk-2.3.4/src/ml_utils/modelLoad.py
+-rw-r--r--   0 marco      (502) staff       (20)     1513 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/ml_utils/multiModelPredictor.py
+-rw-r--r--   0 marco      (502) staff       (20)     1432 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/ml_utils/prepareDataSet.py
+-rw-r--r--   0 marco      (502) staff       (20)     2024 2024-04-15 02:03:11.000000 musicntwrk-2.3.4/src/ml_utils/readModels.py
+-rw-r--r--   0 marco      (502) staff       (20)      814 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/ml_utils/scaleDataSet.py
+-rw-r--r--   0 marco      (502) staff       (20)     3299 2024-04-14 22:01:21.000000 musicntwrk-2.3.4/src/ml_utils/trainCNNmodel.py
+-rw-r--r--   0 marco      (502) staff       (20)     2260 2024-04-14 21:50:15.000000 musicntwrk-2.3.4/src/ml_utils/trainNNmodel.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.268540 musicntwrk-2.3.4/src/msctools/
+-rw-r--r--   0 marco      (502) staff       (20)     8840 2023-01-15 21:28:01.000000 musicntwrk-2.3.4/src/msctools/base.py
+-rw-r--r--   0 marco      (502) staff       (20)      597 2024-04-20 12:53:06.000000 musicntwrk-2.3.4/src/msctools/cfg.py
+-rw-r--r--   0 marco      (502) staff       (20)     2248 2023-09-08 07:15:36.000000 musicntwrk-2.3.4/src/msctools/converters.py
+-rw-r--r--   0 marco      (502) staff       (20)      336 2024-01-30 00:27:07.000000 musicntwrk-2.3.4/src/msctools/decorators.py
+-rw-r--r--   0 marco      (502) staff       (20)     7069 2022-12-03 20:17:50.000000 musicntwrk-2.3.4/src/msctools/devices.py
+-rw-r--r--   0 marco      (502) staff       (20)    78504 2024-01-20 15:29:09.000000 musicntwrk-2.3.4/src/msctools/dictionaries.py
+-rw-r--r--   0 marco      (502) staff       (20)    48647 2023-11-09 23:14:46.000000 musicntwrk-2.3.4/src/msctools/dsp.py
+-rw-r--r--   0 marco      (502) staff       (20)     5940 2024-04-17 17:59:59.000000 musicntwrk-2.3.4/src/msctools/envelopes.py
+-rw-r--r--   0 marco      (502) staff       (20)     6152 2024-04-24 14:23:33.000000 musicntwrk-2.3.4/src/msctools/envelopes_thread.py
+-rw-r--r--   0 marco      (502) staff       (20)    19624 2024-04-20 12:45:11.000000 musicntwrk-2.3.4/src/msctools/networks.py
+-rw-r--r--   0 marco      (502) staff       (20)      865 2023-04-13 16:06:16.000000 musicntwrk-2.3.4/src/msctools/oscserver.py
+-rw-r--r--   0 marco      (502) staff       (20)     1285 2022-12-20 16:04:25.000000 musicntwrk-2.3.4/src/msctools/osctools.py
+-rw-r--r--   0 marco      (502) staff       (20)      472 2022-11-22 00:46:09.000000 musicntwrk-2.3.4/src/msctools/pan.py
+-rw-r--r--   0 marco      (502) staff       (20)     4807 2024-04-20 12:31:37.000000 musicntwrk-2.3.4/src/msctools/players.py
+-rw-r--r--   0 marco      (502) staff       (20)     4914 2024-04-24 14:23:35.000000 musicntwrk-2.3.4/src/msctools/players_thread.py
+-rw-r--r--   0 marco      (502) staff       (20)     1637 2024-02-13 23:17:01.000000 musicntwrk-2.3.4/src/msctools/pyoPlayer.py
+-rw-r--r--   0 marco      (502) staff       (20)    17002 2024-04-20 13:03:26.000000 musicntwrk-2.3.4/src/msctools/pyotools.py
+-rw-r--r--   0 marco      (502) staff       (20)     1355 2024-04-20 12:31:32.000000 musicntwrk-2.3.4/src/msctools/session.py
+-rw-r--r--   0 marco      (502) staff       (20)      434 2023-01-02 23:35:19.000000 musicntwrk-2.3.4/src/msctools/utils.py
+-rw-r--r--   0 marco      (502) staff       (20)     5386 2023-04-13 16:05:54.000000 musicntwrk-2.3.4/src/msctools/videocapture.py
+-rw-r--r--   0 marco      (502) staff       (20)    68822 2024-01-26 02:18:22.000000 musicntwrk-2.3.4/src/musicntwrk.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.280212 musicntwrk-2.3.4/src/networks/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/networks/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2580 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/analysisNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2646 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/orchestralNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2388 2023-04-04 23:24:43.000000 musicntwrk-2.3.4/src/networks/orchestralVector.py
+-rw-r--r--   0 marco      (502) staff       (20)     1695 2024-04-24 21:12:18.000000 musicntwrk-2.3.4/src/networks/orchestralVectorColor.py
+-rw-r--r--   0 marco      (502) staff       (20)     4853 2024-04-24 15:27:50.000000 musicntwrk-2.3.4/src/networks/pcsDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     5852 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/pcsEgoNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4914 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/pcsNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2966 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/rLeadNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2470 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/networks/readScore.py
+-rw-r--r--   0 marco      (502) staff       (20)     3085 2022-01-09 00:40:38.000000 musicntwrk-2.3.4/src/networks/rhythmDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     4322 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/rhythmNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4053 2023-12-28 02:35:13.000000 musicntwrk-2.3.4/src/networks/rhythmPDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     2456 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/networks/scoreDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     1592 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/networks/scoreMIDIDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     5809 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/scoreNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     5791 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/scoreSubNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     3697 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/timbralNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4102 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/vLeadNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4789 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/vLeadNetworkByName.py
+-rw-r--r--   0 marco      (502) staff       (20)     2936 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/vLeadNetworkByNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)     2634 2023-08-02 08:22:01.000000 musicntwrk-2.3.4/src/networks/vLeadNetworkVec.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.286387 musicntwrk-2.3.4/src/plotting/
+-rw-r--r--   0 marco      (502) staff       (20)     1066 2024-04-24 14:50:17.000000 musicntwrk-2.3.4/src/plotting/barplot.py
+-rw-r--r--   0 marco      (502) staff       (20)    24919 2023-12-21 02:30:18.000000 musicntwrk-2.3.4/src/plotting/chordspace.py
+-rw-r--r--   0 marco      (502) staff       (20)     7250 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/plotting/drawMultiLayerNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2888 2023-07-05 22:49:56.000000 musicntwrk-2.3.4/src/plotting/drawNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     6340 2023-08-02 09:17:49.000000 musicntwrk-2.3.4/src/plotting/drawNetwork3D.py
+-rw-r--r--   0 marco      (502) staff       (20)     2256 2021-11-23 20:31:22.000000 musicntwrk-2.3.4/src/plotting/drawNetworkViz.py
+-rw-r--r--   0 marco      (502) staff       (20)     1246 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/plotting/drawNetworkX.py
+-rw-r--r--   0 marco      (502) staff       (20)      895 2024-04-24 14:50:15.000000 musicntwrk-2.3.4/src/plotting/plotCC.py
+-rw-r--r--   0 marco      (502) staff       (20)      716 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/plotting/plotCurveXY.py
+-rw-r--r--   0 marco      (502) staff       (20)      711 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/plotting/plotCurveY.py
+-rw-r--r--   0 marco      (502) staff       (20)     1680 2023-08-02 14:25:53.000000 musicntwrk-2.3.4/src/plotting/plotDegreeAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     1869 2024-04-24 14:50:13.000000 musicntwrk-2.3.4/src/plotting/plotOpsHistogram.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.293596 musicntwrk-2.3.4/src/timbre/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/timbre/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     1743 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/timbre/computeASCBW.py
+-rw-r--r--   0 marco      (502) staff       (20)     1552 2023-04-04 23:13:40.000000 musicntwrk-2.3.4/src/timbre/computeCompMPS.py
+-rw-r--r--   0 marco      (502) staff       (20)     1663 2023-04-04 23:14:32.000000 musicntwrk-2.3.4/src/timbre/computeMFCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     2653 2024-04-24 14:50:11.000000 musicntwrk-2.3.4/src/timbre/computeModifiedASCBW.py
+-rw-r--r--   0 marco      (502) staff       (20)     1475 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/timbre/computePSCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     2263 2023-06-23 21:10:40.000000 musicntwrk-2.3.4/src/timbre/computeStandardizedMFCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     1769 2022-10-29 00:31:52.000000 musicntwrk-2.3.4/src/timbre/computeStandardizedMFPS.py
+-rw-r--r--   0 marco      (502) staff       (20)     1926 2022-10-29 00:31:50.000000 musicntwrk-2.3.4/src/timbre/computeStandardizedPSCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     1194 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/timbre/mfccSoundDecay.py
+-rw-r--r--   0 marco      (502) staff       (20)      848 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/timbre/mfccSoundDecayOptimal.py
+-rw-r--r--   0 marco      (502) staff       (20)     1395 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/timbre/mfccSoundDecayPiecewise.py
+-rw-r--r--   0 marco      (502) staff       (20)     2092 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/timbre/minimizeBKPT.py
+-rw-r--r--   0 marco      (502) staff       (20)      974 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/timbre/normSoundDecay.py
+-rw-r--r--   0 marco      (502) staff       (20)     1342 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/timbre/normSoundDecay2.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-05-01 22:15:44.333411 musicntwrk-2.3.4/src/utils/
+-rw-r--r--   0 marco      (502) staff       (20)     1142 2023-05-25 21:57:17.000000 musicntwrk-2.3.4/src/utils/Remove.py
+-rw-r--r--   0 marco      (502) staff       (20)     1962 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/SegmentedLinearReg.py
+-rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/Sublists.py
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     3121 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/communications.py
+-rw-r--r--   0 marco      (502) staff       (20)     9768 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/diffusionEntropyAnalyis.py
+-rw-r--r--   0 marco      (502) staff       (20)     5511 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/diffusionEntropyAnalyisNew.py
+-rw-r--r--   0 marco      (502) staff       (20)     1758 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/entropyKLdiv.py
+-rw-r--r--   0 marco      (502) staff       (20)     1005 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/extractByString.py
+-rw-r--r--   0 marco      (502) staff       (20)      830 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/fetchWaves.py
+-rw-r--r--   0 marco      (502) staff       (20)     1086 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/findLengthMax.py
+-rw-r--r--   0 marco      (502) staff       (20)      883 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/flatten.py
+-rw-r--r--   0 marco      (502) staff       (20)      591 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/floatize.py
+-rw-r--r--   0 marco      (502) staff       (20)     1669 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/generalizedOpsHistogram.py
+-rw-r--r--   0 marco      (502) staff       (20)     1541 2022-06-24 15:34:43.000000 musicntwrk-2.3.4/src/utils/generalizedOpsName.py
+-rw-r--r--   0 marco      (502) staff       (20)      760 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/init_list_of_objects.py
+-rw-r--r--   0 marco      (502) staff       (20)     1700 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/load_balancing.py
+-rw-r--r--   0 marco      (502) staff       (20)     1398 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/minimalDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1297 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/minimalDistanceVec.py
+-rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/minimalNoBijDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1053 2021-11-19 16:54:18.000000 musicntwrk-2.3.4/src/utils/opsCheckByName.py
+-rw-r--r--   0 marco      (502) staff       (20)      827 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/opsCheckByNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)      878 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/opsDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1653 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/opsHistogram.py
+-rw-r--r--   0 marco      (502) staff       (20)     1537 2021-11-12 22:37:47.000000 musicntwrk-2.3.4/src/utils/opsName.py
+-rw-r--r--   0 marco      (502) staff       (20)     2413 2021-11-19 01:35:52.000000 musicntwrk-2.3.4/src/utils/opsNameFull.py
+-rw-r--r--   0 marco      (502) staff       (20)     1638 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/opsNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)      721 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/play_with_simpleaudio.py
+-rw-r--r--   0 marco      (502) staff       (20)     4681 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/powerFit.py
+-rw-r--r--   0 marco      (502) staff       (20)     1384 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/rhythmDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     2605 2021-08-06 01:36:29.000000 musicntwrk-2.3.4/src/utils/scaleFreeFit.py
+-rw-r--r--   0 marco      (502) staff       (20)     1130 2021-11-22 17:37:40.000000 musicntwrk-2.3.4/src/utils/score2vLead.py
+-rw-r--r--   0 marco      (502) staff       (20)      730 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/str2float.py
+-rw-r--r--   0 marco      (502) staff       (20)      702 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/str2frac.py
+-rw-r--r--   0 marco      (502) staff       (20)      963 2021-06-25 20:55:30.000000 musicntwrk-2.3.4/src/utils/vectorDistance.py
```

### Comparing `musicntwrk-2.3.3/PKG-INFO` & `musicntwrk-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicntwrk
-Version: 2.3.3
+Version: 2.3.4
 Summary: music as data, data as music
 Home-page: https://www.musicntwrk.com
 Author: Marco Buongiorno Nardelli
 Author-email: mbn@unt.edu
 Platform: OS independent
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: musicntwrk Version: 2.3.3 Summary: music as data,
+Metadata-Version: 2.1 Name: musicntwrk Version: 2.3.4 Summary: music as data,
 data as music Home-page: https://www.musicntwrk.com Author: Marco Buongiorno
 Nardelli Author-email: mbn@unt.edu Platform: OS independent Description-
 Content-Type: text/markdown Requires-Dist: numpy Requires-Dist: scipy Requires-
 Dist: pandas Requires-Dist: python-louvain Requires-Dist: networkx Requires-
 Dist: music21 Requires-Dist: librosa Requires-Dist: numba Requires-Dist: pyo
 Requires-Dist: matplotlib Requires-Dist: tensorflow Requires-Dist: powerlaw
 Requires-Dist: vpython Requires-Dist: wget Requires-Dist: PySimpleGUI Requires-
```

### Comparing `musicntwrk-2.3.3/README.md` & `musicntwrk-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/musicntwrk.egg-info/PKG-INFO` & `musicntwrk-2.3.4/musicntwrk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicntwrk
-Version: 2.3.3
+Version: 2.3.4
 Summary: music as data, data as music
 Home-page: https://www.musicntwrk.com
 Author: Marco Buongiorno Nardelli
 Author-email: mbn@unt.edu
 Platform: OS independent
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: musicntwrk Version: 2.3.3 Summary: music as data,
+Metadata-Version: 2.1 Name: musicntwrk Version: 2.3.4 Summary: music as data,
 data as music Home-page: https://www.musicntwrk.com Author: Marco Buongiorno
 Nardelli Author-email: mbn@unt.edu Platform: OS independent Description-
 Content-Type: text/markdown Requires-Dist: numpy Requires-Dist: scipy Requires-
 Dist: pandas Requires-Dist: python-louvain Requires-Dist: networkx Requires-
 Dist: music21 Requires-Dist: librosa Requires-Dist: numba Requires-Dist: pyo
 Requires-Dist: matplotlib Requires-Dist: tensorflow Requires-Dist: powerlaw
 Requires-Dist: vpython Requires-Dist: wget Requires-Dist: PySimpleGUI Requires-
```

### Comparing `musicntwrk-2.3.3/musicntwrk.egg-info/SOURCES.txt` & `musicntwrk-2.3.4/musicntwrk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/setup.py` & `musicntwrk-2.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 with open(path.join(this_directory, 'README.md')) as f:
 	long_description = f.read()
 
 
 setup(name='musicntwrk',
 
-	version='2.3.3',
+	version='2.3.4',
 
 	description='music as data, data as music',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='Marco Buongiorno Nardelli',
 	author_email='mbn@unt.edu',
 	platforms='OS independent',
```

### Comparing `musicntwrk-2.3.3/src/comptools/MidiFile.py` & `musicntwrk-2.3.4/src/comptools/MidiFile.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/comptools/displayNotes.py` & `musicntwrk-2.3.4/src/comptools/displayNotes.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/comptools/genmidi.py` & `musicntwrk-2.3.4/src/comptools/genmidi.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/comptools/music.py` & `musicntwrk-2.3.4/src/comptools/music.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/comptools/notation.py` & `musicntwrk-2.3.4/src/comptools/notation.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/MIDImap.py` & `musicntwrk-2.3.4/src/data/MIDImap.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/MIDImidi.py` & `musicntwrk-2.3.4/src/data/MIDImidi.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/MIDIscore.py` & `musicntwrk-2.3.4/src/data/MIDIscore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/WRITEscore.py` & `musicntwrk-2.3.4/src/data/WRITEscore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/WRITEscoreNoTime.py` & `musicntwrk-2.3.4/src/data/WRITEscoreNoTime.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/WRITEscoreOps.py` & `musicntwrk-2.3.4/src/data/WRITEscoreOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/WRITEscoreOpsMIDI.py` & `musicntwrk-2.3.4/src/data/WRITEscoreOpsMIDI.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/analyzeSound.py` & `musicntwrk-2.3.4/src/data/analyzeSound.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/analyzeTimbre.py` & `musicntwrk-2.3.4/src/data/analyzeTimbre.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/ctcsound.py` & `musicntwrk-2.3.4/src/data/ctcsound.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/i_spectral.py` & `musicntwrk-2.3.4/src/data/i_spectral.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/i_spectral2.py` & `musicntwrk-2.3.4/src/data/i_spectral2.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/i_spectral_pure.py` & `musicntwrk-2.3.4/src/data/i_spectral_pure.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/i_spectral_pyo.py` & `musicntwrk-2.3.4/src/data/i_spectral_pyo.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/i_time_series.py` & `musicntwrk-2.3.4/src/data/i_time_series.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/r_1Ddata.py` & `musicntwrk-2.3.4/src/data/r_1Ddata.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/data/scaleMapping.py` & `musicntwrk-2.3.4/src/data/scaleMapping.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/applyOps.py` & `musicntwrk-2.3.4/src/harmony/applyOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/changePoint.py` & `musicntwrk-2.3.4/src/harmony/changePoint.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/chinese_postman.py` & `musicntwrk-2.3.4/src/harmony/chinese_postman.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/enharmonicDictionary.py` & `musicntwrk-2.3.4/src/harmony/enharmonicDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/getRN.py` & `musicntwrk-2.3.4/src/harmony/getRN.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/harmonicDesign.py` & `musicntwrk-2.3.4/src/harmony/harmonicDesign.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,15 @@
             ch.append(c)
     eulerseq.append(m21.chord.Chord(ch).normalOrder)
     if reverse: eulerseq = eulerseq[::-1]
     if display:
         eunodes,euedges,_,_,_,_,_ = mk.network(space='score',seq=eulerseq,ntx=True,general=True,
                                                distance='euclidean',grphtype='directed')
         drawNetwork(nodes=eunodes,edges=euedges,grphtype='directed')
+        return(eulerseq,eunodes,euedges,avgdeg,None)
     if write:
         WRITEscoreOps(eulerseq,w=write)
     
     if not scfree.is_directed():
         return(eulerseq,avgdeg,modul)
     else:
         return(eulerseq,avgdeg,None)
```

### Comparing `musicntwrk-2.3.3/src/harmony/keySections.py` & `musicntwrk-2.3.4/src/harmony/keySections.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/lookupOps.py` & `musicntwrk-2.3.4/src/harmony/lookupOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/lookupProgr.py` & `musicntwrk-2.3.4/src/harmony/lookupProgr.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/lookupWrapper.py` & `musicntwrk-2.3.4/src/harmony/lookupWrapper.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/networkHarmonyGen.py` & `musicntwrk-2.3.4/src/harmony/networkHarmonyGen.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/plotHarmonicTable.py` & `musicntwrk-2.3.4/src/harmony/plotHarmonicTable.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/rhythmicDesign.py` & `musicntwrk-2.3.4/src/harmony/rhythmicDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/scoreAnalysis.py` & `musicntwrk-2.3.4/src/harmony/scoreAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/scoreDesign.py` & `musicntwrk-2.3.4/src/harmony/scoreDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/scoreFilter.py` & `musicntwrk-2.3.4/src/harmony/scoreFilter.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/shortHands.py` & `musicntwrk-2.3.4/src/harmony/shortHands.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/showAnalysis.py` & `musicntwrk-2.3.4/src/harmony/showAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/spiralChordSpace.py` & `musicntwrk-2.3.4/src/harmony/spiralChordSpace.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/tonalAnalysis.py` & `musicntwrk-2.3.4/src/harmony/tonalAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/tonalHarmonyCalculator.py` & `musicntwrk-2.3.4/src/harmony/tonalHarmonyCalculator.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/tonalHarmonyModels.py` & `musicntwrk-2.3.4/src/harmony/tonalHarmonyModels.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/tonalPartition.py` & `musicntwrk-2.3.4/src/harmony/tonalPartition.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/harmony/tonnentz.py` & `musicntwrk-2.3.4/src/harmony/tonnentz.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/ml_utils/checkRun.py` & `musicntwrk-2.3.4/src/ml_utils/checkRun.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/ml_utils/modelDump.py` & `musicntwrk-2.3.4/src/ml_utils/modelDump.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/ml_utils/modelLoad.py` & `musicntwrk-2.3.4/src/ml_utils/modelLoad.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/ml_utils/multiModelPredictor.py` & `musicntwrk-2.3.4/src/ml_utils/multiModelPredictor.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/ml_utils/prepareDataSet.py` & `musicntwrk-2.3.4/src/ml_utils/prepareDataSet.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/ml_utils/readModels.py` & `musicntwrk-2.3.4/src/ml_utils/readModels.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/ml_utils/scaleDataSet.py` & `musicntwrk-2.3.4/src/ml_utils/scaleDataSet.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/ml_utils/trainCNNmodel.py` & `musicntwrk-2.3.4/src/ml_utils/trainCNNmodel.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/ml_utils/trainNNmodel.py` & `musicntwrk-2.3.4/src/ml_utils/trainNNmodel.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/base.py` & `musicntwrk-2.3.4/src/msctools/base.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/cfg.py` & `musicntwrk-2.3.4/src/msctools/cfg.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/converters.py` & `musicntwrk-2.3.4/src/msctools/converters.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/devices.py` & `musicntwrk-2.3.4/src/msctools/devices.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/dictionaries.py` & `musicntwrk-2.3.4/src/msctools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/dsp.py` & `musicntwrk-2.3.4/src/msctools/dsp.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/envelopes.py` & `musicntwrk-2.3.4/src/msctools/envelopes.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/envelopes_thread.py` & `musicntwrk-2.3.4/src/msctools/envelopes_thread.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/networks.py` & `musicntwrk-2.3.4/src/msctools/networks.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/oscserver.py` & `musicntwrk-2.3.4/src/msctools/oscserver.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/osctools.py` & `musicntwrk-2.3.4/src/msctools/osctools.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/players.py` & `musicntwrk-2.3.4/src/msctools/players.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/players_thread.py` & `musicntwrk-2.3.4/src/msctools/players_thread.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/pyoPlayer.py` & `musicntwrk-2.3.4/src/msctools/pyoPlayer.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/pyotools.py` & `musicntwrk-2.3.4/src/msctools/pyotools.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/session.py` & `musicntwrk-2.3.4/src/msctools/session.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/msctools/videocapture.py` & `musicntwrk-2.3.4/src/msctools/videocapture.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/musicntwrk.py` & `musicntwrk-2.3.4/src/musicntwrk.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/analysisNetwork.py` & `musicntwrk-2.3.4/src/networks/analysisNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/orchestralNetwork.py` & `musicntwrk-2.3.4/src/networks/orchestralNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/orchestralVector.py` & `musicntwrk-2.3.4/src/networks/orchestralVector.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/orchestralVectorColor.py` & `musicntwrk-2.3.4/src/networks/orchestralVectorColor.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/pcsDictionary.py` & `musicntwrk-2.3.4/src/networks/pcsDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/pcsEgoNetwork.py` & `musicntwrk-2.3.4/src/networks/pcsEgoNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/pcsNetwork.py` & `musicntwrk-2.3.4/src/networks/pcsNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/rLeadNetwork.py` & `musicntwrk-2.3.4/src/networks/rLeadNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/readScore.py` & `musicntwrk-2.3.4/src/networks/readScore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/rhythmDictionary.py` & `musicntwrk-2.3.4/src/networks/rhythmDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/rhythmNetwork.py` & `musicntwrk-2.3.4/src/networks/rhythmNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/rhythmPDictionary.py` & `musicntwrk-2.3.4/src/networks/rhythmPDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/scoreDictionary.py` & `musicntwrk-2.3.4/src/networks/scoreDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/scoreMIDIDictionary.py` & `musicntwrk-2.3.4/src/networks/scoreMIDIDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/scoreNetwork.py` & `musicntwrk-2.3.4/src/networks/scoreNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/scoreSubNetwork.py` & `musicntwrk-2.3.4/src/networks/scoreSubNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/timbralNetwork.py` & `musicntwrk-2.3.4/src/networks/timbralNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/vLeadNetwork.py` & `musicntwrk-2.3.4/src/networks/vLeadNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/vLeadNetworkByName.py` & `musicntwrk-2.3.4/src/networks/vLeadNetworkByName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/vLeadNetworkByNameVec.py` & `musicntwrk-2.3.4/src/networks/vLeadNetworkByNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/networks/vLeadNetworkVec.py` & `musicntwrk-2.3.4/src/networks/vLeadNetworkVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/barplot.py` & `musicntwrk-2.3.4/src/plotting/barplot.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/chordspace.py` & `musicntwrk-2.3.4/src/plotting/chordspace.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/drawMultiLayerNetwork.py` & `musicntwrk-2.3.4/src/plotting/drawMultiLayerNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/drawNetwork.py` & `musicntwrk-2.3.4/src/plotting/drawNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/drawNetwork3D.py` & `musicntwrk-2.3.4/src/plotting/drawNetwork3D.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/drawNetworkViz.py` & `musicntwrk-2.3.4/src/plotting/drawNetworkViz.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/drawNetworkX.py` & `musicntwrk-2.3.4/src/plotting/drawNetworkX.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/plotCC.py` & `musicntwrk-2.3.4/src/plotting/plotCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/plotCurveXY.py` & `musicntwrk-2.3.4/src/plotting/plotCurveXY.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/plotCurveY.py` & `musicntwrk-2.3.4/src/plotting/plotCurveY.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/plotDegreeAnalysis.py` & `musicntwrk-2.3.4/src/plotting/plotDegreeAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/plotting/plotOpsHistogram.py` & `musicntwrk-2.3.4/src/plotting/plotOpsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/computeASCBW.py` & `musicntwrk-2.3.4/src/timbre/computeASCBW.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/computeCompMPS.py` & `musicntwrk-2.3.4/src/timbre/computeCompMPS.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/computeMFCC.py` & `musicntwrk-2.3.4/src/timbre/computeMFCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/computeModifiedASCBW.py` & `musicntwrk-2.3.4/src/timbre/computeModifiedASCBW.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/computePSCC.py` & `musicntwrk-2.3.4/src/timbre/computePSCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/computeStandardizedMFCC.py` & `musicntwrk-2.3.4/src/timbre/computeStandardizedMFCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/computeStandardizedMFPS.py` & `musicntwrk-2.3.4/src/timbre/computeStandardizedMFPS.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/computeStandardizedPSCC.py` & `musicntwrk-2.3.4/src/timbre/computeStandardizedPSCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/mfccSoundDecay.py` & `musicntwrk-2.3.4/src/timbre/mfccSoundDecay.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/mfccSoundDecayOptimal.py` & `musicntwrk-2.3.4/src/timbre/mfccSoundDecayOptimal.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/mfccSoundDecayPiecewise.py` & `musicntwrk-2.3.4/src/timbre/mfccSoundDecayPiecewise.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/minimizeBKPT.py` & `musicntwrk-2.3.4/src/timbre/minimizeBKPT.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/normSoundDecay.py` & `musicntwrk-2.3.4/src/timbre/normSoundDecay.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/timbre/normSoundDecay2.py` & `musicntwrk-2.3.4/src/timbre/normSoundDecay2.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/Remove.py` & `musicntwrk-2.3.4/src/utils/Remove.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/SegmentedLinearReg.py` & `musicntwrk-2.3.4/src/utils/SegmentedLinearReg.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/Sublists.py` & `musicntwrk-2.3.4/src/utils/Sublists.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/communications.py` & `musicntwrk-2.3.4/src/utils/communications.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/diffusionEntropyAnalyis.py` & `musicntwrk-2.3.4/src/utils/diffusionEntropyAnalyis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/diffusionEntropyAnalyisNew.py` & `musicntwrk-2.3.4/src/utils/diffusionEntropyAnalyisNew.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/entropyKLdiv.py` & `musicntwrk-2.3.4/src/utils/entropyKLdiv.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/extractByString.py` & `musicntwrk-2.3.4/src/utils/extractByString.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/fetchWaves.py` & `musicntwrk-2.3.4/src/utils/fetchWaves.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/findLengthMax.py` & `musicntwrk-2.3.4/src/utils/findLengthMax.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/flatten.py` & `musicntwrk-2.3.4/src/utils/flatten.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/floatize.py` & `musicntwrk-2.3.4/src/utils/floatize.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/generalizedOpsHistogram.py` & `musicntwrk-2.3.4/src/utils/generalizedOpsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/generalizedOpsName.py` & `musicntwrk-2.3.4/src/utils/generalizedOpsName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/init_list_of_objects.py` & `musicntwrk-2.3.4/src/utils/init_list_of_objects.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/load_balancing.py` & `musicntwrk-2.3.4/src/utils/load_balancing.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/minimalDistance.py` & `musicntwrk-2.3.4/src/utils/minimalDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/minimalDistanceVec.py` & `musicntwrk-2.3.4/src/utils/minimalDistanceVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/minimalNoBijDistance.py` & `musicntwrk-2.3.4/src/utils/minimalNoBijDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/opsCheckByName.py` & `musicntwrk-2.3.4/src/utils/opsCheckByName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/opsCheckByNameVec.py` & `musicntwrk-2.3.4/src/utils/opsCheckByNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/opsDistance.py` & `musicntwrk-2.3.4/src/utils/opsDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/opsHistogram.py` & `musicntwrk-2.3.4/src/utils/opsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/opsName.py` & `musicntwrk-2.3.4/src/utils/opsName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/opsNameFull.py` & `musicntwrk-2.3.4/src/utils/opsNameFull.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/opsNameVec.py` & `musicntwrk-2.3.4/src/utils/opsNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/play_with_simpleaudio.py` & `musicntwrk-2.3.4/src/utils/play_with_simpleaudio.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/powerFit.py` & `musicntwrk-2.3.4/src/utils/powerFit.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/rhythmDistance.py` & `musicntwrk-2.3.4/src/utils/rhythmDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/scaleFreeFit.py` & `musicntwrk-2.3.4/src/utils/scaleFreeFit.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/score2vLead.py` & `musicntwrk-2.3.4/src/utils/score2vLead.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/str2float.py` & `musicntwrk-2.3.4/src/utils/str2float.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/str2frac.py` & `musicntwrk-2.3.4/src/utils/str2frac.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.3.3/src/utils/vectorDistance.py` & `musicntwrk-2.3.4/src/utils/vectorDistance.py`

 * *Files identical despite different names*

