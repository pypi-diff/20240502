# Comparing `tmp/ressimpy-2.1.0.tar.gz` & `tmp/ressimpy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ressimpy-2.1.0.tar", max compression
+gzip compressed data, was "ressimpy-2.1.1.tar", max compression
```

## Comparing `ressimpy-2.1.0.tar` & `ressimpy-2.1.1.tar`

### file list

```diff
@@ -1,194 +1,197 @@
--rw-r--r--   0        0        0     9156 2024-04-15 14:16:46.310383 ressimpy-2.1.0/LICENSE.MD
--rw-r--r--   0        0        0     5660 2024-04-15 14:16:46.310383 ressimpy-2.1.0/README.md
--rw-r--r--   0        0        0      504 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Aquifer.py
--rw-r--r--   0        0        0    10562 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Completion.py
--rw-r--r--   0        0        0     1620 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Constraint.py
--rw-r--r--   0        0        0     1908 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Constraints.py
--rw-r--r--   0        0        0     4148 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/DataObjectMixin.py
--rw-r--r--   0        0        0     4373 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/DynamicProperty.py
--rw-r--r--   0        0        0      358 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/FluidTypeEnums.py
--rw-r--r--   0        0        0      369 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/FrequencyEnum.py
--rw-r--r--   0        0        0      413 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/GridFunctionTypes.py
--rw-r--r--   0        0        0      168 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/HowEnum.py
--rw-r--r--   0        0        0      214 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/OutputType.py
--rw-r--r--   0        0        0      282 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/PenetrationDirectionEnum.py
--rw-r--r--   0        0        0      253 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/TimeSteppingMethodEnum.py
--rw-r--r--   0        0        0      507 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/UnitsEnum.py
--rw-r--r--   0        0        0      377 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/WellTypeEnum.py
--rw-r--r--   0        0        0       62 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/__init__.py
--rw-r--r--   0        0        0      606 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Equilibration.py
--rw-r--r--   0        0        0     9279 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/File.py
--rw-r--r--   0        0        0     2257 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/FileBase.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/FileOperations/__init__.py
--rw-r--r--   0        0        0    23457 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/FileOperations/file_operations.py
--rw-r--r--   0        0        0      413 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Gaslift.py
--rw-r--r--   0        0        0     4554 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Grid.py
--rw-r--r--   0        0        0     1713 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/GridArrayFunction.py
--rw-r--r--   0        0        0      393 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Grids.py
--rw-r--r--   0        0        0      470 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Hydraulics.py
--rw-r--r--   0        0        0     3785 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/ISODateTime.py
--rw-r--r--   0        0        0     1443 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Network.py
--rw-r--r--   0        0        0      768 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/FcsConfig.py
--rw-r--r--   0        0        0    27814 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/FcsFile.py
--rw-r--r--   0        0        0    21507 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
--rw-r--r--   0        0        0    18204 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
--rw-r--r--   0        0        0     1872 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNode.py
--rw-r--r--   0        0        0     5081 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
--rw-r--r--   0        0        0     6609 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
--rw-r--r--   0        0        0     6806 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
--rw-r--r--   0        0        0     4071 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusProc.py
--rw-r--r--   0        0        0     1286 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
--rw-r--r--   0        0        0     2242 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
--rw-r--r--   0        0        0     6924 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
--rw-r--r--   0        0        0     7148 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
--rw-r--r--   0        0        0     6675 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
--rw-r--r--   0        0        0     2367 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
--rw-r--r--   0        0        0     2936 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
--rw-r--r--   0        0        0     6153 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
--rw-r--r--   0        0        0     4691 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
--rw-r--r--   0        0        0     5980 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
--rw-r--r--   0        0        0      329 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     8894 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
--rw-r--r--   0        0        0    19487 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusCompletion.py
--rw-r--r--   0        0        0    11368 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
--rw-r--r--   0        0        0    33223 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusFile.py
--rw-r--r--   0        0        0     6727 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
--rw-r--r--   0        0        0    13660 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
--rw-r--r--   0        0        0    31918 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
--rw-r--r--   0        0        0     5635 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
--rw-r--r--   0        0        0    20322 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
--rw-r--r--   0        0        0    10027 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRockMethod.py
--rw-r--r--   0        0        0     9709 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
--rw-r--r--   0        0        0    15015 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
--rw-r--r--   0        0        0     6629 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusValveMethod.py
--rw-r--r--   0        0        0    11840 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
--rw-r--r--   0        0        0     8933 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWell.py
--rw-r--r--   0        0        0     1069 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWellList.py
--rw-r--r--   0        0        0     3044 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWellMod.py
--rw-r--r--   0        0        0    40063 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
--rw-r--r--   0        0        0      822 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py
--rw-r--r--   0        0        0       67 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
--rw-r--r--   0        0        0       77 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/__init__.py
--rw-r--r--   0        0        0     3812 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusAquiferMethods.py
--rw-r--r--   0        0        0      381 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
--rw-r--r--   0        0        0      106 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusEnums/__init__.py
--rw-r--r--   0        0        0     3802 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusEquilMethods.py
--rw-r--r--   0        0        0     3761 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusGasliftMethods.py
--rw-r--r--   0        0        0       43 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusGrids.py
--rw-r--r--   0        0        0     3850 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusHydraulicsMethods.py
--rw-r--r--   0        0        0       47 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
--rw-r--r--   0        0        0      757 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
--rw-r--r--   0        0        0     1210 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
--rw-r--r--   0        0        0     1368 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
--rw-r--r--   0        0        0      170 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
--rw-r--r--   0        0        0     1159 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
--rw-r--r--   0        0        0     2658 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
--rw-r--r--   0        0        0      795 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/options_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
--rw-r--r--   0        0        0     5130 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
--rw-r--r--   0        0        0     2547 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
--rw-r--r--   0        0        0     1579 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
--rw-r--r--   0        0        0      896 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
--rw-r--r--   0        0        0     4957 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
--rw-r--r--   0        0        0      880 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
--rw-r--r--   0        0        0     3121 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
--rw-r--r--   0        0        0     4492 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
--rw-r--r--   0        0        0      306 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
--rw-r--r--   0        0        0      243 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/water_keywords.py
--rw-r--r--   0        0        0      902 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
--rw-r--r--   0        0        0    17204 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusNetwork.py
--rw-r--r--   0        0        0     3709 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusPVTMethods.py
--rw-r--r--   0        0        0     3997 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusRelPermMethods.py
--rw-r--r--   0        0        0    12720 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusReporting.py
--rw-r--r--   0        0        0     3763 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusRockMethods.py
--rw-r--r--   0        0        0     4132 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusSeparatorMethods.py
--rw-r--r--   0        0        0    35469 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusSimulator.py
--rw-r--r--   0        0        0    16873 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusSolverParameters.py
--rw-r--r--   0        0        0     3806 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusValveMethods.py
--rw-r--r--   0        0        0     3801 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusWaterMethods.py
--rw-r--r--   0        0        0    23296 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusWells.py
--rw-r--r--   0        0        0      404 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/__init__.py
--rw-r--r--   0        0        0    22968 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/array_function_operations.py
--rw-r--r--   0        0        0      115 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/constants.py
--rw-r--r--   0        0        0    24390 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/load_wells.py
--rw-r--r--   0        0        0    14101 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/logfile_operations.py
--rw-r--r--   0        0        0    16640 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_add_new_object_to_file.py
--rw-r--r--   0        0        0     8573 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_collect_tables.py
--rw-r--r--   0        0        0     7107 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_constraint_operations.py
--rw-r--r--   0        0        0    23162 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_file_operations.py
--rw-r--r--   0        0        0     4132 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_load_well_list.py
--rw-r--r--   0        0        0     2212 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_modify_object_in_file.py
--rw-r--r--   0        0        0     8133 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_remove_object_from_file.py
--rw-r--r--   0        0        0     5422 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/rel_perm_operations.py
--rw-r--r--   0        0        0    18379 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/runcontrol_operations.py
--rw-r--r--   0        0        0    20201 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/structured_grid_operations.py
--rw-r--r--   0        0        0      744 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Node.py
--rw-r--r--   0        0        0      918 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/NodeConnection.py
--rw-r--r--   0        0        0      456 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/NodeConnections.py
--rw-r--r--   0        0        0      398 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nodes.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     3041 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
--rw-r--r--   0        0        0     3090 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/__init__.py
--rw-r--r--   0        0        0      199 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/Enums/__init__.py
--rw-r--r--   0        0        0      640 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/Model_Parts/__init__.py
--rw-r--r--   0        0        0     2892 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
--rw-r--r--   0        0        0    10910 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
--rw-r--r--   0        0        0      462 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimWells.py
--rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/__init__.py
--rw-r--r--   0        0        0     2553 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OperationsMixin.py
--rw-r--r--   0        0        0      442 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/PVT.py
--rw-r--r--   0        0        0      467 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/RelPerm.py
--rw-r--r--   0        0        0     6301 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/RelPermEndPoint.py
--rw-r--r--   0        0        0      573 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Rock.py
--rw-r--r--   0        0        0      594 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Separator.py
--rw-r--r--   0        0        0     4365 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Simulator.py
--rw-r--r--   0        0        0      407 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/SolverParameter.py
--rw-r--r--   0        0        0      671 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/SolverParameters.py
--rw-r--r--   0        0        0     1484 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Target.py
--rw-r--r--   0        0        0      412 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Targets.py
--rw-r--r--   0        0        0     1223 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMapping.py
--rw-r--r--   0        0        0     2249 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
--rw-r--r--   0        0        0     8727 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
--rw-r--r--   0        0        0    17410 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
--rw-r--r--   0        0        0    31056 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
--rw-r--r--   0        0        0    15398 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
--rw-r--r--   0        0        0       96 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/__init__.py
--rw-r--r--   0        0        0    14870 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/Units.py
--rw-r--r--   0        0        0       45 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/__init__.py
--rw-r--r--   0        0        0       95 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Utils/__init__.py
--rw-r--r--   0        0        0     2355 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/factory_methods.py
--rw-r--r--   0        0        0      365 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/general_utilities.py
--rw-r--r--   0        0        0     1315 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/generic_repr.py
--rw-r--r--   0        0        0     1585 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/invert_nexus_map.py
--rw-r--r--   0        0        0      453 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/obj_to_dataframe.py
--rw-r--r--   0        0        0     1364 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/obj_to_table_string.py
--rw-r--r--   0        0        0     2359 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/to_dict_generic.py
--rw-r--r--   0        0        0      477 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Valve.py
--rw-r--r--   0        0        0      479 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Water.py
--rw-r--r--   0        0        0     4790 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Well.py
--rw-r--r--   0        0        0     1411 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/WellConnection.py
--rw-r--r--   0        0        0     1946 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/WellConnections.py
--rw-r--r--   0        0        0     1057 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/WellLists.py
--rw-r--r--   0        0        0      755 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wellbore.py
--rw-r--r--   0        0        0      439 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wellbores.py
--rw-r--r--   0        0        0      809 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wellhead.py
--rw-r--r--   0        0        0      426 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wellheads.py
--rw-r--r--   0        0        0     3244 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wells.py
--rw-r--r--   0        0        0      289 2024-04-15 14:16:57.954518 ressimpy-2.1.0/ResSimpy/__init__.py
--rw-r--r--   0        0        0     2733 2024-04-15 14:16:57.950518 ressimpy-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 ressimpy-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9156 2024-05-02 13:21:26.865630 ressimpy-2.1.1/LICENSE.MD
+-rw-r--r--   0        0        0     5639 2024-05-02 13:21:26.865630 ressimpy-2.1.1/README.md
+-rw-r--r--   0        0        0      504 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Aquifer.py
+-rw-r--r--   0        0        0    10562 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Completion.py
+-rw-r--r--   0        0        0     1620 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Constraint.py
+-rw-r--r--   0        0        0     1908 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Constraints.py
+-rw-r--r--   0        0        0     4148 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/DataObjectMixin.py
+-rw-r--r--   0        0        0     4373 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/DynamicProperty.py
+-rw-r--r--   0        0        0      358 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/FluidTypeEnums.py
+-rw-r--r--   0        0        0      369 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/FrequencyEnum.py
+-rw-r--r--   0        0        0      413 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/GridFunctionTypes.py
+-rw-r--r--   0        0        0      168 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/HowEnum.py
+-rw-r--r--   0        0        0      214 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/OutputType.py
+-rw-r--r--   0        0        0      282 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/PenetrationDirectionEnum.py
+-rw-r--r--   0        0        0      253 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/TimeSteppingMethodEnum.py
+-rw-r--r--   0        0        0      507 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/UnitsEnum.py
+-rw-r--r--   0        0        0      377 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/WellTypeEnum.py
+-rw-r--r--   0        0        0       62 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Equilibration.py
+-rw-r--r--   0        0        0     9284 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/File.py
+-rw-r--r--   0        0        0     2262 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/FileBase.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/FileOperations/__init__.py
+-rw-r--r--   0        0        0    23490 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/FileOperations/file_operations.py
+-rw-r--r--   0        0        0      413 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Gaslift.py
+-rw-r--r--   0        0        0     4634 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Grid.py
+-rw-r--r--   0        0        0     1713 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/GridArrayFunction.py
+-rw-r--r--   0        0        0      393 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Grids.py
+-rw-r--r--   0        0        0      470 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Hydraulics.py
+-rw-r--r--   0        0        0     3785 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/ISODateTime.py
+-rw-r--r--   0        0        0     1443 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Network.py
+-rw-r--r--   0        0        0      780 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/FcsConfig.py
+-rw-r--r--   0        0        0    27814 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/FcsFile.py
+-rw-r--r--   0        0        0    21507 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
+-rw-r--r--   0        0        0    22102 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
+-rw-r--r--   0        0        0     1872 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py
+-rw-r--r--   0        0        0     5081 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
+-rw-r--r--   0        0        0     6617 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
+-rw-r--r--   0        0        0     6806 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
+-rw-r--r--   0        0        0     4085 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusProc.py
+-rw-r--r--   0        0        0     1286 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
+-rw-r--r--   0        0        0     2242 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
+-rw-r--r--   0        0        0     6924 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
+-rw-r--r--   0        0        0     7148 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
+-rw-r--r--   0        0        0     6891 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
+-rw-r--r--   0        0        0     2367 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
+-rw-r--r--   0        0        0     2936 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
+-rw-r--r--   0        0        0     6153 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
+-rw-r--r--   0        0        0     4691 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
+-rw-r--r--   0        0        0     5980 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
+-rw-r--r--   0        0        0      329 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     8894 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
+-rw-r--r--   0        0        0    19527 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusCompletion.py
+-rw-r--r--   0        0        0    11368 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
+-rw-r--r--   0        0        0    33370 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusFile.py
+-rw-r--r--   0        0        0     6727 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
+-rw-r--r--   0        0        0    13660 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
+-rw-r--r--   0        0        0    31926 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
+-rw-r--r--   0        0        0     5635 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
+-rw-r--r--   0        0        0    20322 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
+-rw-r--r--   0        0        0     1515 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusReportingRequests.py
+-rw-r--r--   0        0        0    10027 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py
+-rw-r--r--   0        0        0     9709 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
+-rw-r--r--   0        0        0    15023 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
+-rw-r--r--   0        0        0     6629 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusValveMethod.py
+-rw-r--r--   0        0        0    11840 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
+-rw-r--r--   0        0        0     8945 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWell.py
+-rw-r--r--   0        0        0     1069 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWellList.py
+-rw-r--r--   0        0        0     3044 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWellMod.py
+-rw-r--r--   0        0        0    40449 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
+-rw-r--r--   0        0        0      822 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py
+-rw-r--r--   0        0        0       67 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/__init__.py
+-rw-r--r--   0        0        0     3812 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusAquiferMethods.py
+-rw-r--r--   0        0        0      381 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
+-rw-r--r--   0        0        0      106 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusEnums/__init__.py
+-rw-r--r--   0        0        0     3802 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusEquilMethods.py
+-rw-r--r--   0        0        0     3761 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusGasliftMethods.py
+-rw-r--r--   0        0        0       43 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusGrids.py
+-rw-r--r--   0        0        0     3850 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusHydraulicsMethods.py
+-rw-r--r--   0        0        0       47 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
+-rw-r--r--   0        0        0      757 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
+-rw-r--r--   0        0        0     1210 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
+-rw-r--r--   0        0        0     1368 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
+-rw-r--r--   0        0        0      170 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
+-rw-r--r--   0        0        0     1159 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
+-rw-r--r--   0        0        0     2658 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
+-rw-r--r--   0        0        0      795 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
+-rw-r--r--   0        0        0     5130 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
+-rw-r--r--   0        0        0     2547 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
+-rw-r--r--   0        0        0     1579 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
+-rw-r--r--   0        0        0      896 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
+-rw-r--r--   0        0        0     4957 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
+-rw-r--r--   0        0        0      880 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
+-rw-r--r--   0        0        0     3121 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
+-rw-r--r--   0        0        0     4492 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
+-rw-r--r--   0        0        0      306 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
+-rw-r--r--   0        0        0      243 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/water_keywords.py
+-rw-r--r--   0        0        0      902 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
+-rw-r--r--   0        0        0    17362 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusNetwork.py
+-rw-r--r--   0        0        0     3709 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusPVTMethods.py
+-rw-r--r--   0        0        0     3997 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusRelPermMethods.py
+-rw-r--r--   0        0        0    12606 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusReporting.py
+-rw-r--r--   0        0        0     3763 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusRockMethods.py
+-rw-r--r--   0        0        0     4132 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusSeparatorMethods.py
+-rw-r--r--   0        0        0    38960 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusSimulator.py
+-rw-r--r--   0        0        0    16873 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusSolverParameters.py
+-rw-r--r--   0        0        0     3806 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusValveMethods.py
+-rw-r--r--   0        0        0     3801 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusWaterMethods.py
+-rw-r--r--   0        0        0    23564 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusWells.py
+-rw-r--r--   0        0        0      404 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/__init__.py
+-rw-r--r--   0        0        0    23806 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/array_function_operations.py
+-rw-r--r--   0        0        0      115 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/constants.py
+-rw-r--r--   0        0        0    24390 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/load_wells.py
+-rw-r--r--   0        0        0    14101 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/logfile_operations.py
+-rw-r--r--   0        0        0    16640 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_add_new_object_to_file.py
+-rw-r--r--   0        0        0     8573 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_collect_tables.py
+-rw-r--r--   0        0        0     7135 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_constraint_operations.py
+-rw-r--r--   0        0        0    23328 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_file_operations.py
+-rw-r--r--   0        0        0     4132 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_load_well_list.py
+-rw-r--r--   0        0        0     2212 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_modify_object_in_file.py
+-rw-r--r--   0        0        0     8133 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_remove_object_from_file.py
+-rw-r--r--   0        0        0     5422 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/rel_perm_operations.py
+-rw-r--r--   0        0        0    18503 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/runcontrol_operations.py
+-rw-r--r--   0        0        0    20201 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/structured_grid_operations.py
+-rw-r--r--   0        0        0      744 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Node.py
+-rw-r--r--   0        0        0      918 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/NodeConnection.py
+-rw-r--r--   0        0        0      456 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/NodeConnections.py
+-rw-r--r--   0        0        0      398 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nodes.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     3041 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
+-rw-r--r--   0        0        0     3090 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/__init__.py
+-rw-r--r--   0        0        0      199 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/Enums/__init__.py
+-rw-r--r--   0        0        0      640 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/Model_Parts/__init__.py
+-rw-r--r--   0        0        0     2892 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
+-rw-r--r--   0        0        0    11017 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
+-rw-r--r--   0        0        0      462 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimWells.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/__init__.py
+-rw-r--r--   0        0        0     2561 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OperationsMixin.py
+-rw-r--r--   0        0        0      442 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/PVT.py
+-rw-r--r--   0        0        0      467 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/RelPerm.py
+-rw-r--r--   0        0        0     6301 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/RelPermEndPoint.py
+-rw-r--r--   0        0        0     1624 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Reporting.py
+-rw-r--r--   0        0        0      573 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Rock.py
+-rw-r--r--   0        0        0      594 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Separator.py
+-rw-r--r--   0        0        0     4437 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Simulator.py
+-rw-r--r--   0        0        0      407 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/SolverParameter.py
+-rw-r--r--   0        0        0      671 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/SolverParameters.py
+-rw-r--r--   0        0        0     1484 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Target.py
+-rw-r--r--   0        0        0      412 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Targets.py
+-rw-r--r--   0        0        0     1223 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMapping.py
+-rw-r--r--   0        0        0     2249 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
+-rw-r--r--   0        0        0     8727 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
+-rw-r--r--   0        0        0    17410 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
+-rw-r--r--   0        0        0    31056 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
+-rw-r--r--   0        0        0    15398 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
+-rw-r--r--   0        0        0       96 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/__init__.py
+-rw-r--r--   0        0        0    14870 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/Units.py
+-rw-r--r--   0        0        0       45 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/__init__.py
+-rw-r--r--   0        0        0       95 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/__init__.py
+-rw-r--r--   0        0        0     2355 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/factory_methods.py
+-rw-r--r--   0        0        0      365 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/general_utilities.py
+-rw-r--r--   0        0        0     1315 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/generic_repr.py
+-rw-r--r--   0        0        0     1585 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/invert_nexus_map.py
+-rw-r--r--   0        0        0      453 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/obj_to_dataframe.py
+-rw-r--r--   0        0        0     1364 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/obj_to_table_string.py
+-rw-r--r--   0        0        0     2359 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/to_dict_generic.py
+-rw-r--r--   0        0        0      477 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Valve.py
+-rw-r--r--   0        0        0      479 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Water.py
+-rw-r--r--   0        0        0     4790 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Well.py
+-rw-r--r--   0        0        0     1411 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/WellConnection.py
+-rw-r--r--   0        0        0     1946 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/WellConnections.py
+-rw-r--r--   0        0        0     1057 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/WellLists.py
+-rw-r--r--   0        0        0      755 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wellbore.py
+-rw-r--r--   0        0        0      439 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wellbores.py
+-rw-r--r--   0        0        0      809 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wellhead.py
+-rw-r--r--   0        0        0      426 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wellheads.py
+-rw-r--r--   0        0        0     3244 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wells.py
+-rw-r--r--   0        0        0      482 2024-05-02 13:21:39.969567 ressimpy-2.1.1/ResSimpy/__init__.py
+-rw-r--r--   0        0        0     1530 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/output_request.py
+-rw-r--r--   0        0        0     2690 2024-05-02 13:21:39.965567 ressimpy-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6529 1970-01-01 00:00:00.000000 ressimpy-2.1.1/PKG-INFO
```

### Comparing `ressimpy-2.1.0/LICENSE.MD` & `ressimpy-2.1.1/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/README.md` & `ressimpy-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 code to the project.
 
 ## Getting Started
 The following Python code examples demonstrate how to perform some simple operations on a model using ResSimpy:
 
 ### Step 1: Import the library
 ```python
-from ResSimpy.Nexus.NexusSimulator import NexusSimulator as Simulator
+from ResSimpy import NexusSimulator as Simulator
 ```
 
 ###  Step 2: Initialise the model
 ```python
 nexus_fcs_file = '/path/to/fcsfile.fcs'
 model = Simulator(origin=nexus_fcs_file) # Create the 'Simulator' model object
 ```
