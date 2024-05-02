# Comparing `tmp/CageCavityCalc-1.0.4.tar.gz` & `tmp/CageCavityCalc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CageCavityCalc-1.0.4.tar", last modified: Mon Apr 15 18:26:50 2024, max compression
+gzip compressed data, was "CageCavityCalc-1.0.5.tar", last modified: Thu May  2 18:20:09 2024, max compression
```

## Comparing `CageCavityCalc-1.0.4.tar` & `CageCavityCalc-1.0.5.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.539184 CageCavityCalc-1.0.4/
--rw-r--r--   0 chem1540 (20152) fd        (6900)        7 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/.gitignore
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.507183 CageCavityCalc-1.0.4/.idea/
--rw-r--r--   0 chem1540 (20152) fd        (6900)       39 2022-09-12 17:18:36.000000 CageCavityCalc-1.0.4/.idea/.gitignore
--rw-r--r--   0 chem1540 (20152) fd        (6900)      552 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/CageCavityCalc.iml
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.508183 CageCavityCalc-1.0.4/.idea/inspectionProfiles/
--rw-r--r--   0 chem1540 (20152) fd        (6900)      174 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 chem1540 (20152) fd        (6900)      194 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/misc.xml
--rw-r--r--   0 chem1540 (20152) fd        (6900)      280 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/modules.xml
--rw-r--r--   0 chem1540 (20152) fd        (6900)      180 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.4/.idea/vcs.xml
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.509183 CageCavityCalc-1.0.4/CageCavityCalc/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    29950 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/CageCavityCalc.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)       90 2023-09-06 16:21:44.000000 CageCavityCalc-1.0.4/CageCavityCalc/__init__.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     4446 2024-04-12 14:48:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/__main__.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1862 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.4/CageCavityCalc/calculations.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    18977 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/data.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     3248 2024-04-12 14:52:13.000000 CageCavityCalc-1.0.4/CageCavityCalc/electrostatics.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.506183 CageCavityCalc-1.0.4/CageCavityCalc/examples/
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.510183 CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/
--rwxr-xr-x   0 chem1540 (20152) fd        (6900)    36659 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage.gro
--rw-r--r--   0 chem1540 (20152) fd        (6900)   190548 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      245 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/example_10.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.510183 CageCavityCalc-1.0.4/CageCavityCalc/examples/11_errors/
--rw-r--r--   0 chem1540 (20152) fd        (6900)      332 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/11_errors/example_11.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.513183 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/
--rw-r--r--   0 chem1540 (20152) fd        (6900)   342847 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_1.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)    80747 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_2.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)    81842 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_3.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)   118370 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_4.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)    93217 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_5.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)    87207 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_6.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)    11688 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test.mol2
--rw-r--r--   0 chem1540 (20152) fd        (6900)     8219 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    73728 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test.spartan
--rw-r--r--   0 chem1540 (20152) fd        (6900)   188164 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_box_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    30968 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      250 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)   626971 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity.pse
--rw-r--r--   0 chem1540 (20152) fd        (6900)      137 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity_vol_calc.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)   255592 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_extra_data.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)      973 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_hydrophobicity_cavity_dummy_atoms.txt
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.523183 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    11744 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/1148701.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    85162 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/1148701_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)       97 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/1148701_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    20960 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/210396.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    28203 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/210396_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/210396_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    25196 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/218828.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    49454 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/218828_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/218828_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)   100017 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   178145 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      127 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)   162704 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   340174 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      127 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    17348 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/646911.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    24016 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/646911_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/646911_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    21656 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/664973.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    40369 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/664973_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/664973_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    26387 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/759106.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    45188 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/759106_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/759106_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    22922 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/794242.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    40290 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/794242_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/794242_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)     7146 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_ACIE_2016-CCDC_1492902.xyz
--rw-r--r--   0 chem1540 (20152) fd        (6900)    10812 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    53167 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      143 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    33191 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1.mol2
--rw-r--r--   0 chem1540 (20152) fd        (6900)    50718 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      129 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    18764 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    39579 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      134 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    78911 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    30924 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    48269 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      142 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    15997 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_24_OrgLett_2010_12_1740_cage_ol.xyz
--rw-r--r--   0 chem1540 (20152) fd        (6900)    13100 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    18012 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    58196 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   138645 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      119 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    29116 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    49770 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      121 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    18844 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    25991 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      117 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    57771 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage.mol2
--rw-r--r--   0 chem1540 (20152) fd        (6900)   144017 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      123 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    35519 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    22910 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene_removed_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      141 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene_removed_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    57359 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    30189 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.xyz
--rw-r--r--   0 chem1540 (20152) fd        (6900)    88796 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      119 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)     6662 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    57354 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      128 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)     8078 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   110284 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      123 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    62792 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_002.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   140936 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_002_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      106 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_002_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    62792 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_003.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   141884 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_003_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      106 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_003_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)    64640 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_004.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    87532 2023-07-25 17:12:38.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_004_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      264 2023-07-25 17:12:38.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_004_cavity.pml
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.523183 CageCavityCalc-1.0.4/CageCavityCalc/examples/14_esp/
--rw-r--r--   0 chem1540 (20152) fd        (6900)      400 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/14_esp/example_14.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     9129 2022-12-08 14:47:43.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/14_esp/ncage.xyz
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.523183 CageCavityCalc-1.0.4/CageCavityCalc/examples/15_from_table/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    40230 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/15_from_table/example_15.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.525184 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    63832 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120.mol2
--rw-r--r--   0 chem1540 (20152) fd        (6900)    49764 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   342187 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pse
--rw-r--r--   0 chem1540 (20152) fd        (6900)      146 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity_vol_calc.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-01 19:14:55.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)       92 2023-02-01 19:14:55.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_cavity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)      246 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/example_1.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)   151889 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/file.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    83899 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/file.xyz
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.528184 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    18404 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   210710 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pse
--rw-r--r--   0 chem1540 (20152) fd        (6900)    63831 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.mol2
--rw-r--r--   0 chem1540 (20152) fd        (6900)    44996 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   106484 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_box_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   118804 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   524484 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pse
--rw-r--r--   0 chem1540 (20152) fd        (6900)      145 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity_vol_calc.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)      186 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/example_2.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)   231083 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/file.pdb
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.528184 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/test/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    44996 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/test/cage_ACIE_2006_45_901.pdb
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.528184 CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    16216 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/cage_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      300 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/example_3.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    16216 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/file.pdb
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.529184 CageCavityCalc-1.0.4/CageCavityCalc/examples/4_mdanalysis/
--rwxr-xr-x   0 chem1540 (20152) fd        (6900)    36659 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/4_mdanalysis/cage.gro
--rw-r--r--   0 chem1540 (20152) fd        (6900)      243 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/4_mdanalysis/example_4.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.529184 CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/
--rwxr-xr-x   0 chem1540 (20152) fd        (6900)    25859 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/cage.gro
--rw-r--r--   0 chem1540 (20152) fd        (6900)    30224 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/cage_cavity.gro
--rw-r--r--   0 chem1540 (20152) fd        (6900)      152 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/example_5.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.530184 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1068 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/.short.xtc_offsets.npz
--rw-r--r--   0 chem1540 (20152) fd        (6900)      265 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/example_6.py
--rwxr-xr-x   0 chem1540 (20152) fd        (6900)    21919 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/short.gro
--rwxr-xr-x   0 chem1540 (20152) fd        (6900)    11948 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/short.xtc
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.530184 CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    57903 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/cage.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   496989 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/cage_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)       62 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/run.sh
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.532184 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    16384 2023-07-25 17:12:29.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/.cage_cavity_hydrophobicity.pdb.swp
--rw-r--r--   0 chem1540 (20152) fd        (6900)    63832 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_1_JACS_2006_128_14120.mol2
--rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_aromatic_contact.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:22.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_esp.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_hydrophobicity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      263 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_hydrophobicity.pml
--rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_solvent_accessibility.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      472 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/example_8.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.533184 CageCavityCalc-1.0.4/CageCavityCalc/examples/9_large/
--rw-r--r--   0 chem1540 (20152) fd        (6900)   157210 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/9_large/cage.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)      519 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/9_large/example_9.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.534184 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    17795 2022-09-14 13:56:58.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    34049 2022-09-14 14:09:50.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    17795 2022-09-14 13:56:58.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/646911_exported_spartan_replace_spaces_before_after_Pd.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    28352 2022-09-14 15:28:29.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/Cage6_opt.xyz
--rw-r--r--   0 chem1540 (20152) fd        (6900)    57354 2022-09-14 15:29:14.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/Cage6_opt_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)    37525 2022-09-14 15:30:50.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/Cage6_opt_cavity_cluster.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   161261 2022-09-12 17:13:04.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/cage_pdb.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)   201845 2022-09-12 17:22:41.000000 CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/cage_pdb_cavity.pdb
--rw-r--r--   0 chem1540 (20152) fd        (6900)     3843 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/grid_classes.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     2773 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.4/CageCavityCalc/hydrophobicity.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    10095 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.4/CageCavityCalc/input_output.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)      843 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/log.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.537184 CageCavityCalc-1.0.4/CageCavityCalc/pic/
--rw-r--r--   0 chem1540 (20152) fd        (6900)   453532 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/cage.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)   425171 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/cavity.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)   531480 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/hydrophobicity.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)   619706 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/principle
--rw-r--r--   0 chem1540 (20152) fd        (6900)  1051047 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/principle.png
--rw-r--r--   0 chem1540 (20152) fd        (6900)   619827 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/CageCavityCalc/pic/principle.svg
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.538184 CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/
--rw-r--r--   0 chem1540 (20152) fd        (6900)    10170 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/__init__.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)    12998 2023-07-25 17:12:38.000000 CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/cavecav_widget.ui
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1065 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/simple.py
--rw-r--r--   0 chem1540 (20152) fd        (6900)     3962 2023-09-06 13:17:45.000000 CageCavityCalc-1.0.4/CageCavityCalc/window_size.py
-drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-04-15 18:26:50.509183 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/
--rw-r--r--   0 chem1540 (20152) fd        (6900)      171 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/PKG-INFO
--rw-r--r--   0 chem1540 (20152) fd        (6900)    11321 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/SOURCES.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)        1 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/dependency_links.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)       64 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/entry_points.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)       31 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/requires.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)       15 2024-04-15 18:26:50.000000 CageCavityCalc-1.0.4/CageCavityCalc.egg-info/top_level.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1078 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/LICENSE
--rw-r--r--   0 chem1540 (20152) fd        (6900)      171 2024-04-15 18:26:50.538184 CageCavityCalc-1.0.4/PKG-INFO
--rw-r--r--   0 chem1540 (20152) fd        (6900)     1697 2024-04-15 18:25:39.000000 CageCavityCalc-1.0.4/README.md
--rw-r--r--   0 chem1540 (20152) fd        (6900)      296 2024-04-15 18:26:23.000000 CageCavityCalc-1.0.4/pyproject.toml
--rw-r--r--   0 chem1540 (20152) fd        (6900)      261 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.4/readme_testing.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)        0 2023-09-06 12:38:38.000000 CageCavityCalc-1.0.4/requirements.txt
--rw-r--r--   0 chem1540 (20152) fd        (6900)       38 2024-04-15 18:26:50.539184 CageCavityCalc-1.0.4/setup.cfg
--rw-r--r--   0 chem1540 (20152) fd        (6900)      359 2023-09-06 18:50:04.000000 CageCavityCalc-1.0.4/setup.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.299240 CageCavityCalc-1.0.5/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)        7 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/.gitignore
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.265239 CageCavityCalc-1.0.5/.idea/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       39 2022-09-12 17:18:36.000000 CageCavityCalc-1.0.5/.idea/.gitignore
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      552 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.5/.idea/CageCavityCalc.iml
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.266239 CageCavityCalc-1.0.5/.idea/inspectionProfiles/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      174 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      194 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.5/.idea/misc.xml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      280 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.5/.idea/modules.xml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      180 2022-09-12 17:18:35.000000 CageCavityCalc-1.0.5/.idea/vcs.xml
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.267239 CageCavityCalc-1.0.5/CageCavityCalc/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    29949 2024-05-02 18:10:20.000000 CageCavityCalc-1.0.5/CageCavityCalc/CageCavityCalc.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       90 2023-09-06 16:21:44.000000 CageCavityCalc-1.0.5/CageCavityCalc/__init__.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     5294 2024-05-02 18:10:20.000000 CageCavityCalc-1.0.5/CageCavityCalc/__main__.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     1862 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.5/CageCavityCalc/calculations.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18977 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/data.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     3248 2024-04-12 14:52:13.000000 CageCavityCalc-1.0.5/CageCavityCalc/electrostatics.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.264239 CageCavityCalc-1.0.5/CageCavityCalc/examples/
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.268239 CageCavityCalc-1.0.5/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    36659 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage.gro
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   190548 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      245 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/example_10.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.268239 CageCavityCalc-1.0.5/CageCavityCalc/examples/11_errors/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      332 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/11_errors/example_11.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.271239 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   342847 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_1.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    80747 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_2.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    81842 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_3.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   118370 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_4.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    93217 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_5.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    87207 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_6.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    11688 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     8219 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    73728 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test.spartan
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   188164 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_box_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    30968 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      250 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   626971 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_cavity.pse
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      137 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_cavity_vol_calc.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   255592 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_extra_data.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      973 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_hydrophobicity_cavity_dummy_atoms.txt
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.282240 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    11744 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/1148701.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    85162 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/1148701_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       97 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/1148701_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    20960 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/210396.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    28203 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/210396_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/210396_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    25196 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/218828.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    49454 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/218828_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/218828_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   100017 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   178145 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      127 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   162704 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   340174 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      127 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    17348 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/646911.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    24016 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/646911_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/646911_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    21656 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/664973.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    40369 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/664973_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/664973_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    26387 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/759106.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    45188 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/759106_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/759106_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    22922 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/794242.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    40290 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/794242_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       96 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/794242_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     7146 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_ACIE_2016-CCDC_1492902.xyz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    10812 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    53167 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      143 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    33191 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    50718 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      129 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18764 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    39579 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      134 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    78911 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    30924 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    48269 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      142 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    15997 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_24_OrgLett_2010_12_1740_cage_ol.xyz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    13100 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18012 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    58196 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   138645 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      119 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    29116 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    49770 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      121 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18844 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    25991 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      117 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57771 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   144017 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      123 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    35519 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    22910 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene_removed_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      141 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene_removed_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57359 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    30189 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.xyz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    88796 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      119 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     6662 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57354 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      128 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     8078 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   110284 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      123 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    62792 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_002.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   140936 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_002_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      106 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_002_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    62792 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_003.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   141884 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_003_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      106 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_003_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    64640 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_004.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    87532 2023-07-25 17:12:38.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_004_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      264 2023-07-25 17:12:38.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_004_cavity.pml
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.283239 CageCavityCalc-1.0.5/CageCavityCalc/examples/14_esp/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      400 2024-05-02 18:10:20.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/14_esp/example_14.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     9129 2022-12-08 14:47:43.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/14_esp/ncage.xyz
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.283239 CageCavityCalc-1.0.5/CageCavityCalc/examples/15_from_table/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    40230 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/15_from_table/example_15.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.285240 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    63832 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    49764 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   342187 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pse
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      146 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity_vol_calc.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-01 19:14:55.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       92 2023-02-01 19:14:55.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_cavity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      246 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/example_1.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   151889 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/file.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    83899 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/file.xyz
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.287240 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    18404 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   210710 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pse
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    63831 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    44996 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   106484 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_box_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   118804 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   524484 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pse
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      145 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity_vol_calc.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      186 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/example_2.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   231083 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/file.pdb
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.288240 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/test/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    44996 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/test/cage_ACIE_2006_45_901.pdb
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.288240 CageCavityCalc-1.0.5/CageCavityCalc/examples/3_cgbind/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    16216 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/3_cgbind/cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      300 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/3_cgbind/example_3.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    16216 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/3_cgbind/file.pdb
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.288240 CageCavityCalc-1.0.5/CageCavityCalc/examples/4_mdanalysis/
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    36659 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/4_mdanalysis/cage.gro
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      245 2024-05-02 18:10:20.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/4_mdanalysis/example_4.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.289240 CageCavityCalc-1.0.5/CageCavityCalc/examples/5_other_formats/
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    25859 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/5_other_formats/cage.gro
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    30224 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/5_other_formats/cage_cavity.gro
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      152 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/5_other_formats/example_5.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.289240 CageCavityCalc-1.0.5/CageCavityCalc/examples/6_trajectory/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     1068 2024-05-02 18:10:20.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/6_trajectory/.short.xtc_offsets.npz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      265 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/6_trajectory/example_6.py
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    21919 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/6_trajectory/short.gro
+-rwxr-xr-x   0 chem1540 (20152) fd        (6900)    11948 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/6_trajectory/short.xtc
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.290240 CageCavityCalc-1.0.5/CageCavityCalc/examples/7_bash/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57903 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/7_bash/cage.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   496989 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/7_bash/cage_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       62 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/7_bash/run.sh
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.293240 CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    16384 2023-07-25 17:12:29.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/.cage_cavity_hydrophobicity.pdb.swp
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    63832 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_1_JACS_2006_128_14120.mol2
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_aromatic_contact.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:22.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_esp.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_hydrophobicity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      263 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_hydrophobicity.pml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   179093 2023-02-02 20:06:21.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_solvent_accessibility.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      472 2024-05-02 18:10:20.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/example_8.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.293240 CageCavityCalc-1.0.5/CageCavityCalc/examples/9_large/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   157210 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/9_large/cage.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      519 2024-04-16 10:11:12.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/9_large/example_9.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.294240 CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    17795 2022-09-14 13:56:58.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    34049 2022-09-14 14:09:50.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    17795 2022-09-14 13:56:58.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/646911_exported_spartan_replace_spaces_before_after_Pd.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    28352 2022-09-14 15:28:29.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/Cage6_opt.xyz
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    57354 2022-09-14 15:29:14.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/Cage6_opt_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    37525 2022-09-14 15:30:50.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/Cage6_opt_cavity_cluster.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   161261 2022-09-12 17:13:04.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/cage_pdb.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   201845 2022-09-12 17:22:41.000000 CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/cage_pdb_cavity.pdb
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     3843 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/grid_classes.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     2773 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.5/CageCavityCalc/hydrophobicity.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    10095 2023-09-06 13:17:28.000000 CageCavityCalc-1.0.5/CageCavityCalc/input_output.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      843 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/log.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.298240 CageCavityCalc-1.0.5/CageCavityCalc/pic/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   453532 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/pic/cage.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   425171 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/pic/cavity.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   531480 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/pic/hydrophobicity.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   619706 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/pic/principle
+-rw-r--r--   0 chem1540 (20152) fd        (6900)  1051047 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/pic/principle.png
+-rw-r--r--   0 chem1540 (20152) fd        (6900)   619827 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/CageCavityCalc/pic/principle.svg
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.298240 CageCavityCalc-1.0.5/CageCavityCalc/pymol_plugin/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    10170 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/pymol_plugin/__init__.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    12998 2023-07-25 17:12:38.000000 CageCavityCalc-1.0.5/CageCavityCalc/pymol_plugin/cavecav_widget.ui
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     1065 2023-09-06 13:10:18.000000 CageCavityCalc-1.0.5/CageCavityCalc/pymol_plugin/simple.py
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     3962 2023-09-06 13:17:45.000000 CageCavityCalc-1.0.5/CageCavityCalc/window_size.py
+drwxr-xr-x   0 chem1540 (20152) fd        (6900)        0 2024-05-02 18:20:09.267239 CageCavityCalc-1.0.5/CageCavityCalc.egg-info/
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      171 2024-05-02 18:20:09.000000 CageCavityCalc-1.0.5/CageCavityCalc.egg-info/PKG-INFO
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    11321 2024-05-02 18:20:09.000000 CageCavityCalc-1.0.5/CageCavityCalc.egg-info/SOURCES.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)        1 2024-05-02 18:20:09.000000 CageCavityCalc-1.0.5/CageCavityCalc.egg-info/dependency_links.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       64 2024-05-02 18:20:09.000000 CageCavityCalc-1.0.5/CageCavityCalc.egg-info/entry_points.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       31 2024-05-02 18:20:09.000000 CageCavityCalc-1.0.5/CageCavityCalc.egg-info/requires.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       15 2024-05-02 18:20:09.000000 CageCavityCalc-1.0.5/CageCavityCalc.egg-info/top_level.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)     1078 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/LICENSE
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      171 2024-05-02 18:20:09.299240 CageCavityCalc-1.0.5/PKG-INFO
+-rw-r--r--   0 chem1540 (20152) fd        (6900)    14762 2024-05-02 18:10:20.000000 CageCavityCalc-1.0.5/README.md
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      296 2024-05-02 18:16:59.000000 CageCavityCalc-1.0.5/pyproject.toml
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      261 2022-09-09 18:38:07.000000 CageCavityCalc-1.0.5/readme_testing.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)        0 2023-09-06 12:38:38.000000 CageCavityCalc-1.0.5/requirements.txt
+-rw-r--r--   0 chem1540 (20152) fd        (6900)       38 2024-05-02 18:20:09.299240 CageCavityCalc-1.0.5/setup.cfg
+-rw-r--r--   0 chem1540 (20152) fd        (6900)      359 2023-09-06 18:50:04.000000 CageCavityCalc-1.0.5/setup.py
```

### Comparing `CageCavityCalc-1.0.4/.idea/CageCavityCalc.iml` & `CageCavityCalc-1.0.5/.idea/CageCavityCalc.iml`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/CageCavityCalc.py` & `CageCavityCalc-1.0.5/CageCavityCalc/CageCavityCalc.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def __init__(self):
         '''
         Initilalize the methodology, set up all the variables
         '''
 
         self.grid_spacing = 1 # spacing between grid points
 
-        self.distance_threshold_for_90_deg_angle = 7
+        self.distance_threshold_for_90_deg_angle = 5
         calculate_bfactor = True
         compute_aromatic_contacts = False
         compute_hydrophobicity = True
         self.dummy_atom_radii = 1 #radius of the dummy atom use for the cavity calculations
         self.clustering_to_remove_cavity_noise = "false" #"Size" select largest cluster, "Dist" select closte cluster to the center
         
         # With the modified code we can always use distanceFromCOMFactor = 1
@@ -509,15 +509,14 @@
         for dummy_atom in self.dummy_atoms_positions:
             #if (printLevel == 2): fileExtraData.write("-------------\n")
             dummy_hydrophobicity = []
             dummy_aromatic_contacts = []
             dummy_solvent_accessibility = []
 
             for atom_type in self.atom_type_list:
-
                 dist = self.KDTree_dict[atom_type].query(dummy_atom, k=self.n_atoms, p=2,
                                                     distance_upper_bound=self.distThreshold_atom_contacts)
                 '''
                 if (printLevel == 2):
                     fileExtraData.write(str(atom_type) + ": " + str(dist[0]) + "\n")
                     fileExtraData.write(str(atom_type) + " Index: " + str(
                         [x + 1 for x in dist[1]]) + "\n")  # Add 1 to key as atom number starts with 1 and list number with 0
```

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/__main__.py` & `CageCavityCalc-1.0.5/CageCavityCalc/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from CageCavityCalc import cavity
 import argparse
