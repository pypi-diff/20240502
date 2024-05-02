# Comparing `tmp/femagtools-1.6.6.tar.gz` & `tmp/femagtools-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femagtools-1.6.6.tar", last modified: Tue Apr 30 15:54:56 2024, max compression
+gzip compressed data, was "femagtools-1.6.7.tar", last modified: Thu May  2 15:08:16 2024, max compression
```

## Comparing `femagtools-1.6.6.tar` & `femagtools-1.6.7.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.695255 femagtools-1.6.6/
--rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.6.6/LICENSE
--rw-r--r--   0 tar        (210) tar        (210)       39 2023-08-31 09:32:32.000000 femagtools-1.6.6/MANIFEST.in
--rw-r--r--   0 tar        (210) tar        (210)     5827 2024-04-30 15:54:56.695255 femagtools-1.6.6/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.6.6/README.md
--rw-r--r--   0 tar        (210) tar        (210)     1414 2024-04-30 15:50:23.000000 femagtools-1.6.6/pyproject.toml
--rw-r--r--   0 tar        (210) tar        (210)       38 2024-04-30 15:54:56.695255 femagtools-1.6.6/setup.cfg
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.649256 femagtools-1.6.6/src/
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.661256 femagtools-1.6.6/src/femagtools/
--rw-r--r--   0 tar        (210) tar        (210)     1615 2024-04-30 15:51:21.000000 femagtools-1.6.6/src/femagtools/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     1577 2024-01-31 08:22:56.000000 femagtools-1.6.6/src/femagtools/airgap.py
--rw-r--r--   0 tar        (210) tar        (210)    12069 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/amazon.py
--rw-r--r--   0 tar        (210) tar        (210)    13891 2023-12-15 11:25:08.000000 femagtools-1.6.6/src/femagtools/amela.py
--rw-r--r--   0 tar        (210) tar        (210)     7660 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    71680 2024-03-06 12:39:21.000000 femagtools-1.6.6/src/femagtools/bch.py
--rw-r--r--   0 tar        (210) tar        (210)     3142 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/bchxml.py
--rw-r--r--   0 tar        (210) tar        (210)    10766 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/condor.py
--rw-r--r--   0 tar        (210) tar        (210)     1076 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     3136 2023-10-30 08:37:24.000000 femagtools-1.6.6/src/femagtools/config.py
--rw-r--r--   0 tar        (210) tar        (210)    26478 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/convert.py
--rw-r--r--   0 tar        (210) tar        (210)     6901 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/dakota.py
--rwxr-xr-x   0 tar        (210) tar        (210)     4068 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/dakota_femag.py
--rw-r--r--   0 tar        (210) tar        (210)     5573 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/dakotaout.py
--rw-r--r--   0 tar        (210) tar        (210)     7460 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/docker.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.666256 femagtools-1.6.6/src/femagtools/dxfsl/
--rw-r--r--   0 tar        (210) tar        (210)       76 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/dxfsl/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    58872 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/area.py
--rw-r--r--   0 tar        (210) tar        (210)    26928 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/areabuilder.py
--rw-r--r--   0 tar        (210) tar        (210)    13385 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/concat.py
--rw-r--r--   0 tar        (210) tar        (210)     9236 2024-02-16 13:30:18.000000 femagtools-1.6.6/src/femagtools/dxfsl/conv.py
--rw-r--r--   0 tar        (210) tar        (210)    21322 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/converter.py
--rw-r--r--   0 tar        (210) tar        (210)     1266 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/dxfsl/corner.py
--rw-r--r--   0 tar        (210) tar        (210)     1861 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/dxfsl/dumprenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    13451 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/dxfparser.py
--rw-r--r--   0 tar        (210) tar        (210)     2120 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/femparser.py
--rw-r--r--   0 tar        (210) tar        (210)    23377 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/dxfsl/fslrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    11705 2024-04-30 15:49:42.000000 femagtools-1.6.6/src/femagtools/dxfsl/functions.py
--rw-r--r--   0 tar        (210) tar        (210)   149449 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/geom.py
--rw-r--r--   0 tar        (210) tar        (210)     3239 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/journal.py
--rw-r--r--   0 tar        (210) tar        (210)    42548 2024-04-30 15:49:42.000000 femagtools-1.6.6/src/femagtools/dxfsl/machine.py
--rw-r--r--   0 tar        (210) tar        (210)    12710 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/dxfsl/plotrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    48608 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/shape.py
--rw-r--r--   0 tar        (210) tar        (210)     2905 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/svgparser.py
--rw-r--r--   0 tar        (210) tar        (210)    13835 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/symmetry.py
--rw-r--r--   0 tar        (210) tar        (210)    12832 2024-01-05 09:49:19.000000 femagtools-1.6.6/src/femagtools/ecloss.py
--rw-r--r--   0 tar        (210) tar        (210)     1224 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/erg.py
--rw-r--r--   0 tar        (210) tar        (210)    43124 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/femag.py
--rw-r--r--   0 tar        (210) tar        (210)     7415 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)    31994 2024-04-30 15:49:42.000000 femagtools-1.6.6/src/femagtools/fsl.py
--rw-r--r--   0 tar        (210) tar        (210)     3017 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/getset.py
--rw-r--r--   0 tar        (210) tar        (210)     3903 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/gmsh.py
--rw-r--r--   0 tar        (210) tar        (210)    17144 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/google.py
--rw-r--r--   0 tar        (210) tar        (210)     1561 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/grid.py
--rw-r--r--   0 tar        (210) tar        (210)     6275 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/femagtools/hxy.py
--rw-r--r--   0 tar        (210) tar        (210)    58332 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/isa7.py
--rw-r--r--   0 tar        (210) tar        (210)     1779 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/jhb.py
--rw-r--r--   0 tar        (210) tar        (210)    11320 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/job.py
--rw-r--r--   0 tar        (210) tar        (210)     5397 2023-11-29 08:38:16.000000 femagtools-1.6.6/src/femagtools/losscoeffs.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.668256 femagtools-1.6.6/src/femagtools/machine/
--rw-r--r--   0 tar        (210) tar        (210)     7174 2024-03-06 12:39:21.000000 femagtools-1.6.6/src/femagtools/machine/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    24766 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/machine/afpm.py
--rw-r--r--   0 tar        (210) tar        (210)    13151 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/machine/effloss.py
--rw-r--r--   0 tar        (210) tar        (210)    37925 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/machine/im.py
--rwxr-xr-x   0 tar        (210) tar        (210)    58517 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/machine/pm.py
--rw-r--r--   0 tar        (210) tar        (210)    23096 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/femagtools/machine/sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    34398 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/machine/sm.py
--rw-r--r--   0 tar        (210) tar        (210)    18621 2024-04-30 15:49:42.000000 femagtools-1.6.6/src/femagtools/machine/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     1093 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/magnet.py
--rw-r--r--   0 tar        (210) tar        (210)    40673 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/me.py
--rw-r--r--   0 tar        (210) tar        (210)    15119 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/model.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.669256 femagtools-1.6.6/src/femagtools/moo/
--rw-r--r--   0 tar        (210) tar        (210)      175 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5445 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/moo/algorithm.py
--rw-r--r--   0 tar        (210) tar        (210)    10100 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/population.py
--rw-r--r--   0 tar        (210) tar        (210)     2391 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/problem.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.669256 femagtools-1.6.6/src/femagtools/moo/test/
--rwxr-xr-x   0 tar        (210) tar        (210)     2535 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/test/AlgorithmTest.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5529 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/test/PopulationTest.py
--rwxr-xr-x   0 tar        (210) tar        (210)      505 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/test/ProblemTest.py
--rw-r--r--   0 tar        (210) tar        (210)     2825 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moproblem.py
--rw-r--r--   0 tar        (210) tar        (210)     8435 2023-12-15 11:25:08.000000 femagtools-1.6.6/src/femagtools/multiproc.py
--rw-r--r--   0 tar        (210) tar        (210)     2151 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/mxw2msh.py
--rw-r--r--   0 tar        (210) tar        (210)    14532 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     2052 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/netlist.py
--rw-r--r--   0 tar        (210) tar        (210)     3099 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/ntib.py
--rw-r--r--   0 tar        (210) tar        (210)     8687 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/opt.py
--rw-r--r--   0 tar        (210) tar        (210)    18799 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/parstudy.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.671255 femagtools-1.6.6/src/femagtools/plot/
--rw-r--r--   0 tar        (210) tar        (210)      920 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/plot/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    28525 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/plot/bch.py
--rw-r--r--   0 tar        (210) tar        (210)    11192 2023-11-29 08:38:16.000000 femagtools-1.6.6/src/femagtools/plot/char.py
--rw-r--r--   0 tar        (210) tar        (210)     1136 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/plot/fieldlines.py
--rw-r--r--   0 tar        (210) tar        (210)     1082 2023-10-30 08:37:24.000000 femagtools-1.6.6/src/femagtools/plot/fluxdens.py
--rw-r--r--   0 tar        (210) tar        (210)     2996 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/plot/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)     2960 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/plot/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     9548 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/plot/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     4765 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/plot/phasor.py
--rw-r--r--   0 tar        (210) tar        (210)     8462 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/plot/wdg.py
--rw-r--r--   0 tar        (210) tar        (210)     6536 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/poc.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.672256 femagtools-1.6.6/src/femagtools/svgfsl/
--rw-r--r--   0 tar        (210) tar        (210)     2738 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/svgfsl/converter.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.683255 femagtools-1.6.6/src/femagtools/templates/
--rw-r--r--   0 tar        (210) tar        (210)      874 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/FE-losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     3112 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/templates/afm_rotor.mako
--rw-r--r--   0 tar        (210) tar        (210)     5344 2023-12-15 11:25:08.000000 femagtools-1.6.6/src/femagtools/templates/afm_stator.mako
--rw-r--r--   0 tar        (210) tar        (210)      246 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/airgapinduc.mako
--rw-r--r--   0 tar        (210) tar        (210)     2879 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/asyn_motor.mako
--rw-r--r--   0 tar        (210) tar        (210)     3259 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/templates/basic_modpar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1346 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/templates/bertotti.mako
--rw-r--r--   0 tar        (210) tar        (210)     1911 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/calc_field_ts.mako
--rw-r--r--   0 tar        (210) tar        (210)     1600 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/calc_therm_field.mako
--rw-r--r--   0 tar        (210) tar        (210)     1867 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/cogg_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)      400 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/colorgrad.mako
--rw-r--r--   0 tar        (210) tar        (210)     1264 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/com_motor_sim.mako
--rw-r--r--   0 tar        (210) tar        (210)      472 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/conduct-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      663 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/connect_models.mako
--rw-r--r--   0 tar        (210) tar        (210)     1339 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/cu_losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     1672 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/ec-rotorbar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1983 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/fe-contr.mako
--rw-r--r--   0 tar        (210) tar        (210)      806 2023-12-15 11:25:08.000000 femagtools-1.6.6/src/femagtools/templates/fieldcalc.mako
--rw-r--r--   0 tar        (210) tar        (210)     3834 2023-11-06 06:50:13.000000 femagtools-1.6.6/src/femagtools/templates/gen_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)      560 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/inductances.mako
--rw-r--r--   0 tar        (210) tar        (210)     1359 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/ld_lq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      600 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/leak_dist_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      770 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/leak_evol_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      431 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/leak_tooth_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)     1271 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnet-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      788 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetFC2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2268 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron.mako
--rw-r--r--   0 tar        (210) tar        (210)     1426 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2315 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1413 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron4.mako
--rw-r--r--   0 tar        (210) tar        (210)     1376 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron5.mako
--rw-r--r--   0 tar        (210) tar        (210)     3960 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIronV.mako
--rw-r--r--   0 tar        (210) tar        (210)     3520 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/templates/magnetSector.mako
--rw-r--r--   0 tar        (210) tar        (210)      727 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetSectorLinear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1295 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetShell.mako
--rw-r--r--   0 tar        (210) tar        (210)     4080 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetShell2.mako
--rw-r--r--   0 tar        (210) tar        (210)     3425 2023-11-06 06:50:13.000000 femagtools-1.6.6/src/femagtools/templates/mesh-airgap.mako
--rw-r--r--   0 tar        (210) tar        (210)     2298 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/modal_analysis.mako
--rw-r--r--   0 tar        (210) tar        (210)     1327 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/templates/modified_steinmetz.mako
--rw-r--r--   0 tar        (210) tar        (210)     1255 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/mult_cal_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      345 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/new_model.mako
--rw-r--r--   0 tar        (210) tar        (210)     3209 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/noloadflux-rot.mako
--rw-r--r--   0 tar        (210) tar        (210)     4661 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/noloadflux.mako
--rw-r--r--   0 tar        (210) tar        (210)     3146 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/noloadfluxdc.mako
--rw-r--r--   0 tar        (210) tar        (210)      344 2023-08-31 09:32:32.000000 femagtools-1.6.6/src/femagtools/templates/open.mako
--rw-r--r--   0 tar        (210) tar        (210)      630 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/plots.mako
--rw-r--r--   0 tar        (210) tar        (210)     1464 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/pm_sym_f_cur.mako
--rw-r--r--   0 tar        (210) tar        (210)     2361 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/pm_sym_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)     1009 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/pm_sym_loss.mako
--rw-r--r--   0 tar        (210) tar        (210)     1339 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/psd_psq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      643 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/ring.mako
--rw-r--r--   0 tar        (210) tar        (210)      973 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rot_hsm.mako
--rw-r--r--   0 tar        (210) tar        (210)     2280 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rotorAsyn.mako
--rw-r--r--   0 tar        (210) tar        (210)     1908 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rotorKs2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1910 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rotor_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)      753 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rotor_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)     1981 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/shortcircuit.mako
--rw-r--r--   0 tar        (210) tar        (210)     2077 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/srm.mako
--rw-r--r--   0 tar        (210) tar        (210)      761 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator1.mako
--rw-r--r--   0 tar        (210) tar        (210)      599 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator2.mako
--rw-r--r--   0 tar        (210) tar        (210)      760 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator3Linear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1179 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator4.mako
--rw-r--r--   0 tar        (210) tar        (210)      893 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/statorBG.mako
--rw-r--r--   0 tar        (210) tar        (210)     2071 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/statorRing.mako
--rw-r--r--   0 tar        (210) tar        (210)     4942 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/statorRotor3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1799 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)     3142 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/therm-dynamic.mako
--rw-r--r--   0 tar        (210) tar        (210)     1427 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/templates/therm-static.mako
--rw-r--r--   0 tar        (210) tar        (210)     2264 2024-01-31 08:22:56.000000 femagtools-1.6.6/src/femagtools/templates/torq_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)     6228 2023-11-29 08:38:16.000000 femagtools-1.6.6/src/femagtools/tks.py
--rw-r--r--   0 tar        (210) tar        (210)    47216 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/ts.py
--rw-r--r--   0 tar        (210) tar        (210)     1581 2024-02-16 13:30:18.000000 femagtools-1.6.6/src/femagtools/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     2444 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/vbf.py
--rw-r--r--   0 tar        (210) tar        (210)    10723 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/femagtools/vtu.py
--rw-r--r--   0 tar        (210) tar        (210)    22197 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/windings.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.694255 femagtools-1.6.6/src/femagtools.egg-info/
--rw-r--r--   0 tar        (210) tar        (210)     5827 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     7054 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/SOURCES.txt
--rw-r--r--   0 tar        (210) tar        (210)        1 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/dependency_links.txt
--rw-r--r--   0 tar        (210) tar        (210)      248 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/entry_points.txt
--rw-r--r--   0 tar        (210) tar        (210)      182 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/requires.txt
--rw-r--r--   0 tar        (210) tar        (210)       17 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/top_level.txt
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.692255 femagtools-1.6.6/src/tests/
--rwxr-xr-x   0 tar        (210) tar        (210)        0 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/__init__.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.692255 femagtools-1.6.6/src/tests/engines/
--rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/engines/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     2014 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/engines/test_amazon.py
--rw-r--r--   0 tar        (210) tar        (210)      663 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/engines/test_config.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.693255 femagtools-1.6.6/src/tests/geom/
--rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/geom/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     1219 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/geom/test_functions.py
--rw-r--r--   0 tar        (210) tar        (210)     3183 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/geom/test_point_inside.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.693255 femagtools-1.6.6/src/tests/moo/
--rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/moo/__init__.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2563 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/moo/test_algorithm.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5471 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/moo/test_population.py
--rwxr-xr-x   0 tar        (210) tar        (210)      467 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/moo/test_problem.py
--rw-r--r--   0 tar        (210) tar        (210)    11031 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_afpm.py
--rw-r--r--   0 tar        (210) tar        (210)     1065 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_airgap_induction.py
--rw-r--r--   0 tar        (210) tar        (210)      637 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_amela.py
--rw-r--r--   0 tar        (210) tar        (210)     1398 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    15497 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/tests/test_bchreader.py
--rw-r--r--   0 tar        (210) tar        (210)      332 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     6497 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_convert.py
--rw-r--r--   0 tar        (210) tar        (210)      383 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/tests/test_dxfsl.py
--rw-r--r--   0 tar        (210) tar        (210)     1142 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_effloss.py
--rw-r--r--   0 tar        (210) tar        (210)      523 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_erg.py
--rw-r--r--   0 tar        (210) tar        (210)     1934 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/tests/test_femag.py
--rw-r--r--   0 tar        (210) tar        (210)      536 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_forcedens.py
--rwxr-xr-x   0 tar        (210) tar        (210)    16623 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/tests/test_fsl.py
--rw-r--r--   0 tar        (210) tar        (210)      640 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/tests/test_hxy.py
--rw-r--r--   0 tar        (210) tar        (210)      662 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_im.py
--rw-r--r--   0 tar        (210) tar        (210)     3001 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_isa7.py
--rw-r--r--   0 tar        (210) tar        (210)      824 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_jhb.py
--rw-r--r--   0 tar        (210) tar        (210)      981 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_job.py
--rw-r--r--   0 tar        (210) tar        (210)     2012 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_losscoeffs.py
--rwxr-xr-x   0 tar        (210) tar        (210)    12881 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_machine.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2608 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_magncurv.py
--rw-r--r--   0 tar        (210) tar        (210)      276 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_magnet.py
--rw-r--r--   0 tar        (210) tar        (210)      283 2023-09-08 08:10:31.000000 femagtools-1.6.6/src/tests/test_mcv.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2118 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_mcvreader.py
--rwxr-xr-x   0 tar        (210) tar        (210)     3986 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_mcvwriter.py
--rw-r--r--   0 tar        (210) tar        (210)      196 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_me.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2372 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_model.py
--rw-r--r--   0 tar        (210) tar        (210)     4205 2024-01-31 08:22:56.000000 femagtools-1.6.6/src/tests/test_nc.py
--rw-r--r--   0 tar        (210) tar        (210)     1340 2024-01-31 08:22:56.000000 femagtools-1.6.6/src/tests/test_parident.py
--rw-r--r--   0 tar        (210) tar        (210)     3200 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_parstudy.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5816 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_pocfile.py
--rw-r--r--   0 tar        (210) tar        (210)     1131 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/tests/test_sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    83524 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_sm.py
--rwxr-xr-x   0 tar        (210) tar        (210)      766 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_tksreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_ts.py
--rwxr-xr-x   0 tar        (210) tar        (210)      832 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_vbfreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1469 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/tests/test_vtu.py
--rw-r--r--   0 tar        (210) tar        (210)     4912 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.963812 femagtools-1.6.7/
+-rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.6.7/LICENSE
+-rw-r--r--   0 tar        (210) tar        (210)       39 2023-08-31 09:32:32.000000 femagtools-1.6.7/MANIFEST.in
+-rw-r--r--   0 tar        (210) tar        (210)     5827 2024-05-02 15:08:16.963812 femagtools-1.6.7/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.6.7/README.md
+-rw-r--r--   0 tar        (210) tar        (210)     1414 2024-04-30 15:50:23.000000 femagtools-1.6.7/pyproject.toml
+-rw-r--r--   0 tar        (210) tar        (210)       38 2024-05-02 15:08:16.963812 femagtools-1.6.7/setup.cfg
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.937812 femagtools-1.6.7/src/
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.941812 femagtools-1.6.7/src/femagtools/
+-rw-r--r--   0 tar        (210) tar        (210)     1615 2024-05-02 15:07:02.000000 femagtools-1.6.7/src/femagtools/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     1577 2024-01-31 08:22:56.000000 femagtools-1.6.7/src/femagtools/airgap.py
+-rw-r--r--   0 tar        (210) tar        (210)    12069 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)    13891 2023-12-15 11:25:08.000000 femagtools-1.6.7/src/femagtools/amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     7660 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    71680 2024-03-06 12:39:21.000000 femagtools-1.6.7/src/femagtools/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)     3142 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/bchxml.py
+-rw-r--r--   0 tar        (210) tar        (210)    10766 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/condor.py
+-rw-r--r--   0 tar        (210) tar        (210)     1076 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     3136 2023-10-30 08:37:24.000000 femagtools-1.6.7/src/femagtools/config.py
+-rw-r--r--   0 tar        (210) tar        (210)    26478 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     6901 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/dakota.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     4068 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/dakota_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     5573 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/dakotaout.py
+-rw-r--r--   0 tar        (210) tar        (210)     7460 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/docker.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.943812 femagtools-1.6.7/src/femagtools/dxfsl/
+-rw-r--r--   0 tar        (210) tar        (210)       76 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/dxfsl/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    58872 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/area.py
+-rw-r--r--   0 tar        (210) tar        (210)    29780 2024-05-02 15:06:12.000000 femagtools-1.6.7/src/femagtools/dxfsl/areabuilder.py
+-rw-r--r--   0 tar        (210) tar        (210)    13385 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/concat.py
+-rw-r--r--   0 tar        (210) tar        (210)     9236 2024-02-16 13:30:18.000000 femagtools-1.6.7/src/femagtools/dxfsl/conv.py
+-rw-r--r--   0 tar        (210) tar        (210)    21322 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/converter.py
+-rw-r--r--   0 tar        (210) tar        (210)     1266 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/dxfsl/corner.py
+-rw-r--r--   0 tar        (210) tar        (210)     1861 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/dxfsl/dumprenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    13451 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/dxfparser.py
+-rw-r--r--   0 tar        (210) tar        (210)     2120 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/femparser.py
+-rw-r--r--   0 tar        (210) tar        (210)    23377 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/dxfsl/fslrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    11705 2024-04-30 15:49:42.000000 femagtools-1.6.7/src/femagtools/dxfsl/functions.py
+-rw-r--r--   0 tar        (210) tar        (210)   149449 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/geom.py
+-rw-r--r--   0 tar        (210) tar        (210)     3239 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/journal.py
+-rw-r--r--   0 tar        (210) tar        (210)    42548 2024-04-30 15:49:42.000000 femagtools-1.6.7/src/femagtools/dxfsl/machine.py
+-rw-r--r--   0 tar        (210) tar        (210)    12710 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/dxfsl/plotrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    48608 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/shape.py
+-rw-r--r--   0 tar        (210) tar        (210)     2905 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/svgparser.py
+-rw-r--r--   0 tar        (210) tar        (210)    13835 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/dxfsl/symmetry.py
+-rw-r--r--   0 tar        (210) tar        (210)    12832 2024-01-05 09:49:19.000000 femagtools-1.6.7/src/femagtools/ecloss.py
+-rw-r--r--   0 tar        (210) tar        (210)     1224 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/erg.py
+-rw-r--r--   0 tar        (210) tar        (210)    43124 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     7415 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)    31994 2024-04-30 15:49:42.000000 femagtools-1.6.7/src/femagtools/fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     3017 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/getset.py
+-rw-r--r--   0 tar        (210) tar        (210)     3903 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/gmsh.py
+-rw-r--r--   0 tar        (210) tar        (210)    17144 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/google.py
+-rw-r--r--   0 tar        (210) tar        (210)     1561 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/grid.py
+-rw-r--r--   0 tar        (210) tar        (210)     6275 2023-12-20 15:28:20.000000 femagtools-1.6.7/src/femagtools/hxy.py
+-rw-r--r--   0 tar        (210) tar        (210)    58332 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)     1779 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)    11320 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/job.py
+-rw-r--r--   0 tar        (210) tar        (210)     5397 2023-11-29 08:38:16.000000 femagtools-1.6.7/src/femagtools/losscoeffs.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.943812 femagtools-1.6.7/src/femagtools/machine/
+-rw-r--r--   0 tar        (210) tar        (210)     7174 2024-03-06 12:39:21.000000 femagtools-1.6.7/src/femagtools/machine/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    24766 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/machine/afpm.py
+-rw-r--r--   0 tar        (210) tar        (210)    13315 2024-05-02 15:06:12.000000 femagtools-1.6.7/src/femagtools/machine/effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)    37925 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/machine/im.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    58517 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/machine/pm.py
+-rw-r--r--   0 tar        (210) tar        (210)    23096 2023-12-20 15:28:20.000000 femagtools-1.6.7/src/femagtools/machine/sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    34398 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/machine/sm.py
+-rw-r--r--   0 tar        (210) tar        (210)    18621 2024-04-30 15:49:42.000000 femagtools-1.6.7/src/femagtools/machine/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     1093 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)    40673 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/me.py
+-rw-r--r--   0 tar        (210) tar        (210)    15119 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/model.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.944812 femagtools-1.6.7/src/femagtools/moo/
+-rw-r--r--   0 tar        (210) tar        (210)      175 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/moo/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5445 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/moo/algorithm.py
+-rw-r--r--   0 tar        (210) tar        (210)    10100 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/moo/population.py
+-rw-r--r--   0 tar        (210) tar        (210)     2391 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/moo/problem.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.944812 femagtools-1.6.7/src/femagtools/moo/test/
+-rwxr-xr-x   0 tar        (210) tar        (210)     2535 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/moo/test/AlgorithmTest.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5529 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/moo/test/PopulationTest.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      505 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/moo/test/ProblemTest.py
+-rw-r--r--   0 tar        (210) tar        (210)     2825 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/moproblem.py
+-rw-r--r--   0 tar        (210) tar        (210)     8435 2023-12-15 11:25:08.000000 femagtools-1.6.7/src/femagtools/multiproc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2151 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/mxw2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)    14532 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2052 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/netlist.py
+-rw-r--r--   0 tar        (210) tar        (210)     3099 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/ntib.py
+-rw-r--r--   0 tar        (210) tar        (210)     8687 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/opt.py
+-rw-r--r--   0 tar        (210) tar        (210)    18799 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/parstudy.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.944812 femagtools-1.6.7/src/femagtools/plot/
+-rw-r--r--   0 tar        (210) tar        (210)      920 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/plot/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    28525 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/plot/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)    11192 2023-11-29 08:38:16.000000 femagtools-1.6.7/src/femagtools/plot/char.py
+-rw-r--r--   0 tar        (210) tar        (210)     1136 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/plot/fieldlines.py
+-rw-r--r--   0 tar        (210) tar        (210)     1082 2023-10-30 08:37:24.000000 femagtools-1.6.7/src/femagtools/plot/fluxdens.py
+-rw-r--r--   0 tar        (210) tar        (210)     2996 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/plot/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)     2960 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/plot/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     9548 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/femagtools/plot/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     4765 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/plot/phasor.py
+-rw-r--r--   0 tar        (210) tar        (210)     8462 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/plot/wdg.py
+-rw-r--r--   0 tar        (210) tar        (210)     6536 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/poc.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.945812 femagtools-1.6.7/src/femagtools/svgfsl/
+-rw-r--r--   0 tar        (210) tar        (210)     2748 2024-05-02 15:06:12.000000 femagtools-1.6.7/src/femagtools/svgfsl/converter.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.960812 femagtools-1.6.7/src/femagtools/templates/
+-rw-r--r--   0 tar        (210) tar        (210)      874 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/FE-losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3112 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/templates/afm_rotor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     5344 2023-12-15 11:25:08.000000 femagtools-1.6.7/src/femagtools/templates/afm_stator.mako
+-rw-r--r--   0 tar        (210) tar        (210)      246 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/airgapinduc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2879 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/asyn_motor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3259 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/templates/basic_modpar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1346 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/templates/bertotti.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1911 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/calc_field_ts.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1600 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/calc_therm_field.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1867 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/cogg_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      400 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/colorgrad.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1264 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/com_motor_sim.mako
+-rw-r--r--   0 tar        (210) tar        (210)      472 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/conduct-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      663 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/connect_models.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1339 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/cu_losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1672 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/ec-rotorbar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1983 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/fe-contr.mako
+-rw-r--r--   0 tar        (210) tar        (210)      806 2023-12-15 11:25:08.000000 femagtools-1.6.7/src/femagtools/templates/fieldcalc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3834 2023-11-06 06:50:13.000000 femagtools-1.6.7/src/femagtools/templates/gen_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)      560 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/inductances.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1359 2023-09-06 13:17:09.000000 femagtools-1.6.7/src/femagtools/templates/ld_lq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      600 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/leak_dist_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      770 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/leak_evol_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      431 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/leak_tooth_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1271 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnet-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      788 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetFC2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2268 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetIron.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1426 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetIron2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2315 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetIron3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1413 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetIron4.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1376 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetIron5.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3960 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetIronV.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3520 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/templates/magnetSector.mako
+-rw-r--r--   0 tar        (210) tar        (210)      727 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetSectorLinear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1295 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetShell.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4080 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/magnetShell2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3425 2023-11-06 06:50:13.000000 femagtools-1.6.7/src/femagtools/templates/mesh-airgap.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2298 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/modal_analysis.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1327 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/templates/modified_steinmetz.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1255 2023-09-06 13:17:09.000000 femagtools-1.6.7/src/femagtools/templates/mult_cal_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      345 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/new_model.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3209 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/noloadflux-rot.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4661 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/noloadflux.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3146 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/noloadfluxdc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      344 2023-08-31 09:32:32.000000 femagtools-1.6.7/src/femagtools/templates/open.mako
+-rw-r--r--   0 tar        (210) tar        (210)      630 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/plots.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1464 2023-09-06 13:17:09.000000 femagtools-1.6.7/src/femagtools/templates/pm_sym_f_cur.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2361 2023-09-06 13:17:09.000000 femagtools-1.6.7/src/femagtools/templates/pm_sym_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1009 2023-09-06 13:17:09.000000 femagtools-1.6.7/src/femagtools/templates/pm_sym_loss.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1339 2023-09-06 13:17:09.000000 femagtools-1.6.7/src/femagtools/templates/psd_psq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      643 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/ring.mako
+-rw-r--r--   0 tar        (210) tar        (210)      973 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/rot_hsm.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2280 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/rotorAsyn.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1908 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/rotorKs2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1910 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/rotor_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)      753 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/rotor_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1981 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/shortcircuit.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2077 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/srm.mako
+-rw-r--r--   0 tar        (210) tar        (210)      761 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/stator1.mako
+-rw-r--r--   0 tar        (210) tar        (210)      599 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/stator2.mako
+-rw-r--r--   0 tar        (210) tar        (210)      760 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/stator3Linear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1179 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/stator4.mako
+-rw-r--r--   0 tar        (210) tar        (210)      893 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/statorBG.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2071 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/statorRing.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4942 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/statorRotor3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1799 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/stator_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3142 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/templates/therm-dynamic.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1427 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/templates/therm-static.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2264 2024-01-31 08:22:56.000000 femagtools-1.6.7/src/femagtools/templates/torq_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     6228 2023-11-29 08:38:16.000000 femagtools-1.6.7/src/femagtools/tks.py
+-rw-r--r--   0 tar        (210) tar        (210)    47216 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/femagtools/ts.py
+-rw-r--r--   0 tar        (210) tar        (210)     1581 2024-02-16 13:30:18.000000 femagtools-1.6.7/src/femagtools/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     2444 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/femagtools/vbf.py
+-rw-r--r--   0 tar        (210) tar        (210)    10723 2023-12-20 15:28:20.000000 femagtools-1.6.7/src/femagtools/vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)    22197 2023-10-25 05:52:21.000000 femagtools-1.6.7/src/femagtools/windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.963812 femagtools-1.6.7/src/femagtools.egg-info/
+-rw-r--r--   0 tar        (210) tar        (210)     5827 2024-05-02 15:08:16.000000 femagtools-1.6.7/src/femagtools.egg-info/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     7054 2024-05-02 15:08:16.000000 femagtools-1.6.7/src/femagtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tar        (210) tar        (210)        1 2024-05-02 15:08:16.000000 femagtools-1.6.7/src/femagtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tar        (210) tar        (210)      248 2024-05-02 15:08:16.000000 femagtools-1.6.7/src/femagtools.egg-info/entry_points.txt
+-rw-r--r--   0 tar        (210) tar        (210)      182 2024-05-02 15:08:16.000000 femagtools-1.6.7/src/femagtools.egg-info/requires.txt
+-rw-r--r--   0 tar        (210) tar        (210)       17 2024-05-02 15:08:16.000000 femagtools-1.6.7/src/femagtools.egg-info/top_level.txt
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.962812 femagtools-1.6.7/src/tests/
+-rwxr-xr-x   0 tar        (210) tar        (210)        0 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/__init__.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.962812 femagtools-1.6.7/src/tests/engines/
+-rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/engines/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     2014 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/engines/test_amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)      663 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/engines/test_config.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.962812 femagtools-1.6.7/src/tests/geom/
+-rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/geom/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     1219 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/geom/test_functions.py
+-rw-r--r--   0 tar        (210) tar        (210)     3183 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/geom/test_point_inside.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-05-02 15:08:16.962812 femagtools-1.6.7/src/tests/moo/
+-rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/moo/__init__.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2563 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/moo/test_algorithm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5471 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/moo/test_population.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      467 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/moo/test_problem.py
+-rw-r--r--   0 tar        (210) tar        (210)    11031 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_afpm.py
+-rw-r--r--   0 tar        (210) tar        (210)     1065 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_airgap_induction.py
+-rw-r--r--   0 tar        (210) tar        (210)      637 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     1398 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    15497 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/tests/test_bchreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      332 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     6497 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_convert.py
+-rw-r--r--   0 tar        (210) tar        (210)      383 2024-04-30 15:50:23.000000 femagtools-1.6.7/src/tests/test_dxfsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     1142 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)      523 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_erg.py
+-rw-r--r--   0 tar        (210) tar        (210)     1934 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/tests/test_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)      536 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_forcedens.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    16623 2024-02-08 08:06:18.000000 femagtools-1.6.7/src/tests/test_fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)      640 2023-12-20 15:28:20.000000 femagtools-1.6.7/src/tests/test_hxy.py
+-rw-r--r--   0 tar        (210) tar        (210)      662 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_im.py
+-rw-r--r--   0 tar        (210) tar        (210)     3001 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)      824 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)      981 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2012 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_losscoeffs.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    12881 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_machine.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2608 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_magncurv.py
+-rw-r--r--   0 tar        (210) tar        (210)      276 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)      283 2023-09-08 08:10:31.000000 femagtools-1.6.7/src/tests/test_mcv.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2118 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_mcvreader.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     3986 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_mcvwriter.py
+-rw-r--r--   0 tar        (210) tar        (210)      196 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_me.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2372 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_model.py
+-rw-r--r--   0 tar        (210) tar        (210)     4205 2024-01-31 08:22:56.000000 femagtools-1.6.7/src/tests/test_nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1340 2024-01-31 08:22:56.000000 femagtools-1.6.7/src/tests/test_parident.py
+-rw-r--r--   0 tar        (210) tar        (210)     3200 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_parstudy.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5816 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_pocfile.py
+-rw-r--r--   0 tar        (210) tar        (210)     1131 2023-12-20 15:28:20.000000 femagtools-1.6.7/src/tests/test_sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    83524 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_sm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      766 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_tksreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_ts.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      832 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_vbfreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1469 2023-12-20 15:28:20.000000 femagtools-1.6.7/src/tests/test_vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)     4912 2023-08-30 14:12:51.000000 femagtools-1.6.7/src/tests/test_windings.py
```

### Comparing `femagtools-1.6.6/LICENSE` & `femagtools-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/PKG-INFO` & `femagtools-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <dzhang@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.6.6/README.md` & `femagtools-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/pyproject.toml` & `femagtools-1.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/__init__.py` & `femagtools-1.6.7/src/femagtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Python API for FEMAG
 
 """
 __title__ = 'femagtools'
-__version__ = '1.6.6'
+__version__ = '1.6.7'
 __author__ = 'Ronald Tanner'
 __license__ = 'BSD'
 __copyright__ = 'Copyright 2016-2022 SEMAFOR Informatik & Energie AG'
 
 from .asm import read
 from .bch import Reader
 from .model import MachineModel
```

### Comparing `femagtools-1.6.6/src/femagtools/airgap.py` & `femagtools-1.6.7/src/femagtools/airgap.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/amazon.py` & `femagtools-1.6.7/src/femagtools/amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/amela.py` & `femagtools-1.6.7/src/femagtools/amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/asm.py` & `femagtools-1.6.7/src/femagtools/asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/bch.py` & `femagtools-1.6.7/src/femagtools/bch.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/bchxml.py` & `femagtools-1.6.7/src/femagtools/bchxml.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/condor.py` & `femagtools-1.6.7/src/femagtools/condor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/conductor.py` & `femagtools-1.6.7/src/femagtools/conductor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/config.py` & `femagtools-1.6.7/src/femagtools/config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/convert.py` & `femagtools-1.6.7/src/femagtools/convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dakota.py` & `femagtools-1.6.7/src/femagtools/dakota.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dakota_femag.py` & `femagtools-1.6.7/src/femagtools/dakota_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dakotaout.py` & `femagtools-1.6.7/src/femagtools/dakotaout.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/docker.py` & `femagtools-1.6.7/src/femagtools/docker.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/area.py` & `femagtools-1.6.7/src/femagtools/dxfsl/area.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/areabuilder.py` & `femagtools-1.6.7/src/femagtools/dxfsl/areabuilder.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,46 @@
 from femagtools.dxfsl.functions import alpha_line, alpha_points, alpha_angle
 from femagtools.dxfsl.functions import less, is_same_angle
 from femagtools.dxfsl.functions import Timer
 from femagtools.dxfsl.journal import getJournal
 import io
 import time
 
-logger = logging.getLogger('femagtools.concat')
+logger = logging.getLogger('femagtools.areabuilder')
+original_log_level = None
 
+def disable_logging():
+    logger
+    global original_log_level
+    # Store the current log level to restore it later
+    original_log_level = logger.getEffectiveLevel()
+    logger.debug("Logging level %s disabled", original_log_level)
+
+    # Set the log level to a higher level, e.g., WARNING or CRITICAL
+    logging.disable(logging.CRITICAL)
+
+
+def enable_logging():
+    #if original_log_level is not None:
+    # Restore the original log level after the tests
+    logging.disable(logging.NOTSET)
+    logger.debug("Logging level %s enabled", original_log_level)
 
+    
 def log_lefthand(left, edge1, edge2):
     if left:
         edge1.log_edge("**** left")
     else:
         edge2.log_edge("**** left")
 
 
 #############################
 #        areabuilder        #
 #############################
 
-
 class EdgeInfo(object):
     def __init__(self,
                  edge_data=None,
                  n1 = None,
                  n2 = None,
                  handmade=False):
         assert(edge_data)
@@ -109,26 +126,55 @@
     def is_tracked(self):
         return self.tracked
 
     def set_start_angle(self):
         start_angle = positive_angle(self.n2_angle_ingoing())
         self.startangle = start_angle
 
-    def set_direction_angle(self, start_angle):
-        angle = positive_angle(alpha_angle(start_angle, self.n1_angle_ingoing()))
-        if is_same_angle(0.0, angle, atol=0.008):  # 1/2 degree
+    def set_direction_angle(self, start_edge):
+        start_angle = start_edge.startangle
+        logger.debug("begin set_direction_angle: of %s", self.name)
+        self.angle = positive_angle(alpha_angle(start_angle, self.n1_angle_ingoing()))
+        logger.debug("set_direction_angle: angle is %s", self.angle)
+
+        if is_same_angle(0.0, self.angle, atol=0.008):  # 1/2 degree
             # reverse direction
-            if self.n1_direction_righthand():
-                self.angle = 2.0 * np.pi
-            elif self.n1_direction_lefthand():
-                self.angle = 0.0
-            else:
-                self.angle = angle
-        else:
-            self.angle = angle
+            logger.debug("set_direction_angle: reverse direction( nearly 180 degrees)")
+
+            if start_edge.is_arc():
+                start_lefthand = start_edge.n1_direction_lefthand()
+                if self.is_arc():
+                    myself_lefthand = self.n1_direction_lefthand()
+                    if start_lefthand:
+                        if not myself_lefthand:  # righthand => same side
+                            left = self.radius() < start_edge.radius()
+                        else:
+                            left = False
+                    else:
+                        if myself_lefthand:  # lefthand => same side
+                            left = self.radius() > start_edge.radius()
+                        else:
+                            left = True
+                    if left:  # self is left
+                        self.angle = np.pi * 2.0
+                    else:
+                        self.angle = 0.0
+                elif self.is_line():
+                    if start_lefthand:
+                        self.angle = 0.0
+                    else:
+                        self.angle = np.pi * 2.0
+            else:  # start is a line
+                if self.is_arc():
+                    if self.n1_direction_righthand():
+                        self.angle = np.pi * 2.0
+                    else:
+                        self.angle = 0.0
+
+        logger.debug("end set_direction_angle: angle is %s", self.angle)
 
     def n1_angle_outgoing(self):
         return self.element.get_alpha(self.n1)
 
     def n1_angle_ingoing(self):
         return normalise_angle(self.element.get_alpha(self.n1) + np.pi)
 
@@ -162,107 +208,89 @@
         #    return False
 
         dist_n2 = distance(self.element.center, info.n2)
         return np.isclose(self.element.radius, dist_n2, 0.005, 0.005)
 
     def myself_direction_lefthand(self, start_edge, nbr_edge, builder, ignore_start=False):
         logger.debug("start of myself_direction_lefthand")
+        start_edge.log_edge("===> start")
         self.log_edge("---> self")
         nbr_edge.log_edge("---> nbr")
 
         myself_angle = self.angle
         other_angle = nbr_edge.angle
 
         if is_same_angle(0.0, myself_angle):
             # 360 or 0 degrees => turn 180 degrees
             logger.debug("-- ATTENTION: myself %s turns nearly 180 degrees", self.classname())
             logger.debug("   the angle is %s", myself_angle)
+
             if start_edge.is_arc():
                 if self.is_line() and not ignore_start:
                     if start_edge.line_arc_close_together(self):
                         logger.debug("START ARC and SELF LINE close")
                         arc_edge = start_edge.get_reverse_edge()  # reverse start edge
                         arc_edge.log_name("REVERSE")
-                        arc_edge.set_direction_angle(start_edge.startangle)
+                        arc_edge.set_direction_angle(start_edge)
                         left = not arc_edge.arc_line_direction_lefthand(start_edge, self, builder)
                         log_lefthand(left, self, arc_edge)
                         if left:  # self is left
                             myself_angle = 0.0
                         else:
                             myself_angle = np.pi * 2.0
                         left = myself_angle > other_angle
 
                         log_lefthand(left, self, nbr_edge)
-                        logger.debug("#3: end of myself_direction_lefthand: ==> %s", left)
+                        logger.debug("#1a: end of myself_direction_lefthand: ==> %s", left)
                         return left
-                    
-                if start_edge.n1_direction_lefthand():
-                    myself_angle = 0.0
-                else:
-                    myself_angle = np.pi * 2.0
     
             elif self.is_arc():
                 if not ignore_start:
                     if self.line_arc_close_together(start_edge):
                         logger.debug("START LINE and SELF ARC close")
                         line_edge = start_edge.get_reverse_edge()  # reverse start edge
                         line_edge.log_name("REVERSE")
-                        line_edge.set_direction_angle(start_edge.startangle)
+                        line_edge.set_direction_angle(start_edge)
                         left = self.arc_line_direction_lefthand(start_edge, line_edge, builder)
                         log_lefthand(left, self, line_edge)
                         if left:  # self is left
                             myself_angle = 0.0
                         else:
                             myself_angle = np.pi * 2.0
                         left = myself_angle > other_angle
 
                         log_lefthand(left, self, nbr_edge)
                         logger.debug("#4: end of myself_direction_lefthand: ==> %s", left)
                         return left
 
-                if self.n1_direction_lefthand():
-                    myself_angle = 0.0
-                else:
-                    myself_angle = np.pi * 2.0
-
         if is_same_angle(0.0, other_angle, atol=0.008):  # 1/2 degree
             # 360 or 0 degrees => turn 180 degrees
             logger.debug("-- ATTENTION: other %s turns nearly 180 degrees", nbr_edge.classname())
             logger.debug("   the angle is %s", other_angle)
             if start_edge.is_arc():
                 if nbr_edge.is_line() and not ignore_start:
                     if start_edge.line_arc_close_together(nbr_edge):
                         logger.debug("START ARC and SELF LINE close")
                         arc_edge = start_edge.get_reverse_edge()  # reverse start edge
-                        arc_edge.set_direction_angle(start_edge.startangle)
+                        arc_edge.set_direction_angle(start_edge)
                         left = arc_edge.arc_line_direction_lefthand(start_edge, nbr_edge, builder)
-                        log_lefthand(left, self, line_edge)
+                        log_lefthand(left, self, nbr_edge)
                         logger.debug("#5: end of myself_direction_lefthand: ==> %s", not left)
                         return not left
 
-                if start_edge.n1_direction_lefthand():
-                    other_angle = 0.0
-                else:
-                    other_angle = np.pi * 2.0
-
             elif nbr_edge.is_arc():
                 if not ignore_start:
                     if nbr_edge.line_arc_close_together(start_edge):
                         logger.debug("START LINE and NEIGHBOR ARC close")
                         line_edge = start_edge.get_reverse_edge()  # reverse start edge
-                        line_edge.set_direction_angle(start_edge.startangle)
+                        line_edge.set_direction_angle(start_edge)
                         left = nbr_edge.arc_line_direction_lefthand(start_edge, line_edge, builder)
                         logger.debug("#6: end of myself_direction_lefthand: ==> %s", left)
                         return left
 
-                if nbr_edge.n1_direction_lefthand():
-                    other_angle = 0.0
-                else:
-                    other_angle = np.pi * 2.0
-
         logger.debug("-- angles: myself = %s,  other = %s",
                      myself_angle, other_angle)
         if not is_same_angle(myself_angle, other_angle, atol=0.008):  # 1/2 degree
             logger.debug("-- angles are different")
             left = myself_angle > other_angle
             log_lefthand(left, self, nbr_edge)
             logger.debug("end of myself_direction_lefthand: ==> %s", left)
@@ -324,35 +352,54 @@
             logger.debug("end of arc_line_direction_lefthand: arc lefthand = %s", left)
             return left
 
         logger.debug("-- ATTENTION: line look ahead")
         line_edge.startangle = start_edge.startangle
         # Line is start-edge now
         next_edge = builder.next_edge_lefthand_side(line_edge)  # next of line
-        next_edge.set_direction_angle(start_edge.startangle)
+        next_edge.set_direction_angle(start_edge)
         left = self.myself_direction_lefthand(start_edge,
                                               next_edge,
                                               builder,
                                               ignore_start=True)
         logger.debug("end of arc_line_direction_lefthand: arc lefthand = %s", left)
         return left
 
+    def get_alpha_points(self, prev_n):
+        n1 = self.n1
+        n2 = self.n2
+        a = 0.0
+        if self.is_arc():
+            angle = self.element.get_angle_of_arc()
+            if angle > np.pi * 0.75:
+                n = self.element.center_of_connection()
+                a = normalise_angle(alpha_points(prev_n,
+                                                 n1,
+                                                 n))
+                n1 = n
+
+        a += normalise_angle(alpha_points(prev_n,
+                                          n1,
+                                          n2))
+        return a, n1
 
 class AreaBuilder(object):
     def __init__(self,
                  geom=None,
+                 nolog=True,
                  rtol=1e-04,
                  atol=1e-04,
                  ndec=6):
         self.rtol = rtol
         self.atol = atol
         self.ndec = ndec
         self.geom = geom
         self.area_list = []
         self.journal = getJournal()
+        self.nolog = nolog
 
     def __str__(self):
         return "rtol: {}\n".format(self.rtol) + \
                "atol: {}\n".format(self.atol)
 
     def all_neighbors(self, n):
         for n in self.geom.g.neighbors(n):
@@ -375,28 +422,30 @@
         def append(area_list, a):
             for area in area_list:
                 if area.is_identical(a):
                     return
             area_list.append(a)
 
         timer = Timer(start_it=True)
-
+        if self.nolog:
+            disable_logging()
         self.set_edge_attributes()
         
         for n in self.geom.nodes():
             finished = False
             while not finished:
                 finished = True
                 nbrs = [nbr for nbr in self.geom.g.neighbors(n)]
                 for next_n in nbrs:
                     result = self.get_new_area(n, next_n)
                     if result['ok']:
                         a = self.append_new_area(self.area_list, result['area'])
                         logger.debug("Area %s found", a.identifier())
-
+        if self.nolog:
+            enable_logging()
         t = timer.stop("{} areas created in %0.4f seconds".format(len(self.area_list)))
         if main:
             self.journal.put('time_build_areas', t)
         if self.errors > 0:
             logger.warning("WARNING: %s errors while creating %s areas",
                            self.errors, len(self.area_list))
         self.journal.put_areas(len(self.area_list))
@@ -457,22 +506,21 @@
         if not info_next:
             result['msg'] = ("dead end ({}, {})"
                              .format(info_curr.n1, info_curr.n2))
             logger.debug("<== %s", result['msg'])
             self.errors += 1
             return result
 
-        prev_n1 = info_curr.n1
+        prev_node = info_curr.n1
         next_n1 = info_next.n1
         next_n2 = info_next.n2
 
-        alpha = normalise_angle(alpha_points(prev_n1,
-                                             next_n1,
-                                             next_n2))
+        alpha, prev_node = info_next.get_alpha_points(prev_node)
 
+        logger.debug("--> alpha %s <--", alpha)
         c = 1
         while not (nodes_are_equal(next_n1, start_n1) and
                    nodes_are_equal(next_n2, start_n2)):
             c += 1
             if c > self.geom.num_edges * 2:
                 logger.error("FATAL: *** over %s elements in area ? ***",
                              self.geom.num_edges)
@@ -501,22 +549,20 @@
                 result['msg'] = ("<== dead end ({},{})"
                                  .format(info_curr.n1, info_curr.n2))
                 logger.debug("<== %s", result['msg'])
                 result['elements'] = c
                 self.errors += 1
                 return result
 
-            prev_n1 = info_curr.n1
             next_n1 = info_next.n1
             next_n2 = info_next.n2
 
-            a = normalise_angle(alpha_points(prev_n1,
-                                             next_n1,
-                                             next_n2))
+            a, prev_node = info_next.get_alpha_points(prev_node)
             alpha += a
+            logger.debug("--> alpha %s (+ %s) <--", alpha, a)
 
         logger.debug("  END OF get_new_area")
 
         if less(alpha, 0.0):
             result['msg'] = ("turn left expected, but it turned right ({})"
                              .format(alpha))
             logger.debug("<== %s", result['msg'])
@@ -539,38 +585,40 @@
                      start_edge.n2)
 
         nbrs = self.get_neighbors(start_edge)
         if len(nbrs) == 0:
             logger.debug("WARNING: no neighbors available ???")
             return None  # unexpected end => appendix
 
-        logger.debug("-- NODE %s has %s neighbors", start_edge.n2, len(nbrs))
-        logger.debug("-- startangle is %s", start_edge.startangle)
-
         if len(nbrs) == 1:
             logger.debug("end of next_edge_lefthand_side: one neighbor")
             return nbrs[0]
 
+        logger.debug("-- NODE %s has %s neighbors", start_edge.n2, len(nbrs))
+        logger.debug("-- startangle is %s", start_edge.startangle)
+
         all_nbrs = []
         logger.debug("candidates are:") 
         for i, nbr in enumerate(nbrs):
-            nbr.set_direction_angle(start_edge.startangle)
+            nbr.set_direction_angle(start_edge)
             nbr.log_name("EDG-{}".format(i))
             nbr.log_edge("++++ candidate")
             all_nbrs.append((nbr.angle, i, nbr))
+        logger.debug("--")
         all_nbrs.sort()
 
         a1, i1, nbr1 = all_nbrs[0]  # lefthandside
         nbr1.log_edge("==== first")
         for a2, i2, nbr2 in all_nbrs[1:]:
             nbr2.log_edge("==== next")
             if nbr2.myself_direction_lefthand(start_edge, nbr1, self):
                 nbr1 = nbr2
-                logger.debug("-- is new lefthand neighbor")
-
+                logger.debug("-- %s ist neuer lefthand neighbor", nbr1.name)
+            else:
+                logger.debug("-- %s bleibt lefthand neighbor", nbr1.name)
         nbr1.log_edge(">>>> LEFT")
         logger.debug("end of next_edge_lefthand_side")
         return nbr1
 
     def create_inner_corner_auxiliary_areas(self):
         logger.debug("begin of create_inner_corner_auxiliary_areas")
         if not self.geom.is_inner:
@@ -707,7 +755,31 @@
                 return []
             n2 = info.n2
             nodes.append(n2)
             elements.append(info.element)
 
         logger.debug("end of get_inner_airgap_line #%s", len(nodes))
         return nodes, elements
+
+    def get_element_line(self, start_node, end_node):
+        logger.debug("begin of get_element_line")
+        assert(self.geom.area_list)
+
+        logger.debug("-- get line from %s to %s", start_node, end_node)
+
+        logger.debug("EDGE FOUND: %s - %s", n1, n2)
+        nodes = [n1, n2]
+        info = self.get_edge_info(n1, n2)
+        elements = [info.element]
+
+        while not points_are_close(start_corner, n2):
+            info.set_start_angle()
+            info = self.next_edge_lefthand_side(info)
+            if not info:  # bad
+                return []
+            n2 = info.n2
+            nodes.append(n2)
+            elements.append(info.element)
+
+        logger.debug("end of get_inner_airgap_line #%s", len(nodes))
+        return nodes, elements
+
```

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/concat.py` & `femagtools-1.6.7/src/femagtools/dxfsl/concat.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/conv.py` & `femagtools-1.6.7/src/femagtools/dxfsl/conv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/converter.py` & `femagtools-1.6.7/src/femagtools/dxfsl/converter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/corner.py` & `femagtools-1.6.7/src/femagtools/dxfsl/corner.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/dumprenderer.py` & `femagtools-1.6.7/src/femagtools/dxfsl/dumprenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/dxfparser.py` & `femagtools-1.6.7/src/femagtools/dxfsl/dxfparser.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/femparser.py` & `femagtools-1.6.7/src/femagtools/dxfsl/femparser.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/fslrenderer.py` & `femagtools-1.6.7/src/femagtools/dxfsl/fslrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/functions.py` & `femagtools-1.6.7/src/femagtools/dxfsl/functions.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/geom.py` & `femagtools-1.6.7/src/femagtools/dxfsl/geom.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/journal.py` & `femagtools-1.6.7/src/femagtools/dxfsl/journal.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/machine.py` & `femagtools-1.6.7/src/femagtools/dxfsl/machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/plotrenderer.py` & `femagtools-1.6.7/src/femagtools/dxfsl/plotrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/shape.py` & `femagtools-1.6.7/src/femagtools/dxfsl/shape.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/svgparser.py` & `femagtools-1.6.7/src/femagtools/dxfsl/svgparser.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/dxfsl/symmetry.py` & `femagtools-1.6.7/src/femagtools/dxfsl/symmetry.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/ecloss.py` & `femagtools-1.6.7/src/femagtools/ecloss.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/erg.py` & `femagtools-1.6.7/src/femagtools/erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/femag.py` & `femagtools-1.6.7/src/femagtools/femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/forcedens.py` & `femagtools-1.6.7/src/femagtools/forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/fsl.py` & `femagtools-1.6.7/src/femagtools/fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/getset.py` & `femagtools-1.6.7/src/femagtools/getset.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/gmsh.py` & `femagtools-1.6.7/src/femagtools/gmsh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/google.py` & `femagtools-1.6.7/src/femagtools/google.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/grid.py` & `femagtools-1.6.7/src/femagtools/grid.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/hxy.py` & `femagtools-1.6.7/src/femagtools/hxy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/isa7.py` & `femagtools-1.6.7/src/femagtools/isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/jhb.py` & `femagtools-1.6.7/src/femagtools/jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/job.py` & `femagtools-1.6.7/src/femagtools/job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/losscoeffs.py` & `femagtools-1.6.7/src/femagtools/losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/machine/__init__.py` & `femagtools-1.6.7/src/femagtools/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/machine/afpm.py` & `femagtools-1.6.7/src/femagtools/machine/afpm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/machine/effloss.py` & `femagtools-1.6.7/src/femagtools/machine/effloss.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,14 +194,15 @@
       driving_only: (bool) do not calculate braking speed/torque samples if True
       with_mtpv -- (optional) use mtpv if True (default)
       with_pmconst -- (optional) use pmax if True (default)
       with_mtpa -- (optional) use mtpa if True (default), disables mtpv if False
       with_tmech -- (optional) use friction and windage losses (default)
       num_proc -- (optional) number of parallel processes (default 0)
       progress  -- (optional) custom function for progress logging
+      with_torque_corr -- (optional) T is corrected if out of range (default False)
 
     Returns:
       list of speed, current, voltage, torque, eta and losses
 
     """
     if isinstance(eecpars, dict):
         if isinstance(temp, (list, tuple)):