```

### Comparing `ressimpy-2.1.0/ResSimpy/Completion.py` & `ressimpy-2.1.1/ResSimpy/Completion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Constraint.py` & `ressimpy-2.1.1/ResSimpy/Constraint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Constraints.py` & `ressimpy-2.1.1/ResSimpy/Constraints.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/DataObjectMixin.py` & `ressimpy-2.1.1/ResSimpy/DataObjectMixin.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/DynamicProperty.py` & `ressimpy-2.1.1/ResSimpy/DynamicProperty.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Equilibration.py` & `ressimpy-2.1.1/ResSimpy/Equilibration.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/File.py` & `ressimpy-2.1.1/ResSimpy/File.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     def get_flat_list_str_file(self) -> list[str]:
         raise NotImplementedError("Implement this in the derived class")
 
     def add_object_locations(self, obj_uuid: UUID, line_indices: list[int]) -> None:
         raise NotImplementedError("Implement this in the derived class")
 
     @staticmethod
-    def insert_comments(additional_content: list[str], comments) -> list[str]:
+    def insert_comments(additional_content: list[str], comments: str) -> list[str]:
         raise NotImplementedError("Implement this in the derived class")
 
     def get_object_locations_for_id(self, obj_id: UUID) -> list[int]:
         raise NotImplementedError("Implement this in the derived class")
 
     def remove_object_from_file_as_list(self, objects_to_remove: list[UUID]) -> None:
         raise NotImplementedError("Implement this in the derived class")