+import numpy as np
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("-f", default=None, help="input file (*pdb, *mol2, ...)")
     parser.add_argument("-o", default="cage_cavity.pdb", help="output file (*pdb, *mol2, ...)")
     parser.add_argument("-hydrophobicity", "-hydro", default=False, action='store_true',
                         help="Calculate hydrophobicity")
     parser.add_argument("-esp", default=False, action='store_true', help="Calculate ESP")
+    parser.add_argument("-metal", default="", help="Metal used in the ESP")
+    parser.add_argument("-metal_charge", default=0, help="Charge of the metal used in the ESP")
+    parser.add_argument("-charge_method", default="eem", help="Charge method used in the ESP: eem, mmff94, gasteiger, qeq, qtpie, eem2015ha, eem2015hm, eem2015hn, eem2015ba, eem2015bm, eem2015bn")
     parser.add_argument("-method", default="Ghose", help="Method to calculate the hydrophobicity: Ghose or Crippen")
     parser.add_argument("-pymol", default=False, action='store_true', help="create pymol script")
     parser.add_argument("-distfun", default="Fauchere",
                         help="Method to calculate the hydrophobicity: Audry, Fauchere, Fauchere2, OnlyValues")
     parser.add_argument("-gr", default=1.0, help="Grid spacing resolution (Angstroms)")
     parser.add_argument("-info", default=False, action='store_true', help="Print log INFO on the terminal")
     parser.add_argument("-cluster", default="false", help="Remove cavity noise by dbscan clustering (size or dist)")