@@ -216,35 +217,37 @@
         rb = {'T': [], 'n': []}
     else:  # calculate speed,torque characteristics
         nmax = n
         nsamples = npoints[0]
         rb = {}
         r = m.characteristics(T, nmax, u1, nsamples=nsamples,
                               with_mtpv=with_mtpv, with_mtpa=with_mtpa,
-                              with_pmconst=with_pmconst, with_tmech=with_tmech)  # driving mode
+                              with_pmconst=with_pmconst, with_tmech=with_tmech,
+                              **kwargs)  # driving mode
         if driving_only:
             rb['n'] = None
             rb['T'] = None
         elif isinstance(m, (PmRelMachineLdq, SynchronousMachineLdq)):
             if min(m.betarange) >= -np.pi/2:  # driving mode only
                 rb['n'] = None
                 rb['T'] = None
         elif isinstance(m, (PmRelMachinePsidq, SynchronousMachinePsidq)):
             if min(m.iqrange) >= 0:  # driving mode only
                 rb['n'] = None
                 rb['T'] = None
         if 'n' not in rb:
             rb = m.characteristics(-T, max(r['n']), u1, nsamples=nsamples,
                                    with_mtpv=with_mtpv, with_mtpa=with_mtpa,
-                                   with_pmconst=with_pmconst, with_tmech=with_tmech)  # braking mode
-    
+                                   with_pmconst=with_pmconst, with_tmech=with_tmech,
+                                   **kwargs)  # braking mode
+
     if kwargs.get('mesh_func', 0):
         ntmesh = kwargs['mesh_func'](r['n_type'], r['n'], r['T'],
                                     rb['n'], rb['T'], npoints)