```

### Comparing `ressimpy-2.1.0/ResSimpy/FileBase.py` & `ressimpy-2.1.1/ResSimpy/FileBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     @abstractmethod
     def add_object_locations(self, obj_uuid: UUID, line_indices: list[int]) -> None:
         raise NotImplementedError("Implement this in the derived class")
 
     @staticmethod
     @abstractmethod
-    def insert_comments(additional_content: list[str], comments) -> list[str]:
+    def insert_comments(additional_content: list[str], comments: str) -> list[str]:
         raise NotImplementedError("Implement this in the derived class")
 
     @abstractmethod
     def get_object_locations_for_id(self, obj_id: UUID) -> list[int]:
         raise NotImplementedError("Implement this in the derived class")
 
     @abstractmethod
```

### Comparing `ressimpy-2.1.0/ResSimpy/FileOperations/file_operations.py` & `ressimpy-2.1.1/ResSimpy/FileOperations/file_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,16 @@
 
         # stop adding to the value once we hit an invalid_character
         if value_character in invalid_characters and value != '':
             break
     return character_location, new_search_string, search_string, value
 
 
-def __replace_with_variable_entry(new_line: str, original_line: str, replace_with: GridArrayDefinition, value: str):
+def __replace_with_variable_entry(new_line: str, original_line: str, replace_with: GridArrayDefinition, value: str)\
+        -> tuple[str, str, str]:
     new_value = replace_with.value if replace_with.value is not None else ''
     if replace_with.modifier != 'VALUE':
         new_line = new_line.replace('INCLUDE ', '')
     elif 'INCLUDE' not in original_line:
         new_value = 'INCLUDE ' + replace_with.value if replace_with.value is not None else ''
     # If we are replacing the first value from a mult, remove the space as well
     if replace_with.modifier == 'MULT' and replace_with.value == '':
```

### Comparing `ressimpy-2.1.0/ResSimpy/Grid.py` & `ressimpy-2.1.1/ResSimpy/Grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 import pandas as pd
-from typing import Optional, Sequence
-
+from typing import Optional, Sequence, TYPE_CHECKING
 from ResSimpy.GridArrayFunction import GridArrayFunction
 
+if TYPE_CHECKING:
+    from ResSimpy.File import File
+
 
 @dataclass
 class GridArrayDefinition:
     """Initialises the NexusGrid class.
 
     Args:
         modifier (Optional[str]): the modifier for the grid array property (e.g. CON, MULT, etc.)
@@ -119,15 +121,15 @@
 
     @property
     def kz(self):
         self.load_grid_properties_if_not_loaded()
         return self._kz
 
     @abstractmethod
-    def load_structured_grid_file(self, structure_grid_file, lazy_loading) -> Grid:
+    def load_structured_grid_file(self, structure_grid_file: File, lazy_loading: bool) -> Grid:
         raise NotImplementedError("Implement this in the derived class")
 
     @abstractmethod
     def load_grid_properties_if_not_loaded(self) -> None:
         raise NotImplementedError("Implement this in the derived class")
 
     @abstractmethod
```

### Comparing `ressimpy-2.1.0/ResSimpy/GridArrayFunction.py` & `ressimpy-2.1.1/ResSimpy/GridArrayFunction.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/ISODateTime.py` & `ressimpy-2.1.1/ResSimpy/ISODateTime.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Network.py` & `ressimpy-2.1.1/ResSimpy/Network.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/FcsConfig.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/FcsConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 
 
 @dataclass
 class FcsConfig:
-    def __init__(self, destination, nexus_data_name="data") -> None:
+    def __init__(self, destination: str, nexus_data_name: str = "data") -> None:
         """Initialises the FcsConfig class.
 
         Args:
             destination: The destination directory for the output data.
             nexus_data_name: The name of the data directory in the Nexus model.
         """
         self.output_dir = destination
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/FcsFile.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/FcsFile.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py`

 * *Files 19% similar despite different names*

```diff
@@ -109,15 +109,19 @@
 
         Args:
         ----
             additional_constraints (Optional[dict[str, list[NexusConstraint]]]): additional constraints to add as a list
         """
         if additional_constraints is None:
             return
-        self._constraints.update(additional_constraints)
+        for name, constraints in additional_constraints.items():
+            # this does not guarantee the constraints are ordered by datetime
+            existing_constraints = self._constraints.get(name, [])
+            existing_constraints.extend(constraints)
+            self._constraints[name] = existing_constraints
 
     def find_by_properties(self, object_name: str, constraint_dict: dict[str, None | float | str | int]) -> \
             NexusConstraint:
         """Finds a uniquely matching constraint from a given set of properties in a dictionary of attributes.
 
         Args:
             object_name (str): name of the node to which the constraint is applied (node name/well name)
@@ -165,18 +169,62 @@
             constraint_id = constraint_to_remove.id
         if constraint_id is None:
             raise ValueError(f'No constraint found with {constraint_id=}')
         # find which file and remove from the file as list
         surface_file = self.__find_which_surface_file_from_id(constraint_id)
         surface_file.remove_object_from_file_as_list([constraint_id])
         # remove from memory
+        removed_constraint = None
         for name, list_constraints in self._constraints.items():
             for i, constraint in enumerate(list_constraints):
                 if constraint.id == constraint_id:
-                    list_constraints.pop(i)
+                    removed_constraint = list_constraints.pop(i)
+        # remove the constraints table if there are no more for that date timestamp
+        if removed_constraint is None:
+            raise ValueError(f'No constraint found with {constraint_id=}')
+        date_of_constraint_removed = removed_constraint.date
+        if date_of_constraint_removed is None:
+            return
+        # search the loaded constraints for constraints on the same date as the removed constraint
+        # if there are none then remove the table
+        if not any(z for x, y in self._constraints.items() for z in y if z.date == date_of_constraint_removed):
+            self.__remove_empty_token_table(date_of_constraint_removed, surface_file=surface_file, token='CONSTRAINTS')
+            self.__remove_empty_token_table(date_of_constraint_removed, surface_file=surface_file, token='QMULT',
+                                            remove_header=True)
+        return
+
+    def __remove_empty_token_table(self, date: str, surface_file: NexusFile, token: str = 'CONSTRAINTS',
+                                   remove_header: bool = False) -> None:
+        """Removes a table for a given date if it has no other dates for that constraint."""
+        # TODO promote this to a higher level function
+        keyword_map = {x: y[0] for x, y in NexusConstraint.get_keyword_mapping().items()}
+        file_content = surface_file.get_flat_list_str_file
+        token_line_number = -1
+        end_token_line_number = -1
+        found_date = False
+        for i, line in enumerate(file_content):
+            if nfo.check_token('TIME', line) and \
+                    nfo.get_expected_token_value(token='TIME', token_line=line, file_list=file_content[i:]) == date:
+                found_date = True
+            if found_date and nfo.check_token(token, line):
+                token_line_number = i
+            elif found_date and nfo.check_token('END' + token, line):
+                end_token_line_number = i
+            if token_line_number > 0 and end_token_line_number > 0:
+                break
+        if end_token_line_number > token_line_number:
+            if remove_header:
+                header_index, headers = nfo.get_table_header(file_content[token_line_number:end_token_line_number],
+                                                             keyword_map)
+                header_index = token_line_number + header_index
+            # remove the last one first to avoid index errors
+            surface_file.remove_from_file_as_list(end_token_line_number)
+            if remove_header:
+                surface_file.remove_from_file_as_list(header_index)
+            surface_file.remove_from_file_as_list(token_line_number)
 
     def __find_which_surface_file_from_id(self, constraint_id: UUID) -> NexusFile:
         """Finds the surface file with the object id requested."""
         # TODO: make this generic with the find_which_wellspec_file_from_completion_id.
 
         if self.__model.model_files.surface_files is None:
             raise ValueError(f'No surface file found in fcs file at {self.__model.model_files.location}')
@@ -235,66 +283,84 @@
         date_comparison = -1
         date_index = -1
         new_constraint_index = -1
         id_line_locs = []
         new_table_needed = False
         new_date_needed = False
         new_qmults_table_needed = False
+        correct_for_padding = 0
         # check for need to add qmult table
         qmult_keywords = ['qmult_oil_rate', 'qmult_gas_rate', 'qmult_water_rate']
         # if any of the qmults are defined in the new constraint then add a qmult table
         add_qmults = any(getattr(new_constraint, x, None) for x in qmult_keywords)
-
+        if len(file_as_list) < 2:
+            # pad the file if it is empty or only has one line
+            new_table_needed = True
+            file_as_list.append('\n')
+            # ensure the padding is added to the file through the new_constraint_text at the end of the file.
+            new_constraint_text.append('\n')
+            correct_for_padding = -1
         for index, line in enumerate(file_as_list):
             if nfo.check_token('TIME', line):
                 constraint_date_from_file = nfo.get_expected_token_value('TIME', line, [line])
                 date_comparison = self.__model._sim_controls.compare_dates(constraint_date_from_file, constraint_date)
                 if date_comparison == 0:
                     date_index = index
                     continue
 
                 elif date_comparison > 0 and date_index >= 0:
                     # if a date that is greater than the additional constraint then we have overshot and need to
                     # add in a new table or time card
                     # this is the case where we don't need to write a new time card
                     new_table_needed = True
                     new_constraint_index = index - 1
+
                 elif date_comparison > 0:
                     new_table_needed = True
                     new_date_needed = True
                     new_constraint_index = index
                 else:
                     continue
             if nfo.check_token('ENDCONSTRAINTS', line) and date_comparison == 0:
                 # find the end of a constraint table and add the new constraint
                 new_constraint_index = index
                 constraint_string = new_constraint.to_table_line([])
                 new_constraint_text.append(constraint_string)
                 id_line_locs = [new_constraint_index]
-            elif index == len(file_as_list) - 1 and date_index >= 0 and not nfo.check_token('ENDQMULT', line):
+            elif index == len(file_as_list) - 1 and date_index < 0 and not nfo.check_token('ENDQMULT', line):
                 # if we're on the final line of the file and we haven't yet set a constraint index
                 new_table_needed = True
-                new_constraint_index = index
+                new_constraint_index = index + 1
+                new_date_needed = True
+                if add_qmults:
+                    new_qmults_table_needed = True
+            elif index == len(file_as_list) - 1 and date_index == 0 and not nfo.check_token('ENDQMULT', line):
+                new_table_needed = True
+                new_constraint_index = index + 1
+                new_date_needed = False
                 if add_qmults:
                     new_qmults_table_needed = True
 
             if new_date_needed:
                 # if the date card doesn't exist then add it to the file first
                 new_constraint_text.append(f'TIME {constraint_date}\n')
 
             if new_table_needed:
                 new_constraint_text.append('CONSTRAINTS\n')
                 new_constraint_text.append(new_constraint.to_table_line([]))
                 new_constraint_text.append('ENDCONSTRAINTS\n')
-                id_line_locs = [new_constraint_index + len(new_constraint_text) - 2]
+                new_constraint_text.append('\n')
+                line_id = new_constraint_index + len(new_constraint_text) - 3 + correct_for_padding
+                id_line_locs = [line_id]
 
             if add_qmults and new_qmults_table_needed:
                 new_constraint_text.extend(new_constraint.write_qmult_table())
                 # add id location for the qmult table as well
-                id_line_locs.append(new_constraint_index + len(new_constraint_text) - 2)
+                line_id = new_constraint_index + len(new_constraint_text) - 2 + correct_for_padding
+                id_line_locs.append(line_id)
                 add_qmults = False
             elif add_qmults and nfo.check_token('ENDQMULT', line) and date_comparison == 0:
                 # find the end of the table of qmults that already exist
                 new_qmult_index = index
                 qmult_string = new_constraint.write_qmult_values()
                 new_qmult_object_ids = {new_constraint.id: [new_qmult_index]}
                 file_to_add_to.add_to_file_as_list(additional_content=[qmult_string], index=new_qmult_index,
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNode.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             object.
         """
         new_connections, _ = collect_all_tables_to_objects(surface_file, {self.table_header: NexusNodeConnection},
                                                            start_date=start_date, default_units=default_units)
         cons_list = new_connections.get(self.table_header)
         self._add_to_memory(cons_list)
 