-    parser.add_argument("-d90a", default=3.0,
+    parser.add_argument("-d90a", default=2.0,
                         help="Automatic distance threshold to calculate 90 deg angle as X times window radious")
     parser.add_argument("-d90m", default=None, help="Manual distance threshold to calculate 90 deg angle in Angstroms")
     return parser.parse_args()
 
 
 def main():
     args = get_args()
@@ -33,60 +37,71 @@
         args.o = args.f[:args.f.find('.')] + "_cavity.pdb"
     # Initialze the cavity
     cav = cavity()
     # Set the grid spacing resolution from the args input. Default = 1 Angstrom
     if args.gr:
         cav.grid_spacing = float(args.gr)
         cav.dummy_atom_radii = float(args.gr)
-    # Set the
+    # Set the cluster
     if args.cluster:
         cav.clustering_to_remove_cavity_noise = args.cluster
     # Read the input file
     cav.read_file(args.f)
-    # Set the distance_threshold_for_90_deg_angle as 3 times the window radius by default or read from input line
+    
     window_radius = cav.calculate_window()
 
     cav.distance_threshold_for_90_deg_angle = window_radius * float(args.d90a)
+    if cav.distance_threshold_for_90_deg_angle < 5:
+        cav.distance_threshold_for_90_deg_angle = 5
+
     if args.d90m:
         cav.distance_threshold_for_90_deg_angle = float(args.d90m)
 
-    if cav.distance_threshold_for_90_deg_angle < 5:
-        cav.distance_threshold_for_90_deg_angle = 5
-    logger.info(f"Distance threshold for 90 deg angle = {cav.distance_threshold_for_90_deg_angle:.2f}")
+    print(f"Distance threshold for 90 deg angle = {cav.distance_threshold_for_90_deg_angle:.2f}")
     volume = cav.calculate_volume()
+    
+    #save the PDB file with the computed cavity
+    cav.print_to_file(args.o)
+
+    if args.pymol == True:
+        cav.print_to_pymol(args.o[:args.o.find('.')] + "_cavity.pml")
+    
     print("Cage cavity volume = ", volume, " A3")
 
     if args.esp == True:
-        cav.calculate_esp()  # this is problematic if there is metal
-        cav.print_to_file(args.o, 'esp')
+        if (args.metal and args.metal_charge):
+            print(f"Metal = {args.metal}, Charge = {args.metal_charge}")
+            cav.calculate_esp(metal_name=args.metal, metal_charge=int(args.metal_charge))
+            if (args.charge_method):
+                cav.calculate_esp(metal_name=args.metal, metal_charge=int(args.metal_charge), method=args.charge_method)
+        else:
+            cav.calculate_esp()  # this is problematic if there is metal
+            if (args.charge_method):
+                cav.calculate_esp(method=args.charge_method)
+        cav.print_to_file(args.o[:args.o.find('.')] + "_esp.pdb", 'esp')
         if args.pymol == True:
-            pymol_filename = args.o[:args.o.find('.')] + ".pml"
+            pymol_filename = args.o[:args.o.find('.')] + "_esp.pml"
             cav.print_to_pymol(pymol_filename, 'esp')
-    elif args.hydrophobicity == True:
+    if args.hydrophobicity == True:
         cav.hydrophMethod = args.method
         cav.distance_function = args.distfun  # Audry, Fauchere, Fauchere2, OnlyValues
         cavity_hydrophobicity_values = cav.calculate_hydrophobicity()
         average_cavity_hydrophobicity = np.mean(cavity_hydrophobicity_values)
         print(f"Hydrophobicity method and distance function = {cav.hydrophMethod}, {cav.distance_function}")
         print(f"Average cavity hydrophobicity = {average_cavity_hydrophobicity:.5f} A^-3")
         print(f"Total cavity hydrophobicity = {average_cavity_hydrophobicity * volume:.5f}")
         mlp_pos = [i for i in cavity_hydrophobicity_values if i > 0]
         mlp_neg = [i for i in cavity_hydrophobicity_values if i < 0]
         hydrophobic_index = sum(mlp_pos) / (sum(mlp_pos) - sum(mlp_neg))
         print(f"Hydrophobic_index (HI) = {hydrophobic_index:.3f}")
 
-        cav.print_to_file(args.o, 'h')
+        cav.print_to_file(args.o[:args.o.find('.')] + "_hydrophob.pdb", 'h')
         if args.pymol == True:
-            pymol_filename = args.o[:args.o.find('.')] + ".pml"
+            pymol_filename = args.o[:args.o.find('.')] + "_hydrophob.pml"
             cav.print_to_pymol(pymol_filename, 'h')
-    else:
-        cav.print_to_file(args.o)
-        if args.pymol == True:
-            pymol_filename = args.o[:args.o.find('.')] + ".pml"
-            cav.print_to_pymol(pymol_filename)
 
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/calculations.py` & `CageCavityCalc-1.0.5/CageCavityCalc/calculations.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/data.py` & `CageCavityCalc-1.0.5/CageCavityCalc/data.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/electrostatics.py` & `CageCavityCalc-1.0.5/CageCavityCalc/electrostatics.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage.gro` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage.gro`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/10_mdanalysis_hydrophobicity/cage_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_1.png` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_1.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_2.png` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_2.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_3.png` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_3.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_4.png` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_4.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_5.png` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_5.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/fig_6.png` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/fig_6.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test.mol2` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test.mol2`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test.spartan` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test.spartan`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_box_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_box_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_cavity.pse` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_cavity.pse`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_extra_data.txt` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_extra_data.txt`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/12_test_cage/test_hydrophobicity_cavity_dummy_atoms.txt` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/12_test_cage/test_hydrophobicity_cavity_dummy_atoms.txt`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/1148701.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/1148701.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/1148701_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/1148701_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/210396.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/210396.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/210396_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/210396_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/218828.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/218828.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/218828_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/218828_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM527_ESM_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/41586_2016_BFnature20771_MOESM528_ESM_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/646911.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/646911.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/646911_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/646911_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/664973.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/664973.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/664973_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/664973_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/759106.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/759106.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/759106_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/759106_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/794242.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/794242.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/794242_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/794242_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_ACIE_2016-CCDC_1492902.xyz` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_ACIE_2016-CCDC_1492902.xyz`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/CageOTf_Pentacenedione_removed_ACIE_2016-CCDC_1492902_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1.mol2` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1.mol2`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_113_ChemEurJ_2014_20_16707_cage1_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_130_ChemCommun_1997_118_497_cage_cram_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_132_ChemEurJ_2019_25_3091_cage_x-ray_no_guest_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_24_OrgLett_2010_12_1740_cage_ol.xyz` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_24_OrgLett_2010_12_1740_cage_ol.xyz`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_31_JPhysChemC_2014_118_12734_CC3_869701_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_55_JACS_2020_142_18060_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_73_ChemEurJ_2020_26_1558_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_76_PNAS_2002_99_4962_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage.mol2` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage.mol2`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_87_ChemEurJ_202005046_cage_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene_removed_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_93_ChemSci2011_2_1719_cage1_coronene_removed_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.xyz` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021.xyz`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/Figure_96_AngewChemIntEd_2021_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-badjic_lzq-8-38_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/anie202211304-sup-0001-compound-8_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_002.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_002.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_002_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_002_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_003.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_003.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_003_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_003_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_004.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_004.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/13_cages_review/ja4043609_si_004_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/13_cages_review/ja4043609_si_004_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/14_esp/ncage.xyz` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/14_esp/ncage.xyz`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/15_from_table/example_15.py` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/15_from_table/example_15.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120.mol2` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120.mol2`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pse` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_1_JACS_2006_128_14120_cavity.pse`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/cage_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/cage_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/file.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/file.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/1_mol2/file.xyz` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/1_mol2/file.xyz`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pse` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.cavity.pse`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.mol2` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.mol2`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_box_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_box_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pse` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/cage_ACIE_2006_45_901_cavity.pse`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/file.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/file.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/2_pdb/test/cage_ACIE_2006_45_901.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/2_pdb/test/cage_ACIE_2006_45_901.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/cage_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/3_cgbind/cage_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/3_cgbind/file.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/3_cgbind/file.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/4_mdanalysis/cage.gro` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/4_mdanalysis/cage.gro`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/cage.gro` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/5_other_formats/cage.gro`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/5_other_formats/cage_cavity.gro` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/5_other_formats/cage_cavity.gro`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/.short.xtc_offsets.npz` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/6_trajectory/.short.xtc_offsets.npz`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/short.gro` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/6_trajectory/short.gro`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/6_trajectory/short.xtc` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/6_trajectory/short.xtc`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/cage.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/7_bash/cage.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/7_bash/cage_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/7_bash/cage_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/.cage_cavity_hydrophobicity.pdb.swp` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/.cage_cavity_hydrophobicity.pdb.swp`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_1_JACS_2006_128_14120.mol2` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_1_JACS_2006_128_14120.mol2`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_aromatic_contact.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_aromatic_contact.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_esp.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_esp.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_hydrophobicity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_hydrophobicity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_solvent_accessibility.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/8_hydrophobicity/cage_cavity_solvent_accessibility.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/9_large/cage.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/9_large/cage.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/9_large/example_9.py` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/9_large/example_9.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/646911_exported_spartan_gives_error_Pd_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/646911_exported_spartan_replace_spaces_before_after_Pd.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/646911_exported_spartan_replace_spaces_before_after_Pd.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/Cage6_opt.xyz` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/Cage6_opt.xyz`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/Cage6_opt_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/Cage6_opt_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/Cage6_opt_cavity_cluster.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/Cage6_opt_cavity_cluster.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/cage_pdb.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/cage_pdb.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/examples/more_tests/cage_pdb_cavity.pdb` & `CageCavityCalc-1.0.5/CageCavityCalc/examples/more_tests/cage_pdb_cavity.pdb`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/grid_classes.py` & `CageCavityCalc-1.0.5/CageCavityCalc/grid_classes.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/hydrophobicity.py` & `CageCavityCalc-1.0.5/CageCavityCalc/hydrophobicity.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/input_output.py` & `CageCavityCalc-1.0.5/CageCavityCalc/input_output.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/log.py` & `CageCavityCalc-1.0.5/CageCavityCalc/log.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/pic/cage.png` & `CageCavityCalc-1.0.5/CageCavityCalc/pic/cage.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/pic/cavity.png` & `CageCavityCalc-1.0.5/CageCavityCalc/pic/cavity.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/pic/hydrophobicity.png` & `CageCavityCalc-1.0.5/CageCavityCalc/pic/hydrophobicity.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/pic/principle` & `CageCavityCalc-1.0.5/CageCavityCalc/pic/principle`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/pic/principle.png` & `CageCavityCalc-1.0.5/CageCavityCalc/pic/principle.png`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/pic/principle.svg` & `CageCavityCalc-1.0.5/CageCavityCalc/pic/principle.svg`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/__init__.py` & `CageCavityCalc-1.0.5/CageCavityCalc/pymol_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/cavecav_widget.ui` & `CageCavityCalc-1.0.5/CageCavityCalc/pymol_plugin/cavecav_widget.ui`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/pymol_plugin/simple.py` & `CageCavityCalc-1.0.5/CageCavityCalc/pymol_plugin/simple.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc/window_size.py` & `CageCavityCalc-1.0.5/CageCavityCalc/window_size.py`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/CageCavityCalc.egg-info/SOURCES.txt` & `CageCavityCalc-1.0.5/CageCavityCalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CageCavityCalc-1.0.4/LICENSE` & `CageCavityCalc-1.0.5/LICENSE`

 * *Files identical despite different names*