-    else: 
+    else:
         ntmesh = _generate_mesh(r['n'], r['T'],
                                 rb['n'], rb['T'], npoints)
 
     logger.info("total speed,torque samples %d", ntmesh.shape[1])
     if isinstance(m, (PmRelMachine, SynchronousMachine)):
         if num_proc > 1:
             iqd = iqd_tmech_umax_multi(num_proc, ntmesh, m, u1, with_mtpa)
```

### Comparing `femagtools-1.6.6/src/femagtools/machine/im.py` & `femagtools-1.6.7/src/femagtools/machine/im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/machine/pm.py` & `femagtools-1.6.7/src/femagtools/machine/pm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/machine/sizing.py` & `femagtools-1.6.7/src/femagtools/machine/sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/machine/sm.py` & `femagtools-1.6.7/src/femagtools/machine/sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/machine/utils.py` & `femagtools-1.6.7/src/femagtools/machine/utils.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/magnet.py` & `femagtools-1.6.7/src/femagtools/magnet.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/mcv.py` & `femagtools-1.6.7/src/femagtools/mcv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/me.py` & `femagtools-1.6.7/src/femagtools/me.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/model.py` & `femagtools-1.6.7/src/femagtools/model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/moo/algorithm.py` & `femagtools-1.6.7/src/femagtools/moo/algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/moo/population.py` & `femagtools-1.6.7/src/femagtools/moo/population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/moo/problem.py` & `femagtools-1.6.7/src/femagtools/moo/problem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/moo/test/AlgorithmTest.py` & `femagtools-1.6.7/src/femagtools/moo/test/AlgorithmTest.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/moo/test/PopulationTest.py` & `femagtools-1.6.7/src/femagtools/moo/test/PopulationTest.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/moproblem.py` & `femagtools-1.6.7/src/femagtools/moproblem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/multiproc.py` & `femagtools-1.6.7/src/femagtools/multiproc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/mxw2msh.py` & `femagtools-1.6.7/src/femagtools/mxw2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/nc.py` & `femagtools-1.6.7/src/femagtools/nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/netlist.py` & `femagtools-1.6.7/src/femagtools/netlist.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/ntib.py` & `femagtools-1.6.7/src/femagtools/ntib.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/opt.py` & `femagtools-1.6.7/src/femagtools/opt.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/parstudy.py` & `femagtools-1.6.7/src/femagtools/parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/__init__.py` & `femagtools-1.6.7/src/femagtools/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/bch.py` & `femagtools-1.6.7/src/femagtools/plot/bch.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/char.py` & `femagtools-1.6.7/src/femagtools/plot/char.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/fieldlines.py` & `femagtools-1.6.7/src/femagtools/plot/fieldlines.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/fluxdens.py` & `femagtools-1.6.7/src/femagtools/plot/fluxdens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/forcedens.py` & `femagtools-1.6.7/src/femagtools/plot/forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/mcv.py` & `femagtools-1.6.7/src/femagtools/plot/mcv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/nc.py` & `femagtools-1.6.7/src/femagtools/plot/nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/phasor.py` & `femagtools-1.6.7/src/femagtools/plot/phasor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/plot/wdg.py` & `femagtools-1.6.7/src/femagtools/plot/wdg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/poc.py` & `femagtools-1.6.7/src/femagtools/poc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/svgfsl/converter.py` & `femagtools-1.6.7/src/femagtools/svgfsl/converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+import sys
+import pathlib
+import argparse
+import logging
+import logging.config
+from femagtools.dxfsl.converter import convert
 