-    def _add_to_memory(self, additional_list: Optional[Sequence[NexusNodeConnection]]):
+    def _add_to_memory(self, additional_list: Optional[Sequence[NexusNodeConnection]]) -> None:
         """Extends the nodes object by a list of nodes provided to it.
 
         Args:
             additional_list (Sequence[NexusNodeConnection]): list of connections to add to the connection list.
         """
         if additional_list is None:
             return
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodes.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusProc.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusProc.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     @property
     def contents_breakdown(self) -> dict[str, int]:
         """Returns the dictionary counts of the proc functions."""
         return self.__contents_breakdown
 
     @contents_breakdown.setter
-    def contents_breakdown(self, value):
+    def contents_breakdown(self, value: dict) -> None:
         # ensures this param is a dict with length equal to the Nexus proc functions
         if (isinstance(value, dict)) and (len(value) == len(self.reset_nexus_proc_function_counts())):
             self.__contents_breakdown = value
         else:
             raise SetError('This parameter is for internal use and should not be set by the user.\n'
                            'This parameter must be a dictionary where the keys are defined according to the 2022\n'
                            'Nexus Keyword Manual page 1013.')
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusProcs.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusProcs.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusTarget.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusTarget.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusTargets.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusTargets.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,19 +75,22 @@
         self.__parent_network.get_load_status()
         return obj_to_dataframe(self._well_connections)
 
     def get_overview(self) -> str:
         raise NotImplementedError('To be implemented')
 
     def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
-        new_well_connections, _ = collect_all_tables_to_objects(surface_file, {'WELLS': NexusWellConnection},
+        new_well_connections, _ = collect_all_tables_to_objects(surface_file, {'WELLS': NexusWellConnection,
+                                                                               'GASWELLS': NexusWellConnection},
                                                                 start_date=start_date,
                                                                 default_units=default_units)
         cons_list = new_well_connections.get('WELLS')
+        gas_cons_list = new_well_connections.get('GASWELLS')
         self._add_to_memory(cons_list)
+        self._add_to_memory(gas_cons_list)
 
     def remove(self, obj_to_remove: dict[str, None | str | float | int] | UUID) -> None:
         """Remove a wellbore from the network based on the properties matching a dictionary or id.
 
         Args:
             obj_to_remove (UUID | dict[str, None | str | float | int]): UUID of the wellbore to remove or a dictionary \
             with sufficient matching parameters to uniquely identify a wellbore
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusCompletion.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusCompletion.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,16 @@
     def depth_to_top_str(self):
         return self.__depth_to_top_str
 
     @property
     def depth_to_bottom_str(self):
         return self.__depth_to_bottom_str
 
-    def to_dict(self, keys_in_keyword_style: bool = False, add_date=True, add_units=False, include_nones=True) -> \
+    def to_dict(self, keys_in_keyword_style: bool = False, add_date: bool = True, add_units: bool = False,
+                include_nones: bool = True) -> \
             dict[str, None | str | int | float]:
 
         attribute_dict = to_dict(self, keys_in_keyword_style, add_date=add_date,
                                  add_units=add_units, include_nones=include_nones)
         parent_attribute_dict = super().to_dict(keys_in_keyword_style=keys_in_keyword_style, add_date=add_date,
                                                 add_units=add_units, include_nones=include_nones)
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusEquilMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusFile.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusFile.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             top_level_file (bool): If set to True, the code assumes this is a 'top level' file rather than an included
             one.
 
         Returns:
             NexusFile: a class instance for NexusFile with knowledge of include files
         """
 
-        def __get_pathlib_path_details(full_file_path: str):
+        def __get_pathlib_path_details(full_file_path: str) -> None | str:
             if full_file_path == "" or full_file_path is None:
                 return None
             pathlib_path = pathlib.Path(full_file_path)
             owner: str = ''
             group: str = ''
             try:
                 owner = pathlib_path.owner()  # type: ignore
@@ -124,15 +124,15 @@
 
             if owner is not None and group is not None:
                 return f"{owner}:{group}"
             elif owner is not None:
                 return owner
             return None
 
-        def __get_datetime_from_os_stat(full_file_path: str):
+        def __get_datetime_from_os_stat(full_file_path: str) -> None | datetime:
             if full_file_path == "" or full_file_path is None:
                 return None
             stat_obj = os.stat(full_file_path)
             timestamp = stat_obj.st_mtime
             if timestamp is None:
                 return None
             return datetime.fromtimestamp(timestamp, tz=timezone.utc)
@@ -260,15 +260,15 @@
 
     @dataclass
     class FileIndex:
         index: int
 
     def iterate_line(self, file_index: Optional[FileIndex] = None, max_depth: Optional[int] = None,
                      parent: Optional[NexusFile] = None, prefix_line: Optional[str] = None,
-                     keep_include_references=False) -> \
+                     keep_include_references: bool = False) -> \
             Generator[str, None, None]:
         """Generator object for iterating over a list of strings with nested NexusFile objects in them.
 
         Yields:
             str: sequential line from the file.
         """
 
@@ -331,15 +331,16 @@
                 if (max_depth is None or depth > 0) and include_file is not None:
                     level_down_max_depth = None if max_depth is None else depth - 1
 
                     if keep_include_references:
                         yield row
 
                     yield from include_file.iterate_line(file_index=file_index, max_depth=level_down_max_depth,
-                                                         parent=parent, prefix_line=prefix_line)
+                                                         parent=parent, prefix_line=prefix_line,
+                                                         keep_include_references=keep_include_references)
 
                     new_entry = (file_index.index, self.id)
                     if new_entry not in parent.line_locations:
                         parent.line_locations.append(new_entry)
                     if suffix_line:
                         file_index.index += 1
                         # Add in space between include location and the rest of the line
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusPVTMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
                         printable_str += f' {subkey} {subvalue}'
                     printable_str += '\n'
                 elif key not in ['EOS_METHOD']:
                     printable_str += f'    {key} {value}\n'
         return printable_str
 
     def __populate_eos_opts_to_tertiary_keys(self, primary_key: str, primary_key_default_val: str, single_line: str,
-                                             line_list: list[str], list_of_secondary_keys: list[str]):
+                                             line_list: list[str], list_of_secondary_keys: list[str]) -> None:
         """Utility function to populate complex EOS options structures, from primary to tertiary keyword level.
         Applies to TRANSITION, TRANS_TEST and PHASEID Nexus EOS options.
 
         Args:
             primary_key (str): primary keyword, e.g., TRANSITION or PHASEID
             primary_key_default_val (str): default secondary keyword, or primary key value, e.g., TEST
             single_line (str): single line as read from input PVT file
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRockMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusSolverParameter.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusSolverParameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     dvmax_vip_impes: float | None = None
     dvmax_vip_all: float | None = None
 
     dsmax_vip_implicit: float | None = None
     dsmax_vip_impes: float | None = None
     dsmax_vip_all: float | None = None
 
-    def _write_out_solver_param_block(self):
+    def _write_out_solver_param_block(self) -> None:
         """Writes out the solver parameter block for an instance of NexusSolverParameter."""
         raise NotImplementedError
 
     @staticmethod
     def dt_keyword_mapping() -> dict[str, tuple[str, type]]:
         """Gets the keyword mapping from simulator keyword to ResSimpy attribute and the type of the object.
         Associated with the DT keywords in Nexus. e.g. of the form "DT MAX 50".
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusValveMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusValveMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWaterMethod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWell.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWell.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from ResSimpy.Nexus.NexusWells import NexusWells
 
 
 @dataclass(kw_only=True)
 class NexusWell(Well):
     """Class for representing a well in Nexus. Consists of a list of completions and a well name."""
     _wellmods: list[NexusWellMod]
-    _parent_wells_instance: NexusWells = field(compare=False)
+    _parent_wells_instance: NexusWells = field(compare=False, repr=False)
 
     def __init__(self, well_name: str, completions: Sequence[NexusCompletion], unit_system: UnitSystem,
                  parent_wells_instance: NexusWells, wellmods: Sequence[NexusWellMod] | None = None,
                  well_type: Optional[WellType] = None) -> None:
         """Initialises the NexusWell class.
 
         Args:
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWellList.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWellList.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWellMod.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWellMod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Nexus grid file class for loading in a structured grid file and extracting the grid properties."""
 from __future__ import annotations
 
 import copy
 import pandas as pd
 from dataclasses import dataclass
-from typing import Optional, TYPE_CHECKING
+from typing import Optional, TYPE_CHECKING, Any
 import warnings
 
+from ResSimpy.File import File
 from ResSimpy.Grid import Grid, GridArrayDefinition
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Nexus.DataModels.StructuredGrid.NexusGridArrayFunction import NexusGridArrayFunction
 from ResSimpy.Nexus.NexusKeywords.structured_grid_keywords import GRID_ARRAY_FORMAT_KEYWORDS
 from ResSimpy.Nexus.structured_grid_operations import StructuredGridOperations
 import ResSimpy.Nexus.nexus_file_operations as nfo
 import ResSimpy.Nexus.array_function_operations as afo
