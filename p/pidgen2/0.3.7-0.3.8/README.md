# Comparing `tmp/pidgen2-0.3.7.tar.gz` & `tmp/pidgen2-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pidgen2-0.3.7.tar", last modified: Mon Apr  3 20:35:52 2023, max compression
+gzip compressed data, was "pidgen2-0.3.8.tar", last modified: Thu May  2 18:00:46 2024, max compression
```

## Comparing `pidgen2-0.3.7.tar` & `pidgen2-0.3.8.tar`

### file list

```diff
@@ -1,117 +1,122 @@
-drwxrwxr-x   0 poluekt   (1000) poluekt   (1000)        0 2023-04-03 20:35:52.212045 pidgen2-0.3.7/
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)    35065 2021-06-28 09:42:13.000000 pidgen2-0.3.7/LICENSE
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)       34 2023-01-23 09:37:39.000000 pidgen2-0.3.7/MANIFEST.in
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     2147 2023-04-03 20:35:52.212045 pidgen2-0.3.7/PKG-INFO
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1574 2022-04-07 11:48:37.000000 pidgen2-0.3.7/README.md
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)      104 2021-06-28 09:42:13.000000 pidgen2-0.3.7/pyproject.toml
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1481 2023-04-03 20:35:52.216045 pidgen2-0.3.7/setup.cfg
-drwxrwxr-x   0 poluekt   (1000) poluekt   (1000)        0 2023-04-03 20:35:52.192045 pidgen2-0.3.7/src/
-drwxrwxr-x   0 poluekt   (1000) poluekt   (1000)        0 2023-04-03 20:35:52.200045 pidgen2-0.3.7/src/pidgen2/
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)        0 2021-06-28 09:42:13.000000 pidgen2-0.3.7/src/pidgen2/__init__.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)      414 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/add_brunel.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     2848 2022-06-30 09:06:23.000000 pidgen2-0.3.7/src/pidgen2/cache.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)    13562 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/correct.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1235 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/create_correction_example.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1255 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/create_photon_correction_example.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1232 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/create_resampling_example.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     9486 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/datasets.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)    18358 2022-08-29 09:16:56.000000 pidgen2-0.3.7/src/pidgen2/density_estimation.py
-drwxrwxr-x   0 poluekt   (1000) poluekt   (1000)        0 2023-04-03 20:35:52.200045 pidgen2-0.3.7/src/pidgen2/examples/
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     8145 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/examples/example_correct.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     6459 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/examples/example_correct_photon.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     8165 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/examples/example_resample.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1126 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/init.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1406 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/list_mc_samples.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     2235 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/list_mc_variables.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1369 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/list_samples.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     2170 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/list_variables.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     5247 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/mc_datasets.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)    14212 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/plotting.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)    11067 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/resample.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)    49139 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/resampling.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)    48522 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/resampling_new.py
-drwxrwxr-x   0 poluekt   (1000) poluekt   (1000)        0 2023-04-03 20:35:52.204045 pidgen2-0.3.7/src/pidgen2/samples/
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     5212 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4031 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi_M.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4374 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi_P.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4395 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi_PIDKgt4.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4210 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi_PtEta.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1011 2021-06-28 09:42:13.000000 pidgen2-0.3.7/src/pidgen2/samples/__init__.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     3023 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/e_B2JpsieeK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     3068 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/e_B2JpsieeK_Brem.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     3068 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/e_B2JpsieeK_NoBrem.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4044 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/samples/gamma_B2KstarGamma.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4074 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/samples/gamma_B2KstarGammaType0.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4074 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/samples/gamma_B2KstarGammaType1.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     5409 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/mu_Jpsi2mumu.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     5707 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/mu_Jpsi2mumu_isMuon.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     5602 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/mu_Jpsi2mumunopt.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     5737 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/mu_Jpsi2mumunopt_isMuon.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4501 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/p_IncLc.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4871 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/p_Lambda2ppi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     3886 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/p_Lambda2ppi_Prompt.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     3087 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/p_Lambda2ppi_Prompt_PIDpgt0.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4510 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/p_Lb2Lcmu.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     2996 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/p_Lb2Lcpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     2424 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/p_Test.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     5234 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4455 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi_M.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4455 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi_P.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4477 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4300 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi_PtEta.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     5223 2021-06-30 09:47:32.000000 pidgen2-0.3.7/src/pidgen2/systematics.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     7014 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/tuples.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     5061 2021-10-12 07:36:40.000000 pidgen2-0.3.7/src/pidgen2/validate.py
-drwxrwxr-x   0 poluekt   (1000) poluekt   (1000)        0 2023-04-03 20:35:52.212045 pidgen2-0.3.7/src/pidgen2/variables/
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1288 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1365 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1437 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpip.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1287 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNe.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1289 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNmu.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1290 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNp.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1363 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1437 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotpiK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1292 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1365 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1437 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotKp.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1226 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/variables/CombDLLK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1223 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/CombDLLe.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1225 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/CombDLLmu.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1225 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/variables/CombDLLp.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1234 2022-08-29 09:16:56.000000 pidgen2-0.3.7/src/pidgen2/variables/IsPhoton.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1274 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV2_ProbNNK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1276 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV2_ProbNNmu.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1274 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV2_ProbNNp.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1276 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV2_ProbNNpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1274 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1337 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1395 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpip.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1273 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNe.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1275 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNmu.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1273 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNp.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1335 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpNotK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1395 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpNotpiK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1275 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1337 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1395 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1281 2022-08-29 09:16:56.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1337 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1395 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1280 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNe.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1282 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNmu.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1283 2023-01-23 09:37:39.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNp.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1335 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1395 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpNotpiK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1285 2022-08-29 09:16:56.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpi.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1337 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotK.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1395 2022-04-07 11:48:37.000000 pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotKp.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1213 2022-08-29 09:16:56.000000 pidgen2-0.3.7/src/pidgen2/variables/PhotonCL.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1272 2023-04-03 20:19:59.000000 pidgen2-0.3.7/src/pidgen2/variables/Test_ProbNNp.py
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     1011 2021-06-28 09:42:13.000000 pidgen2-0.3.7/src/pidgen2/variables/__init__.py
-drwxrwxr-x   0 poluekt   (1000) poluekt   (1000)        0 2023-04-03 20:35:52.200045 pidgen2-0.3.7/src/pidgen2.egg-info/
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     2147 2023-04-03 20:35:52.000000 pidgen2-0.3.7/src/pidgen2.egg-info/PKG-INFO
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)     4207 2023-04-03 20:35:52.000000 pidgen2-0.3.7/src/pidgen2.egg-info/SOURCES.txt
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)        1 2023-04-03 20:35:52.000000 pidgen2-0.3.7/src/pidgen2.egg-info/dependency_links.txt
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)      629 2023-04-03 20:35:52.000000 pidgen2-0.3.7/src/pidgen2.egg-info/entry_points.txt
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)       61 2023-04-03 20:35:52.000000 pidgen2-0.3.7/src/pidgen2.egg-info/requires.txt
--rw-rw-r--   0 poluekt   (1000) poluekt   (1000)        8 2023-04-03 20:35:52.000000 pidgen2-0.3.7/src/pidgen2.egg-info/top_level.txt
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:46.182192 pidgen2-0.3.8/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    35065 2021-08-03 09:00:33.000000 pidgen2-0.3.8/LICENSE
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)       34 2023-03-22 19:27:38.000000 pidgen2-0.3.8/MANIFEST.in
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     2313 2024-05-02 18:00:46.159193 pidgen2-0.3.8/PKG-INFO
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1574 2022-05-06 07:27:54.000000 pidgen2-0.3.8/README.md
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)      104 2021-08-03 09:00:33.000000 pidgen2-0.3.8/pyproject.toml
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1481 2024-05-02 18:00:46.187196 pidgen2-0.3.8/setup.cfg
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:45.664198 pidgen2-0.3.8/src/
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:45.811193 pidgen2-0.3.8/src/pidgen2/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)        0 2021-08-03 09:00:33.000000 pidgen2-0.3.8/src/pidgen2/__init__.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)      414 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/add_brunel.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2848 2022-06-29 14:48:08.000000 pidgen2-0.3.8/src/pidgen2/cache.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)    13726 2024-05-01 18:11:53.000000 pidgen2-0.3.8/src/pidgen2/correct.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1235 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/create_correction_example.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1255 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/create_photon_correction_example.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1232 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/create_resampling_example.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     9486 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/datasets.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)    18360 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/density_estimation.py
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:45.845193 pidgen2-0.3.8/src/pidgen2/examples/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     8145 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/examples/example_correct.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     6459 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/examples/example_correct_photon.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     8165 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/examples/example_resample.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1126 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/init.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1406 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/list_mc_samples.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2235 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/list_mc_variables.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1369 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/list_samples.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2170 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/list_variables.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5660 2024-05-02 15:55:27.000000 pidgen2-0.3.8/src/pidgen2/mc_datasets.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    14212 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/plotting.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)    11205 2024-05-01 18:14:27.000000 pidgen2-0.3.8/src/pidgen2/resample.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     4647 2024-05-01 18:32:35.000000 pidgen2-0.3.8/src/pidgen2/resampler.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    50273 2024-05-02 17:12:20.000000 pidgen2-0.3.8/src/pidgen2/resampling.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    48522 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/resampling_new.py
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:45.972194 pidgen2-0.3.8/src/pidgen2/samples/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5812 2024-05-02 16:50:02.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4031 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_M.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4374 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_P.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4395 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_PIDKgt4.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4210 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_PtEta.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5824 2024-05-02 17:32:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1011 2021-08-03 09:00:33.000000 pidgen2-0.3.8/src/pidgen2/samples/__init__.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     3023 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     3068 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK_Brem.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     3068 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK_NoBrem.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4044 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGamma.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4074 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGammaType0.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4074 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGammaType1.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5409 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumu.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5707 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumu_isMuon.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5602 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumunopt.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5737 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumunopt_isMuon.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5094 2024-05-02 16:59:58.000000 pidgen2-0.3.8/src/pidgen2/samples/p_IncLc.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5461 2024-05-02 17:02:57.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     3886 2023-03-27 18:03:02.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi_Prompt.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     3087 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi_Prompt_PIDpgt0.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5103 2024-05-02 17:04:47.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lb2Lcmu.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     2996 2024-05-02 16:48:07.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lb2Lcpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2424 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Test.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5837 2024-05-02 15:56:06.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4455 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_M.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4455 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_P.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4477 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4300 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_PtEta.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5837 2024-05-02 17:09:14.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5223 2021-09-17 08:50:28.000000 pidgen2-0.3.8/src/pidgen2/systematics.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     7050 2024-05-01 18:15:27.000000 pidgen2-0.3.8/src/pidgen2/tuples.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5061 2021-10-10 20:12:28.000000 pidgen2-0.3.8/src/pidgen2/validate.py
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:46.150193 pidgen2-0.3.8/src/pidgen2/variables/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1288 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1365 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1437 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpip.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1287 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNe.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1289 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNmu.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1290 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1363 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1437 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotpiK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1292 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1365 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1437 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotKp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1226 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/CombDLLK.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1223 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/CombDLLe.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1225 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/CombDLLmu.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1225 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/CombDLLp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1234 2022-08-28 19:47:05.000000 pidgen2-0.3.8/src/pidgen2/variables/IsPhoton.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1274 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNK.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1276 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNmu.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1274 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNp.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1276 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNpi.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1274 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpip.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1271 2024-05-01 12:46:16.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNK_scale.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1273 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNe.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1275 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNmu.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1273 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1335 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpNotpiK.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1275 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1272 2024-05-02 17:10:09.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpi_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1281 2022-08-26 20:52:55.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1280 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNe.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1282 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNmu.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1283 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1335 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpNotpiK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1285 2022-08-26 20:52:40.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotKp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1213 2022-08-27 19:02:29.000000 pidgen2-0.3.8/src/pidgen2/variables/PhotonCL.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1272 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/Test_ProbNNp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1011 2021-08-03 09:00:33.000000 pidgen2-0.3.8/src/pidgen2/variables/__init__.py
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:46.154193 pidgen2-0.3.8/src/pidgen2.egg-info/
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     2313 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/PKG-INFO
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4416 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/SOURCES.txt
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)        1 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/dependency_links.txt
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)      629 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/entry_points.txt
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)       61 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/requires.txt
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)        8 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/top_level.txt
```

### Comparing `pidgen2-0.3.7/LICENSE` & `pidgen2-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/PKG-INFO` & `pidgen2-0.3.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: pidgen2
-Version: 0.3.7
+Version: 0.3.8
 Summary: Tools for particle identification (PID) correction for LHCb detector
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidgen2
 Author: Anton Poluektov
 Author-email: anton.poluektov@cern.ch
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidgen2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: jax
+Requires-Dist: uproot<5,>=4.2
+Requires-Dist: xrootd>=5.2
 
 # PIDGen2 
 
 ## Introduction
 
 PIDGen is a tool to resample PID variables in the full MC bases on distributions from calibration samples. PIDGen2 is a successor of the old PIDGen package. PIDGen2 is available via `lb-conda` and is supposed to replace the old PIDGen, both for Run 3 data, and for Run 1/Run 2. 
 An analogous solution updating PIDCorr is under development (see [here](https://groups.cern.ch/group/lhcb-phys-pid-calibration/Lists/Archive/Flat.aspx?RootFolder=%2Fgroup%2Flhcb%2Dphys%2Dpid%2Dcalibration%2FLists%2FArchive%2Fresampling%20in%20PIDCalib2&FolderCTID=0x01200200428956A5A0587D4CA9DBE3C7098FA903)).
```

### Comparing `pidgen2-0.3.7/README.md` & `pidgen2-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/setup.cfg` & `pidgen2-0.3.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pidgen2
-version = 0.3.7
+version = 0.3.8
 author = Anton Poluektov
 author_email = anton.poluektov@cern.ch
 description = Tools for particle identification (PID) correction for LHCb detector
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.cern.ch/lhcb-rta/pidgen2
 project_urls =
```

### Comparing `pidgen2-0.3.7/src/pidgen2/cache.py` & `pidgen2-0.3.8/src/pidgen2/cache.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/correct.py` & `pidgen2-0.3.8/src/pidgen2/correct.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,33 +61,36 @@
 
   config = get_samples()[sample][dataset]
   mc_config = get_mc_samples()[sample][f"{simversion}_{dataset}"]
   mc_variable = variable
 
   if "aliases" in config and variable in config["aliases"] : 
     aliased_variable = config["aliases"][variable]
-    print(f"Using alias '{aliased_variable}' for variable name '{variable}' in dataset '{dataset}', sample '{sample}'")
+    if verbose >= 0 : 
+      print(f"Using alias '{aliased_variable}' for variable name '{variable}' in dataset '{dataset}', sample '{sample}'")
     variable = aliased_variable
 
   if "aliases" in mc_config and variable in mc_config["aliases"] : 
     aliased_variable = mc_config["aliases"][variable]
-    print(f"Using alias '{aliased_variable}' for variable name '{variable}' in MC dataset '{simversion}_{dataset}', sample '{sample}'")
+    if verbose >= 0 : 
+      print(f"Using alias '{aliased_variable}' for variable name '{variable}' in MC dataset '{simversion}_{dataset}', sample '{sample}'")
     mc_variable = aliased_variable
 
   vardef = get_variables()[variable]
   mc_vardef = get_variables()[mc_variable]
 
   pp = pprint.PrettyPrinter(indent = 4)
 
-  if (verbose) : 
+  if verbose >= 1 : 
     print(f"Calibration sample config: {pp.pformat(config)}")
     print(f"MC sample config: {pp.pformat(mc_config)}")
     print(f"Variable definition: {pp.pformat(vardef)}")
 
-  print(f"Checking if data template exists in the storage")
+  if verbose >= 0 :
+    print(f"Checking if data template exists in the storage")
 
   # Create PID resampling template based on calibration sample
   counts, counts2, edges, normaliser = get_or_create_template(sample, dataset, variable, 
                              vardef, config, 
                              use_calib_cache = usecache, max_files = maxfiles, 
                              interactive_plots = interactive, 
                              control_plots = plot, verbose = verbose, 
@@ -110,22 +113,22 @@
   input_data = input_df[input_branches].to_numpy()
 
   start_event = start
   stop_event = stop
 
   if (stop_event is not None) and stop_event > len(input_data) : stop_event = len(input_data)
   else : input_data = input_data[start_event:stop_event]
-  if (verbose) : print (f"Shape of the array for resampling: {input_data.shape}")
+  if verbose >= 1 : print (f"Shape of the array for resampling: {input_data.shape}")
 
   if eta_from_p : 
     # Replace momentum by eta calculated from p (index 1) and pT (index 2)
     input_data[:,2] = -np.log(np.tan(np.arcsin(input_data[:,1]/input_data[:,2])/2.))
 
   if not friend :
-    if (verbose) :
+    if verbose >= 1 :
       all_branches = list(uproot.open(input).keys())
       print (f"List of all input tree branches: {pp.pformat(all_branches)}")
 
   # Loop over kernels
   kernel_list = kernels
   if not isinstance(kernels, (list, tuple)) : 
     kernel_list = [ kernels ]
@@ -161,31 +164,34 @@
     else : 
       template_sigma = kernel_name
       kernel_name = f"kern{kernel_num}"
 
     for template_seed in template_seeds : 
 
       if not ((template_seed is None) or (template_seed == 0) ) : 
-        print(f"Random sampling of raw template with seed {template_seed}")
+        if verbose >= 0 :
+          print(f"Random sampling of raw template with seed {template_seed}")
         onp.random.seed(template_seed)
         sampled_counts = onp.random.normal(counts, counts2)
         sampled_mc_counts = onp.random.normal(mc_counts, mc_counts2)
       else : 
         sampled_counts = counts
         sampled_mc_counts = mc_counts
 
-      print(f"Applying Gaussian smearing with kernel {template_sigma}")
+      if verbose >= 0 :
+        print(f"Applying Gaussian smearing with kernel {template_sigma}")
 
       smooth_counts = gaussian_filter(sampled_counts, template_sigma)
       template = smooth_counts, edges, normaliser
 
       smooth_mc_counts = gaussian_filter(sampled_mc_counts, template_sigma)
       mc_template = smooth_mc_counts, edges, normaliser  # or mc_normaliser? - no
 
-      print(f"Smeared template ready, starting resampling")
+      if verbose >= 0 :
+        print(f"Smeared template ready, starting resampling")
 
       #onp.random.seed(resampling_seed) # - remove?
 
       kine_data = data_transform(input_data[:,1:], config, scale = scale_list )
       pid_data = transform_forward(input_data[:,0])[:,np.newaxis]
       data = np.concatenate([pid_data, kine_data], axis=1)
       
@@ -196,15 +202,15 @@
 
       output_arrays += [ pid_arr, calib_stat, mc_stat ]
       if (template_seed is None) or (template_seed == 0) : 
         output_branches += [ f"{pidcorr}_{kernel_name}", f"{stat}_{kernel_name}", f"{mcstat}_{kernel_name}" ]
       else : 
         output_branches += [ f"{pidcorr}_{kernel_name}_{template_seed}", f"{stat}_{kernel_name}_{template_seed}", f"{mcstat}_{kernel_name}_{template_seed}" ]
 
-      if (verbose) : 
+      if verbose >= 1 : 
         print(f"Input data array: {input_data[:100]}")
         print(f"Data array after variable transformation: {data[:100]}")
         print(f"Resampled PID array: {pid_arr[:100]}")
         print(f"Resampling statistics array: {calib_stat[:100]}")
         print(f"Resampling MC statistics array: {mc_stat[:100]}")
 
   # End of loop over kernels
```

### Comparing `pidgen2-0.3.7/src/pidgen2/create_correction_example.py` & `pidgen2-0.3.8/src/pidgen2/create_correction_example.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/create_photon_correction_example.py` & `pidgen2-0.3.8/src/pidgen2/create_photon_correction_example.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/create_resampling_example.py` & `pidgen2-0.3.8/src/pidgen2/create_resampling_example.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/datasets.py` & `pidgen2-0.3.8/src/pidgen2/datasets.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/density_estimation.py` & `pidgen2-0.3.8/src/pidgen2/density_estimation.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
       denorm_data += [ np.interp(data[:,i], cum_values, edges, left = edges[0], right = edges[-1]) ]
     elif methods[i] == "gauss" : 
       flat = 0.5*(scipy.special.erf( data[:,i] ) + 1.)
       denorm_data += [ np.interp(flat, cum_values, edges, left = edges[0], right = edges[-1]) ]
     elif methods[i] == "scale" : 
       left = edges[0]
       right = edges[-1]
-      norm_data += [ data[:,i]*(right-left)+left ]
+      denorm_data += [ data[:,i]*(right-left)+left ]
   return np.stack(denorm_data, axis = 1)
 
 def resample(counts, edges, data, rnd, range = (-2.5, 2.5), bins = 100) : 
   """
   Perform random sampling of a single variable following the binned 
   multidimensional density function and the array of input data.
```

### Comparing `pidgen2-0.3.7/src/pidgen2/examples/example_correct.py` & `pidgen2-0.3.8/src/pidgen2/examples/example_correct.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/examples/example_correct_photon.py` & `pidgen2-0.3.8/src/pidgen2/examples/example_correct_photon.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/examples/example_resample.py` & `pidgen2-0.3.8/src/pidgen2/examples/example_resample.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/init.py` & `pidgen2-0.3.8/src/pidgen2/init.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/list_mc_samples.py` & `pidgen2-0.3.8/src/pidgen2/list_mc_samples.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/list_mc_variables.py` & `pidgen2-0.3.8/src/pidgen2/list_mc_variables.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/list_samples.py` & `pidgen2-0.3.8/src/pidgen2/list_samples.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/list_variables.py` & `pidgen2-0.3.8/src/pidgen2/list_variables.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/mc_datasets.py` & `pidgen2-0.3.8/src/pidgen2/mc_datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,25 @@
 Definitions of LHCb PID MC datasets (ROOT files produced by WG productions). 
 The ROOT files can contain several trees corresponding to different calibration samples. 
 These dictionaries are used further in the definitions of calibration samples (see samples/ subdir). 
 """
 
 run2sim09_dir = "root://eoslhcb.cern.ch//eos/lhcb/wg/PID/PIDGen/MC/Run2Sim09"
 run2sim09_muon_dir = "root://eoslhcb.cern.ch//eos/lhcb/wg/PID/PIDGen2/mc/muon"
+run1sim09_dir = "root://eoslhcb.cern.ch//eos/lhcb/wg/PID/PIDGen/MC/Run1Sim09"
 run1sim09_muon_dir = "root://eoslhcb.cern.ch//eos/lhcb/wg/PID/PIDGen2/mc/muon"
 photon_dir = "root://eoslhcb.cern.ch//eos/lhcb/wg/PID/PIDGen2/calibration/photon/"
 
+lcmu_run1sim09_datasets = {
+  'MagDown_2011' : [f"{run1sim09_dir}/tuple_lcmu_mc11_sim09_magdown.root"], 
+  'MagUp_2011'   : [f"{run1sim09_dir}/tuple_lcmu_mc11_sim09_magup.root"], 
+  'MagDown_2012' : [f"{run1sim09_dir}/tuple_lcmu_mc12_sim09_magdown.root"], 
+  'MagUp_2012'   : [f"{run1sim09_dir}/tuple_lcmu_mc12_sim09_magup.root"], 
+}
+
 dstar_run2sim09_datasets = {
   'MagDown_2018': [f"{run2sim09_dir}/tuple_dstar_mc18_magdown.root" ], 
   'MagUp_2018':   [f"{run2sim09_dir}/tuple_dstar_mc18_magup.root" ], 
   'MagDown_2017': [f"{run2sim09_dir}/tuple_dstar_mc17_magdown.root" ], 
   'MagUp_2017':   [f"{run2sim09_dir}/tuple_dstar_mc17_magup.root" ], 
   'MagDown_2016': [f"{run2sim09_dir}/tuple_dstar_mc16_magdown.root" ], 
   'MagUp_2016':   [f"{run2sim09_dir}/tuple_dstar_mc16_magup.root" ],
```

### Comparing `pidgen2-0.3.7/src/pidgen2/plotting.py` & `pidgen2-0.3.8/src/pidgen2/plotting.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/resample.py` & `pidgen2-0.3.8/src/pidgen2/resample.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,24 +58,26 @@
 
   config = get_samples()[sample][dataset]
 
   pp = pprint.PrettyPrinter(indent = 4)
 
   if "aliases" in config and variable in config["aliases"] : 
     aliased_variable = config["aliases"][variable]
-    print(f"Using alias '{aliased_variable}' for variable name '{variable}' in dataset '{dataset}', sample '{sample}'")
+    if verbose >= 0 :
+      print(f"Using alias '{aliased_variable}' for variable name '{variable}' in dataset '{dataset}', sample '{sample}'")
     variable = aliased_variable
 
   vardef = get_variables()[variable]
 
-  if (verbose) : 
+  if verbose >= 1 : 
     print(f"Calibration sample config: {pp.pformat(config)}")
     print(f"Variable definition: {pp.pformat(vardef)}")
 
-  print(f"Checking if template exists in the storage")
+  if verbose >= 0 :
+    print(f"Checking if template exists in the storage")
 
   #print(cachedir is None)
 
   # Create PID resampling template based on calibration sample
   counts, counts2, edges, normaliser = get_or_create_template(sample, dataset, variable, 
                              vardef, config, 
                              use_calib_cache = usecache, max_files = maxfiles, 
@@ -89,22 +91,22 @@
   input_data = input_df[input_branches].to_numpy()
 
   start_event = start
   stop_event = stop
 
   if (stop_event is not None) and stop_event > len(input_data) : stop_event = len(input_data)
   else : input_data = input_data[start_event:stop_event]
-  if (verbose) : print (f"Shape of the array for resampling: {input_data.shape}")
+  if verbose >= 1 : print (f"Shape of the array for resampling: {input_data.shape}")
 
   if eta_from_p : 
     # Replace momentum by eta calculated from p and pT
     input_data[:,1] = -np.log(np.tan(np.arcsin(input_data[:,0]/input_data[:,1])/2.))
 
   if not friend :
-    if (verbose) :
+    if verbose >= 1 :
       all_branches = list(uproot.open(input).keys())
       print (f"List of all input tree branches: {pp.pformat(all_branches)}")
 
   # Loop over kernels
   kernel_list = kernels
   if not isinstance(kernels, (list, tuple)) : 
     kernel_list = [ kernels ]
@@ -138,26 +140,29 @@
     else : 
       template_sigma = kernel_name
       kernel_name = f"kern{kernel_num}"
 
     for template_seed in template_seeds : 
 
       if not ((template_seed is None) or (template_seed == 0) ) : 
-        print(f"Random sampling of raw template with seed {template_seed}")
+        if verbose >= 0 :
+          print(f"Random sampling of raw template with seed {template_seed}")
         onp.random.seed(template_seed)
         sampled_counts = onp.random.normal(counts, counts2)
       else : 
         sampled_counts = counts
 
-      print(f"Applying Gaussian smearing with kernel {template_sigma}")
+      if verbose >= 0 :
+        print(f"Applying Gaussian smearing with kernel {template_sigma}")
 
       smooth_counts = gaussian_filter(sampled_counts, template_sigma)
       template = smooth_counts, edges, normaliser
 
-      print(f"Smeared template ready, starting resampling")
+      if verbose >= 0 :
+        print(f"Smeared template ready, starting resampling")
 
       onp.random.seed(resampling_seed)
 
       data = data_transform(input_data, config, scale = scale_list )
       pid_arr, calib_stat = resample_data(data, config, vardef, template, verbose = verbose)
 
       if not (nan is None) : 
@@ -165,15 +170,15 @@
 
       output_arrays += [ pid_arr, calib_stat ]
       if (template_seed is None) or (template_seed == 0) : 
         output_branches += [ f"{pidgen}_{kernel_name}", f"{stat}_{kernel_name}" ]
       else : 
         output_branches += [ f"{pidgen}_{kernel_name}_{template_seed}", f"{stat}_{kernel_name}_{template_seed}" ]
 
-      if (verbose) : 
+      if verbose >= 1 : 
         print(f"Input data array: {input_data[:100]}")
         print(f"Data array after variable transformation: {data[:100]}")
         print(f"Resampled PID array: {pid_arr[:100]}")
         print(f"Resampling statistics array: {calib_stat[:100]}")
 
   # End of loop over kernels
```

### Comparing `pidgen2-0.3.7/src/pidgen2/resampling.py` & `pidgen2-0.3.8/src/pidgen2/resampling_new.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,23 +173,30 @@
   datasets = []
   if cachedir : 
     cache_filename = cachedir + "/" + filename.split("/")[-1]
     if cache_action == "store" : 
       os.system(f"mkdir -p {cachedir}")
       file = uproot.recreate(cache_filename, compression=uproot.ZLIB(4))
 
+  # Make branches a list of lists, if not. 
+  if not isinstance(branches[0], list) : 
+    branches = [ branches ]
+    cut = [ cut ]
+    expressions = [ expressions ]
+
   for tree in trees : 
     cache_tree = tree.replace("/", "_") # Subdirs are not supported by uproot
     if cache_action != "read" or cachedir is None : 
       try : 
         #print(f"Branches = {branches}, expressions = {expressions}, file = {filename}, tree = {tree}")
-        for t in uproot.iterate(filename + ":" + tree, library = "pd", expressions = branches, cut = cut) :
-          arr = np.stack([ t.eval(b).values for b in expressions ], axis = 1)
-          if cachedir : file[cache_tree] = { b : arr[:,i] for i,b in enumerate(expressions) }
-          datasets += [ arr ]
+        for br,c,expr in zip(branches, cut, expressions) : 
+          for t in uproot.iterate(filename + ":" + tree, library = "pd", expressions = br, cut = c) :
+            arr = np.stack([ t.eval(b).values for b in expr ], axis = 1)
+            if cachedir : file[cache_tree] = { b : arr[:,i] for i,b in enumerate(expr) }
+            datasets += [ arr ]
 
       except FileNotFoundError : 
         print(f"\n... file not found, skipping")
         break
 
       except OSError : 
         print(f"\n... XRootD error reading calibration file {filename}. Please check your Kerberos ticket and try again. ")
@@ -274,19 +281,15 @@
   for i,(s,t) in enumerate(zip(config["smear"], transform_sample)) : 
     # If "smear" not None, do uniform random smearing before transformation
     if s : 
       xs = x[:,i+1] + s[0] + (s[1]-s[0])*onp.random.uniform(size = x.shape[0])
     else : 
       xs = x[:,i+1]
     arr += [ t(xs) ]
-
-  if x.shape[1] > len(transform_sample)+1 : 
-    arr += [ x[:,-1] ] # sWeight
-  else : 
-    arr += [ np.ones_like(x[:,0]) ] # No sWeight, make unit weights
+  arr += [ x[:,-1] ] # sWeight
 
   return np.stack(arr, axis = 1)
 
 def data_transform(x, config, scale = None) :
   """
   Apply variable transformation to the data array. 
 
@@ -315,19 +318,17 @@
     variable: variable definition dictionary.
     config: calibration sample configuration dictionary.
     max_files: Maximum number of calibration files to load (0 for unlimited)
 
   """
   sample = config['sample']
   trees = config['trees']
-
-  track_prefix = config.get("prefix", "probe") + "_"
-  expressions = [variable["expression"].replace("probe_", track_prefix)] + config["branches"]
+  expressions = [variable["expression"]] + config["branches"]
   if "branches" in variable :
-    calib_branches = [v.replace("probe_", track_prefix) for v in variable["branches"]] + config["branches"]
+    calib_branches = variable["branches"] + config["branches"]
   else : 
     calib_branches = expressions
 
   calib_cache_dirname = cachedir
 
   var_cut = variable.get("cut", None)
   sample_cut = config.get("cut", None)
@@ -349,15 +350,15 @@
   hash_config = {
     "variable"  : deepcopy(variable), 
     "config"    : deepcopy(config), 
     "max_files" : max_files, 
   }
 
   # Remove keys that raw (unsmeared) template does not depend on
-  config_keys_to_ignore = ["labels", "template_sigma", "variables", "aliases"]
+  config_keys_to_ignore = ["labels", "template_sigma", "variables"]
   variable_keys_to_ignore = ["template_sigma"]
   if not mc : variable_keys_to_ignore += ["mc_expression"]
 
   for k in config_keys_to_ignore : 
     if k in hash_config["config"] : hash_config["config"].pop(k)
   for k in variable_keys_to_ignore : 
     if k in hash_config["variable"] : hash_config["variable"].pop(k)
@@ -407,15 +408,15 @@
     try : 
 
       template = load_template(template_storage + "/template.root")
       print(f"Read template from {truncate_middle(template_storage, 80)}")
 
     except FileNotFoundError : 
 
-      print(f"Template in local storage {truncate_middle(template_storage, 80)} not found.")
+      print(f"Template in local storage {truncate_middle(template_storage, 80)} not found, will create one. Be patient...")
 
   else : 
     if local_prefix == None : 
       print("Local storage location is None, will not be used")
       template_storage = None
 
   if template == None : 
@@ -443,18 +444,14 @@
 def get_or_create_mc_template(sim_version, sample_name, dataset_name, variable_name, 
                     variable, config, kernels = None, use_calib_cache = False, control_plots = False, 
                     interactive_plots = False, local_prefix = ".", global_prefix = None, 
                     max_files = 0, verbose = False, cachedir = None, external_normaliser = None) : 
   """
 
   """
-  if (verbose) : 
-    print(f"Variable definition: {variable}")
-    print(f"Sample config: {config}")
-
   hash_config = get_hash_config(sample_name, dataset_name, variable_name, variable, config, max_files, mc = True)
   config_hash = sha1(str(hash_config).encode('utf-8')).hexdigest()
 
   print(f"MC template configuration hash : {config_hash}")
 
   if cachedir is None : 
     calib_cache_dirname = None 
@@ -768,44 +765,33 @@
     template structure to be used for resampling. 
   """
   sample = config['sample']
   trees = config['trees']
 
   track_prefix = config.get("prefix")
   if not mc : 
-    if variable["expression"].find("{prefix}")>=0 : 
-      expressions = [variable["expression"].format(prefix = track_prefix)]
-    else : 
-      if track_prefix : 
-        # Fix for Lb2Lcpi sample, where track prefix differs from "probe"
-        expressions = [ variable["expression"].replace("probe_", track_prefix+"_") ]
-      else : 
-        expressions = [ variable["expression"] ]
+    expressions = [variable["expression"].format(prefix = track_prefix)]
     if "branches" in variable :
       calib_branches = [ v.format(prefix = track_prefix) for v in variable["branches"]]
     else : 
       calib_branches = copy(expressions)
   else : 
     expressions = [variable["mc_expression"].format(prefix = track_prefix)]
     if "mc_branches" in variable :
-      calib_branches = [ v.format(prefix = track_prefix) for v in variable["branches"]]
+      calib_branches = [ v.format(prefix = track_prefix) for v in variable["mc_branches"]]
     else : 
       calib_branches = copy(expressions)
 
   if "expressions" in config : 
     expressions += config["expressions"]
     calib_branches += config["branches"]
   else : 
     expressions += config["branches"]
     calib_branches += config["branches"]
 
-  if (verbose) : 
-    print(f"Expressions: {expressions}")
-    print(f"Calib branches: {calib_branches}")
-
   ranges = [ variable["data_range"]] + config["data_ranges"]
   calib_cache_branches = ["pid"] + config["calib_cache_branches"]
   normalise_bins = [variable["normalise_bins"]] + config["normalise_bins"]
   normalise_methods = [variable["normalise_method"]] + config["normalise_methods"]
   normalise_ranges = [variable["normalise_range"]] + config["normalise_ranges"]
   template_bins = [variable["template_bins"]] + config["template_bins"]
   if kernels : 
@@ -861,25 +847,24 @@
     for i,filename in enumerate(sample) : 
       sys.stdout.write(f"\rReading file ({i+1}/{len(sample)}) {truncate_middle(filename, 80)}")
       sys.stdout.flush()
       data = read_calib_file(filename, trees, expressions, calib_branches, cachedir = cachedir, cut = cut, cache_action = "store")
       if data is None : continue
       data = calib_transform(data, config, variable)
       data = de.filter_data(data, ranges + [ (-1000., 1000.) ] )
-      histograms = de.append_histograms(data, ranges = ranges, bins = normalise_bins, hists = histograms, weights = data[:,-1])
+      histograms = de.append_histograms(data, ranges = ranges, bins = normalise_bins, weights = data[:,-1])
 
   print(f"\nRead {len(sample)} calibration subsamples from remote storage.")
 
   if external_normaliser is not None : 
     print(f"Using external normaliser")
     normaliser = external_normaliser
   else : 
     print(f"Creating normaliser structure")
     normaliser = de.create_normaliser_from_histograms(histograms)
-  if (verbose) : print(f"Normaliser: {normaliser}")
 
   print(f"Pass: filling resampling template")
 
   counts = None
   counts2 = None
   edges = None
```

### Comparing `pidgen2-0.3.7/src/pidgen2/resampling_new.py` & `pidgen2-0.3.8/src/pidgen2/resampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,29 +132,30 @@
             outtree = tree.replace("/", "_") # Subdirs are not supported by uproot
             file[outtree] = { b : arr[:,i] for i,b in enumerate(expressions) }
 
           #if verbose : print(f"Reading tree {tree}, {arr.shape[0]} events")
           datasets += [ arr ]
 
       except FileNotFoundError : 
-        print(f"... file not found, skipping")
+        if verbose >= -1 : print(f"... file not found, skipping")
         break
 
       except OSError : 
-        print(f"... XRootD error reading calibration file {filename}. Please check your Kerberos ticket and try again. ")
+        if verbose >= -1 : print(f"... XRootD error reading calibration file {filename}. Please check your Kerberos ticket and try again. ")
         raise SystemExit
 
     if cachedir : 
       file.close()
 
   print("")
 
   if len(datasets) == 0 : 
-    print(f"No input calibration files found. Do you have a valid Kerberos ticket to access EOS?")
-    print(f"Will not create PID template, exiting...\n\n")
+    if verbose >= -1 : 
+      print(f"No input calibration files found. Do you have a valid Kerberos ticket to access EOS?")
+      print(f"Will not create PID template, exiting...\n\n")
     raise SystemExit
 
   return datasets
 
 def read_calib_file(filename, trees, expressions, branches, cachedir = None, cut = None, cache_action = None) : 
   """ 
   Read calibration sample from the calibration file into numpy array. 
@@ -173,30 +174,23 @@
   datasets = []
   if cachedir : 
     cache_filename = cachedir + "/" + filename.split("/")[-1]
     if cache_action == "store" : 
       os.system(f"mkdir -p {cachedir}")
       file = uproot.recreate(cache_filename, compression=uproot.ZLIB(4))
 
-  # Make branches a list of lists, if not. 
-  if not isinstance(branches[0], list) : 
-    branches = [ branches ]
-    cut = [ cut ]
-    expressions = [ expressions ]
-
   for tree in trees : 
     cache_tree = tree.replace("/", "_") # Subdirs are not supported by uproot
     if cache_action != "read" or cachedir is None : 
       try : 
         #print(f"Branches = {branches}, expressions = {expressions}, file = {filename}, tree = {tree}")
-        for br,c,expr in zip(branches, cut, expressions) : 
-          for t in uproot.iterate(filename + ":" + tree, library = "pd", expressions = br, cut = c) :
-            arr = np.stack([ t.eval(b).values for b in expr ], axis = 1)
-            if cachedir : file[cache_tree] = { b : arr[:,i] for i,b in enumerate(expr) }
-            datasets += [ arr ]
+        for t in uproot.iterate(filename + ":" + tree, library = "pd", expressions = branches, cut = cut) :
+          arr = np.stack([ t.eval(b).values for b in expressions ], axis = 1)
+          if cachedir : file[cache_tree] = { b : arr[:,i] for i,b in enumerate(expressions) }
+          datasets += [ arr ]
 
       except FileNotFoundError : 
         print(f"\n... file not found, skipping")
         break
 
       except OSError : 
         print(f"\n... XRootD error reading calibration file {filename}. Please check your Kerberos ticket and try again. ")
@@ -238,30 +232,32 @@
   """
   datasets = []
   
   for i,filename in enumerate(sample) : 
 
     calib_cache_filename = cachedir + "/" + filename.split("/")[-1]
 
-    sys.stdout.write(f"\rReading cached file ({i+1}/{len(sample)}) {truncate_middle(calib_cache_filename, 80)}")
-    sys.stdout.flush()
+    if verbose >= 0 :
+      sys.stdout.write(f"\rReading cached file ({i+1}/{len(sample)}) {truncate_middle(calib_cache_filename, 80)}")
+      sys.stdout.flush()
 
     for tree in trees : 
 
       treename = tree.replace("/", "_") # Subdirs are not supported by uproot in cache files
 
       with uproot.open(calib_cache_filename + ":" + treename) as t :
         arr = t.arrays(branches, library = "pd")[branches].to_numpy()
         datasets += [ arr ]
 
-  print("")
+  if verbose >= 0 : print("")
 
   if len(datasets) == 0 : 
-    print(f"No input cache files found.")
-    print(f"Will not create PID template, exiting...\n\n")
+    if verbose >= -1 : 
+      print(f"No input cache files found.")
+      print(f"Will not create PID template, exiting...\n\n")
     raise SystemExit
 
   return datasets
 
 def calib_transform(x, config, variable) :
   """
   Apply variable transformation to the calibration array. 
@@ -281,15 +277,19 @@
   for i,(s,t) in enumerate(zip(config["smear"], transform_sample)) : 
     # If "smear" not None, do uniform random smearing before transformation
     if s : 
       xs = x[:,i+1] + s[0] + (s[1]-s[0])*onp.random.uniform(size = x.shape[0])
     else : 
       xs = x[:,i+1]
     arr += [ t(xs) ]
-  arr += [ x[:,-1] ] # sWeight
+
+  if x.shape[1] > len(transform_sample)+1 : 
+    arr += [ x[:,-1] ] # sWeight
+  else : 
+    arr += [ np.ones_like(x[:,0]) ] # No sWeight, make unit weights
 
   return np.stack(arr, axis = 1)
 
 def data_transform(x, config, scale = None) :
   """
   Apply variable transformation to the data array. 
 
@@ -318,17 +318,19 @@
     variable: variable definition dictionary.
     config: calibration sample configuration dictionary.
     max_files: Maximum number of calibration files to load (0 for unlimited)
 
   """
   sample = config['sample']
   trees = config['trees']
-  expressions = [variable["expression"]] + config["branches"]
+
+  track_prefix = config.get("prefix", "probe") + "_"
+  expressions = [variable["expression"].replace("probe_", track_prefix)] + config["branches"]
   if "branches" in variable :
-    calib_branches = variable["branches"] + config["branches"]
+    calib_branches = [v.replace("probe_", track_prefix) for v in variable["branches"]] + config["branches"]
   else : 
     calib_branches = expressions
 
   calib_cache_dirname = cachedir
 
   var_cut = variable.get("cut", None)
   sample_cut = config.get("cut", None)
@@ -340,25 +342,26 @@
   if verbose: 
     print(f"Cut: {cut}")
 
   if max_files == 0 : 
     raw_data = read_calib_tuple(sample, trees, expressions, calib_branches, verbose = verbose, cachedir = calib_cache_dirname, cut = cut)
   else : 
     raw_data = read_calib_tuple(sample[:max_files], trees, expressions, calib_branches, verbose = verbose, cachedir = calib_cache_dirname, cut = cut)
-  print(f"Read {len(raw_data)} calibration subsamples from remote storage.")
+  if verbose >= 0 :
+    print(f"Read {len(raw_data)} calibration subsamples from remote storage.")
 
 def get_hash_config(sample_name, dataset_name, variable_name, variable, config, max_files, mc = False) : 
   hash_config = {
     "variable"  : deepcopy(variable), 
     "config"    : deepcopy(config), 
     "max_files" : max_files, 
   }
 
   # Remove keys that raw (unsmeared) template does not depend on
-  config_keys_to_ignore = ["labels", "template_sigma", "variables"]
+  config_keys_to_ignore = ["labels", "template_sigma", "variables", "aliases"]
   variable_keys_to_ignore = ["template_sigma"]
   if not mc : variable_keys_to_ignore += ["mc_expression"]
 
   for k in config_keys_to_ignore : 
     if k in hash_config["config"] : hash_config["config"].pop(k)
   for k in variable_keys_to_ignore : 
     if k in hash_config["variable"] : hash_config["variable"].pop(k)
@@ -370,15 +373,16 @@
                     max_files = 0, verbose = False, cachedir = None) : 
   """
 
   """
   hash_config = get_hash_config(sample_name, dataset_name, variable_name, variable, config, max_files)
   config_hash = sha1(str(hash_config).encode('utf-8')).hexdigest()
 
-  print(f"Template configuration hash : {config_hash}")
+  if verbose >= 0 :
+    print(f"Template configuration hash : {config_hash}")
 
   if cachedir is None : 
     calib_cache_dirname = None 
   else : 
     calib_cache_dirname = f"{cachedir}/{sample_name}/{dataset_name}/{variable_name}/"
 
   template = None
@@ -389,43 +393,50 @@
 
       #f = open(template_storage + "/config.json")
       #f.close()
       #data = onp.load(template_storage + "/template.npz", allow_pickle = True)
       #template = data["arr_0"], data["arr_1"], data["arr_2"], data["arr_3"]
       template = load_template(template_storage + "/template.root")
 
-      print(f"Read template from {truncate_middle(template_storage, 80)}")
+      if verbose >= 0 :
+        print(f"Read template from {truncate_middle(template_storage, 80)}")
 
     except FileNotFoundError : 
 
-      print(f"Template in global storage {template_storage} not found, will try local storage.")
+      if verbose >= 0 :
+        print(f"Template in global storage {template_storage} not found, will try local storage.")
       
   else : 
-    print("Global storage location is None, will not be used")
+    if verbose >= 0 :
+      print("Global storage location is None, will not be used")
 
   if template == None and local_prefix is not None : 
 
     template_storage = f"{local_prefix}/{sample_name}/{dataset_name}/{variable_name}/{config_hash}/"
     try : 
 
       template = load_template(template_storage + "/template.root")
-      print(f"Read template from {truncate_middle(template_storage, 80)}")
+      if verbose >= 0 :
+        print(f"Read template from {truncate_middle(template_storage, 80)}")
 
     except FileNotFoundError : 
 
-      print(f"Template in local storage {truncate_middle(template_storage, 80)} not found, will create one. Be patient...")
+      if verbose >= 0 :
+        print(f"Template in local storage {truncate_middle(template_storage, 80)} not found.")
 
   else : 
     if local_prefix == None : 
-      print("Local storage location is None, will not be used")
+      if verbose >= 0 : 
+        print("Local storage location is None, will not be used")
       template_storage = None
 
   if template == None : 
 
-    print("Template will be created, be patient...")
+    if verbose >= 0 :
+      print("Template will be created, be patient...")
     
     if template_storage : 
       os.system(f"mkdir -p {template_storage}")
     if (not use_calib_cache) and calib_cache_dirname : 
       os.system(f"mkdir -p {calib_cache_dirname}")
 
     template = create_template_multipass(variable, config, kernels = kernels, use_calib_cache = use_calib_cache, 
@@ -444,60 +455,72 @@
 def get_or_create_mc_template(sim_version, sample_name, dataset_name, variable_name, 
                     variable, config, kernels = None, use_calib_cache = False, control_plots = False, 
                     interactive_plots = False, local_prefix = ".", global_prefix = None, 
                     max_files = 0, verbose = False, cachedir = None, external_normaliser = None) : 
   """
 
   """
+  if verbose >= 1 : 
+    print(f"Variable definition: {variable}")
+    print(f"Sample config: {config}")
+
   hash_config = get_hash_config(sample_name, dataset_name, variable_name, variable, config, max_files, mc = True)
   config_hash = sha1(str(hash_config).encode('utf-8')).hexdigest()
 
-  print(f"MC template configuration hash : {config_hash}")
+  if verbose >= 0 :
+    print(f"MC template configuration hash : {config_hash}")
 
   if cachedir is None : 
     calib_cache_dirname = None 
   else : 
     calib_cache_dirname = f"{cachedir}/{sim_version}/{sample_name}/{dataset_name}/{variable_name}/"
 
   template = None 
 
   if global_prefix is not None : 
     template_storage = f"{global_prefix}/{sim_version}/{sample_name}/{dataset_name}/{variable_name}/{config_hash}/"
 
     try: 
       template = load_template(template_storage + "/template.root")
-      print(f"Read MC template from {truncate_middle(template_storage, 80)}")
+      if verbose >= 0 : 
+        print(f"Read MC template from {truncate_middle(template_storage, 80)}")
 
     except FileNotFoundError : 
-      print(f"MC template in global storage {template_storage} not found, will try local storage.")
+      if verbose >= 0 :
+        print(f"MC template in global storage {template_storage} not found, will try local storage.")
 
   else : 
-    print("Global MC storage location is None, will not be used")
+    if verbose >= 0 :
+      print("Global MC storage location is None, will not be used")
 
   if template == None and local_prefix is not None : 
 
     template_storage = f"{local_prefix}/{sim_version}/{sample_name}/{dataset_name}/{variable_name}/{config_hash}/"
 
     try : 
       template = load_template(template_storage + "/template.root")
-      print(f"Read MC template from {truncate_middle(template_storage, 80)}")
+      if verbose >= 0 :
+        print(f"Read MC template from {truncate_middle(template_storage, 80)}")
 
     except FileNotFoundError : 
 
-      print(f"MC Template in local storage {truncate_middle(template_storage, 80)} not found, will create one. Be patient... ")
+      if verbose >= 0 :
+        print(f"MC Template in local storage {truncate_middle(template_storage, 80)} not found, will create one. Be patient... ")
 
   else : 
 
     if local_prefix == None : 
-      print("Local MC storage location is None, will not be used")
+      if verbose >= 0 :
+        print("Local MC storage location is None, will not be used")
       template_storage = None
 
   if template == None : 
 
-    print("MC template will be created, be patient...")
+    if verbose >= 0 :
+      print("MC template will be created, be patient...")
 
     if template_storage : 
       os.system(f"mkdir -p {template_storage}")
     if (not use_calib_cache) and calib_cache_dirname : 
       os.system(f"mkdir -p {calib_cache_dirname}")
 
     template = create_template_multipass(variable, config, kernels = kernels, use_calib_cache = use_calib_cache, 
@@ -556,15 +579,16 @@
   onp.random.seed(1)  # To make variable transformation of the calibration sample (calib_transform) deterministic
 
   if use_calib_cache : 
     if max_files == 0 : 
       data = read_calib_cache(cachedir, sample, trees, expressions, verbose = verbose)
     else : 
       data = read_calib_cache(cachedir, sample[:max_files], trees, expressions, verbose = verbose)
-    print(f"Read {len(data)} calibration subsamples from local cache.")
+    if verbose >= 0 :
+      print(f"Read {len(data)} calibration subsamples from local cache.")
   else :
 
     var_cut = variable.get("cut", None)
     sample_cut = config.get("cut", None)
     cut = var_cut
     if sample_cut:
       if cut : cut = f"({cut}) & ({sample_cut})"
@@ -572,81 +596,87 @@
 
     if max_files == 0 : 
       data = read_calib_tuple(sample, trees, expressions, calib_branches, verbose = verbose, cachedir = cachedir, cut = cut)
     else : 
       data = read_calib_tuple(sample[:max_files], trees, expressions, calib_branches, verbose = verbose, cachedir = cachedir, cut = cut)
 
     #print(data)
-    print(f"Read {len(data)} calibration subsamples from remote storage.")
+    if verbose >= 0 :
+      print(f"Read {len(data)} calibration subsamples from remote storage.")
 
-  if (verbose) : print(f"Original data array: {data[0]}")
+  if verbose >= 1 : print(f"Original data array: {data[0]}")
 
-  if (verbose) : print(f"Starting to transform data array")
+  if verbose >= 1 : print(f"Starting to transform data array")
   for i, d in enumerate(data) : 
     d1 = calib_transform(d, config, variable)
     data[i] = d1
-  if (verbose) : print(f"Transformed data array: {data[0]}")
+  if verbose >= 1 : print(f"Transformed data array: {data[0]}")
 
   print(f"Starting to filter data, ranges = {ranges}")
   for i, d in enumerate(data) : 
     d1 = de.filter_data(d, ranges + [ (-1000., 1000.) ] )
     data[i] = d1
-  if (verbose) : print(f"Filtered data: {data[0]}")
+  if verbose >= 1 : print(f"Filtered data: {data[0]}")
 
   weights1 = [ d[:,-1] for d in data ]
 
   weights = []
   if max_weights : 
-    print(f"Starting to calculate flattening weights")
+    if verbose >= 0 :
+      print(f"Starting to calculate flattening weights")
     histograms = de.create_histograms_vector(data, ranges = ranges, bins = normalise_bins, weights = weights1)[1:]
     for d,w in zip(data, weights1) : 
       weights2 = de.reweight(d[:,1:-1], histograms, max_weights = max_weights, weights = w)
       weights += [ weights2 ]
-    if (verbose) : print(f"Weights vector: {weights[0]}")
+    if verbose >= 1 : print(f"Weights vector: {weights[0]}")
   else : 
     weights = weights1
 
   if external_normaliser is not None : 
-    print(f"Using external normaliser")
+    if verbose >= 0 :
+      print(f"Using external normaliser")
     normaliser = external_normaliser
   else : 
-    print(f"Creating normaliser structure")
+    if verbose >= 0 :
+      print(f"Creating normaliser structure")
     normaliser = de.create_normaliser_vector(data, ranges = ranges, bins = normalise_bins, weights = weights)
 
-  print(f"Starting to normalise data array")
+  if verbose >= 0 :
+    print(f"Starting to normalise data array")
   norm_data = []
   for d in data : 
     norm_data += [ de.normalise(d[:,:-1], normaliser, normalise_methods) ]
-  if (verbose) : print(f"Normalised data array: {norm_data[0]}")
+  if verbose >= 1 : print(f"Normalised data array: {norm_data[0]}")
 
   #unnorm_data = de.unnormalise(norm_data, normaliser, normalise_methods)
 
   counts = None
   counts2 = None
   edges = None
   for i,(nd,w) in enumerate(zip(norm_data, weights)) : 
-    sys.stdout.write(f"\rFilling histogram for subsample {i+1}/{len(norm_data)}")
-    sys.stdout.flush()
+    if verbose >= 0 :
+      sys.stdout.write(f"\rFilling histogram for subsample {i+1}/{len(norm_data)}")
+      sys.stdout.flush()
     c, e = np.histogramdd(nd, bins = template_bins, range = normalise_ranges, weights = w)
     c2, e2 = np.histogramdd(nd, bins = template_bins, range = normalise_ranges, weights = w**2)
     if counts is None : 
       counts = c
       counts2 = c2
       edges = e
     else : 
       counts += c
       counts2 += c2
 
-  print("")
+  if verbose >= 0 : print("")
 
   if control_plots : 
 
-    print(f"Producing control plots")
+    if verbose >= 0 : print(f"Producing control plots")
 
-    print(f"Applying default Gaussian smearing")
+    if verbose >= 0 : print(f"Applying default Gaussian smearing")
     smooth_counts = gaussian_filter(counts, template_sigma)
 
     labels = config["labels"]
     names = config["names"]
 
     log = True
 
@@ -765,33 +795,44 @@
     template structure to be used for resampling. 
   """
   sample = config['sample']
   trees = config['trees']
 
   track_prefix = config.get("prefix")
   if not mc : 
-    expressions = [variable["expression"].format(prefix = track_prefix)]
+    if variable["expression"].find("{prefix}")>=0 : 
+      expressions = [variable["expression"].format(prefix = track_prefix)]
+    else : 
+      if track_prefix : 
+        # Fix for Lb2Lcpi sample, where track prefix differs from "probe"
+        expressions = [ variable["expression"].replace("probe_", track_prefix+"_") ]
+      else : 
+        expressions = [ variable["expression"] ]
     if "branches" in variable :
       calib_branches = [ v.format(prefix = track_prefix) for v in variable["branches"]]
     else : 
       calib_branches = copy(expressions)
   else : 
     expressions = [variable["mc_expression"].format(prefix = track_prefix)]
     if "mc_branches" in variable :
-      calib_branches = [ v.format(prefix = track_prefix) for v in variable["mc_branches"]]
+      calib_branches = [ v.format(prefix = track_prefix) for v in variable["branches"]]
     else : 
       calib_branches = copy(expressions)
 
   if "expressions" in config : 
     expressions += config["expressions"]
     calib_branches += config["branches"]
   else : 
     expressions += config["branches"]
     calib_branches += config["branches"]
 
+  if verbose >= 1 : 
+    print(f"Expressions: {expressions}")
+    print(f"Calib branches: {calib_branches}")
+
   ranges = [ variable["data_range"]] + config["data_ranges"]
   calib_cache_branches = ["pid"] + config["calib_cache_branches"]
   normalise_bins = [variable["normalise_bins"]] + config["normalise_bins"]
   normalise_methods = [variable["normalise_method"]] + config["normalise_methods"]
   normalise_ranges = [variable["normalise_range"]] + config["normalise_ranges"]
   template_bins = [variable["template_bins"]] + config["template_bins"]
   if kernels : 
@@ -808,96 +849,104 @@
   sample_cut = config.get("cut", None)
   cut = var_cut
   if sample_cut:
     if cut : cut = f"({cut}) & ({sample_cut})"
     else : cut = sample_cut
   
   if max_weights : 
-    print(f"Pass: filling histograms for flattening weights")
+    if verbose >= 0 :
+      print(f"Pass: filling histograms for flattening weights")
     whistograms = None
     for i,filename in enumerate(sample) : 
       sys.stdout.write(f"Reading file ({i+1}/{len(sample)}) {truncate_middle(filename, 80)}\r")
       sys.stdout.flush()
       data = read_calib_file(filename, trees, expressions, calib_branches, cachedir = cachedir, cut = cut, cache_action = "store")
       if data is None : continue
       data = calib_transform(data, config, variable)
       data = de.filter_data(data, ranges + [ (-1000., 1000.) ] )
       whistograms = de.append_histograms(data, ranges = ranges, bins = normalise_bins, hists = whistograms, weights = data[:,-1])
 
     whistograms = whistograms[1:]  # Don't need the histogram for PID response itself
 
-    if (verbose) : print(f"\nFlattening weight histograms: {whistograms}")
+    if verbose >= 1 : print(f"\nFlattening weight histograms: {whistograms}")
 
-    print(f"\nPass: filling cumulative distributions for data preprocessing")
+    if verbose >= 0 : 
+      print(f"\nPass: filling cumulative distributions for data preprocessing")
     histograms = None
     for i,filename in enumerate(sample) : 
       sys.stdout.write(f"\rReading file ({i+1}/{len(sample)}) {truncate_middle(filename, 80)}")
       sys.stdout.flush()
       data = read_calib_file(filename, trees, expressions, calib_branches, cachedir = cachedir, cut = cut, cache_action = "read")
       if data is None : continue
       data = calib_transform(data, config, variable)
       data = de.filter_data(data, ranges + [ (-1000., 1000.) ] )
       w = data[:,-1]
       w2 = de.reweight(data[:,1:-1], whistograms, max_weights = max_weights, weights = w)
  
-      if (verbose) : print(f"\nFlattening weights: {w2/w}")
+      if verbose >= 1 : print(f"\nFlattening weights: {w2/w}")
       histograms = de.append_histograms(data, ranges = ranges, bins = normalise_bins, hists = histograms, weights = w2)
   else : 
-    print(f"\nPass: filling cumulative distributions for data preprocessing")
+    if verbose >= 0 :
+      print(f"\nPass: filling cumulative distributions for data preprocessing")
     histograms = None
     for i,filename in enumerate(sample) : 
       sys.stdout.write(f"\rReading file ({i+1}/{len(sample)}) {truncate_middle(filename, 80)}")
       sys.stdout.flush()
       data = read_calib_file(filename, trees, expressions, calib_branches, cachedir = cachedir, cut = cut, cache_action = "store")
       if data is None : continue
       data = calib_transform(data, config, variable)
       data = de.filter_data(data, ranges + [ (-1000., 1000.) ] )
-      histograms = de.append_histograms(data, ranges = ranges, bins = normalise_bins, weights = data[:,-1])
+      histograms = de.append_histograms(data, ranges = ranges, bins = normalise_bins, hists = histograms, weights = data[:,-1])
 
-  print(f"\nRead {len(sample)} calibration subsamples from remote storage.")
+  if verbose >= 0 : 
+    print(f"\nRead {len(sample)} calibration subsamples from remote storage.")
 
   if external_normaliser is not None : 
-    print(f"Using external normaliser")
+    if verbose >= 0 :
+      print(f"Using external normaliser")
     normaliser = external_normaliser
   else : 
-    print(f"Creating normaliser structure")
+    if verbose >= 0 :
+      print(f"Creating normaliser structure")
     normaliser = de.create_normaliser_from_histograms(histograms)
+  if verbose >= 1 : print(f"Normaliser: {normaliser}")
 
-  print(f"Pass: filling resampling template")
+  if verbose >= 0 : print(f"Pass: filling resampling template")
 
   counts = None
   counts2 = None
   edges = None
 
   transformed_hists = len(ranges)*[ None ]
   weighted_hists = len(ranges)*[ None ]
   normalised_hists = len(ranges)*[ None ]
 
   for i,filename in enumerate(sample) : 
-    sys.stdout.write(f"\rReading file ({i+1}/{len(sample)}) {truncate_middle(filename, 80)}")
-    sys.stdout.flush()
+    if verbose >= 0 :
+      sys.stdout.write(f"\rReading file ({i+1}/{len(sample)}) {truncate_middle(filename, 80)}")
+      sys.stdout.flush()
     data0 = read_calib_file(filename, trees, expressions, calib_branches, cachedir = cachedir, cut = cut, cache_action = "read")
     if data0 is None : continue
     data = calib_transform(data0, config, variable)
     data = de.filter_data(data, ranges + [ (-1000., 1000.) ] )
 
-    if (verbose) : print(f"\nFiltered data: {data}")
+    if verbose >= 1 : print(f"\nFiltered data: {data}")
 
     if max_weights : 
       w1 = data[:,-1]
       w2 = de.reweight(data[:,1:-1], whistograms, max_weights = max_weights, weights = w1)
       w = w2
-      if (verbose) : 
+      if verbose >= 1 : 
         print(f"sWeights: {w1}")
         print(f"Flattening weights: {w2}")
     else : 
       w = data[:,-1]
 
     norm_data = de.normalise(data[:,:-1], normaliser, normalise_methods)
-    if (verbose) : print(f"Normalised data array: {norm_data}")
+    if verbose >= 1 : print(f"Normalised data array: {norm_data}")
 
     c, e = np.histogramdd(norm_data, bins = template_bins, range = normalise_ranges, weights = w)
     c2, e2 = np.histogramdd(norm_data, bins = template_bins, range = normalise_ranges, weights = w**2)
     if counts is None : 
       counts = c
       counts2 = c2
       edges = e
@@ -921,21 +970,23 @@
 
         c,e = np.histogram(norm_data[:,v], bins = 50, range = normalise_ranges[v], weights = w)
         if normalised_hists[v] is None : 
           normalised_hists[v] = [c, e]
         else : 
           normalised_hists[v][0] += c          
 
-  print("")
+  if verbose >= 0 : print("")
 
   if control_plots : 
 
-    print(f"Producing control plots")
+    if verbose >= 0 :
+      print(f"Producing control plots")
 
-    print(f"Applying default Gaussian smearing")
+    if verbose >= 0 :
+      print(f"Applying default Gaussian smearing")
     smooth_counts = gaussian_filter(counts, template_sigma)
 
     labels = config["labels"]
     names = config["names"]
 
     log = True
 
@@ -1120,26 +1171,27 @@
   normalise_methods = [variable["normalise_method"]] + config["normalise_methods"]
   normalise_ranges = [variable["normalise_range"]] + config["normalise_ranges"]
   resample_bins = variable["resample_bins"]
   transform_backward = eval("lambda x : (" + variable["transform_backward"] + ")")
 
   norm_data = de.normalise(data, normaliser[1:], normalise_methods[1:])
 
-  if (verbose) : 
+  if verbose >= 1 : 
     print(f"Normalised data: {norm_data[:100]}")
 
   start_index = 0
   chunk = 0
   resampled_pid_arrs = []
   pid_calib_stats = []
   stop = False
   chunks = (len(norm_data)-1)//chunk_size+1
 
   while not stop : 
-    print(f"Resampling chunk {chunk+1}/{chunks}, index={start_index}/{len(norm_data)}")
+    if verbose >= 0 :
+      print(f"Resampling chunk {chunk+1}/{chunks}, index={start_index}/{len(norm_data)}")
     end_index = start_index + chunk_size
     if end_index >= len(norm_data) :
       end_index = len(norm_data)
       stop = True
 
     rnd = onp.random.uniform(size = (end_index-start_index, ))
     norm_pid, stats = de.resample(counts, edges, norm_data[start_index:end_index,], 
@@ -1189,27 +1241,28 @@
   normalise_methods = [variable["normalise_method"]] + config["normalise_methods"]
   normalise_ranges = [variable["normalise_range"]] + config["normalise_ranges"]
   resample_bins = variable["resample_bins"]
   transform_backward = eval("lambda x : (" + variable["transform_backward"] + ")")
 
   norm_data = de.normalise(data, normaliser, normalise_methods)
 
-  if (verbose) : 
+  if verbose >= 1 : 
     print(f"Normalised data: {norm_data[:100]}")
 
   start_index = 0
   chunk = 0
   pid_calib_stats = []
   pid_mc_stats = []
   corrected_pid_arrs = []
   stop = False
   chunks = (len(norm_data)-1)//chunk_size+1
 
   while not stop : 
-    print(f"Correcting chunk {chunk+1}/{chunks}, index={start_index}/{len(norm_data)}")
+    if verbose >= 0 :
+      print(f"Correcting chunk {chunk+1}/{chunks}, index={start_index}/{len(norm_data)}")
     end_index = start_index + chunk_size
     if end_index >= len(norm_data) :
       end_index = len(norm_data)
       stop = True
 
     prob, mc_stats = de.probability(mc_counts, edges, norm_data[start_index:end_index,1:], 
                           norm_data[start_index:end_index,0],
```

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi.py` & `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 
 from ..datasets import converted_run1_pidcalib_datasets_dstar_k as ds_run1
 from ..datasets import legacy_run2_pidcalib_datasets as ds_run2
 from ..mc_datasets import dstar_run2sim09_datasets as mc_ds_run2sim09
+from ..mc_datasets import lcmu_run1sim09_datasets as mc_ds_run1sim09
 
 from itertools import product
 
 probnn_responses = ["pi", "K", "p", "e", "mu", "piNotK", "piNotKp", "KNotpi", "KNotpip", "pNotK", "pNotpiK"]
 
 def brunel_aliases(year) : 
     """
@@ -89,14 +90,32 @@
                    "MC12TuneV3_ProbNNpNotK", "MC12TuneV3_ProbNNpNotpiK", 
                   ], 
     **common_params, 
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
 }
 
+mc_sample_run1 = {
+  f"Sim09_{pol}_{year}" : {
+    "sample" : mc_ds_run1sim09[f"{pol}_{year}"],
+    "prefix" : "k", 
+    "branches" : [
+      "k_PT", 
+      "k_ETA", 
+      "nTracks", 
+    ], 
+    "trees" : ["lc/nt"], 
+    "variables" : [ f"MC12TuneV2_ProbNN{i}" for i in probnn_responses_mc ] + 
+                  [ f"MC12TuneV3_ProbNN{i}" for i in probnn_responses_mc ] + 
+                  ["CombDLLp", "CombDLLK"], 
+    **common_params, 
+  } 
+  for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
+}
+
 mc_sample_run2 = {
   f"Sim09_{pol}_{year}" : {
     "sample" : mc_ds_run2sim09[f"{pol}_{year}"], 
     "prefix" : "dk", 
     "branches" : [
       "dk_PT", 
       "dk_ETA", 
@@ -110,8 +129,8 @@
   }
   for pol in ["MagUp", "MagDown"] for year in ["2015", "2016", "2017", "2018"]
 }
 
 # The visible dictionaries with data and MC sample definitions
 
 sample = {**sample_run1, **sample_run2}
-mc_sample = {**mc_sample_run2 }
+mc_sample = {**mc_sample_run1, **mc_sample_run2 }
```

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi_M.py` & `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_M.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi_P.py` & `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_P.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi_PIDKgt4.py` & `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_PIDKgt4.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/K_Dstar2Dpi_PtEta.py` & `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_PtEta.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/__init__.py` & `pidgen2-0.3.8/src/pidgen2/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/e_B2JpsieeK.py` & `pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/e_B2JpsieeK_Brem.py` & `pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK_Brem.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/e_B2JpsieeK_NoBrem.py` & `pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK_NoBrem.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/gamma_B2KstarGamma.py` & `pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGamma.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/gamma_B2KstarGammaType0.py` & `pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGammaType0.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/gamma_B2KstarGammaType1.py` & `pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGammaType1.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/mu_Jpsi2mumu.py` & `pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/mu_Jpsi2mumu_isMuon.py` & `pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumu_isMuon.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/mu_Jpsi2mumunopt.py` & `pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumunopt.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/mu_Jpsi2mumunopt_isMuon.py` & `pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumunopt_isMuon.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/p_IncLc.py` & `pidgen2-0.3.8/src/pidgen2/samples/p_IncLc.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 
 from ..datasets import legacy_run2_pidcalib_datasets as ds_run2
 from ..datasets import converted_run1_pidcalib_datasets_inclc_p as ds_run1
 from ..mc_datasets import lb2jpsipk_run2sim09_datsets as mc_run2sim09
+from ..mc_datasets import lcmu_run1sim09_datasets as mc_run1sim09
 
 from itertools import product
 
 probnn_responses = ["pi", "K", "p", "e", "mu", "piNotK", "piNotKp", "KNotpi", "KNotpip", "pNotK", "pNotpiK"]
 
 def brunel_aliases(year) : 
     """
@@ -89,14 +90,32 @@
                    "MC12TuneV3_ProbNNpNotK", "MC12TuneV3_ProbNNpNotpiK", 
                   ], 
     **common_params
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
 }
 
+mc_sample_run1 = {
+  f"Sim09_{pol}_{year}" : {
+    "sample" : mc_run1sim09[f"{pol}_{year}"],
+    "prefix" : "p", 
+    "branches" : [
+      "p_PT", 
+      "p_ETA", 
+      "nTracks", 
+    ], 
+    "trees" : ["lc/nt"], 
+    "variables" : [ f"MC12TuneV2_ProbNN{i}" for i in probnn_responses_mc ] + 
+                  [ f"MC12TuneV3_ProbNN{i}" for i in probnn_responses_mc ] + 
+                  ["CombDLLp", "CombDLLK"], 
+    **common_params, 
+  } 
+  for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
+}
+
 mc_sample_run2 = {
   f"Sim09_{pol}_{year}" : {
     "sample" : mc_run2sim09[f"{pol}_{year}"], 
     "prefix" : "p", 
     "branches" : [
       "p_PT", 
       "p_ETA", 
@@ -108,8 +127,8 @@
     "aliases" : brunel_aliases_mc, 
     **common_params, 
   }
   for pol in ["MagUp", "MagDown"] for year in ["2016", "2017", "2018"]
 }
 
 sample = {**sample_run1, **sample_run2}
-mc_sample = {**mc_sample_run2 }
+mc_sample = {**mc_sample_run1, **mc_sample_run2}
```

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/p_Lambda2ppi.py` & `pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 
 from ..datasets import legacy_run2_pidcalib_datasets as ds_run2
 from ..datasets import converted_run1_pidcalib_datasets_lam0_p as ds_run1
 from ..mc_datasets import lb2jpsipk_run2sim09_datsets as mc_run2sim09
+from ..mc_datasets import lcmu_run1sim09_datasets as mc_run1sim09
 
 from itertools import product
 from copy import copy
 
 probnn_responses = ["pi", "K", "p", "e", "mu", "piNotK", "piNotKp", "KNotpi", "KNotpip", "pNotK", "pNotpiK"]
 
 def brunel_aliases(year) : 
@@ -98,14 +99,32 @@
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
 }
 
 mc_params = copy(common_params)
 mc_params['max_weights'] = None
 
+mc_sample_run1 = {
+  f"Sim09_{pol}_{year}" : {
+    "sample" : mc_run1sim09[f"{pol}_{year}"],
+    "prefix" : "p", 
+    "branches" : [
+      "p_PT", 
+      "p_ETA", 
+      "nTracks", 
+    ], 
+    "trees" : ["lc/nt"], 
+    "variables" : [ f"MC12TuneV2_ProbNN{i}" for i in probnn_responses_mc ] + 
+                  [ f"MC12TuneV3_ProbNN{i}" for i in probnn_responses_mc ] + 
+                  ["CombDLLp", "CombDLLK"], 
+    **mc_params, 
+  } 
+  for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
+}
+
 mc_sample_run2 = {
   f"Sim09_{pol}_{year}" : {
     "sample" : mc_run2sim09[f"{pol}_{year}"], 
     "prefix" : "p", 
     "branches" : [
       "p_PT", 
       "p_ETA", 
@@ -117,8 +136,8 @@
     "aliases" : brunel_aliases_mc, 
     **mc_params, 
   }
   for pol in ["MagUp", "MagDown"] for year in ["2015", "2016", "2017", "2018"]
 }
 
 sample = {**sample_run1, **sample_run2}
-mc_sample = {**mc_sample_run2 }
+mc_sample = {**mc_sample_run1, **mc_sample_run2 }
```

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/p_Lambda2ppi_Prompt.py` & `pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi_Prompt.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/p_Lambda2ppi_Prompt_PIDpgt0.py` & `pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi_Prompt_PIDpgt0.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/p_Lb2Lcmu.py` & `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_M.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,111 +5,88 @@
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 
+from ..datasets import converted_run1_pidcalib_datasets_dstar_pi as ds_run1
 from ..datasets import legacy_run2_pidcalib_datasets as ds_run2
-from ..datasets import converted_run1_pidcalib_datasets_lblcmu_p as ds_run1
-from ..mc_datasets import lb2jpsipk_run2sim09_datsets as mc_run2sim09
-
 from itertools import product
 
 probnn_responses = ["pi", "K", "p", "e", "mu", "piNotK", "piNotKp", "KNotpi", "KNotpip", "pNotK", "pNotpiK"]
 
 def brunel_aliases(year) : 
     """
       Define aliases for Brunel variables in 2017, 2018 samples
       to point to Online versions. 
     """
     if year in ["2017", "2018"] : 
         return { "Brunel_MC15TuneV1_ProbNN" + var : "MC15TuneV1_ProbNN" + var for var in probnn_responses }
     else : return {}
 
-probnn_responses_mc = ["pi", "K", "p"]
-brunel_aliases_mc = { "Brunel_MC15TuneV1_ProbNN" + var : "MC15TuneV1_ProbNN" + var for var in probnn_responses_mc }
-
 common_params = {
+    "calib_cache_branches" : ["pt", "eta", "ntr", "sw"],          # Names of variable branches in ROOT tree of the cache file 
+    "data_ranges" : [ (2.4, 4.4), (1.9, 5.0), (0.7, 3.1) ],       # Ranges of each variable after transformation
+    "labels" : [r"PID", r"$p_T$", r"$\eta$", r"$N_{\rm tr}$"],    # Labels for plots
+    "names" : ["pid", "pt", "eta", "ntr"],                        # Short names of each variable for plot file names
+    "max_weights" : None, 
     "smear" : [ None, None, (-0.5, 0.5) ], 
-    "transform" : [ 
+    "transform" : [                                               # Transformation functions for each variable
       "np.log10(x)",   # pT transformation
       "x",             # eta
       "np.log10(x)",   # number of tracks
     ], 
-    "calib_cache_branches" : ["pt", "eta", "ntr", "sw"], 
-    "data_ranges" : [ (2.4, 4.4), (1.9, 5.0), (0.7, 3.1) ], 
-    "labels" : [r"PID", r"$p_T$", r"$\eta$", r"$N_{\rm tr}$"],    # Labels for plots
-    "names" : ["pid", "pt", "eta", "ntr"],                        # Short names of each variable for plot file names
-    "max_weights" : None, 
-    "normalise_bins" : [100, 100, 100], 
-    "normalise_methods" : ["scale", "scale", "flatten"], 
-    "normalise_ranges" : 3*[ (0., 1.) ], 
-    "template_bins" : [70, 70, 20], 
+    "normalise_bins" : [100, 100, 100],                           # Number of bins for normalisation of each variable
+    "normalise_methods" : ["scale", "scale", "flatten"],          # Normalisation method for each variable ("scale", "normalise", "flatten")
+    "normalise_ranges" : 2*[ (0., 1.) ] + [ (0., 1.) ],           # Ranges of each variable after normalisation
+    "template_bins" : [70, 70, 20],                               # Number of bins for each variable in the template 
     "template_sigma" : {
-      "default" : [2., 4., 4.], 
-      "syst1"   : [3., 6., 6.], 
+      "default" : [2., 4., 4.],                              # Smearing parameter for the template for each variable. 
+      "syst1"   : [3., 6., 6.],                              # Smearing parameter for the template for each variable. 
     }
 }
 
 sample_run2 = {
   f"{pol}_{year}" : { 
     "sample" : ds_run2[f"{pol}_{year}"], 
     "branches" : [ 
       "probe_Brunel_PT", 
       "probe_Brunel_ETA", 
       "nTracks_Brunel", 
       "probe_sWeight" 
     ], 
-    "trees" : ["LbLcMu_PTuple/DecayTree", "LbLcMu_PbarTuple/DecayTree"], 
+    "trees" : ['DSt_PiMTuple/DecayTree'], 
     "variables" : ["CombDLLK", "CombDLLmu", "CombDLLe", "CombDLLp"] + 
                   [ f"{b}MC15TuneV1_ProbNN{i}" for b, i in product(["", "Brunel_"], probnn_responses) ], 
     "aliases" : brunel_aliases(year), 
-    **common_params
+    **common_params, 
   } 
-  for pol in ["MagUp", "MagDown"] for year in ["2016", "2017", "2018"]
+  for pol in ["MagUp", "MagDown"] for year in ["2015", "2016", "2017", "2018"]
 }
 
 sample_run1 = {
   f"{pol}_{year}" : { 
     "sample" : ds_run1[f"{pol}_{year}"], 
     "branches" : [ 
       "probe_PT", 
       "probe_ETA", 
       "nTracks", 
       "probe_sWeight" 
     ], 
-    "trees" : ["DecayTree"], 
+    "trees" : ['DecayTree'], 
     "variables" : [
                    "CombDLLK", "CombDLLmu", "CombDLLe", "CombDLLp", 
                    "MC12TuneV2_ProbNNpi", "MC12TuneV2_ProbNNK", "MC12TuneV2_ProbNNp", 
                    "MC12TuneV3_ProbNNpi", "MC12TuneV3_ProbNNK", "MC12TuneV3_ProbNNp", 
                    "MC12TuneV3_ProbNNe", "MC12TuneV3_ProbNNmu", 
                    "MC12TuneV3_ProbNNpiNotK", "MC12TuneV3_ProbNNpiNotKp", 
                    "MC12TuneV3_ProbNNKNotpi", "MC12TuneV3_ProbNNKNotpip", 
                    "MC12TuneV3_ProbNNpNotK", "MC12TuneV3_ProbNNpNotpiK", 
                   ], 
-    **common_params
+    "cut" : "probe_trackcharge<0", 
+    **common_params, 
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
 }
 
-mc_sample_run2 = {
-  f"Sim09_{pol}_{year}" : {
-    "sample" : mc_run2sim09[f"{pol}_{year}"], 
-    "prefix" : "p", 
-    "branches" : [
-      "p_PT", 
-      "p_ETA", 
-      "nTracks",
-    ], 
-    "trees" : ["lc/nt"], 
-    "variables" : [ f"{b}MC15TuneV1_ProbNN{i}" for b, i in product(["", "Brunel_"], probnn_responses_mc) ] + 
-                  ["CombDLLp", "CombDLLK"], 
-    "aliases" : brunel_aliases_mc, 
-    **common_params, 
-  }
-  for pol in ["MagUp", "MagDown"] for year in ["2016", "2017", "2018"]
-}
-
 sample = {**sample_run1, **sample_run2}
-mc_sample = {**mc_sample_run2 }
```

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/p_Lb2Lcpi.py` & `pidgen2-0.3.8/src/pidgen2/samples/p_Lb2Lcpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/p_Test.py` & `pidgen2-0.3.8/src/pidgen2/samples/p_Test.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi.py` & `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_scale.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 
-from ..datasets import converted_run1_pidcalib_datasets_dstar_pi as ds_run1
+from ..datasets import converted_run1_pidcalib_datasets_dstar_k as ds_run1
 from ..datasets import legacy_run2_pidcalib_datasets as ds_run2
 from ..mc_datasets import dstar_run2sim09_datasets as mc_ds_run2sim09
+from ..mc_datasets import lcmu_run1sim09_datasets as mc_ds_run1sim09
 
 from itertools import product
 
 probnn_responses = ["pi", "K", "p", "e", "mu", "piNotK", "piNotKp", "KNotpi", "KNotpip", "pNotK", "pNotpiK"]
 
 def brunel_aliases(year) : 
     """
@@ -38,33 +39,33 @@
     "smear" : [ None, None, (-0.5, 0.5) ], 
     "transform" : [                                               # Transformation functions for each variable
       "np.log10(x)",   # pT transformation
       "x",             # eta
       "np.log10(x)",   # number of tracks
     ], 
     "normalise_bins" : [100, 100, 100],                           # Number of bins for normalisation of each variable
-    "normalise_methods" : ["scale", "scale", "flatten"],          # Normalisation method for each variable ("scale", "normalise", "flatten")
+    "normalise_methods" : ["scale", "scale", "scale"],            # Normalisation method for each variable ("scale", "normalise", "flatten")
     "normalise_ranges" : 2*[ (0., 1.) ] + [ (0., 1.) ],           # Ranges of each variable after normalisation
     "template_bins" : [70, 70, 20],                               # Number of bins for each variable in the template 
-    "template_sigma" : {
-      "default" : [2., 4., 4.],                              # Smearing parameter for the template for each variable. 
-      "syst1"   : [3., 6., 6.],                              # Smearing parameter for the template for each variable. 
+    "template_sigma" : { 
+      "default" : [2., 4., 4.],                                   # Smearing parameter for the template for each variable. 
+      "syst1"   : [3., 6., 6.], 
     }
 }
 
 sample_run2 = {
   f"{pol}_{year}" : { 
     "sample" : ds_run2[f"{pol}_{year}"], 
     "branches" : [ 
       "probe_Brunel_PT", 
       "probe_Brunel_ETA", 
       "nTracks_Brunel", 
       "probe_sWeight" 
     ], 
-    "trees" : ['DSt_PiPTuple/DecayTree', 'DSt_PiMTuple/DecayTree'], 
+    "trees" : ['DSt_KPTuple/DecayTree', 'DSt_KMTuple/DecayTree'], 
     "variables" : ["CombDLLK", "CombDLLmu", "CombDLLe", "CombDLLp"] + 
                   [ f"{b}MC15TuneV1_ProbNN{i}" for b, i in product(["", "Brunel_"], probnn_responses) ], 
     "aliases" : brunel_aliases(year), 
     **common_params, 
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2015", "2016", "2017", "2018"]
 }
@@ -78,38 +79,58 @@
       "nTracks", 
       "probe_sWeight" 
     ], 
     "trees" : ['DecayTree'], 
     "variables" : [
                    "CombDLLK", "CombDLLmu", "CombDLLe", "CombDLLp", 
                    "MC12TuneV2_ProbNNpi", "MC12TuneV2_ProbNNK", "MC12TuneV2_ProbNNp", 
-                   "MC12TuneV3_ProbNNpi", "MC12TuneV3_ProbNNK", "MC12TuneV3_ProbNNp", 
+                   "MC12TuneV3_ProbNNpi", "MC12TuneV3_ProbNNK_scale", "MC12TuneV3_ProbNNp", 
                    "MC12TuneV3_ProbNNe", "MC12TuneV3_ProbNNmu", 
                    "MC12TuneV3_ProbNNpiNotK", "MC12TuneV3_ProbNNpiNotKp", 
                    "MC12TuneV3_ProbNNKNotpi", "MC12TuneV3_ProbNNKNotpip", 
                    "MC12TuneV3_ProbNNpNotK", "MC12TuneV3_ProbNNpNotpiK", 
                   ], 
     **common_params, 
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
 }
 
+mc_sample_run1 = {
+  f"Sim09_{pol}_{year}" : {
+    "sample" : mc_ds_run1sim09[f"{pol}_{year}"],
+    "prefix" : "k", 
+    "branches" : [
+      "k_PT", 
+      "k_ETA", 
+      "nTracks", 
+    ], 
+    "trees" : ["lc/nt"], 
+    "variables" : [ f"MC12TuneV2_ProbNN{i}" for i in probnn_responses_mc ] + 
+                  [ f"MC12TuneV3_ProbNN{i}_scale" for i in probnn_responses_mc ] + 
+                  ["CombDLLp", "CombDLLK"], 
+    **common_params, 
+  } 
+  for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
+}
+
 mc_sample_run2 = {
   f"Sim09_{pol}_{year}" : {
     "sample" : mc_ds_run2sim09[f"{pol}_{year}"], 
-    "prefix" : "dpi", 
+    "prefix" : "dk", 
     "branches" : [
-      "dpi_PT", 
-      "dpi_ETA", 
+      "dk_PT", 
+      "dk_ETA", 
       "nTracks",
     ], 
     "trees" : ["dstar/dstar"], 
     "variables" : [ f"{b}MC15TuneV1_ProbNN{i}" for b, i in product(["", "Brunel_"], probnn_responses_mc) ] + 
                   ["CombDLLp", "CombDLLK"], 
     "aliases" : brunel_aliases_mc, 
     **common_params, 
   }
   for pol in ["MagUp", "MagDown"] for year in ["2015", "2016", "2017", "2018"]
 }
 
+# The visible dictionaries with data and MC sample definitions
+
 sample = {**sample_run1, **sample_run2}
-mc_sample = {**mc_sample_run2 }
+mc_sample = {**mc_sample_run1, **mc_sample_run2 }
```

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi_M.py` & `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_P.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "sample" : ds_run2[f"{pol}_{year}"], 
     "branches" : [ 
       "probe_Brunel_PT", 
       "probe_Brunel_ETA", 
       "nTracks_Brunel", 
       "probe_sWeight" 
     ], 
-    "trees" : ['DSt_PiMTuple/DecayTree'], 
+    "trees" : ['DSt_PiPTuple/DecayTree'], 
     "variables" : ["CombDLLK", "CombDLLmu", "CombDLLe", "CombDLLp"] + 
                   [ f"{b}MC15TuneV1_ProbNN{i}" for b, i in product(["", "Brunel_"], probnn_responses) ], 
     "aliases" : brunel_aliases(year), 
     **common_params, 
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2015", "2016", "2017", "2018"]
 }
@@ -79,14 +79,14 @@
                    "MC12TuneV2_ProbNNpi", "MC12TuneV2_ProbNNK", "MC12TuneV2_ProbNNp", 
                    "MC12TuneV3_ProbNNpi", "MC12TuneV3_ProbNNK", "MC12TuneV3_ProbNNp", 
                    "MC12TuneV3_ProbNNe", "MC12TuneV3_ProbNNmu", 
                    "MC12TuneV3_ProbNNpiNotK", "MC12TuneV3_ProbNNpiNotKp", 
                    "MC12TuneV3_ProbNNKNotpi", "MC12TuneV3_ProbNNKNotpip", 
                    "MC12TuneV3_ProbNNpNotK", "MC12TuneV3_ProbNNpNotpiK", 
                   ], 
-    "cut" : "probe_trackcharge<0", 
+    "cut" : "probe_trackcharge>0", 
     **common_params, 
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
 }
 
 sample = {**sample_run1, **sample_run2}
```

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi_P.py` & `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,27 +39,28 @@
     "normalise_bins" : [100, 100, 100],                           # Number of bins for normalisation of each variable
     "normalise_methods" : ["scale", "scale", "flatten"],          # Normalisation method for each variable ("scale", "normalise", "flatten")
     "normalise_ranges" : 2*[ (0., 1.) ] + [ (0., 1.) ],           # Ranges of each variable after normalisation
     "template_bins" : [70, 70, 20],                               # Number of bins for each variable in the template 
     "template_sigma" : {
       "default" : [2., 4., 4.],                              # Smearing parameter for the template for each variable. 
       "syst1"   : [3., 6., 6.],                              # Smearing parameter for the template for each variable. 
-    }
+    }, 
+    "cut" : "probe_PIDK<2.", 
 }
 
 sample_run2 = {
   f"{pol}_{year}" : { 
     "sample" : ds_run2[f"{pol}_{year}"], 
     "branches" : [ 
       "probe_Brunel_PT", 
       "probe_Brunel_ETA", 
       "nTracks_Brunel", 
       "probe_sWeight" 
     ], 
-    "trees" : ['DSt_PiPTuple/DecayTree'], 
+    "trees" : ['DSt_PiPTuple/DecayTree', 'DSt_PiMTuple/DecayTree'], 
     "variables" : ["CombDLLK", "CombDLLmu", "CombDLLe", "CombDLLp"] + 
                   [ f"{b}MC15TuneV1_ProbNN{i}" for b, i in product(["", "Brunel_"], probnn_responses) ], 
     "aliases" : brunel_aliases(year), 
     **common_params, 
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2015", "2016", "2017", "2018"]
 }
@@ -79,14 +80,13 @@
                    "MC12TuneV2_ProbNNpi", "MC12TuneV2_ProbNNK", "MC12TuneV2_ProbNNp", 
                    "MC12TuneV3_ProbNNpi", "MC12TuneV3_ProbNNK", "MC12TuneV3_ProbNNp", 
                    "MC12TuneV3_ProbNNe", "MC12TuneV3_ProbNNmu", 
                    "MC12TuneV3_ProbNNpiNotK", "MC12TuneV3_ProbNNpiNotKp", 
                    "MC12TuneV3_ProbNNKNotpi", "MC12TuneV3_ProbNNKNotpip", 
                    "MC12TuneV3_ProbNNpNotK", "MC12TuneV3_ProbNNpNotpiK", 
                   ], 
-    "cut" : "probe_trackcharge>0", 
     **common_params, 
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
 }
 
 sample = {**sample_run1, **sample_run2}
```

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py` & `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_PtEta.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,34 +21,32 @@
       to point to Online versions. 
     """
     if year in ["2017", "2018"] : 
         return { "Brunel_MC15TuneV1_ProbNN" + var : "MC15TuneV1_ProbNN" + var for var in probnn_responses }
     else : return {}
 
 common_params = {
-    "calib_cache_branches" : ["pt", "eta", "ntr", "sw"],          # Names of variable branches in ROOT tree of the cache file 
-    "data_ranges" : [ (2.4, 4.4), (1.9, 5.0), (0.7, 3.1) ],       # Ranges of each variable after transformation
-    "labels" : [r"PID", r"$p_T$", r"$\eta$", r"$N_{\rm tr}$"],    # Labels for plots
-    "names" : ["pid", "pt", "eta", "ntr"],                        # Short names of each variable for plot file names
+    "calib_cache_branches" : ["pt", "eta", "sw"],       # Names of variable branches in ROOT tree of the cache file 
+    "data_ranges" : [ (2.4, 4.4), (1.9, 5.0) ],         # Ranges of each variable after transformation
+    "labels" : [r"PID", r"$p_T$", r"$\eta$" ],          # Labels for plots
+    "names" : ["pid", "pt", "eta"],                     # Short names of each variable for plot file names
     "max_weights" : None, 
-    "smear" : [ None, None, (-0.5, 0.5) ], 
+    "smear" : [ None, None ], 
     "transform" : [                                               # Transformation functions for each variable
       "np.log10(x)",   # pT transformation
       "x",             # eta
-      "np.log10(x)",   # number of tracks
     ], 
-    "normalise_bins" : [100, 100, 100],                           # Number of bins for normalisation of each variable
-    "normalise_methods" : ["scale", "scale", "flatten"],          # Normalisation method for each variable ("scale", "normalise", "flatten")
-    "normalise_ranges" : 2*[ (0., 1.) ] + [ (0., 1.) ],           # Ranges of each variable after normalisation
-    "template_bins" : [70, 70, 20],                               # Number of bins for each variable in the template 
+    "normalise_bins" : [100, 100 ],                     # Number of bins for normalisation of each variable
+    "normalise_methods" : ["scale", "scale" ],          # Normalisation method for each variable ("scale", "normalise", "flatten")
+    "normalise_ranges" : 2*[ (0., 1.) ],                # Ranges of each variable after normalisation
+    "template_bins" : [100, 100],                       # Number of bins for each variable in the template 
     "template_sigma" : {
-      "default" : [2., 4., 4.],                              # Smearing parameter for the template for each variable. 
-      "syst1"   : [3., 6., 6.],                              # Smearing parameter for the template for each variable. 
-    }, 
-    "cut" : "probe_PIDK<2.", 
+      "default" : [1.5, 3.],                            # Smearing parameter for the template for each variable. 
+      "syst1"   : [2.,  4.5],                           # Smearing parameter for the template for each variable. 
+    }
 }
 
 sample_run2 = {
   f"{pol}_{year}" : { 
     "sample" : ds_run2[f"{pol}_{year}"], 
     "branches" : [ 
       "probe_Brunel_PT",
```

### Comparing `pidgen2-0.3.7/src/pidgen2/samples/pi_Dstar2Dpi_PtEta.py` & `pidgen2-0.3.8/src/pidgen2/samples/p_Lb2Lcmu.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,86 +5,130 @@
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 
-from ..datasets import converted_run1_pidcalib_datasets_dstar_pi as ds_run1
 from ..datasets import legacy_run2_pidcalib_datasets as ds_run2
+from ..datasets import converted_run1_pidcalib_datasets_lblcmu_p as ds_run1
+from ..mc_datasets import lb2jpsipk_run2sim09_datsets as mc_run2sim09
+from ..mc_datasets import lcmu_run1sim09_datasets as mc_run1sim09
+
 from itertools import product
 
 probnn_responses = ["pi", "K", "p", "e", "mu", "piNotK", "piNotKp", "KNotpi", "KNotpip", "pNotK", "pNotpiK"]
 
 def brunel_aliases(year) : 
     """
       Define aliases for Brunel variables in 2017, 2018 samples
       to point to Online versions. 
     """
     if year in ["2017", "2018"] : 
         return { "Brunel_MC15TuneV1_ProbNN" + var : "MC15TuneV1_ProbNN" + var for var in probnn_responses }
     else : return {}
 
+probnn_responses_mc = ["pi", "K", "p"]
+brunel_aliases_mc = { "Brunel_MC15TuneV1_ProbNN" + var : "MC15TuneV1_ProbNN" + var for var in probnn_responses_mc }
+
 common_params = {
-    "calib_cache_branches" : ["pt", "eta", "sw"],       # Names of variable branches in ROOT tree of the cache file 
-    "data_ranges" : [ (2.4, 4.4), (1.9, 5.0) ],         # Ranges of each variable after transformation
-    "labels" : [r"PID", r"$p_T$", r"$\eta$" ],          # Labels for plots
-    "names" : ["pid", "pt", "eta"],                     # Short names of each variable for plot file names
-    "max_weights" : None, 
-    "smear" : [ None, None ], 
-    "transform" : [                                               # Transformation functions for each variable
+    "smear" : [ None, None, (-0.5, 0.5) ], 
+    "transform" : [ 
       "np.log10(x)",   # pT transformation
       "x",             # eta
+      "np.log10(x)",   # number of tracks
     ], 
-    "normalise_bins" : [100, 100 ],                     # Number of bins for normalisation of each variable
-    "normalise_methods" : ["scale", "scale" ],          # Normalisation method for each variable ("scale", "normalise", "flatten")
-    "normalise_ranges" : 2*[ (0., 1.) ],                # Ranges of each variable after normalisation
-    "template_bins" : [100, 100],                       # Number of bins for each variable in the template 
+    "calib_cache_branches" : ["pt", "eta", "ntr", "sw"], 
+    "data_ranges" : [ (2.4, 4.4), (1.9, 5.0), (0.7, 3.1) ], 
+    "labels" : [r"PID", r"$p_T$", r"$\eta$", r"$N_{\rm tr}$"],    # Labels for plots
+    "names" : ["pid", "pt", "eta", "ntr"],                        # Short names of each variable for plot file names
+    "max_weights" : None, 
+    "normalise_bins" : [100, 100, 100], 
+    "normalise_methods" : ["scale", "scale", "flatten"], 
+    "normalise_ranges" : 3*[ (0., 1.) ], 
+    "template_bins" : [70, 70, 20], 
     "template_sigma" : {
-      "default" : [1.5, 3.],                            # Smearing parameter for the template for each variable. 
-      "syst1"   : [2.,  4.5],                           # Smearing parameter for the template for each variable. 
+      "default" : [2., 4., 4.], 
+      "syst1"   : [3., 6., 6.], 
     }
 }
 
 sample_run2 = {
   f"{pol}_{year}" : { 
     "sample" : ds_run2[f"{pol}_{year}"], 
     "branches" : [ 
       "probe_Brunel_PT", 
       "probe_Brunel_ETA", 
       "nTracks_Brunel", 
       "probe_sWeight" 
     ], 
-    "trees" : ['DSt_PiPTuple/DecayTree', 'DSt_PiMTuple/DecayTree'], 
+    "trees" : ["LbLcMu_PTuple/DecayTree", "LbLcMu_PbarTuple/DecayTree"], 
     "variables" : ["CombDLLK", "CombDLLmu", "CombDLLe", "CombDLLp"] + 
                   [ f"{b}MC15TuneV1_ProbNN{i}" for b, i in product(["", "Brunel_"], probnn_responses) ], 
     "aliases" : brunel_aliases(year), 
-    **common_params, 
+    **common_params
   } 
-  for pol in ["MagUp", "MagDown"] for year in ["2015", "2016", "2017", "2018"]
+  for pol in ["MagUp", "MagDown"] for year in ["2016", "2017", "2018"]
 }
 
 sample_run1 = {
   f"{pol}_{year}" : { 
     "sample" : ds_run1[f"{pol}_{year}"], 
     "branches" : [ 
       "probe_PT", 
       "probe_ETA", 
       "nTracks", 
       "probe_sWeight" 
     ], 
-    "trees" : ['DecayTree'], 
+    "trees" : ["DecayTree"], 
     "variables" : [
                    "CombDLLK", "CombDLLmu", "CombDLLe", "CombDLLp", 
                    "MC12TuneV2_ProbNNpi", "MC12TuneV2_ProbNNK", "MC12TuneV2_ProbNNp", 
                    "MC12TuneV3_ProbNNpi", "MC12TuneV3_ProbNNK", "MC12TuneV3_ProbNNp", 
                    "MC12TuneV3_ProbNNe", "MC12TuneV3_ProbNNmu", 
                    "MC12TuneV3_ProbNNpiNotK", "MC12TuneV3_ProbNNpiNotKp", 
                    "MC12TuneV3_ProbNNKNotpi", "MC12TuneV3_ProbNNKNotpip", 
                    "MC12TuneV3_ProbNNpNotK", "MC12TuneV3_ProbNNpNotpiK", 
                   ], 
+    **common_params
+  } 
+  for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
+}
+
+mc_sample_run1 = {
+  f"Sim09_{pol}_{year}" : {
+    "sample" : mc_run1sim09[f"{pol}_{year}"],
+    "prefix" : "p", 
+    "branches" : [
+      "p_PT", 
+      "p_ETA", 
+      "nTracks", 
+    ], 
+    "trees" : ["lc/nt"], 
+    "variables" : [ f"MC12TuneV2_ProbNN{i}" for i in probnn_responses_mc ] + 
+                  [ f"MC12TuneV3_ProbNN{i}" for i in probnn_responses_mc ] + 
+                  ["CombDLLp", "CombDLLK"], 
     **common_params, 
   } 
   for pol in ["MagUp", "MagDown"] for year in ["2011", "2012"]
 }
 
+mc_sample_run2 = {
+  f"Sim09_{pol}_{year}" : {
+    "sample" : mc_run2sim09[f"{pol}_{year}"], 
+    "prefix" : "p", 
+    "branches" : [
+      "p_PT", 
+      "p_ETA", 
+      "nTracks",
+    ], 
+    "trees" : ["lc/nt"], 
+    "variables" : [ f"{b}MC15TuneV1_ProbNN{i}" for b, i in product(["", "Brunel_"], probnn_responses_mc) ] + 
+                  ["CombDLLp", "CombDLLK"], 
+    "aliases" : brunel_aliases_mc, 
+    **common_params, 
+  }
+  for pol in ["MagUp", "MagDown"] for year in ["2016", "2017", "2018"]
+}
+
 sample = {**sample_run1, **sample_run2}
+mc_sample = {**mc_sample_run1, **mc_sample_run2}
```

### Comparing `pidgen2-0.3.7/src/pidgen2/systematics.py` & `pidgen2-0.3.8/src/pidgen2/systematics.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/tuples.py` & `pidgen2-0.3.8/src/pidgen2/tuples.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,35 +99,36 @@
        input: ROOT output file and tree name
        tree : name of the output tree
        step_size: number of events per iteration
        library: name of library that uproot uses to iterate through the input file and the array,
                 supported options are "np", "pd" and "ak"
        verbose: verbosity of prints
   """
-  if (verbose):
+  if verbose >= 1 :
     print("arguments of write_array function:\n", locals())
 
   # When rootfile is only updated, a temporary version of the tree is created
   if input == rootfile+":"+tree:
     rootfile_tmp = rootfile.replace(".root", "_tmp.root")
-    if (verbose) :
+    if verbose >= 1 :
       print(f"Rename output file from previous step: '{rootfile}'->'{rootfile_tmp}'")
     os.rename(rootfile, rootfile_tmp)
   else:
     rootfile_tmp = input
 
   chunk_index = 0
   chunk = 0
   num_entries = len(array)
   chunks = (num_entries-1)//step_size+1
 
   with uproot.recreate(rootfile, compression=uproot.ZLIB(4)) as file :
     for input_chunks in uproot.iterate(rootfile_tmp, step_size=step_size, library=library):
 
-      print(f"Writing chunk {chunk+1}/{chunks}, index={chunk_index}/{num_entries}")
+      if verbose >= 0 :
+        print(f"Writing chunk {chunk+1}/{chunks}, index={chunk_index}/{num_entries}")
 
       if library == "ak":
         # input chunks is a highlevel awkward array
         # Create output_dict/convert input chunks to be a dict with branches as keys and awkward arrays as values
         import awkward as ak
         output_dict = { b : ak.from_numpy(array[chunk_index:chunk_index+step_size,i]) for i,b in enumerate(branches)}
         input_chunks = {f : input_chunks[f] for f in input_chunks.fields}
@@ -163,10 +164,10 @@
 
       chunk_index = chunk_index + step_size
       chunk = chunk + 1
 
   # Delete temporary version of tree
   # Delete old version of tree, asuming there is only one old version
   if input == rootfile+":"+tree:
-    if (verbose) :
+    if verbose >= 1 :
       print("Delete output file from previous step")
     os.remove(rootfile_tmp)
```

### Comparing `pidgen2-0.3.7/src/pidgen2/validate.py` & `pidgen2-0.3.8/src/pidgen2/validate.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNK.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpi.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpip.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpip.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNe.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNe.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNmu.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNp.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotK.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotpiK.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotpiK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpi.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotK.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotKp.py` & `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotKp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/CombDLLK.py` & `pidgen2-0.3.8/src/pidgen2/variables/CombDLLK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/CombDLLe.py` & `pidgen2-0.3.8/src/pidgen2/variables/CombDLLe.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/CombDLLmu.py` & `pidgen2-0.3.8/src/pidgen2/variables/CombDLLmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/CombDLLp.py` & `pidgen2-0.3.8/src/pidgen2/variables/CombDLLp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/IsPhoton.py` & `pidgen2-0.3.8/src/pidgen2/variables/IsPhoton.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV2_ProbNNK.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV2_ProbNNmu.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV2_ProbNNp.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV2_ProbNNpi.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNK.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpi.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpip.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpip.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNe.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNe.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNmu.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNp.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpNotK.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpNotpiK.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpNotpiK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpi.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNK.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNe.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNe.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNmu.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNp.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpNotpiK.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpNotpiK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpi.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotK.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotKp.py` & `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotKp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/PhotonCL.py` & `pidgen2-0.3.8/src/pidgen2/variables/PhotonCL.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/Test_ProbNNp.py` & `pidgen2-0.3.8/src/pidgen2/variables/Test_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2/variables/__init__.py` & `pidgen2-0.3.8/src/pidgen2/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.7/src/pidgen2.egg-info/PKG-INFO` & `pidgen2-0.3.8/src/pidgen2.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: pidgen2
-Version: 0.3.7
+Version: 0.3.8
 Summary: Tools for particle identification (PID) correction for LHCb detector
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidgen2
 Author: Anton Poluektov
 Author-email: anton.poluektov@cern.ch
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidgen2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: jax
+Requires-Dist: uproot<5,>=4.2
+Requires-Dist: xrootd>=5.2
 
 # PIDGen2 
 
 ## Introduction
 
 PIDGen is a tool to resample PID variables in the full MC bases on distributions from calibration samples. PIDGen2 is a successor of the old PIDGen package. PIDGen2 is available via `lb-conda` and is supposed to replace the old PIDGen, both for Run 3 data, and for Run 1/Run 2. 
 An analogous solution updating PIDCorr is under development (see [here](https://groups.cern.ch/group/lhcb-phys-pid-calibration/Lists/Archive/Flat.aspx?RootFolder=%2Fgroup%2Flhcb%2Dphys%2Dpid%2Dcalibration%2FLists%2FArchive%2Fresampling%20in%20PIDCalib2&FolderCTID=0x01200200428956A5A0587D4CA9DBE3C7098FA903)).
```

### Comparing `pidgen2-0.3.7/src/pidgen2.egg-info/SOURCES.txt` & `pidgen2-0.3.8/src/pidgen2.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/pidgen2/list_mc_samples.py
 src/pidgen2/list_mc_variables.py
 src/pidgen2/list_samples.py
 src/pidgen2/list_variables.py
 src/pidgen2/mc_datasets.py
 src/pidgen2/plotting.py
 src/pidgen2/resample.py
+src/pidgen2/resampler.py
 src/pidgen2/resampling.py
 src/pidgen2/resampling_new.py
 src/pidgen2/systematics.py
 src/pidgen2/tuples.py
 src/pidgen2/validate.py
 src/pidgen2.egg-info/PKG-INFO
 src/pidgen2.egg-info/SOURCES.txt
@@ -35,14 +36,15 @@
 src/pidgen2/examples/example_correct_photon.py
 src/pidgen2/examples/example_resample.py
 src/pidgen2/samples/K_Dstar2Dpi.py
 src/pidgen2/samples/K_Dstar2Dpi_M.py
 src/pidgen2/samples/K_Dstar2Dpi_P.py
 src/pidgen2/samples/K_Dstar2Dpi_PIDKgt4.py
 src/pidgen2/samples/K_Dstar2Dpi_PtEta.py
+src/pidgen2/samples/K_Dstar2Dpi_scale.py
 src/pidgen2/samples/__init__.py
 src/pidgen2/samples/e_B2JpsieeK.py
 src/pidgen2/samples/e_B2JpsieeK_Brem.py
 src/pidgen2/samples/e_B2JpsieeK_NoBrem.py
 src/pidgen2/samples/gamma_B2KstarGamma.py
 src/pidgen2/samples/gamma_B2KstarGammaType0.py
 src/pidgen2/samples/gamma_B2KstarGammaType1.py
@@ -58,14 +60,15 @@
 src/pidgen2/samples/p_Lb2Lcpi.py
 src/pidgen2/samples/p_Test.py
 src/pidgen2/samples/pi_Dstar2Dpi.py
 src/pidgen2/samples/pi_Dstar2Dpi_M.py
 src/pidgen2/samples/pi_Dstar2Dpi_P.py
 src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py
 src/pidgen2/samples/pi_Dstar2Dpi_PtEta.py
+src/pidgen2/samples/pi_Dstar2Dpi_scale.py
 src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNK.py
 src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpi.py
 src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpip.py
 src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNe.py
 src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNmu.py
 src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNp.py
 src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotK.py
@@ -81,22 +84,24 @@
 src/pidgen2/variables/MC12TuneV2_ProbNNK.py
 src/pidgen2/variables/MC12TuneV2_ProbNNmu.py
 src/pidgen2/variables/MC12TuneV2_ProbNNp.py
 src/pidgen2/variables/MC12TuneV2_ProbNNpi.py
 src/pidgen2/variables/MC12TuneV3_ProbNNK.py
 src/pidgen2/variables/MC12TuneV3_ProbNNKNotpi.py
 src/pidgen2/variables/MC12TuneV3_ProbNNKNotpip.py
+src/pidgen2/variables/MC12TuneV3_ProbNNK_scale.py
 src/pidgen2/variables/MC12TuneV3_ProbNNe.py
 src/pidgen2/variables/MC12TuneV3_ProbNNmu.py
 src/pidgen2/variables/MC12TuneV3_ProbNNp.py
 src/pidgen2/variables/MC12TuneV3_ProbNNpNotK.py
 src/pidgen2/variables/MC12TuneV3_ProbNNpNotpiK.py
 src/pidgen2/variables/MC12TuneV3_ProbNNpi.py
 src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py
 src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py
+src/pidgen2/variables/MC12TuneV3_ProbNNpi_scale.py
 src/pidgen2/variables/MC15TuneV1_ProbNNK.py
 src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py
 src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py
 src/pidgen2/variables/MC15TuneV1_ProbNNe.py
 src/pidgen2/variables/MC15TuneV1_ProbNNmu.py
 src/pidgen2/variables/MC15TuneV1_ProbNNp.py
 src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py
```

### Comparing `pidgen2-0.3.7/src/pidgen2.egg-info/entry_points.txt` & `pidgen2-0.3.8/src/pidgen2.egg-info/entry_points.txt`

 * *Files identical despite different names*