+logger = logging.getLogger(__name__)
 
-if __name__ == '__main__':
-    import pathlib
-    import argparse
-    import logging
-    import logging.config
-    from femagtools.dxfsl.converter import convert
-
-    logger = logging.getLogger(__name__)
+def main():
     argparser = argparse.ArgumentParser(
         description='Process SVG file and create a plot or FSL file.')
     argparser.add_argument('svgfile',
                            help='name of SVG file')
     argparser.add_argument('--rotor',
                            help='rotor without airgap in/out',
                            dest='rotor',
@@ -68,7 +68,10 @@
                   write_id=args.write_id)
 
     if args.write_fsl:
         if res is not None:
             p = pathlib.Path(args.svgfile)
             basename = p.stem
             pathlib.Path(basename + '.fsl').write_text('\n'.join(res['fsl']))
+
+if __name__ == '__main__':
+    main()
```

### Comparing `femagtools-1.6.6/src/femagtools/templates/FE-losses.mako` & `femagtools-1.6.7/src/femagtools/templates/FE-losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/afm_rotor.mako` & `femagtools-1.6.7/src/femagtools/templates/afm_rotor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/afm_stator.mako` & `femagtools-1.6.7/src/femagtools/templates/afm_stator.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/asyn_motor.mako` & `femagtools-1.6.7/src/femagtools/templates/asyn_motor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/basic_modpar.mako` & `femagtools-1.6.7/src/femagtools/templates/basic_modpar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/bertotti.mako` & `femagtools-1.6.7/src/femagtools/templates/bertotti.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/calc_field_ts.mako` & `femagtools-1.6.7/src/femagtools/templates/calc_field_ts.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/calc_therm_field.mako` & `femagtools-1.6.7/src/femagtools/templates/calc_therm_field.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/cogg_calc.mako` & `femagtools-1.6.7/src/femagtools/templates/cogg_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/com_motor_sim.mako` & `femagtools-1.6.7/src/femagtools/templates/com_motor_sim.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/connect_models.mako` & `femagtools-1.6.7/src/femagtools/templates/connect_models.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/cu_losses.mako` & `femagtools-1.6.7/src/femagtools/templates/cu_losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/ec-rotorbar.mako` & `femagtools-1.6.7/src/femagtools/templates/ec-rotorbar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/fe-contr.mako` & `femagtools-1.6.7/src/femagtools/templates/fe-contr.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/fieldcalc.mako` & `femagtools-1.6.7/src/femagtools/templates/fieldcalc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/gen_winding.mako` & `femagtools-1.6.7/src/femagtools/templates/gen_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/inductances.mako` & `femagtools-1.6.7/src/femagtools/templates/inductances.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/ld_lq_fast.mako` & `femagtools-1.6.7/src/femagtools/templates/ld_lq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/leak_dist_wind.mako` & `femagtools-1.6.7/src/femagtools/templates/leak_dist_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/leak_evol_wind.mako` & `femagtools-1.6.7/src/femagtools/templates/leak_evol_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnet-data.mako` & `femagtools-1.6.7/src/femagtools/templates/magnet-data.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetFC2.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetFC2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetIron.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetIron.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetIron2.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetIron2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetIron3.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetIron3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetIron4.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetIron4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetIron5.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetIron5.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetIronV.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetIronV.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetSector.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetSector.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetSectorLinear.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetSectorLinear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetShell.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetShell.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/magnetShell2.mako` & `femagtools-1.6.7/src/femagtools/templates/magnetShell2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/mesh-airgap.mako` & `femagtools-1.6.7/src/femagtools/templates/mesh-airgap.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/modal_analysis.mako` & `femagtools-1.6.7/src/femagtools/templates/modal_analysis.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/modified_steinmetz.mako` & `femagtools-1.6.7/src/femagtools/templates/modified_steinmetz.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/mult_cal_fast.mako` & `femagtools-1.6.7/src/femagtools/templates/mult_cal_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/noloadflux-rot.mako` & `femagtools-1.6.7/src/femagtools/templates/noloadflux-rot.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/noloadflux.mako` & `femagtools-1.6.7/src/femagtools/templates/noloadflux.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/noloadfluxdc.mako` & `femagtools-1.6.7/src/femagtools/templates/noloadfluxdc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/plots.mako` & `femagtools-1.6.7/src/femagtools/templates/plots.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/pm_sym_f_cur.mako` & `femagtools-1.6.7/src/femagtools/templates/pm_sym_f_cur.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/pm_sym_fast.mako` & `femagtools-1.6.7/src/femagtools/templates/pm_sym_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/pm_sym_loss.mako` & `femagtools-1.6.7/src/femagtools/templates/pm_sym_loss.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/psd_psq_fast.mako` & `femagtools-1.6.7/src/femagtools/templates/psd_psq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/ring.mako` & `femagtools-1.6.7/src/femagtools/templates/ring.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/rot_hsm.mako` & `femagtools-1.6.7/src/femagtools/templates/rot_hsm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/rotorAsyn.mako` & `femagtools-1.6.7/src/femagtools/templates/rotorAsyn.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/rotorKs2.mako` & `femagtools-1.6.7/src/femagtools/templates/rotorKs2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/rotor_msh.mako` & `femagtools-1.6.7/src/femagtools/templates/rotor_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/rotor_winding.mako` & `femagtools-1.6.7/src/femagtools/templates/rotor_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/shortcircuit.mako` & `femagtools-1.6.7/src/femagtools/templates/shortcircuit.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/srm.mako` & `femagtools-1.6.7/src/femagtools/templates/srm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/stator1.mako` & `femagtools-1.6.7/src/femagtools/templates/stator1.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/stator2.mako` & `femagtools-1.6.7/src/femagtools/templates/stator2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/stator3Linear.mako` & `femagtools-1.6.7/src/femagtools/templates/stator3Linear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/stator4.mako` & `femagtools-1.6.7/src/femagtools/templates/stator4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/statorBG.mako` & `femagtools-1.6.7/src/femagtools/templates/statorBG.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/statorRing.mako` & `femagtools-1.6.7/src/femagtools/templates/statorRing.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/statorRotor3.mako` & `femagtools-1.6.7/src/femagtools/templates/statorRotor3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/stator_msh.mako` & `femagtools-1.6.7/src/femagtools/templates/stator_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/therm-dynamic.mako` & `femagtools-1.6.7/src/femagtools/templates/therm-dynamic.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/therm-static.mako` & `femagtools-1.6.7/src/femagtools/templates/therm-static.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/templates/torq_calc.mako` & `femagtools-1.6.7/src/femagtools/templates/torq_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/tks.py` & `femagtools-1.6.7/src/femagtools/tks.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/ts.py` & `femagtools-1.6.7/src/femagtools/ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/utils.py` & `femagtools-1.6.7/src/femagtools/utils.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/vbf.py` & `femagtools-1.6.7/src/femagtools/vbf.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/vtu.py` & `femagtools-1.6.7/src/femagtools/vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools/windings.py` & `femagtools-1.6.7/src/femagtools/windings.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/femagtools.egg-info/PKG-INFO` & `femagtools-1.6.7/src/femagtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <dzhang@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.6.6/src/femagtools.egg-info/SOURCES.txt` & `femagtools-1.6.7/src/femagtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/engines/__init__.py` & `femagtools-1.6.7/src/tests/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/engines/test_amazon.py` & `femagtools-1.6.7/src/tests/engines/test_amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/engines/test_config.py` & `femagtools-1.6.7/src/tests/engines/test_config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/geom/__init__.py` & `femagtools-1.6.7/src/tests/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/geom/test_functions.py` & `femagtools-1.6.7/src/tests/geom/test_functions.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/geom/test_point_inside.py` & `femagtools-1.6.7/src/tests/geom/test_point_inside.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/moo/__init__.py` & `femagtools-1.6.7/src/tests/moo/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/moo/test_algorithm.py` & `femagtools-1.6.7/src/tests/moo/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/moo/test_population.py` & `femagtools-1.6.7/src/tests/moo/test_population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_afpm.py` & `femagtools-1.6.7/src/tests/test_afpm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_airgap_induction.py` & `femagtools-1.6.7/src/tests/test_airgap_induction.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_amela.py` & `femagtools-1.6.7/src/tests/test_amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_asm.py` & `femagtools-1.6.7/src/tests/test_asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_bchreader.py` & `femagtools-1.6.7/src/tests/test_bchreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_convert.py` & `femagtools-1.6.7/src/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_effloss.py` & `femagtools-1.6.7/src/tests/test_effloss.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_erg.py` & `femagtools-1.6.7/src/tests/test_erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_femag.py` & `femagtools-1.6.7/src/tests/test_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_forcedens.py` & `femagtools-1.6.7/src/tests/test_forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_fsl.py` & `femagtools-1.6.7/src/tests/test_fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_hxy.py` & `femagtools-1.6.7/src/tests/test_hxy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_im.py` & `femagtools-1.6.7/src/tests/test_im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_isa7.py` & `femagtools-1.6.7/src/tests/test_isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_jhb.py` & `femagtools-1.6.7/src/tests/test_jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_job.py` & `femagtools-1.6.7/src/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_losscoeffs.py` & `femagtools-1.6.7/src/tests/test_losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_machine.py` & `femagtools-1.6.7/src/tests/test_machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_magncurv.py` & `femagtools-1.6.7/src/tests/test_magncurv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_mcvreader.py` & `femagtools-1.6.7/src/tests/test_mcvreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_mcvwriter.py` & `femagtools-1.6.7/src/tests/test_mcvwriter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_model.py` & `femagtools-1.6.7/src/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_nc.py` & `femagtools-1.6.7/src/tests/test_nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_parident.py` & `femagtools-1.6.7/src/tests/test_parident.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_parstudy.py` & `femagtools-1.6.7/src/tests/test_parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_pocfile.py` & `femagtools-1.6.7/src/tests/test_pocfile.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_sizing.py` & `femagtools-1.6.7/src/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_sm.py` & `femagtools-1.6.7/src/tests/test_sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_tksreader.py` & `femagtools-1.6.7/src/tests/test_tksreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_ts.py` & `femagtools-1.6.7/src/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_vbfreader.py` & `femagtools-1.6.7/src/tests/test_vbfreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_vtu.py` & `femagtools-1.6.7/src/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.6/src/tests/test_windings.py` & `femagtools-1.6.7/src/tests/test_windings.py`

 * *Files identical despite different names*