@@ -194,15 +195,15 @@
         self.__api: GridArrayDefinition = GridArrayDefinition()
         self.__tmx: GridArrayDefinition = GridArrayDefinition()
         self.__tmy: GridArrayDefinition = GridArrayDefinition()
         self.__tmz: GridArrayDefinition = GridArrayDefinition()
         self.__multbv: GridArrayDefinition = GridArrayDefinition()
         self.__pv: GridArrayDefinition = GridArrayDefinition()
 
-    def __wrap(self, value):
+    def __wrap(self, value: Any) -> Any:
         if isinstance(value, tuple | list | set | frozenset):
             return type(value)([self.__wrap(v) for v in value])
         else:
             return value
 
     def update_properties_from_dict(self, data: dict[str, int | GridArrayDefinition]) -> None:
         """Allows you to update properties on the class using the provided dict of values.
@@ -405,15 +406,15 @@
                 self._range_x = int(first_value)
                 self._range_y = int(second_value)
                 self._range_z = int(third_value)
 
         self._grid_properties_loaded = True
 
     @classmethod
-    def load_structured_grid_file(cls: type[NexusGrid], structured_grid_file: NexusFile,
+    def load_structured_grid_file(cls: type[NexusGrid], structured_grid_file: File,
                                   lazy_loading: bool = True) -> NexusGrid:
         """Loads in a structured grid file with all grid properties, and the array functions defined with 'FUNCTION'.
         Other grid modifiers are currently not supported.
 
         Args:
         ----
             structured_grid_file (NexusFile): the NexusFile representation of a structured grid file for converting \
@@ -422,14 +423,17 @@
             AttributeError: if no value is found for the structured grid file path
             ValueError: if when loading the grid no values can be found for the NX NY NZ line.
         """
         if structured_grid_file.location is None:
             raise ValueError(f"No file path given or found for structured grid file path. \
                 Instead got {structured_grid_file.location}")
 
+        if not isinstance(structured_grid_file, NexusFile):
+            raise ValueError(f"Cannot load file of type {type(structured_grid_file)}.")
+
         loaded_structured_grid_file = cls(grid_nexus_file=structured_grid_file)
 
         if not lazy_loading:
             loaded_structured_grid_file.load_grid_properties_if_not_loaded()
             loaded_structured_grid_file.load_faults()
             loaded_structured_grid_file.load_array_functions()
 
@@ -480,17 +484,19 @@
 
         # Save the new file contents
         new_file_str = "".join(structured_grid_contents)
         with open(grid_file_path, "w") as text_file:
             text_file.write(new_file_str)
 
     def load_array_functions(self) -> None:
-        if self.__grid_file_contents is None:
+        # for function arrays we need the expanded file contents without includes
+        if self.__grid_nexus_file is None or self.__grid_nexus_file.get_flat_list_str_file is None:
             raise ValueError("Cannot load array functions as grid file cannot not found")
-        self.__array_functions_list = afo.collect_all_function_blocks(self.__grid_file_contents)
+        file_contents = self.__grid_nexus_file.get_flat_list_str_file
+        self.__array_functions_list = afo.collect_all_function_blocks(file_contents)
         self.__grid_array_functions = afo.create_grid_array_function_objects(self.__array_functions_list)
         self.__array_functions_df = afo.summarize_model_functions(self.__array_functions_list)
         self.__array_functions_loaded = True
 
     def get_array_functions_list(self) -> Optional[list[list[str]]]:
         """Returns the grid array functions as a list of function lines."""
         if not self.__array_functions_loaded:
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py` & `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusAquiferMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusAquiferMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusEquilMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusEquilMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusGasliftMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusGasliftMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusHydraulicsMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusHydraulicsMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/equil_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/options_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/proc_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/proc_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/rock_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/separator_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/surface_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/wells_keywords.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/wells_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusNetwork.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusNetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
             raise FileNotFoundError('Could not find any surface files associated with the fcs file provided.')
 
         for surface in self.__model.model_files.surface_files.values():
             nexus_obj_dict, constraints = collect_all_tables_to_objects(
                 surface, {'NODECON': NexusNodeConnection,
                           'NODES': NexusNode,
                           'WELLS': NexusWellConnection,
+                          'GASWELLS': NexusWellConnection,
                           'WELLHEAD': NexusWellhead,
                           'WELLBORE': NexusWellbore,
                           'CONSTRAINTS': NexusConstraint,
                           'CONSTRAINT': NexusConstraint,
                           'QMULT': NexusConstraint,
                           'CONDEFAULTS': None,
                           'TARGET': NexusTarget,
@@ -235,14 +236,15 @@
                           },
                 start_date=self.__model.start_date,
                 default_units=self.__model.default_units,
             )
             self.nodes._add_to_memory(type_check_lists(nexus_obj_dict.get('NODES')))
             self.connections._add_to_memory(type_check_lists(nexus_obj_dict.get('NODECON')))
             self.well_connections._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLS')))
+            self.well_connections._add_to_memory(type_check_lists(nexus_obj_dict.get('GASWELLS')))
             self.wellheads._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLHEAD')))
             self.wellbores._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLBORE')))
             self.constraints._add_to_memory(type_check_dicts(constraints))
             self.targets._add_to_memory(type_check_lists(nexus_obj_dict.get('TARGET')))
             self.welllists._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLLIST')))
 
             add_procs_to_mem = self.__load_procs
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusPVTMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusPVTMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusRelPermMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusRelPermMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusReporting.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusReporting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,97 +1,81 @@
 """Class for handling all Reporting and runcontrol related tasks."""
 from __future__ import annotations
 
 import warnings
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
 import ResSimpy.Nexus.nexus_file_operations as nfo
 import ResSimpy.FileOperations.file_operations as fo
-from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Enums.FrequencyEnum import FrequencyEnum
 from ResSimpy.Enums.OutputType import OutputType
+from ResSimpy.Nexus.DataModels.NexusReportingRequests import NexusOutputRequest, NexusOutputContents
 from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
-from ResSimpy.Units.AttributeMappings.BaseUnitMapping import BaseUnitMapping
+from ResSimpy.Reporting import Reporting
+
 if TYPE_CHECKING:
     from ResSimpy.Nexus.NexusSimulator import NexusSimulator
 
 
 @dataclass(kw_only=True)
-class NexusOutputRequest(DataObjectMixin):
-    """Class for handling output requests in Nexus."""
-    date: str
-    output: str
-    output_type: OutputType
-    output_frequency: FrequencyEnum
-    output_frequency_number: None | float
-
-    def to_table_line(self, headers: list[str]) -> str:
-        """String representation of the single line within an Output request table."""
-        _ = headers
-        result = f'{self.output} {self.output_frequency.name}'
-        if self.output_frequency_number is not None:
-            result += ' ' + str(self.output_frequency_number)
-        result += '\n'
-        return result
-
-    @property
-    def units(self) -> BaseUnitMapping:
-        return BaseUnitMapping(unit_system=None)
-
-    @staticmethod
-    def get_keyword_mapping() -> dict[str, tuple[str, type]]:
-        """No keywords for this class, returns an empty dict."""
-        return {}
-
-
-@dataclass(kw_only=True)
-class NexusOutputContents:
-    """Class for handling the output that Nexus produces."""
-    date: str
-    output_contents: list[str]
-    output_type: OutputType
-    output: str
-
-
-@dataclass(kw_only=True)
-class NexusReporting:
+class NexusReporting(Reporting):
     """Class for handling all Reporting and runcontrol related tasks."""
     __ss_output_requests: list[NexusOutputRequest]
     __array_output_requests: list[NexusOutputRequest]
     __ss_output_contents: list[NexusOutputContents]
     __array_output_contents: list[NexusOutputContents]
+    __load_status: bool = field(default=False, repr=False, compare=False)
 
     table_header = 'OUTPUT'
     table_footer = 'ENDOUTPUT'
 
-    def __init__(self, model: NexusSimulator) -> None:
+    def __init__(self, model: NexusSimulator, assume_loaded: bool = False) -> None:
         """Initialises the NexusReporting class.
 
         Args:
             model (NexusSimulator): The Nexus model to get the reporting information from.
         """
-        self.__model = model
+        super().__init__(model)
+        self.__model: NexusSimulator = model
         self.__add_object_operations = AddObjectOperations(NexusOutputRequest, self.table_header, self.table_footer,
                                                            model)
+        if assume_loaded:
+            self.__load_status = True
+        self.__ss_output_requests = []
+        self.__ss_output_contents = []
+        self.__array_output_requests = []
+        self.__array_output_contents = []
 
     @property
     def ss_output_requests(self) -> list[NexusOutputRequest]:
+        """Gets the spreadsheet and tabulated output requests."""
+        if not self.__load_status:
+            self.load_output_requests()
         return self.__ss_output_requests
 
     @property
-    def array_output_requests(self) -> list[NexusOutputRequest]:
-        return self.__array_output_requests
-
-    @property
     def ss_output_contents(self) -> list[NexusOutputContents]:
+        """Gets the contents requested for spreadsheet and tabulated results."""
+        if not self.__load_status:
+            self.load_output_requests()
         return self.__ss_output_contents
 
     @property
+    def array_output_requests(self) -> list[NexusOutputRequest]:
+        """Gets the array output requests."""
+        if not self.__load_status:
+            self.load_output_requests()
+        return self.__array_output_requests
+
+    @property
     def array_output_contents(self) -> list[NexusOutputContents]:
+        """Gets the contents requested to be output for the arrays."""
+        if not self.__load_status:
+            self.load_output_requests()
         return self.__array_output_contents
 
     def add_map_properties_to_start_of_grid_file(self):
         """Adds 'map' statements to the start of the grid file to ensure standalone outputs all the required \
         properties. Writes out to the same structured grid file path provided.
 
         Raises:
@@ -188,14 +172,15 @@
                                                                     output_type=OutputType.ARRAY)
                 array_output_contents.extend(list_of_output_contents)
 
         self.__ss_output_requests = ss_output_requests
         self.__array_output_requests = array_output_requests
         self.__ss_output_contents = ss_output_contents
         self.__array_output_contents = array_output_contents
+        self.__load_status = True
 
     @staticmethod
     def _get_output_request(table_file_as_list: list[str], date: str, output_type: OutputType) \
             -> list[NexusOutputRequest]:
         """Gets the output objects from the runcontrol file.
 
         Args:
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusRockMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusRockMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusSeparatorMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusSeparatorMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusSimulator.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusSimulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The Nexus Simulator class is the main class for interacting with Nexus models."""
 from __future__ import annotations
 
 import os
 import warnings
-from typing import Any, Union, Optional
+from typing import Any, Union, Optional, Sequence
 
 import resqpy.model as rq
 from datetime import datetime
 import ResSimpy.Nexus.nexus_file_operations as nfo
 import ResSimpy.FileOperations.file_operations as fo
 from ResSimpy.Nexus.DataModels.FcsFile import FcsNexusFile
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
@@ -139,14 +139,85 @@
         printable_str = f'Simulation name: {self.root_name}\n'
         printable_str += super().__repr__()
         printable_str += f'Run units: {str(self.default_units)}\n'
         # add details from the fcsfile
         printable_str += self.model_files.__repr__()
         return printable_str
 
+    @staticmethod
+    def _attr_info_to_tuple(sim_attr: Union[dict, Sequence])\
+            -> tuple[tuple[tuple[str, Union[str, bool, float]], ...], ...]:
+        """Convert the network constraints/wells completions attribute to a tuple of tuples so that it is hashable.
+
+        Args: sim_attr (Union[dict, Sequence]): dict of {well name: [NexusConstraint]} for
+        self.network.constraints.get_all(), list of [NexusWell objects] for self.wells.get_all()
+
+        Returns: Tuple[Tuple[Tuple[str, Union[str, float, bool]], ...], ...]: tuple of tuples
+        """
+        lst_of_tuples = []
+        if isinstance(sim_attr, dict):
+            for wells, nexus_constraint in sim_attr.items():
+                for constraints in nexus_constraint:
+                    network_dict = constraints.to_dict(add_units=False, include_nones=False)
+                    lst_of_tuples.append(tuple(network_dict.items()))
+
+        elif isinstance(sim_attr, list):
+            for nexus_completion in sim_attr:
+                for el in nexus_completion.completions:
+                    well_dict = el.to_dict(add_units=False, include_nones=False)
+                    lst_of_tuples.append(tuple(well_dict.items()))
+
+        return tuple(lst_of_tuples)
+
+    def network_wells_tuple(self) -> tuple:
+        """Returns a tuple of the network constraints and wells completions attributes.
+
+        Returns:
+            tuple: tuple of the network constraints and wells completions attributes
+        """
+        network_attr = self.network.constraints.get_all()
+        wells_attr = self.wells.get_all()
+
+        network_tuple = self._attr_info_to_tuple(network_attr)
+        wells_tuple = self._attr_info_to_tuple(wells_attr)
+        return network_tuple, wells_tuple
+
+    def hash_network_wells(self) -> int:
+        """Hashes the network constraints and wells completions attributes.
+
+        Returns:
+            int: hash value of the network constraints and wells completions attributes
+        """
+        hash_attr_tuple = self.network_wells_tuple()
+        return hash(hash_attr_tuple)
+
+    def wells_and_network_equal(self, other: NexusSimulator) -> bool:
+        """Compares the network constraints and wells completions of two NexusSimulator objects.
+
+        Args:
+            other (NexusSimulator): NexusSimulator object to compare with
+
+        Returns:
+            Union[bool]: Returns True if the network constraints and wells completions are equal, False otherwise.
+
+        Raises:
+            ValueError: if both models have no network constraints or wells completions.
+            TypeError: if the other object is not a NexusSimulator object.
+        """
+        if isinstance(other, NexusSimulator):
+            base_class_tuple = self.network_wells_tuple()
+            other_class_tuple = other.network_wells_tuple()
+            if base_class_tuple == ((), ()) and other_class_tuple == ((), ()):
+                # if base_class_tuple and other_class_tuple both return empty tuple, that means both of them /
+                # have no network constraints or wells completions
+                raise ValueError("Both models have empty network constraints or wells completions. Unable to compare.")
+            return self.network_wells_tuple() == other.network_wells_tuple()
+        raise TypeError(f"Unable to compare {type(self)} with {other}. Ensure that {other} is of type NexusSimulator. "
+                        f"{other} has {type(other)}")
+
     def remove_temp_from_properties(self):
         """Updates model values if the files are moved from a temp directory
         Replaces the first instance of temp/ in the file paths in the nexus simulation file paths.
 
         Raises:
             ValueError: if any of [__structured_grid_file_path, __new_fcs_file_path, __surface_file_path] are None.
         """
@@ -411,15 +482,15 @@
         If the file is a different directory to the origin path location the function will set the origin
         to the new destination.
         """
         self.__destination = path
         if self.__destination is not None and os.path.dirname(self._origin) != os.path.dirname(self.__destination):
             self._origin = self.__destination + "/" + os.path.basename(self.__original_fcs_file_path)
 
-    def __load_fcs_file(self):
+    def __load_fcs_file(self) -> None:
         """Loads in the information from the supplied FCS file into the class instance.
         Loads in the paths for runcontrol, structured grid and the first surface network.
         Loads in the values for dateformat and run units.
         Attempts to load the run_control_file.
         Loads the wellspec and dynamic property files.
         """
         # fcs_content_with_includes is used to scan only the fcs file and files specifically called with the INCLUDE
@@ -577,15 +648,15 @@
                 file.append('\n' + token_line)
 
         new_file_str = "".join(file)
 
         with open(file_path, "w") as text_file:
             text_file.write(new_file_str)
 
-    def update_fcs_file_value(self, token, new_value, add_to_start=False):
+    def update_fcs_file_value(self, token: str, new_value: str, add_to_start: bool = False):
         """Updates a value in the FCS file."""
         self.update_file_value(self.__new_fcs_file_path, token=token, new_value=new_value, add_to_start=add_to_start)
 
     @staticmethod
     def comment_out_file_value(token: str, file_path: str) -> None:
         """Comments out an uncommented line containing the specified token.
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusSolverParameters.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusSolverParameters.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusValveMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusValveMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusWaterMethods.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusWaterMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/NexusWells.py` & `ressimpy-2.1.1/ResSimpy/Nexus/NexusWells.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 class NexusWells(Wells):
     """A class for collecting all NexusWell objects in a NexusSimulator. Handles adding and removing completions
     as well as rescheduling wells. This is usually accessed through the model.wells property.
 
     Arguments:
         model (Simulator): NexusSimulator object that has the instance of wells on.
     """
-    __model: NexusSimulator = field(compare=False)
+    __model: NexusSimulator = field(compare=False, repr=False)
     __date_format: DateFormat = field(repr=False)
     _wells: list[NexusWell] = field(default_factory=list)
 
     def __init__(self, model: NexusSimulator) -> None:
         """Initialises the NexusWells class.
 
         Args:
-            model (NexusSimulator)
+            model (NexusSimulator): The model object that contains this NexusWells instance.
         """
         self.__model = model
         self.__add_object_operations = AddObjectOperations(NexusCompletion, self.table_header, self.table_footer, model)
         super().__init__()
 
     @property
     def model(self) -> NexusSimulator:
@@ -373,14 +373,17 @@
         must first check for whether the well has any remaining completions in the wellspec table.
         """
         nexus_mapping = NexusCompletion.get_keyword_mapping()
         completion_date_found = False
         file_content = wellspec_file.get_flat_list_str_file
         wellspec_index = -1
         header_index = -1
+        if not fo.value_in_file('TIME', file_content):
+            # if we have no completion date in the file then we have effectively found the right TIME
+            completion_date_found = True
         for index, line in enumerate(file_content):
             if fo.check_token('TIME', line) and fo.get_expected_token_value('TIME', line, [line]) == \
                     completion_date:
                 completion_date_found = True
             if completion_date_found and fo.check_token('WELLSPEC', line) and \
                     fo.get_token_value('WELLSPEC', line, [line]) == well_name:
                 # get the index in the list as string
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/array_function_operations.py` & `ressimpy-2.1.1/ResSimpy/Nexus/array_function_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,27 +29,27 @@
         if nfo.check_token('FUNCTION', line):
             function_body = []
             reading_function = True
             analyt_flag = False
             look_for_table_end = False
         if reading_function:
             # remove all comments following the first '!' in a line.
-            if 'ANALYT' in line:
+            if nfo.check_token('ANALYT', line):
                 analyt_flag = True
             modified_line = line.split('!', 1)[0]
             function_body.append(modified_line.strip())
             if analyt_flag:
                 if nfo.check_token('OUTPUT', modified_line) and not nfo.check_token('RANGE', modified_line):
                     function_list.append(function_body)
                     reading_function = False
             else:  # tabular form
                 if nfo.check_token('OUTPUT', modified_line) and not nfo.check_token('RANGE', modified_line):
                     look_for_table_end = True
                     continue
-                if i < len(file_as_list)-1 and look_for_table_end:
+                if i < len(file_as_list) - 1 and look_for_table_end:
                     end_function = False
                     for keyword in STRUCTURED_GRID_KEYWORDS + GRID_ARRAY_KEYWORDS + ['INCLUDE']:
                         if nfo.check_token(keyword, file_as_list[i+1]):
                             end_function = True
                     if end_function:
                         function_list.append(function_body)
                         reading_function = False
@@ -91,25 +91,25 @@
         output_array_list: Union[str, list[str]] = ''
         drange_list: Union[str, list[str]] = ''
         blocks_list: Union[str, list[str], list[int]] = ''
 
         for li, line in enumerate(block):
             modified_line = line.upper()
             words = modified_line.split()
-            if 'BLOCKS' in modified_line:
+            if nfo.check_token('BLOCKS', modified_line):
                 i1 = words[1]
                 i2 = words[2]
                 j1 = words[3]
                 j2 = words[4]
                 k1 = words[5]
                 k2 = words[6]
                 blocks_list = words[1:7]
                 blocks_list = [round(float(i)) for i in blocks_list]
 
-            if 'FUNCTION' in modified_line:
+            if nfo.check_token('FUNCTION', modified_line):
                 if len(words) == 1:
                     continue
                 if len(words) == 2:
                     if words[1] not in GRID_ARRAY_KEYWORDS:
                         warnings.warn(f'Function {b + 1}:  Function table entries will be excluded from summary df.')
                         function_type = 'function table'
                     else:
@@ -119,46 +119,46 @@
                             region_number_list = [round(float(i)) for i in region_number_list]
                         except ValueError:
                             warnings.warn(f'ValueError at function {b + 1}: could not convert string to integer.')
 
                 if len(words) > 2:  # TODO: deal with tabular function option keywords
                     warnings.warn(f'Function {b + 1}:  Function table entries will be excluded from summary df.')
                     function_type = 'function table'
-            if 'ANALYT' in modified_line:
+            if nfo.check_token('ANALYT', modified_line):
                 function_type = words[1]
                 if len(words) > 2:
                     # remove the first 2 words in line, and set the rest to coefficients
                     function_coefficients = words[2:]
                     # convert string coefficient values to numerical, if possible:
                     try:
                         function_coefficients = [float(i) for i in function_coefficients]
                     except ValueError:
                         warnings.warn(f'ValueError at function {b + 1}: could not convert string to float.')
 
-            if 'GRID' in modified_line:
+            if nfo.check_token('GRID', modified_line):
                 grid_name = words[1]
-            if 'RANGE' in modified_line and 'INPUT' in modified_line:
+            if nfo.check_token('RANGE', modified_line) and nfo.check_token('INPUT', modified_line):
                 input_arrays_min_max_list = words[2:]
                 # convert string range_input values to numerical, if possible:
                 try:
                     input_arrays_min_max_list = [float(i) for i in input_arrays_min_max_list]
                 except ValueError:
                     warnings.warn(f'ValueError at function {b + 1}: could not convert string to float.')
-            if 'RANGE' in modified_line and 'OUTPUT' in modified_line:
+            if nfo.check_token('RANGE', modified_line) and nfo.check_token('OUTPUT', modified_line):
                 output_arrays_min_max_list = words[2:]
                 # convert string range_input values to numerical, if possible:
                 try:
                     output_arrays_min_max_list = [float(i) for i in output_arrays_min_max_list]
                 except ValueError:
                     warnings.warn(f'ValueError at function {b + 1}: could not convert string to float.')
-            if 'DRANGE' in modified_line:
+            if nfo.check_token('DRANGE', modified_line):
                 warnings.warn(f'Function {b + 1}: Function table entries will be excluded from summary df.')
                 drange_list = words[1:]
                 function_type = 'function table'
-            if 'OUTPUT' in modified_line and 'RANGE' not in modified_line:
+            if nfo.check_token('OUTPUT', modified_line) and not nfo.check_token('RANGE', modified_line):
                 input_array_list = words[:words.index('OUTPUT')]
                 output_array_list = words[words.index('OUTPUT') + 1:]
         # Create the row that holds function data
         function_row = [b + 1, blocks_list, region_type, region_number_list, function_type,
                         function_coefficients,
                         grid_name, input_arrays_min_max_list, output_arrays_min_max_list, drange_list, input_array_list,
                         output_array_list, i1, i2, j1, j2, k1, k2]
@@ -358,15 +358,15 @@
     function_table_m: Optional[int] = None
     function_table_p_list: Optional[list[float]] = None
 
     output_line_headers: list[str] = []
     for li, line in enumerate(array_function):
         modified_line = line.upper()
         words = modified_line.split()
-        if 'FUNCTION' in modified_line:
+        if nfo.check_token('FUNCTION', modified_line):
             if len(words) == 1:  # When FUNCTION is the only word in the line
                 continue
             if len(words) == 2:  # When FUNCTION reg_type are the only words on the line
                 if words[1] not in GRID_ARRAY_KEYWORDS:
                     function_type_enum = GridFunctionTypeEnum.FUNCTION_TABLE
                     try:
                         function_table_m = int(words[1])
@@ -410,52 +410,58 @@
                     if len(words) > 2:
                         try:
                             function_table_p_list = [float(i) for i in words[2:]]
                         except ValueError:
                             warnings.warn(f'ValueError at function {function_number}: '
                                           'could not convert string to float.')
 
-        if 'BLOCKS' in modified_line:
+        if nfo.check_token('BLOCKS', modified_line):
             block_array = [int(x) for x in words[1:7]]
 
-        if 'GRID' in modified_line:
+        if nfo.check_token('GRID', modified_line):
             grid_indx = words.index('GRID')
             if len(words) > grid_indx+1:
                 grid_name = words[grid_indx+1]
 
-        if 'RANGE' in modified_line and 'INPUT' in modified_line:
+        if nfo.check_token('RANGE', modified_line) and nfo.check_token('INPUT', modified_line):
             split_range_input = modified_line.split('INPUT')[1].split()
-            if len(split_range_input) % 2 == 0:  # Should be an even number of entries
-                try:
-                    # Create pair-wise min-max tuples in a list
-                    input_range_iterator = iter([float(i) for i in split_range_input])
-                    input_range_list = list(zip(input_range_iterator, input_range_iterator))
-                except ValueError:
-                    warnings.warn(f'ValueError at function {function_number}: could not convert string to float.')
-            else:
-                raise ValueError(f'RANGE INPUT for function {function_number} has an odd number of entries.')
+            if len(split_range_input) % 2 == 1:  # Should be an even number of entries
+                # Remove the last entry, which is not a pair
+                dropped_range_input = split_range_input.pop()
+                warnings.warn(f'RANGE INPUT for function {function_number} has an odd number of entries.\n'
+                              f'Ignoring the last value: "{dropped_range_input}" from the range input.\n'
+                              f'In line: "{modified_line}"')
+            try:
+                # Create pair-wise min-max tuples in a list
+                input_range_iterator = iter([float(i) for i in split_range_input])
+                input_range_list = list(zip(input_range_iterator, input_range_iterator))
+            except ValueError:
+                warnings.warn(f'ValueError at function {function_number}: could not convert string to float.')
 
-        if 'RANGE' in modified_line and 'OUTPUT' in modified_line:
+        if nfo.check_token('RANGE', modified_line) and nfo.check_token('OUTPUT', modified_line):
             split_range_output = modified_line.split('OUTPUT')[1].split()
-            if len(split_range_output) % 2 == 0:  # Should be an even number of entries
-                try:
-                    # Create pair-wise min-max tuples in a list
-                    output_range_iterator = iter([float(i) for i in split_range_output])
-                    output_range_list = list(zip(output_range_iterator, output_range_iterator))
-                except ValueError:
-                    warnings.warn(f'ValueError at function {function_number}: could not convert string to float.')
-            else:
-                raise ValueError(f'RANGE OUTPUT for function {function_number} has an odd number of entries.')
+            if len(split_range_output) % 2 == 1:  # Should be an even number of entries
+                # Remove the last entry, which is not a pair
+                dropped_range_output = split_range_output.pop()
+                warnings.warn(f'RANGE OUTPUT for function {function_number} has an odd number of entries.\n'
+                              f'Ignoring the last value "{dropped_range_output}" from range output.\n'
+                              f'In line: "{modified_line}"')
+            try:
+                # Create pair-wise min-max tuples in a list
+                output_range_iterator = iter([float(i) for i in split_range_output])
+                output_range_list = list(zip(output_range_iterator, output_range_iterator))
+            except ValueError:
+                warnings.warn(f'ValueError at function {function_number}: could not convert string to float.')
 
-        if 'DRANGE' in modified_line:
+        if nfo.check_token('DRANGE', modified_line):
             warnings.warn(f'Function {function_number}: Function table entries will be excluded from summary df.')
             drange_list = [float(x) for x in words[1:]]
             function_type_enum = GridFunctionTypeEnum.FUNCTION_TABLE
 
-        if 'ANALYT' in modified_line:
+        if nfo.check_token('ANALYT', modified_line):
             function_type_enum = GridFunctionTypeEnum[words[1]]
             if len(words) > 2:
                 # remove the first 2 words in line, and set the rest to coefficients
                 function_coefficients0 = words[2:]
                 # convert string coefficient values to numerical, if possible:
                 try:
                     function_coefficients = [float(i) for i in function_coefficients0]
@@ -464,15 +470,15 @@
 
         if len(output_line_headers) > 0:
             function_type_enum = GridFunctionTypeEnum.FUNCTION_TABLE
             function_table = nfo.read_table_to_df(array_function[li:], noheader=True)
             function_table.columns = output_line_headers
             output_line_headers = []
 
-        if 'OUTPUT' in modified_line and 'RANGE' not in modified_line:
+        if nfo.check_token('OUTPUT', modified_line) and not nfo.check_token('RANGE', modified_line):
             input_array_list = words[:words.index('OUTPUT')]
             output_array_list = words[words.index('OUTPUT') + 1:]
             output_line_headers = input_array_list + output_array_list
 
     # Create output NexusGridArrayFunction object
     new_grid_array_function = NexusGridArrayFunction(
         region_type=region_type,
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/load_wells.py` & `ressimpy-2.1.1/ResSimpy/Nexus/load_wells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/logfile_operations.py` & `ressimpy-2.1.1/ResSimpy/Nexus/logfile_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/nexus_add_new_object_to_file.py` & `ressimpy-2.1.1/ResSimpy/Nexus/nexus_add_new_object_to_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/nexus_collect_tables.py` & `ressimpy-2.1.1/ResSimpy/Nexus/nexus_collect_tables.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/nexus_constraint_operations.py` & `ressimpy-2.1.1/ResSimpy/Nexus/nexus_constraint_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                     nexus_file.add_object_locations(new_constraint.id, [index + start_line_index])
             else:
                 new_constraint = constraint(properties_dict)
                 existing_constraints[name_of_node] = [new_constraint]
                 nexus_file.add_object_locations(new_constraint.id, [index + start_line_index])
 
 
-def __clear_constraints(token_value, constraint) -> dict[str, None]:
+def __clear_constraints(token_value: str, constraint: type[NexusConstraint]) -> dict[str, None]:
     """Replicates behaviour of the clear keyword in nexus constraints by creating a dictionary filled with
     Nones for the relevant parameters.
     """
     match token_value:
         case 'CLEAR':
             constraint_clearing_dict = constraint.get_rate_constraints_map()
             constraint_clearing_dict.update(constraint.get_pressure_constraints_map())
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/nexus_file_operations.py` & `ressimpy-2.1.1/ResSimpy/Nexus/nexus_file_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,52 +37,55 @@
     split_line = set(strip_comments[0].split())
 
     return not valid_set.isdisjoint(split_line)
 
 
 def get_previous_value(file_as_list: list[str], search_before: Optional[str] = None,
                        ignore_values: Optional[list[str]] = None) -> Optional[str]:
-    """Gets the previous non blank value in a list of lines. Starts from the last line working backwards.
+    """Gets the previous non-blank value in a list of lines. Starts from the last instance of search_before,
+    working backwards.
 
     Args:
         file_as_list (list[str]): a list of strings containing each line of the file as a new entry,
         ending with the line to start searching from.
         search_before (Optional[str]): The string to start the search from in a backwards direction
         ignore_values (Optional[list[str]], optional): a list of values that should be ignored if found. \
                     Defaults to None.
 
     Returns:
-        Optional[str]: Next non blank value from the list, if none found returns None
+        Optional[str]: Next non-blank value from the list, if none found returns None
     """
 
     # Reverse the order of the lines
     file_as_list.reverse()
 
     # If we are searching before a specific token, remove that and the rest of the line.
     if search_before is not None:
         search_before_location = file_as_list[0].upper().rfind(search_before)
         file_as_list[0] = file_as_list[0][0: search_before_location]
 
     previous_value: str = ''
-
+    first_line = True
     for line in file_as_list:
         string_to_search: str = line
-
         # Retrieve all of the values in the line, then return the last one found if one is found.
         # Otherwise search the next line
         next_value = get_next_value(0, [string_to_search], ignore_values=ignore_values)
 
-        while next_value is not None and search_before != next_value:
+        while next_value is not None and (search_before != next_value or not first_line):
             previous_value = next_value
             string_to_search = string_to_search.replace(next_value, '')
             next_value = get_next_value(0, [string_to_search], ignore_values=ignore_values)
 
         if previous_value != '':
             return previous_value
 
+        # If we are not on the first line, we can search the whole line
+        first_line = False
+
     # Start of file reached, no values found
     return None
 
 
 def create_templated_file(template_location: str, substitutions: dict, output_file_name: str):
     """Creates a new text file at the requested destination substituting the supplied values.
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/nexus_load_well_list.py` & `ressimpy-2.1.1/ResSimpy/Nexus/nexus_load_well_list.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/nexus_modify_object_in_file.py` & `ressimpy-2.1.1/ResSimpy/Nexus/nexus_modify_object_in_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/nexus_remove_object_from_file.py` & `ressimpy-2.1.1/ResSimpy/Nexus/nexus_remove_object_from_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/rel_perm_operations.py` & `ressimpy-2.1.1/ResSimpy/Nexus/rel_perm_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/runcontrol_operations.py` & `ressimpy-2.1.1/ResSimpy/Nexus/runcontrol_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import warnings
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from functools import cmp_to_key
-from typing import Sequence
+from typing import Sequence, TYPE_CHECKING
 
 import pandas as pd
 
 import ResSimpy.Nexus.nexus_file_operations as nfo
 import ResSimpy.FileOperations.file_operations as fo
 from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
+
 from ResSimpy.Nexus.NexusSolverParameters import NexusSolverParameters
 from ResSimpy.Nexus.constants import DATE_WITH_TIME_LENGTH
 from ResSimpy.SolverParameter import SolverParameter
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
 
 
 @dataclass
 class GridToProc:
     """Class for storing the GRIDTOPROC table information from the Options file."""
     grid_to_proc_table: None | pd.DataFrame = None
     auto_distribute: None | str = None
@@ -45,15 +48,15 @@
             return self.grid_to_proc_table['PROCESS'].max()
         else:
             return 0
 
 
 class SimControls:
     """Class for controlling all runcontrol and time related functionality."""
-    def __init__(self, model) -> None:
+    def __init__(self, model: NexusSimulator) -> None:
         """Class for controlling all runcontrol and time related functionality.
 
         Args:
             model: NexusSimulator instance
             __times (None | list[str]): list of times to be included in the runcontrol file
             __date_format_string (str): How the dates should be formatted based on date_format.
             __number_of_processors (int): number of processors to use for the simulation. Comes from Options file in
@@ -67,15 +70,15 @@
         self.__solver_parameters: NexusSolverParameters = NexusSolverParameters(model)
 
     @property
     def date_format_string(self):
         return self.__date_format_string
 
     @date_format_string.setter
-    def date_format_string(self, value):
+    def date_format_string(self, value: str) -> None:
         self.__date_format_string = value
 
     @property
     def times(self):
         return self.__times if self.__times is not None else []
 
     @staticmethod
```

### Comparing `ressimpy-2.1.0/ResSimpy/Nexus/structured_grid_operations.py` & `ressimpy-2.1.1/ResSimpy/Nexus/structured_grid_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Node.py` & `ressimpy-2.1.1/ResSimpy/Node.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/NodeConnection.py` & `ressimpy-2.1.1/ResSimpy/NodeConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py` & `ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py` & `ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py` & `ressimpy-2.1.1/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py` & `ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimSimulator.py` & `ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimSimulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ResSimpy.OpenGoSim.DataModels.OpenGoSimWell import OpenGoSimWell
 from ResSimpy.OpenGoSim.Enums.SimulationTypeEnum import SimulationType
 from ResSimpy.OpenGoSim.Model_Parts.OpenGoSimNetwork import OpenGoSimNetwork
 from ResSimpy.OpenGoSim.OpenGoSimKeywords.OpenGoSimKeywords import OPENGOSIM_KEYWORDS
 from ResSimpy.OpenGoSim.OpenGoSimWells import OpenGoSimWells
 from ResSimpy.PVT import PVT
 from ResSimpy.RelPerm import RelPerm
+from ResSimpy.Reporting import Reporting
 from ResSimpy.Rock import Rock
 from ResSimpy.Separator import Separator
 from ResSimpy.Simulator import Simulator
 from ResSimpy.Valve import Valve
 from ResSimpy.Water import Water
 
 
@@ -60,14 +61,15 @@
         self._aquifer = Aquifer()
         self._hydraulics = Hydraulics()
         self._gaslift = Gaslift()
         self._network = OpenGoSimNetwork()
         self._grid = None
         self._model_files = File(location=origin)
         self._default_units = UnitSystem.UNDEFINED
+        self._reporting = Reporting(self)
         self.__load_model()
 
     @property
     def simulation_type(self) -> SimulationType:
         return self.__simulation_type
 
     @property
@@ -99,38 +101,38 @@
 
                     if token.upper() == 'WELL_DATA':
                         self.__load_in_well_data_block(model_as_list[index:])
 
                     if token.upper() == 'TIME':
                         self.__load_in_time_block(model_as_list[index:])
 
-    def __load_in_time_block(self, remaining_text: list[str]):
+    def __load_in_time_block(self, remaining_text: list[str]) -> None:
         # Load in the TIME block of the model.
         for index, line in enumerate(remaining_text):
             if line_contains_block_ending(line):
                 break
             if fo.check_token('START_DATE', line):
                 self._start_date = fo.load_in_three_part_date(initial_token='START_DATE', token_line=line,
                                                               file_as_list=remaining_text, start_index=index)
 
             if fo.check_token('FINAL_DATE', line):
                 self.__final_date = fo.load_in_three_part_date(initial_token='FINAL_DATE', token_line=line,
                                                                file_as_list=remaining_text, start_index=index)
 
-    def __load_in_simulation_block(self, remaining_text: list[str]):
+    def __load_in_simulation_block(self, remaining_text: list[str]) -> None:
         # Load in the SIMULATION block of the model.
         for line in remaining_text:
             if line_contains_block_ending(line):
                 break
             if fo.check_token('SIMULATION_TYPE', line):
                 value = fo.get_expected_token_value(token='SIMULATION_TYPE', token_line=line, file_list=remaining_text)
                 self.__simulation_type = SimulationType.SUBSURFACE if value.upper() == 'SUBSURFACE' \
                     else SimulationType.GEOMECHANICS_SUBSURFACE
 
-    def __load_in_well_data_block(self, remaining_text: list[str]):
+    def __load_in_well_data_block(self, remaining_text: list[str]) -> None:
         # Load in the WELL_DATA block of the model.
         completions_to_add: list[OpenGoSimCompletion] = []
         unique_completions: list[OpenGoSimCompletion] = []
         well_name: str = fo.get_expected_token_value(token='WELL_DATA',
                                                      token_line=remaining_text[0],
                                                      file_list=remaining_text)
         well_type: WellType | None = None
```

### Comparing `ressimpy-2.1.0/ResSimpy/OperationsMixin.py` & `ressimpy-2.1.1/ResSimpy/OperationsMixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         raise NotImplementedError("Implement this in the derived class")
 
     @abstractmethod
     def load(self, file: File, start_date: str, default_units: UnitSystem) -> None:
         raise NotImplementedError("Implement this in the derived class")
 
     @abstractmethod
-    def _add_to_memory(self, additional_objs: Optional[list[Any]]):
+    def _add_to_memory(self, additional_objs: Optional[list[Any]]) -> None:
         raise NotImplementedError("Implement this in the derived class")
 
     @abstractmethod
     def remove(self, obj_to_remove: UUID | dict[str, None | str | float | int]) -> None:
         raise NotImplementedError("Implement this in the derived class")
 
     @abstractmethod
```

### Comparing `ressimpy-2.1.0/ResSimpy/RelPermEndPoint.py` & `ressimpy-2.1.1/ResSimpy/RelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Rock.py` & `ressimpy-2.1.1/ResSimpy/Rock.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Separator.py` & `ressimpy-2.1.1/ResSimpy/Separator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Simulator.py` & `ressimpy-2.1.1/ResSimpy/Simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ResSimpy.File import File
 from ResSimpy.Gaslift import Gaslift
 from ResSimpy.Grid import Grid
 from ResSimpy.Hydraulics import Hydraulics
 from ResSimpy.Network import Network
 from ResSimpy.PVT import PVT
 from ResSimpy.RelPerm import RelPerm
+from ResSimpy.Reporting import Reporting
 from ResSimpy.Rock import Rock
 from ResSimpy.Separator import Separator
 from ResSimpy.Valve import Valve
 from ResSimpy.Water import Water
 from ResSimpy.Wells import Wells
 
 
@@ -36,14 +37,15 @@
     _aquifer: Aquifer
     _hydraulics: Hydraulics
     _gaslift: Gaslift
     _network: Network
     _grid: None | Grid
     _model_files: File
     _default_units: UnitSystem
+    _reporting: Reporting
 
     def __repr__(self) -> str:
         """Pretty printing Simulator data."""
         printable_str = f'Origin: {self.origin}\n'
         printable_str += f'Full path: {self.model_files.location}\n'
         printable_str += f'Start date: {self.start_date}\n'
         printable_str += f'Date format: {self.get_date_format()}\n'
@@ -53,15 +55,15 @@
     """Class Properties"""
 
     @property
     def start_date(self) -> str:
         return self._start_date
 
     @start_date.setter
-    def start_date(self, value) -> None:
+    def start_date(self, value: str) -> None:
         self._start_date = value
 
     @property
     def wells(self) -> Wells:
         return self._wells
 
     @property
```

### Comparing `ressimpy-2.1.0/ResSimpy/SolverParameters.py` & `ressimpy-2.1.1/ResSimpy/SolverParameters.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Target.py` & `ressimpy-2.1.1/ResSimpy/Target.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Units/AttributeMapping.py` & `ressimpy-2.1.1/ResSimpy/Units/AttributeMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py` & `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py` & `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py` & `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py` & `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py` & `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Units/Units.py` & `ressimpy-2.1.1/ResSimpy/Units/Units.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Utils/factory_methods.py` & `ressimpy-2.1.1/ResSimpy/Utils/factory_methods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Utils/generic_repr.py` & `ressimpy-2.1.1/ResSimpy/Utils/generic_repr.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Utils/invert_nexus_map.py` & `ressimpy-2.1.1/ResSimpy/Utils/invert_nexus_map.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Utils/obj_to_table_string.py` & `ressimpy-2.1.1/ResSimpy/Utils/obj_to_table_string.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Utils/to_dict_generic.py` & `ressimpy-2.1.1/ResSimpy/Utils/to_dict_generic.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Well.py` & `ressimpy-2.1.1/ResSimpy/Well.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/WellConnection.py` & `ressimpy-2.1.1/ResSimpy/WellConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/WellConnections.py` & `ressimpy-2.1.1/ResSimpy/WellConnections.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/WellLists.py` & `ressimpy-2.1.1/ResSimpy/WellLists.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Wellbore.py` & `ressimpy-2.1.1/ResSimpy/Wellbore.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Wellhead.py` & `ressimpy-2.1.1/ResSimpy/Wellhead.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/ResSimpy/Wells.py` & `ressimpy-2.1.1/ResSimpy/Wells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.0/pyproject.toml` & `ressimpy-2.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ResSimpy"
-version = "2.1.0" # Set at build time
+version = "2.1.1" # Set at build time
 description = "A Python library for working with Reservoir Simulator Models."
 authors = ["BP"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["ResSimpy", "Reservoir Engineering"]
 classifiers = [
     "Operating System :: OS Independent",
@@ -61,17 +61,15 @@
 line-length = 120
 # Rule codes for ruff can be found at: https://beta.ruff.rs/docs/rules/
 select = ["E", "F", "W", "C90", "N",  "UP", "YTT", "ANN", "S", "BLE", "D", "PLE", "PLW", "RUF", "BLE", "ARG", "I",
     "COM", "C4", "PIE", "T20", "PYI", "TID", "INT", "ERA", "PD", "FLY", "NPY"] # To add later: PL, PLR
 ignore = ["UP007",  "ANN101", "N999", "UP035", "S105", "N802", "S106", "S107", "UP015", "ANN401", "ANN102", "D202",
     "D105", "D203", "D213", "RUF010", "I001", "B028", "COM812", "PD901",
     # To fix later:
-    "ANN001", # Types
    "ANN201", # Types
-   "ANN202", # Types
     "C901", # Complexity
     "D102", "D100", "D103", "D101", "D205", "D401", "D417", "D104", "D106", # Docstrings
     "FA100", # TODO need to remove references to Union, Optional, capital lettered typing (e.g. List)
              # from typings module.
     ]
 exclude = ["./tests"]
```

### Comparing `ressimpy-2.1.0/PKG-INFO` & `ressimpy-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResSimpy
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python library for working with Reservoir Simulator Models.
 License: Apache-2.0
 Keywords: ResSimpy,Reservoir Engineering
 Author: BP
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -55,15 +55,15 @@
 code to the project.
 
 ## Getting Started
 The following Python code examples demonstrate how to perform some simple operations on a model using ResSimpy:
 
 ### Step 1: Import the library
 ```python
-from ResSimpy.Nexus.NexusSimulator import NexusSimulator as Simulator
+from ResSimpy import NexusSimulator as Simulator
 ```
 
 ###  Step 2: Initialise the model
 ```python
 nexus_fcs_file = '/path/to/fcsfile.fcs'
 model = Simulator(origin=nexus_fcs_file) # Create the 'Simulator' model object
 ```
```

