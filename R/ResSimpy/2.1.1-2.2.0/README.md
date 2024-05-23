# Comparing `tmp/ressimpy-2.1.1.tar.gz` & `tmp/ressimpy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ressimpy-2.1.1.tar", max compression
+gzip compressed data, was "ressimpy-2.2.0.tar", max compression
```

## Comparing `ressimpy-2.1.1.tar` & `ressimpy-2.2.0.tar`

### file list

```diff
@@ -1,197 +1,197 @@
--rw-r--r--   0        0        0     9156 2024-05-02 13:21:26.865630 ressimpy-2.1.1/LICENSE.MD
--rw-r--r--   0        0        0     5639 2024-05-02 13:21:26.865630 ressimpy-2.1.1/README.md
--rw-r--r--   0        0        0      504 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Aquifer.py
--rw-r--r--   0        0        0    10562 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Completion.py
--rw-r--r--   0        0        0     1620 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Constraint.py
--rw-r--r--   0        0        0     1908 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Constraints.py
--rw-r--r--   0        0        0     4148 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/DataObjectMixin.py
--rw-r--r--   0        0        0     4373 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/DynamicProperty.py
--rw-r--r--   0        0        0      358 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/FluidTypeEnums.py
--rw-r--r--   0        0        0      369 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/FrequencyEnum.py
--rw-r--r--   0        0        0      413 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/GridFunctionTypes.py
--rw-r--r--   0        0        0      168 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/HowEnum.py
--rw-r--r--   0        0        0      214 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/OutputType.py
--rw-r--r--   0        0        0      282 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/PenetrationDirectionEnum.py
--rw-r--r--   0        0        0      253 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/TimeSteppingMethodEnum.py
--rw-r--r--   0        0        0      507 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/UnitsEnum.py
--rw-r--r--   0        0        0      377 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/WellTypeEnum.py
--rw-r--r--   0        0        0       62 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Enums/__init__.py
--rw-r--r--   0        0        0      606 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Equilibration.py
--rw-r--r--   0        0        0     9284 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/File.py
--rw-r--r--   0        0        0     2262 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/FileBase.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/FileOperations/__init__.py
--rw-r--r--   0        0        0    23490 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/FileOperations/file_operations.py
--rw-r--r--   0        0        0      413 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Gaslift.py
--rw-r--r--   0        0        0     4634 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Grid.py
--rw-r--r--   0        0        0     1713 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/GridArrayFunction.py
--rw-r--r--   0        0        0      393 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Grids.py
--rw-r--r--   0        0        0      470 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Hydraulics.py
--rw-r--r--   0        0        0     3785 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/ISODateTime.py
--rw-r--r--   0        0        0     1443 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Network.py
--rw-r--r--   0        0        0      780 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/FcsConfig.py
--rw-r--r--   0        0        0    27814 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/FcsFile.py
--rw-r--r--   0        0        0    21507 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
--rw-r--r--   0        0        0    22102 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
--rw-r--r--   0        0        0     1872 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py
--rw-r--r--   0        0        0     5081 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
--rw-r--r--   0        0        0     6617 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
--rw-r--r--   0        0        0     6806 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
--rw-r--r--   0        0        0     4085 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusProc.py
--rw-r--r--   0        0        0     1286 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
--rw-r--r--   0        0        0     2242 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
--rw-r--r--   0        0        0     6924 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
--rw-r--r--   0        0        0     7148 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
--rw-r--r--   0        0        0     6891 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
--rw-r--r--   0        0        0     2367 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
--rw-r--r--   0        0        0     2936 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
--rw-r--r--   0        0        0     6153 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
--rw-r--r--   0        0        0     4691 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
--rw-r--r--   0        0        0     5980 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
--rw-r--r--   0        0        0      329 2024-05-02 13:21:26.865630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     8894 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
--rw-r--r--   0        0        0    19527 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusCompletion.py
--rw-r--r--   0        0        0    11368 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
--rw-r--r--   0        0        0    33370 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusFile.py
--rw-r--r--   0        0        0     6727 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
--rw-r--r--   0        0        0    13660 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
--rw-r--r--   0        0        0    31926 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
--rw-r--r--   0        0        0     5635 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
--rw-r--r--   0        0        0    20322 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
--rw-r--r--   0        0        0     1515 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusReportingRequests.py
--rw-r--r--   0        0        0    10027 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py
--rw-r--r--   0        0        0     9709 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
--rw-r--r--   0        0        0    15023 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
--rw-r--r--   0        0        0     6629 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusValveMethod.py
--rw-r--r--   0        0        0    11840 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
--rw-r--r--   0        0        0     8945 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWell.py
--rw-r--r--   0        0        0     1069 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWellList.py
--rw-r--r--   0        0        0     3044 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWellMod.py
--rw-r--r--   0        0        0    40449 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
--rw-r--r--   0        0        0      822 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py
--rw-r--r--   0        0        0       67 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
--rw-r--r--   0        0        0       77 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/DataModels/__init__.py
--rw-r--r--   0        0        0     3812 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusAquiferMethods.py
--rw-r--r--   0        0        0      381 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
--rw-r--r--   0        0        0      106 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusEnums/__init__.py
--rw-r--r--   0        0        0     3802 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusEquilMethods.py
--rw-r--r--   0        0        0     3761 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusGasliftMethods.py
--rw-r--r--   0        0        0       43 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusGrids.py
--rw-r--r--   0        0        0     3850 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusHydraulicsMethods.py
--rw-r--r--   0        0        0       47 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
--rw-r--r--   0        0        0      757 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
--rw-r--r--   0        0        0     1210 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
--rw-r--r--   0        0        0     1368 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
--rw-r--r--   0        0        0      170 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
--rw-r--r--   0        0        0     1159 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
--rw-r--r--   0        0        0     2658 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
--rw-r--r--   0        0        0      795 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
--rw-r--r--   0        0        0     5130 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
--rw-r--r--   0        0        0     2547 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
--rw-r--r--   0        0        0     1579 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
--rw-r--r--   0        0        0      896 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
--rw-r--r--   0        0        0     4957 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
--rw-r--r--   0        0        0      880 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
--rw-r--r--   0        0        0     3121 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
--rw-r--r--   0        0        0     4492 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
--rw-r--r--   0        0        0      306 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
--rw-r--r--   0        0        0      243 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/water_keywords.py
--rw-r--r--   0        0        0      902 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
--rw-r--r--   0        0        0    17362 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusNetwork.py
--rw-r--r--   0        0        0     3709 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusPVTMethods.py
--rw-r--r--   0        0        0     3997 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusRelPermMethods.py
--rw-r--r--   0        0        0    12606 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusReporting.py
--rw-r--r--   0        0        0     3763 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusRockMethods.py
--rw-r--r--   0        0        0     4132 2024-05-02 13:21:26.869630 ressimpy-2.1.1/ResSimpy/Nexus/NexusSeparatorMethods.py
--rw-r--r--   0        0        0    38960 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusSimulator.py
--rw-r--r--   0        0        0    16873 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusSolverParameters.py
--rw-r--r--   0        0        0     3806 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusValveMethods.py
--rw-r--r--   0        0        0     3801 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusWaterMethods.py
--rw-r--r--   0        0        0    23564 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/NexusWells.py
--rw-r--r--   0        0        0      404 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/__init__.py
--rw-r--r--   0        0        0    23806 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/array_function_operations.py
--rw-r--r--   0        0        0      115 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/constants.py
--rw-r--r--   0        0        0    24390 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/load_wells.py
--rw-r--r--   0        0        0    14101 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/logfile_operations.py
--rw-r--r--   0        0        0    16640 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_add_new_object_to_file.py
--rw-r--r--   0        0        0     8573 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_collect_tables.py
--rw-r--r--   0        0        0     7135 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_constraint_operations.py
--rw-r--r--   0        0        0    23328 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_file_operations.py
--rw-r--r--   0        0        0     4132 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_load_well_list.py
--rw-r--r--   0        0        0     2212 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_modify_object_in_file.py
--rw-r--r--   0        0        0     8133 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/nexus_remove_object_from_file.py
--rw-r--r--   0        0        0     5422 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/rel_perm_operations.py
--rw-r--r--   0        0        0    18503 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/runcontrol_operations.py
--rw-r--r--   0        0        0    20201 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nexus/structured_grid_operations.py
--rw-r--r--   0        0        0      744 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Node.py
--rw-r--r--   0        0        0      918 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/NodeConnection.py
--rw-r--r--   0        0        0      456 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/NodeConnections.py
--rw-r--r--   0        0        0      398 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Nodes.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     3041 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
--rw-r--r--   0        0        0     3090 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/__init__.py
--rw-r--r--   0        0        0      199 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/Enums/__init__.py
--rw-r--r--   0        0        0      640 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/Model_Parts/__init__.py
--rw-r--r--   0        0        0     2892 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
--rw-r--r--   0        0        0    11017 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
--rw-r--r--   0        0        0      462 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimWells.py
--rw-r--r--   0        0        0        0 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OpenGoSim/__init__.py
--rw-r--r--   0        0        0     2561 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/OperationsMixin.py
--rw-r--r--   0        0        0      442 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/PVT.py
--rw-r--r--   0        0        0      467 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/RelPerm.py
--rw-r--r--   0        0        0     6301 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/RelPermEndPoint.py
--rw-r--r--   0        0        0     1624 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Reporting.py
--rw-r--r--   0        0        0      573 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Rock.py
--rw-r--r--   0        0        0      594 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Separator.py
--rw-r--r--   0        0        0     4437 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Simulator.py
--rw-r--r--   0        0        0      407 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/SolverParameter.py
--rw-r--r--   0        0        0      671 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/SolverParameters.py
--rw-r--r--   0        0        0     1484 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Target.py
--rw-r--r--   0        0        0      412 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Targets.py
--rw-r--r--   0        0        0     1223 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMapping.py
--rw-r--r--   0        0        0     2249 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
--rw-r--r--   0        0        0     8727 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
--rw-r--r--   0        0        0    17410 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
--rw-r--r--   0        0        0    31056 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
--rw-r--r--   0        0        0    15398 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
--rw-r--r--   0        0        0       96 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/__init__.py
--rw-r--r--   0        0        0    14870 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/Units.py
--rw-r--r--   0        0        0       45 2024-05-02 13:21:26.873630 ressimpy-2.1.1/ResSimpy/Units/__init__.py
--rw-r--r--   0        0        0       95 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/__init__.py
--rw-r--r--   0        0        0     2355 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/factory_methods.py
--rw-r--r--   0        0        0      365 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/general_utilities.py
--rw-r--r--   0        0        0     1315 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/generic_repr.py
--rw-r--r--   0        0        0     1585 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/invert_nexus_map.py
--rw-r--r--   0        0        0      453 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/obj_to_dataframe.py
--rw-r--r--   0        0        0     1364 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/obj_to_table_string.py
--rw-r--r--   0        0        0     2359 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Utils/to_dict_generic.py
--rw-r--r--   0        0        0      477 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Valve.py
--rw-r--r--   0        0        0      479 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Water.py
--rw-r--r--   0        0        0     4790 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Well.py
--rw-r--r--   0        0        0     1411 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/WellConnection.py
--rw-r--r--   0        0        0     1946 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/WellConnections.py
--rw-r--r--   0        0        0     1057 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/WellLists.py
--rw-r--r--   0        0        0      755 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wellbore.py
--rw-r--r--   0        0        0      439 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wellbores.py
--rw-r--r--   0        0        0      809 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wellhead.py
--rw-r--r--   0        0        0      426 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wellheads.py
--rw-r--r--   0        0        0     3244 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/Wells.py
--rw-r--r--   0        0        0      482 2024-05-02 13:21:39.969567 ressimpy-2.1.1/ResSimpy/__init__.py
--rw-r--r--   0        0        0     1530 2024-05-02 13:21:26.877630 ressimpy-2.1.1/ResSimpy/output_request.py
--rw-r--r--   0        0        0     2690 2024-05-02 13:21:39.965567 ressimpy-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     6529 1970-01-01 00:00:00.000000 ressimpy-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     9156 2024-05-23 09:54:09.552856 ressimpy-2.2.0/LICENSE.MD
+-rw-r--r--   0        0        0     5639 2024-05-23 09:54:09.552856 ressimpy-2.2.0/README.md
+-rw-r--r--   0        0        0      618 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Aquifer.py
+-rw-r--r--   0        0        0    10337 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Completion.py
+-rw-r--r--   0        0        0     1496 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Constraint.py
+-rw-r--r--   0        0        0     1908 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Constraints.py
+-rw-r--r--   0        0        0     6119 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/DataObjectMixin.py
+-rw-r--r--   0        0        0     4620 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/DynamicProperty.py
+-rw-r--r--   0        0        0      358 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/FluidTypeEnums.py
+-rw-r--r--   0        0        0      369 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/FrequencyEnum.py
+-rw-r--r--   0        0        0      413 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/GridFunctionTypes.py
+-rw-r--r--   0        0        0      168 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/HowEnum.py
+-rw-r--r--   0        0        0      214 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/OutputType.py
+-rw-r--r--   0        0        0      282 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/PenetrationDirectionEnum.py
+-rw-r--r--   0        0        0      253 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/TimeSteppingMethodEnum.py
+-rw-r--r--   0        0        0      507 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/UnitsEnum.py
+-rw-r--r--   0        0        0      377 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/WellTypeEnum.py
+-rw-r--r--   0        0        0       62 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Enums/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Equilibration.py
+-rw-r--r--   0        0        0     9413 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/File.py
+-rw-r--r--   0        0        0     2262 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/FileBase.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/FileOperations/__init__.py
+-rw-r--r--   0        0        0    23494 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/FileOperations/file_operations.py
+-rw-r--r--   0        0        0      527 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Gaslift.py
+-rw-r--r--   0        0        0     4872 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Grid.py
+-rw-r--r--   0        0        0     1713 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/GridArrayFunction.py
+-rw-r--r--   0        0        0      393 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Grids.py
+-rw-r--r--   0        0        0      584 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Hydraulics.py
+-rw-r--r--   0        0        0     3954 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/ISODateTime.py
+-rw-r--r--   0        0        0     1443 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Network.py
+-rw-r--r--   0        0        0      780 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/FcsConfig.py
+-rw-r--r--   0        0        0    27826 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/FcsFile.py
+-rw-r--r--   0        0        0    23250 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
+-rw-r--r--   0        0        0    22153 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
+-rw-r--r--   0        0        0     3386 2024-05-23 09:54:09.552856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusNode.py
+-rw-r--r--   0        0        0     6493 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
+-rw-r--r--   0        0        0     6617 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
+-rw-r--r--   0        0        0     6806 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
+-rw-r--r--   0        0        0     4085 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusProc.py
+-rw-r--r--   0        0        0     1286 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
+-rw-r--r--   0        0        0     3742 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
+-rw-r--r--   0        0        0     6914 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
+-rw-r--r--   0        0        0     8652 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
+-rw-r--r--   0        0        0     6891 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
+-rw-r--r--   0        0        0     2367 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
+-rw-r--r--   0        0        0     4496 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
+-rw-r--r--   0        0        0     6153 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
+-rw-r--r--   0        0        0     6251 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
+-rw-r--r--   0        0        0     5980 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
+-rw-r--r--   0        0        0      329 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     8755 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
+-rw-r--r--   0        0        0    20340 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusCompletion.py
+-rw-r--r--   0        0        0    11226 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
+-rw-r--r--   0        0        0    33422 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusFile.py
+-rw-r--r--   0        0        0     6641 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
+-rw-r--r--   0        0        0    14067 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
+-rw-r--r--   0        0        0    31597 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
+-rw-r--r--   0        0        0     5635 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
+-rw-r--r--   0        0        0    20084 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
+-rw-r--r--   0        0        0     2715 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusReportingRequests.py
+-rw-r--r--   0        0        0     9885 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusRockMethod.py
+-rw-r--r--   0        0        0     9571 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
+-rw-r--r--   0        0        0    15023 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
+-rw-r--r--   0        0        0     6523 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusValveMethod.py
+-rw-r--r--   0        0        0    11737 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
+-rw-r--r--   0        0        0     9089 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusWell.py
+-rw-r--r--   0        0        0     1069 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusWellList.py
+-rw-r--r--   0        0        0     3043 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusWellMod.py
+-rw-r--r--   0        0        0    42644 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
+-rw-r--r--   0        0        0      822 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py
+-rw-r--r--   0        0        0       67 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/DataModels/__init__.py
+-rw-r--r--   0        0        0     3820 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusAquiferMethods.py
+-rw-r--r--   0        0        0      381 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
+-rw-r--r--   0        0        0      106 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusEnums/__init__.py
+-rw-r--r--   0        0        0     3810 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusEquilMethods.py
+-rw-r--r--   0        0        0     3769 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusGasliftMethods.py
+-rw-r--r--   0        0        0       43 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusGrids.py
+-rw-r--r--   0        0        0     3858 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusHydraulicsMethods.py
+-rw-r--r--   0        0        0       47 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
+-rw-r--r--   0        0        0      757 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
+-rw-r--r--   0        0        0     1210 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
+-rw-r--r--   0        0        0     1368 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
+-rw-r--r--   0        0        0      170 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
+-rw-r--r--   0        0        0     1159 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
+-rw-r--r--   0        0        0     2658 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
+-rw-r--r--   0        0        0      795 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/options_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
+-rw-r--r--   0        0        0     5130 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
+-rw-r--r--   0        0        0     2547 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
+-rw-r--r--   0        0        0     1579 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
+-rw-r--r--   0        0        0      896 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
+-rw-r--r--   0        0        0     4957 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
+-rw-r--r--   0        0        0      880 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
+-rw-r--r--   0        0        0     3121 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
+-rw-r--r--   0        0        0     4492 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
+-rw-r--r--   0        0        0      306 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
+-rw-r--r--   0        0        0      243 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/water_keywords.py
+-rw-r--r--   0        0        0      902 2024-05-23 09:54:09.556856 ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
+-rw-r--r--   0        0        0    17362 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusNetwork.py
+-rw-r--r--   0        0        0     3717 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusPVTMethods.py
+-rw-r--r--   0        0        0     4005 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusRelPermMethods.py
+-rw-r--r--   0        0        0    12838 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusReporting.py
+-rw-r--r--   0        0        0     3771 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusRockMethods.py
+-rw-r--r--   0        0        0     4140 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusSeparatorMethods.py
+-rw-r--r--   0        0        0    39541 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusSimulator.py
+-rw-r--r--   0        0        0    16873 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusSolverParameters.py
+-rw-r--r--   0        0        0     3814 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusValveMethods.py
+-rw-r--r--   0        0        0     3809 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusWaterMethods.py
+-rw-r--r--   0        0        0    23826 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/NexusWells.py
+-rw-r--r--   0        0        0      404 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/__init__.py
+-rw-r--r--   0        0        0    23806 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/array_function_operations.py
+-rw-r--r--   0        0        0      115 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/constants.py
+-rw-r--r--   0        0        0    24849 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/load_wells.py
+-rw-r--r--   0        0        0    14120 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/logfile_operations.py
+-rw-r--r--   0        0        0    16640 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/nexus_add_new_object_to_file.py
+-rw-r--r--   0        0        0     8720 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/nexus_collect_tables.py
+-rw-r--r--   0        0        0     7294 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/nexus_constraint_operations.py
+-rw-r--r--   0        0        0    23454 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/nexus_file_operations.py
+-rw-r--r--   0        0        0     4192 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/nexus_load_well_list.py
+-rw-r--r--   0        0        0     2323 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/nexus_modify_object_in_file.py
+-rw-r--r--   0        0        0     8133 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/nexus_remove_object_from_file.py
+-rw-r--r--   0        0        0     5422 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/rel_perm_operations.py
+-rw-r--r--   0        0        0    18539 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/runcontrol_operations.py
+-rw-r--r--   0        0        0    20202 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nexus/structured_grid_operations.py
+-rw-r--r--   0        0        0      620 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Node.py
+-rw-r--r--   0        0        0      794 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/NodeConnection.py
+-rw-r--r--   0        0        0      456 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/NodeConnections.py
+-rw-r--r--   0        0        0      398 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Nodes.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     3041 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
+-rw-r--r--   0        0        0     3090 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/DataModels/__init__.py
+-rw-r--r--   0        0        0      199 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/Enums/__init__.py
+-rw-r--r--   0        0        0      640 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/Model_Parts/__init__.py
+-rw-r--r--   0        0        0     2892 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
+-rw-r--r--   0        0        0    11092 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
+-rw-r--r--   0        0        0      462 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/OpenGoSimWells.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OpenGoSim/__init__.py
+-rw-r--r--   0        0        0     2561 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/OperationsMixin.py
+-rw-r--r--   0        0        0      556 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/PVT.py
+-rw-r--r--   0        0        0      581 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/RelPerm.py
+-rw-r--r--   0        0        0     6301 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/RelPermEndPoint.py
+-rw-r--r--   0        0        0     1624 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Reporting.py
+-rw-r--r--   0        0        0      694 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Rock.py
+-rw-r--r--   0        0        0      715 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Separator.py
+-rw-r--r--   0        0        0     4512 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Simulator.py
+-rw-r--r--   0        0        0      407 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/SolverParameter.py
+-rw-r--r--   0        0        0      679 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/SolverParameters.py
+-rw-r--r--   0        0        0     1260 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Target.py
+-rw-r--r--   0        0        0      412 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Targets.py
+-rw-r--r--   0        0        0     1223 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Units/AttributeMapping.py
+-rw-r--r--   0        0        0     2249 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
+-rw-r--r--   0        0        0     8727 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
+-rw-r--r--   0        0        0    17410 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
+-rw-r--r--   0        0        0    31095 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
+-rw-r--r--   0        0        0    15398 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
+-rw-r--r--   0        0        0       96 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/__init__.py
+-rw-r--r--   0        0        0    14870 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Units/Units.py
+-rw-r--r--   0        0        0       45 2024-05-23 09:54:09.560856 ressimpy-2.2.0/ResSimpy/Units/__init__.py
+-rw-r--r--   0        0        0       95 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Utils/__init__.py
+-rw-r--r--   0        0        0     2425 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Utils/factory_methods.py
+-rw-r--r--   0        0        0      365 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Utils/general_utilities.py
+-rw-r--r--   0        0        0     1955 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Utils/generic_repr.py
+-rw-r--r--   0        0        0     1585 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Utils/invert_nexus_map.py
+-rw-r--r--   0        0        0      453 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Utils/obj_to_dataframe.py
+-rw-r--r--   0        0        0     1364 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Utils/obj_to_table_string.py
+-rw-r--r--   0        0        0     2563 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Utils/to_dict_generic.py
+-rw-r--r--   0        0        0      591 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Valve.py
+-rw-r--r--   0        0        0      593 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Water.py
+-rw-r--r--   0        0        0     5023 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Well.py
+-rw-r--r--   0        0        0     1287 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/WellConnection.py
+-rw-r--r--   0        0        0     1946 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/WellConnections.py
+-rw-r--r--   0        0        0     1057 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/WellLists.py
+-rw-r--r--   0        0        0      631 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Wellbore.py
+-rw-r--r--   0        0        0      439 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Wellbores.py
+-rw-r--r--   0        0        0      685 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Wellhead.py
+-rw-r--r--   0        0        0      426 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Wellheads.py
+-rw-r--r--   0        0        0     3244 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/Wells.py
+-rw-r--r--   0        0        0      482 2024-05-23 09:54:21.352912 ressimpy-2.2.0/ResSimpy/__init__.py
+-rw-r--r--   0        0        0     2751 2024-05-23 09:54:09.564856 ressimpy-2.2.0/ResSimpy/output_request.py
+-rw-r--r--   0        0        0     2641 2024-05-23 09:54:21.348912 ressimpy-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6529 1970-01-01 00:00:00.000000 ressimpy-2.2.0/PKG-INFO
```

### Comparing `ressimpy-2.1.1/LICENSE.MD` & `ressimpy-2.2.0/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/README.md` & `ressimpy-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Completion.py` & `ressimpy-2.2.0/ResSimpy/Completion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """The base class for all Well Completions."""
 from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Optional, Sequence
 
 from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.ISODateTime import ISODateTime
 from ResSimpy.Nexus.NexusEnums import DateFormatEnum
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 from ResSimpy.Units.AttributeMappings.CompletionUnitMapping import CompletionUnits
 
 
 @dataclass(kw_only=True, repr=False)
 class Completion(DataObjectMixin, ABC):
     """A class representing well completions.
 
@@ -38,15 +39,14 @@
             'KH' in Nexus.
         dfactor (Optional[float]): non-darcy factor to use for rate dependent skin calculations. 'D' in Nexus
         rel_perm_method (Optional[int]): rel perm method to use for the completion. 'IRELPM' in Nexus
         status (Optional[str]): the status of the layer, can be 'ON' or 'OFF'
         peaceman_well_block_radius (Optional[float]): The pressure equivalent radius of the grid block
     """
 
-    __date: str
     __i: Optional[int] = None
     __j: Optional[int] = None
     __k: Optional[int] = None
     __skin: Optional[float] = None
     __depth: Optional[float] = None
     __well_radius: Optional[float] = None
     __x: Optional[float] = None
@@ -56,17 +56,14 @@
     __grid: Optional[str] = None
     __depth_to_top: Optional[float] = None
     __depth_to_bottom: Optional[float] = None
     __perm_thickness_ovr: Optional[float] = None
     __dfactor: Optional[float] = None
     __rel_perm_method: Optional[int] = None
     __status: Optional[str] = None
-    __iso_date: Optional[ISODateTime] = None
-    _date_format: Optional[DateFormatEnum.DateFormat] = None
-    __start_date: Optional[str] = None
     __unit_system: Optional[UnitSystem] = None
     __peaceman_well_block_radius: Optional[float] = None
 
     def __init__(self, date: str, i: Optional[int] = None, j: Optional[int] = None, k: Optional[int] = None,
                  skin: Optional[float] = None, depth: Optional[float] = None, well_radius: Optional[float] = None,
                  x: Optional[float] = None, y: Optional[float] = None, angle_a: Optional[float] = None,
                  angle_v: Optional[float] = None, grid: Optional[str] = None, depth_to_top: Optional[float] = None,
@@ -98,18 +95,19 @@
             rel_perm_method: Optional[int]: rel perm method to use for the completion.
             status: Optional[str]: the status of the layer, can be 'ON' or 'OFF'
             date_format: Optional[DateFormatEnum.DateFormat]: The date format to use for the date as an enum.
             peaceman_well_block_radius: Optional[float]: The pressure equivalent radius of the grid block
             start_date: Optional[str]: The start date of the simulation.
             unit_system: Optional[UnitSystem]: The unit system to use for the completion.
         """
-        super().__init__({})
-        self._date_format = date_format
+        super().__init__()
         self.__well_radius = well_radius
-        self.__date = date
+        self._date_format = date_format
+        self._start_date = start_date
+        self.date = date
         self.__i = i
         self.__j = j
         self.__k = k
         self.__skin = skin
         self.__depth = depth
         self.__x = x
         self.__y = y
@@ -118,113 +116,96 @@
         self.__grid = grid
         self.__depth_to_top = depth_to_top
         self.__depth_to_bottom = depth_to_bottom
         self.__perm_thickness_ovr = perm_thickness_ovr
         self.__dfactor = dfactor
         self.__rel_perm_method = rel_perm_method
         self.__status = status
-        self.__start_date = start_date
-        self.__iso_date = self.set_iso_date()
         self.__unit_system = unit_system
         self.__peaceman_well_block_radius = peaceman_well_block_radius
 
     @property
-    def well_radius(self):
+    def well_radius(self) -> float | None:
         return self.__well_radius
 
     @property
-    def date(self):
-        return self.__date
-
-    @property
-    def iso_date(self):
-        return self.__iso_date
-
-    @property
-    def i(self):
+    def i(self) -> int | None:
         return self.__i
 
     @property
-    def j(self):
+    def j(self) -> int | None:
         return self.__j
 
     @property
-    def k(self):
+    def k(self) -> int | None:
         return self.__k
 
     @property
-    def skin(self):
+    def skin(self) -> float | None:
         return self.__skin
 
     @property
-    def depth(self):
+    def depth(self) -> float | None:
         return self.__depth
 
     @property
-    def x(self):
+    def x(self) -> float | None:
         return self.__x
 
     @property
-    def y(self):
+    def y(self) -> float | None:
         return self.__y
 
     @property
-    def angle_a(self):
+    def angle_a(self) -> float | None:
         return self.__angle_a
 
     @property
-    def angle_v(self):
+    def angle_v(self) -> float | None:
         return self.__angle_v
 
     @property
-    def grid(self):
+    def grid(self) -> str | None:
         return self.__grid
 
     @property
-    def depth_to_top(self):
+    def depth_to_top(self) -> float | None:
         return self.__depth_to_top
 
     @property
-    def depth_to_bottom(self):
+    def depth_to_bottom(self) -> float | None:
         return self.__depth_to_bottom
 
     @property
-    def perm_thickness_ovr(self):
+    def perm_thickness_ovr(self) -> float | None:
         return self.__perm_thickness_ovr
 
     @property
-    def dfactor(self):
+    def dfactor(self) -> float | None:
         return self.__dfactor
 
     @property
-    def rel_perm_method(self):
+    def rel_perm_method(self) -> int | None:
         return self.__rel_perm_method
 
     @property
-    def status(self):
+    def status(self) -> str | None:
         return self.__status
 
     @property
     def peaceman_well_block_radius(self) -> Optional[float]:
         """The Peaceman Well Block Radius for the completion."""
         return self.__peaceman_well_block_radius
 
     @property
-    def date_format(self):
+    def date_format(self) -> Optional[DateFormat]:
         return self._date_format
 
     @property
-    def start_date(self):
-        return self.__start_date
-
-    def set_iso_date(self) -> ISODateTime:
-        return ISODateTime.convert_to_iso(self.date, self.date_format, self.start_date)
-
-    @property
-    def unit_system(self):
+    def unit_system(self) -> UnitSystem | None:
         return self.__unit_system
 
     @property
     def units(self) -> CompletionUnits:
         return CompletionUnits(self.unit_system)
 
     @property
```

### Comparing `ressimpy-2.1.1/ResSimpy/Constraint.py` & `ressimpy-2.2.0/ResSimpy/Constraint.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
 from ResSimpy.DataObjectMixin import DataObjectMixin
-from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.Units.AttributeMappings.ConstraintUnitMapping import ConstraintUnits
 
 
 @dataclass(repr=False)
 class Constraint(DataObjectMixin, ABC):
     """Base class object for storing data related to well and node constraints."""
     # TODO: Add docstrings for this class
     name: Optional[str] = None
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
     max_surface_oil_rate: Optional[float] = None
     max_surface_gas_rate: Optional[float] = None
     max_surface_water_rate: Optional[float] = None
     max_surface_liquid_rate: Optional[float] = None
     max_reservoir_oil_rate: Optional[float] = None
     max_reservoir_gas_rate: Optional[float] = None
     max_reservoir_water_rate: Optional[float] = None
```

### Comparing `ressimpy-2.1.1/ResSimpy/Constraints.py` & `ressimpy-2.2.0/ResSimpy/Constraints.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/DataObjectMixin.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,99 @@
-"""Base class representing a data object in ResSimpy."""
-import uuid
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
+"""Class representing a single Wellbore in a Nexus Network."""
+from __future__ import annotations
+from dataclasses import dataclass
+from typing import Optional
 
 from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Units.AttributeMappings.BaseUnitMapping import BaseUnitMapping
-from ResSimpy.Utils import to_dict_generic
-from ResSimpy.Utils.generic_repr import generic_repr, generic_str
-from ResSimpy.Utils.obj_to_table_string import to_table_line
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
+from ResSimpy.Wellbore import Wellbore
 
 
-@dataclass()
-class DataObjectMixin(ABC):
-    """Base class representing a data object in ResSimpy."""
-    __id: uuid.UUID = field(default_factory=lambda: uuid.uuid4(), compare=False, repr=False)
-
-    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
-        """Initialises the DataObjectMixin class.
+@dataclass(kw_only=True)
+class NexusWellbore(Wellbore):
+    """Class representing a single Wellbore in a Nexus Network.
+
+    Attributes:
+        date (str): string representation of the last defined date
+        unit_system (UnitSystem): unit system enum
+        name (str): Name of the well. (WELL)
+        flowsect (int): Number of the flow section. (FLOWSECT)
+        diameter (float): Diameter of the well. (DIAM)
+        inner_diameter (float): Inner diameter of the well. (INNERDIAM)
+        roughness (float): Roughness of the well. (ROUGHNESS)
+        bore_type (str): Type of well. (TYPE)
+        hyd_method (str): hydraulic method. (METHOD)
+        temperature (float): Temperature of the well. (TEMP)
+        elevation_profile (str): Elevation profile of the well. (ELEVPR)
+        temperature_profile (str): Temperature profile of the well. (TEMPPR)
+        heat_transfer_coeff (float): Heat transfer coefficient of the well. (HTC)
+        pvt_method (int): Method number used for PVT. (IPVT)
+        water_method (int): Method number used for water. (IWAT).
+    """
+
+    flowsect: Optional[int] = None
+    bore_type: Optional[str] = None
+    hyd_method: Optional[str] = None
+    temperature: Optional[float] = None
+    elevation_profile: Optional[str] = None
+    temperature_profile: Optional[str] = None
+    heat_transfer_coeff: Optional[float] = None
+    pvt_method: Optional[int] = None
+    water_method: Optional[int] = None
+
+    def __init__(self, properties_dict: dict[str, None | int | str | float], date: Optional[str] = None,
+                 date_format: Optional[DateFormat] = None, start_date: Optional[str] = None,
+                 unit_system: Optional[UnitSystem] = None) -> None:
+        """Initialises the NexusWellbore class.
 
         Args:
             properties_dict (dict): dict of the properties to set on the object.
+            date (Optional[str]): The date of the object.
+            date_format (Optional[DateFormat]): The date format that the object uses.
+            start_date (Optional[str]): The start date of the model. Required if the object uses a decimal TIME.
+            unit_system (Optional[UnitSystem]): The unit system of the object e.g. ENGLISH, METRIC.
         """
-        # properties dict is a parameter to make the call signature equivalent to subclasses.
-        self.__id = uuid.uuid4()
-        if properties_dict:
-            raise ValueError('No properties should be passed to the DataObjectMixin')
-
-    def __repr__(self) -> str:
-        return generic_repr(self)
+        # call the init of the DataObjectMixin
+        super().__init__(_date_format=date_format, _start_date=start_date, _unit_system=unit_system)
 
-    def __str__(self) -> str:
-        return generic_str(self)
+        # Set the date related properties, then set the date, automatically setting the ISODate
+        protected_attributes = ['date_format', 'start_date', 'unit_system']
 
-    def to_dict(self, keys_in_keyword_style: bool = False, add_date: bool = True, add_units: bool = True,
-                include_nones: bool = True) -> dict[str, None | str | int | float]:
-        """Returns a dictionary of the attributes of the object.
-
-        Args:
-            keys_in_keyword_style (bool): if True returns the key values as simulator keywords, otherwise returns the \
-                attribute name as stored by ressimpy.
-            add_date (bool): if True adds the date to the dictionary
-            add_units (bool): if True adds the units to the dictionary
-            include_nones (bool): if True includes None values from the object in the dictionary.
-
-        Returns:
-            a dictionary keyed by attributes and values as the value of the attribute
-        """
-        result_dict = to_dict_generic.to_dict(self, keys_in_keyword_style, add_date=add_date, add_units=add_units,
-                                              include_nones=include_nones)
-        return result_dict
-
-    def to_table_line(self, headers: list[str]) -> str:
-        """Takes a generic Nexus object and returns the attribute values as a string in the order of headers provided.
-        Requires an implemented to_dict method and get_keyword_mapping() method.
-
-        Args:
-            headers (list[str]): list of header values in keyword format
-
-        Returns:
-            string of the values in the order of the headers provided.
-
-        """
-        return to_table_line(self, headers)
-
-    @property
-    def id(self) -> uuid.UUID:
-        """Unique identifier for each object."""
-        return self.__id
+        for attribute in protected_attributes:
+            if attribute in properties_dict:
+                self.__setattr__(f"_{attribute}", properties_dict[attribute])
+
+        # Loop through the properties dict if one is provided and set those attributes
+        remaining_properties = [x for x in properties_dict.keys() if x not in protected_attributes]
+        for key in remaining_properties:
+            self.__setattr__(key, properties_dict[key])
+
+        if date is None:
+            if 'date' not in properties_dict or not isinstance(properties_dict['date'], str):
+                raise ValueError(f"No valid Date found for object with properties: {properties_dict}")
+            self.date = properties_dict['date']
+        else:
+            self.date = date
 
     @staticmethod
-    @abstractmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
-        """Gets the mapping of keywords to attribute definitions."""
-        raise NotImplementedError("Implement this in the derived class")
+        """Gets the mapping of nexus keywords to attribute definitions."""
+        nexus_mapping = {
+            'WELL': ('name', str),
+            'FLOWSECT': ('flowsect', int),
+            'DIAM': ('diameter', float),
+            'INNERDIAM': ('inner_diameter', float),
+            'ROUGHNESS': ('roughness', float),
+            'TYPE': ('bore_type', str),
+            'METHOD': ('hyd_method', str),
+            'TEMP': ('temperature', float),
+            'ELEVPR': ('elevation_profile', str),
+            'TEMPPR': ('temperature_profile', str),
+            'HTC': ('heat_transfer_coeff', float),
+            'IPVT': ('pvt_method', int),
+            'IWAT': ('water_method', int)
+        }
 
-    @property
-    @abstractmethod
-    def units(self) -> BaseUnitMapping:
-        """Returns the attribute to unit map for the data object."""
-        raise NotImplementedError("Implement this in the derived class")
+        return nexus_mapping
 
-    def get_unit_for_attribute(self, attribute_name: str, unit_system: UnitSystem, uppercase: bool = False) -> str:
-        """Returns the unit variable for the given unit system.
-
-        Args:
-            attribute_name (str): name of the attribute to get the unit for
-            unit_system (UnitSystem): unit system to get the unit for
-            uppercase (bool): if True returns the unit in uppercase
-        """
-        unit_dimension = self.units.attribute_map.get(attribute_name, None)
-        if unit_dimension is None:
-            raise AttributeError(f'Attribute {attribute_name} not recognised and does not have a unit definition')
-        unit = unit_dimension.unit_system_enum_to_variable(unit_system=unit_system)
-        if uppercase:
-            unit = unit.upper()
-        return unit
+    def __repr__(self) -> str:
+        return super().__repr__()
```

### Comparing `ressimpy-2.1.1/ResSimpy/DynamicProperty.py` & `ressimpy-2.2.0/ResSimpy/DynamicProperty.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Base class for handling any dynamic property simulator inputs, for use in inputs such as PVT, relperm, etc."""
 from __future__ import annotations
-from abc import ABC
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 from typing import Optional
 from ResSimpy.File import File
 from ResSimpy.Units.AttributeMappings.BaseUnitMapping import BaseUnitMapping
@@ -29,14 +29,15 @@
             input_number (int): Method, table or input number, in order as entered in the simulation input deck.
             file (File): The File that the dynamic property is read from.
         """
         self.input_number: int = input_number
         self.file: File = file
 
     @property
+    @abstractmethod
     def units(self) -> BaseUnitMapping:
         """Returns the attribute to unit map for the constraint."""
         raise NotImplementedError('Implement in the derived class.')
 
     def __repr__(self) -> str:
         """Pretty printing dynamic property data."""
         printable_str = f'\nFILE_PATH: {self.file.location}\n\n'
@@ -73,14 +74,17 @@
         for prop, prop_value in self.properties.items():
             existing_range: tuple[float, float] = ranges.get(prop, (np.nan, np.nan))
             if isinstance(prop_value, pd.DataFrame):
                 for col in prop_value.columns:
                     existing_range = ranges.get(col, (np.nan, np.nan))
                     ranges[col] = (np.nanmin((*existing_range, prop_value[col].min())),
                                    np.nanmax((*existing_range, prop_value[col].max())))
+            elif isinstance(prop_value, np.ndarray):
+                ranges[prop] = (np.nanmin((*existing_range, min(prop_value))),
+                                np.nanmax((*existing_range, max(prop_value))))
             elif isinstance(prop_value, str):
                 # try to convert the string to a list of floats
                 split_prop_value = prop_value.split()
                 try:
                     split_prop_value_as_float = [float(val) for val in split_prop_value]
                 except ValueError:
                     # if it can't be converted to a list of floats, then continue to the next property
```

### Comparing `ressimpy-2.1.1/ResSimpy/Equilibration.py` & `ressimpy-2.2.0/ResSimpy/Equilibration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """This module contains the abstract base class for a collection of equilibration inputs."""
 from dataclasses import dataclass
 from abc import ABC
+from typing import Mapping
+
+from ResSimpy.DynamicProperty import DynamicProperty
 
 
 @dataclass(kw_only=True)
 class Equilibration(ABC):
     """The abstract base class for a collection of equilibration inputs.
 
     Attributes:
         inputs (dict[int, DynamicProperty]): Collection of equilibration inputs, as a dictionary.
     """
 
     @property
-    def inputs(self):
+    def inputs(self) -> Mapping[int, DynamicProperty]:
         raise NotImplementedError("Implement this in the derived class")
 
-    def to_string(self):
+    def to_string(self) -> str:
         raise NotImplementedError('Implement this in the derived class.')
```

### Comparing `ressimpy-2.1.1/ResSimpy/File.py` & `ressimpy-2.2.0/ResSimpy/File.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,18 @@
     def __init__(self, location: str,
                  file_content_as_list: Optional[list[str]] = None,
                  include_objects: Optional[Sequence[File]] = None, create_as_modified: bool = False,
                  file_loading_skipped: bool = False) -> None:
         """Initialises the File class.
 
         Args:
+            location (str): The location of the file on disk.
             file_content_as_list (Optional[list[str]]): The file content as a list of strings.
             include_objects (Optional[Sequence[File]]): The files included in the file.
+            create_as_modified (bool): Set the object to modified.
             file_loading_skipped (bool): Whether the file loading was skipped due to the file being too large an array.
         """
         self.location = location
         self._location_in_including_file = location
         self.include_objects: Optional[list[File]] = get_empty_list_file() \
             if include_objects is None else include_objects
         if file_content_as_list is None:
```

### Comparing `ressimpy-2.1.1/ResSimpy/FileBase.py` & `ressimpy-2.2.0/ResSimpy/FileBase.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/FileOperations/file_operations.py` & `ressimpy-2.2.0/ResSimpy/FileOperations/file_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
         token (str): the token being searched for.
         token_line (str): string value of the line that the token was found in.
         file_list (list[str]): a list of strings containing each line of the file as a new entry
         ignore_values (list[str], optional): a list of values that should be ignored if found. \
             Defaults to None.
         replace_with (Union[str, VariableEntry, None], optional):  a value to replace the existing value with. \
             Defaults to None.
-        custom_message Optional[str]: A custom error message if no value is found.
+        custom_message (Optional[str]): A custom error message if no value is found.
 
     Returns:
         str:  The value following the supplied token, if it is present.
 
     Raises:
         ValueError if a value is not found
     """
@@ -436,15 +436,15 @@
         start_line_index (int): line number to start reading file_as_list from
         file_as_list (list[str]): a list of strings containing each line of the file as a new entry
         search_string (str): string to search from within the first indexed line
         ignore_values (Optional[list[str]], optional): a list of values that should be ignored if found. \
             Defaults to None.
         replace_with (Union[str, VariableEntry, None], optional): a value to replace the existing value with. \
             Defaults to None.
-        custom_message Optional[str]: A custom error message if no value is found
+        custom_message (Optional[str]): A custom error message if no value is found
 
     Returns:
         str: Next non blank value from the list, if none found raises ValueError
     """
     value = get_next_value(start_line_index, file_as_list, search_string, ignore_values, replace_with)
 
     if value is None:
```

### Comparing `ressimpy-2.1.1/ResSimpy/Grid.py` & `ressimpy-2.2.0/ResSimpy/Grid.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,22 +14,21 @@
     """Initialises the NexusGrid class.
 
     Args:
         modifier (Optional[str]): the modifier for the grid array property (e.g. CON, MULT, etc.)
         value (Optional[str]): the actual values for the grid array property in question. Can be an include file.
         mods (Optional[dict[str, pd.DataFrame]): if the grid array has an associated mod card we capture it.
         keyword_in_include_file (bool): an indicator to tell you if the grid array keyword was found in an inc file
+        absolute_path (Optional[str]): the absolute path to the path if value is an include file.
     """
     modifier: Optional[str] = None
     value: Optional[str] = None
-    # need a parameter for MOD cards
     mods: Optional[dict[str, pd.DataFrame]] = None
-    # make a boolean to indicate if a keyword is found in an include file
-    # assume initially that it is not
     keyword_in_include_file: bool = False
+    absolute_path: Optional[str] = None
 
 
 @dataclass(kw_only=True)
 class Grid(ABC):
     # Grid dimensions
     _range_x: Optional[int]
     _range_y: Optional[int]
@@ -61,70 +60,70 @@
         # Grid dimensions
         self._range_x: Optional[int] = None
         self._range_y: Optional[int] = None
         self._range_z: Optional[int] = None
         self._grid_properties_loaded = assume_loaded
 
     @property
-    def range_x(self):
+    def range_x(self) -> int | None:
         self.load_grid_properties_if_not_loaded()
         return self._range_x
 
     @property
-    def range_y(self):
+    def range_y(self) -> int | None:
         self.load_grid_properties_if_not_loaded()
         return self._range_y
 
     @property
-    def range_z(self):
+    def range_z(self) -> int | None:
         self.load_grid_properties_if_not_loaded()
         return self._range_z
 
     @property
-    def netgrs(self):
+    def netgrs(self) -> GridArrayDefinition:
         self.load_grid_properties_if_not_loaded()
         return self._netgrs
 
     @property
-    def porosity(self):
+    def porosity(self) -> GridArrayDefinition:
         self.load_grid_properties_if_not_loaded()
         return self._porosity
 
     @property
-    def sw(self):
+    def sw(self) -> GridArrayDefinition:
         self.load_grid_properties_if_not_loaded()
         return self._sw
 
     @property
-    def sg(self):
+    def sg(self) -> GridArrayDefinition:
         self.load_grid_properties_if_not_loaded()
         return self._sg
 
     @property
-    def pressure(self):
+    def pressure(self) -> GridArrayDefinition:
         self.load_grid_properties_if_not_loaded()
         return self._pressure
 
     @property
-    def temperature(self):
+    def temperature(self) -> GridArrayDefinition:
         self.load_grid_properties_if_not_loaded()
         return self._temperature
 
     @property
-    def kx(self):
+    def kx(self) -> GridArrayDefinition:
         self.load_grid_properties_if_not_loaded()
         return self._kx
 
     @property
-    def ky(self):
+    def ky(self) -> GridArrayDefinition:
         self.load_grid_properties_if_not_loaded()
         return self._ky
 
     @property
-    def kz(self):
+    def kz(self) -> GridArrayDefinition:
         self.load_grid_properties_if_not_loaded()
         return self._kz
 
     @abstractmethod
     def load_structured_grid_file(self, structure_grid_file: File, lazy_loading: bool) -> Grid:
         raise NotImplementedError("Implement this in the derived class")
```

### Comparing `ressimpy-2.1.1/ResSimpy/GridArrayFunction.py` & `ressimpy-2.2.0/ResSimpy/GridArrayFunction.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/ISODateTime.py` & `ressimpy-2.2.0/ResSimpy/ISODateTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from __future__ import annotations
+
+import warnings
 from typing import Optional
 from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 from datetime import datetime, timedelta
 
 
 class ISODateTime(datetime):
     """A class representing an extension of datetime class,  returns back date in ISO datetime format."""
@@ -27,15 +29,16 @@
                 return True
             except ValueError:
                 return False
         else:
             return False
 
     @classmethod
-    def convert_to_iso(cls, date: str, date_format: DateFormat, start_date: Optional[str] = None) -> ISODateTime:
+    def convert_to_iso(cls: type[ISODateTime], date: str, date_format: Optional[DateFormat],
+                       start_date: Optional[str] = None) -> ISODateTime:
         """Converts an ordinary date to an ISODate format.
 
         Args:
             date (str): The date as it is written in the model file.
             date_format (DateFormat): The date format to use to convert the date.
             start_date (Optional[str]): The start date of the model (required if the date is a number of days from the
                 start).
@@ -45,15 +48,16 @@
 
         Returns:
         ISODateTime: an initialised ISODateTime class instance for the date provided.
         """
         converted_date = None
 
         if date_format is None:
-            raise ValueError('Please provide a date format')
+            warnings.warn(f"No date format provided for date at {date}, assuming MM/DD/YYYY")
+            date_format = DateFormat.MM_DD_YYYY
 
         if ISODateTime.isfloat(date) and start_date is None:
             raise ValueError('Please provide start date when date is numeric')
         elif ISODateTime.isfloat(date) and start_date is not None:
             if date_format == DateFormat.DD_MM_YYYY:
                 converted_date = ISODateTime.strptime(start_date, '%d/%m/%Y') + timedelta(days=float(date))
             elif date_format == DateFormat.MM_DD_YYYY:
@@ -82,10 +86,10 @@
 
         if converted_date is None:
             raise ValueError('Invalid date format or missing start_date.')
 
         return converted_date
 
     @classmethod
-    def datetime_to_iso(cls, date: datetime, datetime_format: str = '%Y-%m-%d') -> ISODateTime:
+    def datetime_to_iso(cls: type[ISODateTime], date: datetime, datetime_format: str = '%Y-%m-%d') -> ISODateTime:
         """Converts datetime object to ISODateTime object."""
         return ISODateTime.strptime(str(date), datetime_format)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Network.py` & `ressimpy-2.2.0/ResSimpy/Network.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/FcsConfig.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/FcsConfig.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/FcsFile.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/FcsFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
                 printable_str += f'\t\t{multi_file_type}: {len(multi_file_list)}\n'
         return printable_str
 
     def __str__(self) -> str:
         return generic_str(self)
 
     @classmethod
-    def generate_fcs_structure(cls, fcs_file_path: str, recursive: bool = True) -> Self:
+    def generate_fcs_structure(cls: type[Self], fcs_file_path: str, recursive: bool = True) -> Self:
         """Creates an instance of the FcsNexusFile, populates it through looking through the different keywords \
             in the FCS and assigning the paths to objects.
 
         Args:
         ----
             fcs_file_path (str): path to the fcs file of interest
             recursive (bool, optional): Whether the NexusFile structure will be recursively created. Defaults to True.
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import warnings
 from dataclasses import dataclass
 from typing import Optional
 
 from ResSimpy.Constraint import Constraint
 from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 
 
 @dataclass(repr=False)
 class NexusConstraint(Constraint):
     """Attributes:
     name (str): name of the well (NAME)
     max_surface_oil_rate (float): max surface oil rate (QOSMAX)
@@ -190,23 +191,46 @@
 
     clear_all: Optional[bool] = None
     clear_q: Optional[bool] = None
     clear_limit: Optional[bool] = None
     clear_alq: Optional[bool] = None
     clear_p: Optional[bool] = None
 
-    def __init__(self, properties_dict: dict[str, None | int | str | float | UnitSystem]) -> None:
+    def __init__(self, properties_dict: dict[str, None | int | str | float | UnitSystem], date: Optional[str] = None,
+                 date_format: Optional[DateFormat] = None, start_date: Optional[str] = None,
+                 unit_system: Optional[UnitSystem] = None) -> None:
         """Initialises the NexusConstraint class.
 
         Args:
             properties_dict (dict): dict of the properties to set on the object.
+            date (Optional[str]): The date of the object.
+            date_format (Optional[DateFormat]): The date format that the object uses.
+            start_date (Optional[str]): The start date of the model. Required if the object uses a decimal TIME.
+            unit_system (Optional[UnitSystem]): The unit system of the object e.g. ENGLISH, METRIC.
         """
-        super(Constraint, self).__init__({})
-        for key, prop in properties_dict.items():
-            self.__setattr__(key, prop)
+        super().__init__(_date_format=date_format, _start_date=start_date, _unit_system=unit_system)
+
+        # Set the date related properties, then set the date, automatically setting the ISODate
+        protected_attributes = ['date_format', 'start_date', 'unit_system']
+
+        for attribute in protected_attributes:
+            if attribute in properties_dict:
+                self.__setattr__(f"_{attribute}", properties_dict[attribute])
+
+        # Loop through the properties dict if one is provided and set those attributes
+        remaining_properties = [x for x in properties_dict.keys() if x not in protected_attributes]
+        for key in remaining_properties:
+            self.__setattr__(key, properties_dict[key])
+
+        if date is None:
+            if 'date' not in properties_dict or not isinstance(properties_dict['date'], str):
+                raise ValueError(f"No valid Date found for object with properties: {properties_dict}")
+            self.date = properties_dict['date']
+        else:
+            self.date = date
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
         """Gets the mapping of nexus keywords to attribute definitions."""
         nexus_mapping: dict[str, tuple[str, type]] = {
             'WELL': ('well_name', str),
             'NAME': ('name', str),
@@ -341,19 +365,23 @@
             'POWER': ('pump_power', float),
             'SPEED': ('pump_speed', float),
             'CHOKELIMIT': ('choke_limit', str),
             'POSITION': ('manifold_position', int),
             }
         return nexus_mapping
 
-    def update(self, new_data: dict[str, None | int | str | float | UnitSystem], nones_overwrite: bool = False):
+    def update(self, new_data: dict[str, None | int | str | float | UnitSystem], nones_overwrite: bool = False) -> None:
         """Updates attributes in the object based on the dictionary provided."""
-        for k, v in new_data.items():
-            if v is not None or nones_overwrite:
-                setattr(self, k, v)
+        protected_attributes = ['date', 'date_format', 'start_date', 'unit_system']
+        for key, value in new_data.items():
+            modified_key = key
+            if key in protected_attributes:
+                modified_key = '_' + key
+            if value is not None or nones_overwrite:
+                setattr(self, modified_key, value)
 
     def to_table_line(self, headers: list[str]) -> str:
         """String representation of the constraint for entry to an inline constraint table.
 
         Args:
             headers (list[str]): Unused for nexusconstraint, provide an empty list
         """
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,19 +381,20 @@
                new_constraint_props: dict[str, None | float | int | str | UnitSystem] | Constraint,
                comments: Optional[str] = None) \
             -> None:
         """Modify an existing constraint. Retains existing constraint values that are not overridden by the new \
         constraint properties.
 
         Args:
-            name (str):
+            name (str): The well name
             current_constraint (dict[str, None | float | int | str] | Constraint): dictionary or constraint object\
-                with enough attributes to identify a unique existing constraint in the model.
+            with enough attributes to identify a unique existing constraint in the model.
             new_constraint_props (dict[str, None | float | int | str] | Constraint): dictionary or constraint to \
             update the constraint with.
+            comments (Optional[str]): ??
         """
 
         def clean_constraint_inputs(constraint: dict[str, None | float | int | str] | Constraint) -> \
                 dict[str, None | float | int | str]:
             """Cleans up an input ensuring consistent type is returned."""
             if isinstance(constraint, Constraint):
                 cleaned_dict = constraint.to_dict()
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusNode.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,58 @@
 """Class that is used to represent a nexus node in the network."""
 from __future__ import annotations
 from dataclasses import dataclass
 from typing import Optional
 
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 from ResSimpy.Node import Node
 
 
 @dataclass(kw_only=True, repr=False)
 class NexusNode(Node):
     """Class that is used to represent a nexus node in the network."""
     x_pos: Optional[float] = None
     y_pos: Optional[float] = None
     number: Optional[int] = None
     temp: Optional[float] = None
     station: Optional[str] = None
 
-    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+    def __init__(self, properties_dict: dict[str, None | int | str | float], date: Optional[str] = None,
+                 date_format: Optional[DateFormat] = None, start_date: Optional[str] = None,
+                 unit_system: Optional[UnitSystem] = None) -> None:
         """Initialises the NexusNode class.
 
         Args:
-            properties_dict (dict): A dictionary of properties to set on the node.
+            properties_dict (dict): dict of the properties to set on the object.
+            date (Optional[str]): The date of the object.
+            date_format (Optional[DateFormat]): The date format that the object uses.
+            start_date (Optional[str]): The start date of the model. Required if the object uses a decimal TIME.
+            unit_system (Optional[UnitSystem]): The unit system of the object e.g. ENGLISH, METRIC.
         """
-        # call the init of the DataObjectMixin
-        super(Node, self).__init__({})
-        for key, prop in properties_dict.items():
-            self.__setattr__(key, prop)
+        super().__init__(_date_format=date_format, _start_date=start_date, _unit_system=unit_system)
+
+        # Set the date related properties, then set the date, automatically setting the ISODate
+        protected_attributes = ['date_format', 'start_date', 'unit_system']
+
+        for attribute in protected_attributes:
+            if attribute in properties_dict:
+                self.__setattr__(f"_{attribute}", properties_dict[attribute])
+
+        # Loop through the properties dict if one is provided and set those attributes
+        remaining_properties = [x for x in properties_dict.keys() if x not in protected_attributes]
+        for key in remaining_properties:
+            self.__setattr__(key, properties_dict[key])
+
+        if date is None:
+            if 'date' not in properties_dict or not isinstance(properties_dict['date'], str):
+                raise ValueError(f"No valid Date found for object with properties: {properties_dict}")
+            self.date = properties_dict['date']
+        else:
+            self.date = date
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
         """Gets the mapping of nexus keywords to attribute definitions."""
         keywords = {
             'NAME': ('name', str),
             'TYPE': ('type', str),
@@ -37,15 +61,15 @@
             'X': ('x_pos', float),
             'Y': ('y_pos', float),
             'NUMBER': ('number', int),
             'STATION': ('station', str),
         }
         return keywords
 
-    def update(self, input_dictionary:  dict[str, None | float | int | str]) -> None:
+    def update(self, input_dictionary: dict[str, None | float | int | str]) -> None:
         """Updates a node based on a dictionary of attributes."""
         for k, v in input_dictionary.items():
             if v is None:
                 continue
             if hasattr(self, '_NexusNode__' + k):
                 setattr(self, '_NexusNode__' + k, v)
             elif hasattr(super(), '_Node__' + k):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Used to represent a connection between two nodes in a Nexus network."""
 from __future__ import annotations
 from dataclasses import dataclass
 from typing import Optional
 from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 from ResSimpy.NodeConnection import NodeConnection
 
 
 @dataclass(repr=False)
 class NexusNodeConnection(NodeConnection):
     """Used to represent a connection between two nodes in a Nexus network.
 
@@ -46,37 +47,58 @@
     temperature_profile: Optional[float] = None
     length: Optional[float] = None
     delta_depth: Optional[float] = None
     connection_number: Optional[int] = None
     seawater_profile: Optional[str] = None
     rate_mult: Optional[float] = None
     polymer: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
     dp_add: Optional[float] = None
     dt_add: Optional[float] = None
     temperature_in: Optional[float] = None
     temperature_out: Optional[float] = None
     tracer: Optional[str] = None
     heat_conductivity: Optional[float] = None
     insulation_thickness: Optional[float] = None
     insulation_conductivity: Optional[float] = None
     gravity_pressure_gradient_mult: Optional[float] = None
     friction_pressure_gradient_mult: Optional[float] = None
     acceleration_pressure_gradient_mult: Optional[float] = None
 
-    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+    def __init__(self, properties_dict: dict[str, None | int | str | float], date: Optional[str] = None,
+                 date_format: Optional[DateFormat] = None, start_date: Optional[str] = None,
+                 unit_system: Optional[UnitSystem] = None) -> None:
         """Initialises the NexusNodeConnection class.
 
         Args:
-            properties_dict (dict): A dictionary of properties to set on the node.
+            properties_dict (dict): dict of the properties to set on the object.
+            date (Optional[str]): The date of the object.
+            date_format (Optional[DateFormat]): The date format that the object uses.
+            start_date (Optional[str]): The start date of the model. Required if the object uses a decimal TIME.
+            unit_system (Optional[UnitSystem]): The unit system of the object e.g. ENGLISH, METRIC.
         """
-        # call the init of the DataObjectMixin
-        super(NodeConnection, self).__init__({})
-        for key, prop in properties_dict.items():
-            self.__setattr__(key, prop)
+        super().__init__(_date_format=date_format, _start_date=start_date, _unit_system=unit_system)
+
+        # Set the date related properties, then set the date, automatically setting the ISODate
+        protected_attributes = ['date_format', 'start_date', 'unit_system']
+
+        for attribute in protected_attributes:
+            if attribute in properties_dict:
+                self.__setattr__(f"_{attribute}", properties_dict[attribute])
+
+        # Loop through the properties dict if one is provided and set those attributes
+        remaining_properties = [x for x in properties_dict.keys() if x not in protected_attributes]
+        for key in remaining_properties:
+            self.__setattr__(key, properties_dict[key])
+
+        if date is None:
+            if 'date' not in properties_dict or not isinstance(properties_dict['date'], str):
+                raise ValueError(f"No valid Date found for object with properties: {properties_dict}")
+            self.date = properties_dict['date']
+        else:
+            self.date = date
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
         """Gets the mapping of nexus keywords to attribute definitions."""
         nexus_mapping = {
             'NAME': ('name', str),
             'NODEIN': ('node_in', str),
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusNodes.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusProc.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusProc.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusProcs.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusProcs.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusTargets.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusTargets.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,17 +129,16 @@
         self.__remove_object_operations.remove_object_from_network_main(
             target_to_remove, self._network_element_name, self.__targets)
 
     def add(self, target_to_add: dict[str, None | str | float | int]) -> None:
         """Adds a target to a network, taking a dictionary with properties for the new node.
 
         Args:
-            target_to_add (dict[str, None | str | float | int]):
-            dictionary taking all the properties for the new target.
-            Requires date and a target name.
+            target_to_add (dict[str, None | str | float | int]): dictionary taking all the properties for the new \
+            target. Requires date and a target name.
         """
         new_object = self.__add_object_operations.add_network_obj(target_to_add, NexusTarget, self.__parent_network)
         self._add_to_memory([new_object])
 
     def modify(self, target_to_modify: dict[str, None | str | float | int],
                new_properties: dict[str, None | str | float | int]) -> None:
         """Modifies an existing node based on a matching dictionary of properties (partial matches allowed if precisely
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Nexus implementation of the Well Connection class."""
 
 from __future__ import annotations
 from dataclasses import dataclass
 from typing import Optional
 
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 from ResSimpy.WellConnection import WellConnection
 
 
 @dataclass(kw_only=True)
 class NexusWellConnection(WellConnection):
     """Nexus implementation of the Well Connection class.
 
@@ -91,24 +93,47 @@
     dt_add: Optional[float] = None
     rate_mult: Optional[float] = None
     polymer: Optional[str] = None
     station: Optional[str] = None
     drill_queue: Optional[str] = None
     drill_order_benefit: Optional[float] = None
 
-    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+    def __init__(self, properties_dict: dict[str, None | int | str | float], date: Optional[str] = None,
+                 date_format: Optional[DateFormat] = None, start_date: Optional[str] = None,
+                 unit_system: Optional[UnitSystem] = None) -> None:
         """Initialises the NexusWellConnection class.
 
         Args:
-            properties_dict (dict): A dictionary of properties to set on the object.
+            properties_dict (dict): dict of the properties to set on the object.
+            date (Optional[str]): The date of the object.
+            date_format (Optional[DateFormat]): The date format that the object uses.
+            start_date (Optional[str]): The start date of the model. Required if the object uses a decimal TIME.
+            unit_system (Optional[UnitSystem]): The unit system of the object e.g. ENGLISH, METRIC.
         """
-        # call the init of the DataObjectMixin
-        super(WellConnection, self).__init__({})
-        for key, prop in properties_dict.items():
-            self.__setattr__(key, prop)
+        super().__init__(_date_format=date_format, _start_date=start_date, _unit_system=unit_system)
+
+        # Set the date related properties, then set the date, automatically setting the ISODate
+        protected_attributes = ['date_format', 'start_date', 'unit_system']
+
+        for attribute in protected_attributes:
+            if attribute in properties_dict:
+                self.__setattr__(f"_{attribute}", properties_dict[attribute])
+
+        # Loop through the properties dict if one is provided and set those attributes
+        remaining_properties = [x for x in properties_dict.keys() if x not in protected_attributes]
+        for key in remaining_properties:
+            self.__setattr__(key, properties_dict[key])
+
+        if date is None:
+            if 'date' not in properties_dict or not isinstance(properties_dict['date'], str):
+                raise ValueError(f"No valid Date found for object with properties: {properties_dict}")
+            self.date = properties_dict['date']
+        else:
+            self.date = date
+
         if self.name is not None:
             self.bh_node_name = self.name + '%bh'
             self.wh_node_name = self.name + '%wh'
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
         """Gets the mapping of nexus keywords to attribute definitions."""
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Class to hold Nexus Aquifer properties."""
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional, Union
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_SINGLE_KEYWORDS, AQUIFER_TABLE_KEYWORDS
 from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_KEYWORDS_VALUE_FLOAT, AQUIFER_KEYWORDS_VALUE_INT
 from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_KEYWORDS, AQUIFER_TYPE_KEYWORDS
 from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
 from ResSimpy.DynamicProperty import DynamicProperty
@@ -26,30 +27,28 @@
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific aquifer properties method. Defaults to empty dictionary.
     """
 
     # General parameters
     file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                 dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         """Initialises the NexusAquiferMethod class.
 
         Args:
             file (NexusFile): NexusFile object associated with the aquifer method.
             input_number (int): method number for the aquifer method.
             model_unit_system (UnitSystem): unit system used in the model.
-            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of properties for the aquifer
-                                 method. Defaults to None.
+            properties: dictionary of properties for the aquifer method. Defaults to None.
         """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusCompletion.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusCompletion.py`

 * *Files 7% similar despite different names*

```diff
@@ -178,125 +178,126 @@
         super().__init__(date=date, i=i, j=j, k=k, skin=skin, depth=depth, well_radius=well_radius, x=x, y=y,
                          angle_a=angle_a, angle_v=angle_v, grid=grid, depth_to_top=depth_to_top,
                          depth_to_bottom=depth_to_bottom, perm_thickness_ovr=perm_thickness_ovr, dfactor=dfactor,
                          rel_perm_method=rel_perm_method, status=status, date_format=date_format, start_date=start_date,
                          unit_system=unit_system, peaceman_well_block_radius=peaceman_well_block_radius)
 
     @property
-    def measured_depth(self):
+    def measured_depth(self) -> float | None:
         return self.__measured_depth
 
     @property
-    def well_indices(self):
+    def well_indices(self) -> float | None:
         return self.__well_indices
 
     @property
-    def partial_perf(self):
+    def partial_perf(self) -> float | None:
         return self.__partial_perf
 
     @property
-    def cell_number(self):
+    def cell_number(self) -> int | None:
         return self.__cell_number
 
     @property
-    def portype(self):
+    def portype(self) -> str | None:
         return self.__portype
 
     @property
-    def fracture_mult(self):
+    def fracture_mult(self) -> float | None:
         return self.__fracture_mult
 
     @property
-    def sector(self):
+    def sector(self) -> None | str | int:
         return self.__sector
 
     @property
-    def well_group(self):
+    def well_group(self) -> str | None:
         return self.__well_group
 
     @property
-    def zone(self):
+    def zone(self) -> int | None:
         return self.__zone
 
     @property
-    def angle_open_flow(self):
+    def angle_open_flow(self) -> float | None:
         return self.__angle_open_flow
 
     @property
-    def temperature(self):
+    def temperature(self) -> float | None:
         return self.__temperature
 
     @property
-    def flowsector(self):
+    def flowsector(self) -> int | None:
         return self.__flowsector
 
     @property
-    def parent_node(self):
+    def parent_node(self) -> str | None:
         return self.__parent_node
 
     @property
-    def mdcon(self):
+    def mdcon(self) -> float | None:
         return self.__mdcon
 
     @property
-    def pressure_avg_pattern(self):
+    def pressure_avg_pattern(self) -> int | None:
         return self.__pressure_avg_pattern
 
     @property
-    def length(self):
+    def length(self) -> float | None:
         return self.__length
 
     @property
-    def permeability(self):
+    def permeability(self) -> float | None:
         return self.__permeability
 
     @property
-    def non_darcy_model(self):
+    def non_darcy_model(self) -> str | None:
         return self.__non_darcy_model
 
     @property
-    def comp_dz(self):
+    def comp_dz(self) -> float | None:
         return self.__comp_dz
 
     @property
-    def layer_assignment(self):
+    def layer_assignment(self) -> int | None:
         return self.__layer_assignment
 
     @property
-    def polymer_block_radius(self):
+    def polymer_block_radius(self) -> float | None:
         return self.__polymer_block_radius
 
     @property
-    def polymer_well_radius(self):
+    def polymer_well_radius(self) -> float | None:
         return self.__polymer_well_radius
 
     @property
-    def rel_perm_end_point(self):
+    def rel_perm_end_point(self) -> NexusRelPermEndPoint | None:
         return self.__rel_perm_end_point
 
     @property
-    def kh_mult(self):
+    def kh_mult(self) -> float | None:
         return self.__kh_mult
 
     @property
-    def depth_to_top_str(self):
+    def depth_to_top_str(self) -> str | None:
         return self.__depth_to_top_str
 
     @property
-    def depth_to_bottom_str(self):
+    def depth_to_bottom_str(self) -> str | None:
         return self.__depth_to_bottom_str
 
     def to_dict(self, keys_in_keyword_style: bool = False, add_date: bool = True, add_units: bool = False,
-                include_nones: bool = True) -> \
+                include_nones: bool = True, units_as_string: bool = True) -> \
             dict[str, None | str | int | float]:
 
         attribute_dict = to_dict(self, keys_in_keyword_style, add_date=add_date,
                                  add_units=add_units, include_nones=include_nones)
         parent_attribute_dict = super().to_dict(keys_in_keyword_style=keys_in_keyword_style, add_date=add_date,
-                                                add_units=add_units, include_nones=include_nones)
+                                                add_units=add_units, include_nones=include_nones,
+                                                units_as_string=units_as_string)
 
         attribute_dict.update(parent_attribute_dict)
         if self.rel_perm_end_point is not None:
             attribute_dict.update(self.rel_perm_end_point.to_dict())
         return attribute_dict
 
     @property
@@ -371,15 +372,16 @@
 
     @staticmethod
     def valid_attributes() -> list[str]:
         """Lists all possible attributes for the object that relate to a Nexus keyword."""
         return [v[0] for v in NexusCompletion.get_keyword_mapping().values()]
 
     @classmethod
-    def from_dict(cls, input_dictionary: dict[str, None | float | int | str], date_format: DateFormat) -> Self:
+    def from_dict(cls: type[Self], input_dictionary: dict[str, None | float | int | str],
+                  date_format: DateFormat) -> Self:
         """Generates a NexusCompletion from a dictionary."""
         skip_mapping_keys = ['date', 'date_format', 'unit_system', 'start_date']
         for input_attr in input_dictionary:
             if input_attr in skip_mapping_keys:
                 continue
             elif input_attr not in cls.valid_attributes():
                 raise AttributeError(f'Unexpected keyword "{input_attr}" found within {input_dictionary}')
@@ -390,15 +392,20 @@
             completion_date_format = DateFormat[converted_date_format_str]
         else:
             completion_date_format = date_format
         if date is None:
             raise AttributeError(f'No date provided for the completion, instead got {date=}')
 
         date = str(date)
-        constructed_class = cls(date=date, date_format=completion_date_format)
+
+        if 'start_date' not in input_dictionary or not isinstance(input_dictionary['start_date'], str):
+            raise ValueError(f"Invalid start date found: {input_dictionary}")
+
+        constructed_class = cls(date=date, date_format=completion_date_format,
+                                start_date=input_dictionary['start_date'])
         constructed_class.update(input_dictionary)
         return constructed_class
 
     def update(self, input_dictionary: dict[str, None | float | int | str]) -> None:
         """Updates a completion based on a dictionary of attributes."""
         for k, v in input_dictionary.items():
             if v is None:
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusEquilMethod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Class storing Nexus Equilibration method properties."""
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Union, Optional
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Enums.UnitsEnum import SUnits, TemperatureUnits, UnitSystem
 from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_INTSAT_KEYWORDS, EQUIL_KEYWORDS_VALUE_FLOAT
 from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_TABLE_KEYWORDS, EQUIL_SINGLE_KEYWORDS
 from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_COMPOSITION_OPTIONS
 from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_KEYWORDS
@@ -28,31 +29,29 @@
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific equilibration method. Defaults to empty dictionary.
     """
 
     # General parameters
     file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str],
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray,
                                 pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
         = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         """Initialises the NexusEquilMethod class.
 
         Args:
             file (NexusFile): NexusFile object associated with the equil method.
             input_number (int): method number for the equil method.
             model_unit_system (UnitSystem): unit system used in the model.
-            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of key properties for the equil
-                                    method. Defaults to None.
+            properties: dictionary of key properties for the equil method. Defaults to None.
         """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusFile.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusFile.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,17 @@
             self.object_locations: dict[UUID, list[int]] = get_empty_dict_uuid_list_int()
         if self.line_locations is None:
             self.line_locations = []
         self.linked_user = linked_user
         self.last_modified = last_modified
 
     @classmethod
-    def generate_file_include_structure(cls, file_path: str, origin: Optional[str] = None, recursive: bool = True,
-                                        skip_arrays: bool = True, top_level_file: bool = True) -> Self:
+    def generate_file_include_structure(cls: type[Self], file_path: str, origin: Optional[str] = None,
+                                        recursive: bool = True, skip_arrays: bool = True,
+                                        top_level_file: bool = True) -> Self:
         """Generates a nexus file instance for a provided text file with information storing the included files.
 
         Args:
             file_path (str): path to a file
             origin (Optional[str], optional): Where the file was opened from. Defaults to None.
             recursive (bool): Whether the method should recursively drill down multiple layers of include_locations.
             skip_arrays (bool): If set True skips the INCLUDE arrays that come after property array and VALUE
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional, Union
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Enums.UnitsEnum import SUnits, TemperatureUnits, UnitSystem
 from ResSimpy.Nexus.NexusKeywords.gaslift_keywords import GL_ARRAY_KEYWORDS, GASLIFT_KEYWORDS, GL_TABLE_HEADER_COLS
 from ResSimpy.DynamicProperty import DynamicProperty
 from ResSimpy.Units.AttributeMappings.DynamicPropertyUnitMapping import HydraulicsUnits
 
@@ -23,29 +24,28 @@
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific gaslift properties method. Defaults to empty dictionary.
     """
 
     # General parameters
     file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                      dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         """Initialises the NexusGasliftMethod class.
 
         Args:
             file (NexusFile): NexusFile object associated with the gaslift method
             input_number (int): method number for the gaslift method
-            model_unit_system (UnitSystem): unit system from the model
-            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of properties for the gaslift
+            model_unit_system (UnitSystem): unit system from the model.
+            properties: dictionary of properties for the gaslift. Defaults to None.
         """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 import re
 from typing import Optional, Union
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_ARRAY_KEYWORDS, HYD_TABLE_HEADER_COLS, HYD_KEYWORDS
 from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_PRESSURE_KEYWORDS, HYD_SINGLE_KEYWORDS
 from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_KEYWORDS_VALUE_FLOAT, HYD_WATINJ_KEYWORDS_VALUE_FLOAT
 from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_ALQ_KEYWORD, HYD_ALQ_OPTIONS
 from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
@@ -27,32 +28,31 @@
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific hydraulics properties method. Defaults to empty dictionary.
     """
 
     # General parameters
     file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                      dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
     ratio_thousands: bool
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  ratio_thousands: bool = True,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         """Initialises the NexusHydraulicsMethod class.
 
         Args:
-            file (NexusFile): ??
-            input_number (int): ??
-            model_unit_system (UnitSystem): ??
+            file (NexusFile): NexusFile object associated with the hydraulics method.
+            input_number (int): method number for the hydraulics method.
+            model_unit_system (UnitSystem): unit system used in the model.
             ratio_thousands (bool): ??
-            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                 dict[str, Union[float, pd.DataFrame]]]]]): ??
+            properties: dictionary of key properties for the hydraulics method. Defaults to None.
         """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         self.ratio_thousands = ratio_thousands
@@ -119,21 +119,26 @@
                     printable_str += f'{value.value}\n'
                 elif isinstance(value, SUnits):
                     printable_str += f'SUNITS {value.value}\n'
             elif key == 'ALQ':
                 printable_str += f'{key}'
                 if 'ALQ_PARAM' in hyd_dict.keys():
                     printable_str += f" {hyd_dict['ALQ_PARAM']}"
-                printable_str += f' {value}\n'
+                if isinstance(value, np.ndarray):
+                    printable_str += f" {' '.join([str(val) for val in value])}\n"
+                else:
+                    printable_str += f' {value}\n'
             elif key == 'WATINJ' and isinstance(value, dict):
                 printable_str += f'{key}\n'
                 for watinj_key in value.keys():
                     printable_str += f'    {watinj_key} {value[watinj_key]}\n'
             elif key not in ['ALQ', 'ALQ_PARAM', 'WATINJ']:
-                if value == '':
+                if isinstance(value, np.ndarray):
+                    printable_str += f"{key} {' '.join([str(val) for val in value])}\n"
+                elif value == '':
                     printable_str += f'{key}\n'
                 else:
                     printable_str += f'{key} {value}\n'
         printable_str += '\n'
         return printable_str
 
     def read_properties(self) -> None:
@@ -180,15 +185,15 @@
                 line_elems = line.split('!')[0].split()
                 next_val = nfo.get_expected_token_value(potential_keyword, line, file_as_list)
                 if potential_keyword == 'ALQ' and next_val in HYD_ALQ_OPTIONS:
                     self.properties['ALQ_PARAM'] = next_val
                     keyword_index = line_elems.index(next_val)
                 else:
                     keyword_index = line_elems.index(potential_keyword)
-                self.properties[potential_keyword] = ' '.join(line_elems[keyword_index+1:])
+                self.properties[potential_keyword] = np.fromstring(' '.join(line_elems[keyword_index+1:]), sep=' ')
 
             # Create WATINJ property if needed
             if nfo.check_token('WATINJ', line):
                 found_waterinj = True
 
             # Handle DATGRAD property
             if nfo.check_token('DATGRAD', line):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusPVTMethod.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Class to hold Nexus PVT properties."""
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional, Union
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_BLACKOIL_PRIMARY_KEYWORDS, PVT_TYPE_KEYWORDS, PVT_KEYWORDS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOS_METHODS, PVT_EOSOPTIONS_PRIMARY_WORDS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_PRIMARY_KEYS_INT, PVT_TABLE_KEYWORDS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_TABLES_WITH_ENDWORDS, PVT_TABLES_WITHOUT_ENDWORDS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT, PVT_EOSOPTIONS_TRANS_KEYS
@@ -48,42 +49,39 @@
     eos_nhc: Optional[int] = None  # Number of hydrocarbon components
     eos_temp: Optional[float] = None  # Default temperature for EOS method
     eos_components: Optional[list[str]] = field(default_factory=get_empty_list_str)
     eos_options: dict[str, Union[
         str, int, float, pd.DataFrame, list[str], dict[str, float], tuple[str, dict[str, float]], dict[
             str, pd.DataFrame]]] \
         = field(default_factory=get_empty_eosopt_dict_union)
-    properties: dict[str, Union[str, int, float, Enum, list[str],
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray,
                                 pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
         = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  pvt_type: Optional[PvtType] = None,
                  eos_nhc: Optional[int] = None, eos_temp: Optional[float] = None,
                  eos_components: Optional[list[str]] = None,
                  eos_options: Optional[dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float],
                                        tuple[str, dict[str, float]], dict[str, pd.DataFrame]]]] = None,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         """Initialises the NexusGasliftMethod class.
 
         Args:
             file (NexusFile): NexusFile object associated with the PVT method.
             input_number (int): method number for the PVT method.
             model_unit_system (UnitSystem): unit system from the model.
             pvt_type (Optional[PvtType]): Type of PVT method, e.g., BLACKOIL, GASWATER or EOS. Defaults to None.
             eos_nhc (Optional[int]): Number of hydrocarbon components for EOS method. Defaults to None.
             eos_temp (Optional[float]): Default temperature for EOS method. Defaults to None.
             eos_components (Optional[list[str]]): Specifies component names for EOS method. Defaults to None.
-            eos_options (Optional[dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float],
-                                       tuple[str, dict[str, float]], dict[str, pd.DataFrame]]]]): Dictionary containing
-                                        various EOS options as specified in the PVT file. Defaults to None.
-            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of properties for the PVT method.
+            eos_options: Dictionary containing various EOS options as specified in the PVT file. Defaults to None.
+            properties: dictionary of properties for the PVT method.
         """
         if pvt_type is not None:
             self.pvt_type = pvt_type
         if eos_nhc is not None:
             self.eos_nhc = eos_nhc
         if eos_temp is not None:
             self.eos_temp = eos_temp
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Class to hold Nexus relative permeability and capillary pressure properties."""
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional, Union
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Nexus.NexusKeywords.relpm_keywords import RELPM_TABLE_KEYWORDS, RELPM_KEYWORDS_VALUE_FLOAT
 from ResSimpy.Nexus.NexusKeywords.relpm_keywords import RELPM_SINGLE_KEYWORDS, RELPM_HYSTERESIS_PRIMARY_KEYWORDS
 from ResSimpy.Nexus.NexusKeywords.relpm_keywords import RELPM_KEYWORDS, RELPM_NONDARCY_KEYWORDS, RELPM_NONDARCY_PARAMS
 from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
 from ResSimpy.DynamicProperty import DynamicProperty
@@ -27,35 +28,33 @@
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific PVT method. Defaults to empty dictionary.
     """
 
     # General parameters
     file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                      dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     hysteresis_params: dict[str, Union[str, float, dict[str, Union[str, float, dict[str, Union[str, float]]]]]] \
         = field(default_factory=get_empty_hysteresis_dict)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None,
                  hysteresis_params: Optional[dict[str, Union[str, float, dict[str, Union[str, float,
                                              dict[str, Union[str, float]]]]]]] = None) -> None:
         """Initialises the NexusRelPermMethod class.
 
         Args:
             file (NexusFile): Nexus file object associated with the relperm method
             input_number (int): method number for the relperm method
             model_unit_system (UnitSystem): unit system from the model
-            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                dict[str, Union[float, pd.DataFrame]]]]]): properties for the relperm method.
-            hysteresis_params (Optional[dict[str, Union[str, float, dict[str, Union[str, float,
-                                dict[str, Union[str, float]]]]]]]): hysteresis parameters for the relperm method.
+            properties: properties for the relperm method.
+            hysteresis_params: hysteresis parameters for the relperm method.
         """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         if hysteresis_params is not None:
             self.hysteresis_params = hysteresis_params
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusReportingRequests.py` & `ressimpy-2.2.0/ResSimpy/output_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,74 @@
-"""Data objects for handling output requests and contents in Nexus."""
-
-from __future__ import annotations
-
 from dataclasses import dataclass
+from abc import ABC
+from typing import Optional
 
+from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Enums.FrequencyEnum import FrequencyEnum
 from ResSimpy.Enums.OutputType import OutputType
-from ResSimpy.output_request import OutputRequest, OutputContents
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
+from ResSimpy.Units.AttributeMappings.BaseUnitMapping import BaseUnitMapping
 
 
 @dataclass(kw_only=True)
-class NexusOutputRequest(OutputRequest):
-    """Class for handling output requests in Nexus.
+class OutputRequest(DataObjectMixin, ABC):
+    """Class to hold data input for an Output Request.
 
     Attributes:
         date (str): Date of the output request.
         output (str): Output request.
         output_type (OutputType): Type of output request.
         output_frequency (FrequencyEnum): Frequency of the output request.
         output_frequency_number (None | float): Number of the frequency of the output request.
     """
-    date: str
+
     output: str
     output_type: OutputType
     output_frequency: FrequencyEnum
     output_frequency_number: None | float
 
-    def to_table_line(self, headers: list[str]) -> str:
-        """String representation of the single line within an Output request table."""
-        _ = headers
-        result = f'{self.output} {self.output_frequency.name}'
-        if self.output_frequency_number is not None:
-            result += ' ' + str(self.output_frequency_number)
-        result += '\n'
-        return result
+    def __init__(self, date: str, output: str, output_type: OutputType, output_frequency: FrequencyEnum,
+                 output_frequency_number: Optional[float] = None, date_format: Optional[DateFormat] = None,
+                 start_date: Optional[str] = None) -> None:
+        """Initialises the OutputRequest class.
+
+        Args:
+            date (str): Date of the output request.
+            output (str): Output request.
+            output_type (OutputType): Type of output request.
+            output_frequency (FrequencyEnum): Frequency of the output request.
+            output_frequency_number (None | float): Number of the frequency of the output request.
+            date_format (Optional[DateFormat]): The date format of the object.
+            start_date (Optional[str]): The start date of the model (required if the date is in numerical format).
+        """
+
+        super().__init__(date=date, date_format=date_format, start_date=start_date)
+
+        self.output = output
+        self.output_type = output_type
+        self.output_frequency = output_frequency
+        self.output_frequency_number = output_frequency_number
+
+    @staticmethod
+    def get_keyword_mapping() -> dict[str, tuple[str, type]]:
+        """No keywords for this class, returns an empty dict."""
+        return {}
+
+    @property
+    def units(self) -> BaseUnitMapping:
+        return BaseUnitMapping(unit_system=None)
 
 
 @dataclass(kw_only=True)
-class NexusOutputContents(OutputContents):
-    """Class for handling the output that Nexus produces."""
+class OutputContents(ABC):
+    """Class to hold data input for an Output Contents.
+
+    Attributes:
+        date (str): Date of the output contents.
+        output (str): Output contents.
+        output_type (OutputType): Type of output contents.
+    """
+
     date: str
+    output: str
     output_contents: list[str]
     output_type: OutputType
-    output: str
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusRockMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Class to hold Nexus Rock properties."""
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional, Union
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_ALL_TABLE_KEYWORDS, ROCK_KEYWORDS_VALUE_FLOAT
 from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_SINGLE_KEYWORDS, ROCK_KEYWORDS_VALUE_STR
 from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_KEYWORDS, ROCK_REV_IRREV_OPTIONS
 from ResSimpy.DynamicProperty import DynamicProperty
 from ResSimpy.Units.AttributeMappings.DynamicPropertyUnitMapping import RockUnits
@@ -26,30 +27,28 @@
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific rock properties method. Defaults to empty dictionary.
     """
 
     # General parameters
     file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                 dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         """Initialises the NexusRockMethod class.
 
         Args:
             file (NexusFile): Nexus file containing the rock method.
             input_number (int): method number for the rock method
             model_unit_system (UnitSystem): unit system from the model
-            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of the properties for the rock
-                                    method. Defaults to None.
+            properties: dictionary of the properties for the rock method. Defaults to None.
         """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Class to hold data input for a Nexus Separator method."""
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional, Union
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Utils.factory_methods import get_empty_dict_union
 import ResSimpy.Nexus.nexus_file_operations as nfo
 from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYS_INT, SEPARATOR_KEYS_FLOAT
 from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYWORDS
 from ResSimpy.DynamicProperty import DynamicProperty
@@ -26,33 +27,32 @@
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific separator method. Defaults to empty dictionary.
     """
 
     file: NexusFile
     separator_type: Optional[SeparatorType] = None
-    properties: dict[str, Union[str, int, float, Enum, list[str],
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray,
                      pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
         = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  separator_type: Optional[SeparatorType] = None,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         """Initialises the NexusSeparatorMethod class.
 
         Args:
             file (NexusFile): NexusFile object associated with the separator method
             input_number (int): method number for the separator method
             model_unit_system (UnitSystem): unit system from the model
             separator_type (Optional[SeparatorType]): type of separator method, e.g., BLACKOIL, GASPLANT or EOS
-            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of properties for the separator
-                                 method.
+
+            properties: dictionary of properties for the separator method.
         """
         if separator_type is not None:
             self.separator_type = separator_type
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusSolverParameter.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusSolverParameter.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusValveMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusValveMethod.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Class to hold Nexus Valve properties."""
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional, Union
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.Nexus.NexusKeywords.valve_keywords import VALVE_TABLE_KEYWORDS, VALVE_RATE_KEYWORDS
 from ResSimpy.DynamicProperty import DynamicProperty
 from ResSimpy.Units.AttributeMappings.DynamicPropertyUnitMapping import HydraulicsUnits
 from ResSimpy.Enums.UnitsEnum import UnitSystem, TemperatureUnits
 from ResSimpy.Utils.factory_methods import get_empty_dict_union
@@ -23,29 +24,28 @@
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific valve properties method. Defaults to empty dictionary.
     """
 
     # General parameters
     file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                      dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         """Initialises the NexusValveMethod class.
 
         Args:
             file (NexusFile): NexusFile object associated with the valve method.
             input_number (int): method number for the valve method.
             model_unit_system (UnitSystem): unit system used in the model.
-            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                 dict[str, Union[float, pd.DataFrame]]]]]): The properties found in the valve method.
+            properties: The properties found in the valve method.
         """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusWaterMethod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Class to hold Nexus Water properties."""
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional, Union
+import numpy as np
 import pandas as pd
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
 from ResSimpy.DynamicProperty import DynamicProperty
 from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
 from ResSimpy.Utils.factory_methods import get_empty_dict_union, get_empty_list_nexus_water_params
 import ResSimpy.Nexus.nexus_file_operations as nfo
 from ResSimpy.Utils.invert_nexus_map import invert_nexus_map
@@ -49,34 +50,32 @@
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding properties for generic dynamic method. Defaults to empty dictionary.
         parameters (list[NexusWaterParams]): list of water parameters, such as density, viscosity, etc.
     """
 
     file: NexusFile
     reference_pressure: Optional[float] = None
-    properties: dict[str, Union[str, int, float, Enum, list[str],
+    properties: dict[str, Union[str, int, float, Enum, list[str], np.ndarray,
                      pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
         = field(default_factory=get_empty_dict_union)
     parameters: list[NexusWaterParams] = field(default_factory=get_empty_list_nexus_water_params)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  reference_pressure: Optional[float] = None,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None,
                  parameters: Optional[list[NexusWaterParams]] = None) -> None:
         """Initialises the NexusWaterMethod class.
 
         Args:
             file (NexusFile): Nexus water file object
             input_number (int): Water method number in Nexus fcs file
             reference_pressure (float): Reference pressure for BW and, if CVW is present, for VISW
-            properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                        dict[str, Union[float, pd.DataFrame]]]]):
-                Dictionary holding properties for generic dynamic method. Defaults to empty dictionary.
+            properties: Dictionary holding properties for generic dynamic method. Defaults to empty dictionary.
             parameters (list[NexusWaterParams]): list of water parameters, such as density, viscosity, etc.
             model_unit_system (UnitSystem): unit system used in the model.
         """
         self.reference_pressure = reference_pressure
         if properties is not None:
             self.properties = properties
         else:
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWell.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusWell.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                         completion_properties: dict[str, None | float | int | str] | NexusCompletion) \
             -> NexusCompletion:
         """Returns precisely one completion which matches all the properties provided.
             If several completions match it raise a ValueError.
 
         Args:
         ----
-            completion_properties (dict | NexusCompletion):
+            completion_properties (dict | NexusCompletion): The completion properties.
 
         Returns:
         -------
             NexusCompletion that matches all completion properties provided.
         """
         matching_completions = self.find_completions(completion_properties)
         if len(matching_completions) != 1:
@@ -127,18 +127,18 @@
 
     def _add_completion_to_memory(self, date: str, completion_properties: dict[str, None | float | int | str],
                                   date_format: DateFormat, completion_index: Optional[int] = None) -> NexusCompletion:
         """Adds a perforation with the properties specified in completion_properties_list,
             if index is none then adds it to the end of the perforation list.
 
         Args:
-        ----
             date (str): date at which the perforation should be added
-            completion_properties (dict[str, str | float | int]):
-            completion_index (Optional[int]):
+            completion_properties (dict[str, str | float | int]): The completion properties.
+            date_format (DateFormat): The date format.
+            completion_index (Optional[int]): The index of the completion being searched for.
         """
         completion_properties['date'] = date
         completion_properties['unit_system'] = self.unit_system
         completion_properties['start_date'] = self._parent_wells_instance.start_date
         new_completion = NexusCompletion.from_dict(completion_properties, date_format)
         if completion_index is None:
             completion_index = len(self._completions)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWellList.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusWellList.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/NexusWellMod.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/NexusWellMod.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from ResSimpy.Utils.generic_repr import generic_repr, generic_str
 from ResSimpy.Utils.to_dict_generic import to_dict
 
 
 @dataclass(kw_only=True)
 class NexusWellMod:
     """Data structure for holding wellmod data for the NexusWell class."""
-
-    well_name: str
     date: str
+    well_name: str
     unit_system: UnitSystem | None = None
     partial_perf: float | list[float] | None = None
     permeability_thickness: float | list[float] | None = None
     skin: float | list[float] | None = None
     well_radius: float | list[float] | None = None
     polymer_well_radius: float | list[float] | None = None
     polymer_block_radius: float | list[float] | None = None
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Nexus grid file class for loading in a structured grid file and extracting the grid properties."""
 from __future__ import annotations
 
 import copy
+import os
+
 import pandas as pd
 from dataclasses import dataclass
 from typing import Optional, TYPE_CHECKING, Any
 import warnings
 
 from ResSimpy.File import File
 from ResSimpy.Grid import Grid, GridArrayDefinition
@@ -112,14 +114,15 @@
 
     def __init__(self, grid_nexus_file: Optional[NexusFile] = None, assume_loaded: bool = False) -> None:
         """Initialises the NexusGrid class.
 
         Args:
             grid_nexus_file (Optional[NexusFile]): the NexusFile representation of a structured grid file for \
                 reading and interpreting the grid properties from.
+            assume_loaded (bool): Create the object assuming the grid has already been loaded into memory.
         """
         super().__init__(assume_loaded=assume_loaded)
         self.__array_functions_list: Optional[list[list[str]]] = None
         self.__array_functions_df: Optional[pd.DataFrame] = None
         self.__array_functions_loaded: bool = False
         self.__grid_file_contents: Optional[list[str]] = None if grid_nexus_file is None else \
             grid_nexus_file.get_flat_list_str_file_including_includes
@@ -206,15 +209,15 @@
             return value
 
     def update_properties_from_dict(self, data: dict[str, int | GridArrayDefinition]) -> None:
         """Allows you to update properties on the class using the provided dict of values.
 
         Args:
         ----
-                data dict[str, int | GridArrayDefinition]: the dictionary of values to update on the class
+                data (dict[str, int | GridArrayDefinition]): the dictionary of values to update on the class
         """
         # Use the dict provided to populate the properties in the class
         if data is not None:
             for name, value in data.items():
                 private_name = '_' + name
                 setattr(self, private_name, self.__wrap(value))
 
@@ -380,14 +383,25 @@
                 token_property = properties_to_load[possible_properties.index(line_start_token)]
                 for modifier in token_property.modifiers:
                     # execute the load
                     StructuredGridOperations.load_token_value_if_present(
                         token_property.token, modifier, token_property.property, line, file_as_list, idx,
                         ['INCLUDE', 'NOLIST'])
 
+                    # check for grid array definitions with paths and add absolute paths
+                    grid_array_def = None
+                    if isinstance(token_property.property, dict):
+                        for ireg_name, grid_array_def in token_property.property.items():
+                            if modifier == 'VALUE' and grid_array_def.value is not None:
+                                self.__add_absolute_path_to_grid_array_definition(grid_array_def, idx)
+                    else:
+                        grid_array_def = token_property.property
+                        if modifier == 'VALUE' and grid_array_def.value is not None:
+                            self.__add_absolute_path_to_grid_array_definition(grid_array_def, idx)
+
             # Load in grid dimensions
             if nfo.check_token('NX', line):
                 # Check that the format of the grid is NX followed by NY followed by NZ
                 current_line = file_as_list[file_as_list.index(line)]
                 remaining_line = current_line[current_line.index('NX') + 2:]
                 if nfo.get_next_value(0, [remaining_line], remaining_line) != 'NY':
                     continue
@@ -412,20 +426,23 @@
     @classmethod
     def load_structured_grid_file(cls: type[NexusGrid], structured_grid_file: File,
                                   lazy_loading: bool = True) -> NexusGrid:
         """Loads in a structured grid file with all grid properties, and the array functions defined with 'FUNCTION'.
         Other grid modifiers are currently not supported.
 
         Args:
-        ----
             structured_grid_file (NexusFile): the NexusFile representation of a structured grid file for converting \
                 into a structured grid file class
+            lazy_loading (bool): If set to True, parts of the grid will only be loaded in when requested via \
+                properties on the object.
+
         Raises:
             AttributeError: if no value is found for the structured grid file path
             ValueError: if when loading the grid no values can be found for the NX NY NZ line.
+
         """
         if structured_grid_file.location is None:
             raise ValueError(f"No file path given or found for structured grid file path. \
                 Instead got {structured_grid_file.location}")
 
         if not isinstance(structured_grid_file, NexusFile):
             raise ValueError(f"Cannot load file of type {type(structured_grid_file)}.")
@@ -440,15 +457,14 @@
         return loaded_structured_grid_file
 
     @staticmethod
     def update_structured_grid_file(grid_dict: dict[str, GridArrayDefinition | int], model: NexusSimulator) -> None:
         """Save values passed from the front end to the structured grid file and update the class.
 
         Args:
-        ----
             grid_dict (dict[str, Union[VariableEntry, int]]): dictionary containing grid properties to be replaced
             model (NexusSimulator): an instance of a NexusSimulator object
         Raises:
             ValueError: If no structured grid file is in the instance of the Simulator class
         """
         # Convert the dictionary back to a class, and update the properties on our class
         structured_grid = model.grid
@@ -552,14 +568,37 @@
     def __keyword_in_include_file_warning(var_entry_obj: GridArrayDefinition) -> None:
 
         if var_entry_obj.keyword_in_include_file is True:
             warnings.warn('Grid array keyword in include file. This is not recommended simulation practice.')
         else:
             return None
 
+    def __add_absolute_path_to_grid_array_definition(self, grid_array_definition: GridArrayDefinition,
+                                                     line_index_of_include_file: int) -> None:
+        # cover the trivial case where the path is already absolute
+        if grid_array_definition.value is None:
+            return
+        if os.path.isabs(grid_array_definition.value):
+            grid_array_definition.absolute_path = grid_array_definition.value
+            return
+        if self.__grid_nexus_file is None:
+            return
+        file_containing_include_line, _ = self.__grid_nexus_file.find_which_include_file(line_index_of_include_file)
+        # find the include path from within this include file
+        if file_containing_include_line.include_objects is None:
+            return
+        matching_includes = [x for x in file_containing_include_line.include_objects if
+                             grid_array_definition.value in x.location]
+        if len(matching_includes) == 0:
+            return
+        include_file = matching_includes[0]
+
+        absolute_file_path = include_file.location
+        grid_array_definition.absolute_path = absolute_file_path
+
     @property
     def array_functions(self) -> Optional[list[NexusGridArrayFunction]]:
         """Returns a list of the array functions defined in the structured grid file."""
         self.load_grid_properties_if_not_loaded()
         if self.__grid_array_functions is None:
             self.load_array_functions()
         return self.__grid_array_functions
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py` & `ressimpy-2.2.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusAquiferMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusAquiferMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             self.load_aquifer_methods()
         return self.__inputs
 
     @property
     def files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_aquifer_methods(self):
+    def load_aquifer_methods(self) -> None:
         # Read in aquifer properties from Nexus aquifer method files
         if self.__files is not None and len(self.__files) > 0:  # Check if aquifer files exist
             for table_num in self.__files.keys():  # For each aquifer property method
                 aquifer_file = self.__files[table_num]
                 if aquifer_file.location is None:
                     raise ValueError(f'Unable to find aquifer file: {aquifer_file.location}')
                 if os.path.isfile(aquifer_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusEquilMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusEquilMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             self.load_equil_methods()
         return self.__inputs
 
     @property
     def files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_equil_methods(self):
+    def load_equil_methods(self) -> None:
         # Read in equil properties from Nexus equil method files
         if self.__files is not None and len(self.__files) > 0:  # Check if equil files exist
             for table_num in self.__files.keys():  # For each equil property method
                 equil_file = self.__files[table_num]
                 if equil_file.location is None:
                     raise ValueError(f'Unable to find equil file: {equil_file}')
                 if os.path.isfile(equil_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusGasliftMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusGasliftMethods.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             self.load_gaslift_methods()
         return self.__inputs
 
     @property
     def files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_gaslift_methods(self):
+    def load_gaslift_methods(self) -> None:
         # Read in gaslift properties from Nexus gaslift method files
         if self.__files is not None and len(self.__files) > 0:  # Check if gaslift files exist
             for table_num in self.__files.keys():  # For each gaslift property method
                 gaslift_file = self.__files[table_num]
                 if gaslift_file.location is None:
                     raise ValueError(f'Unable to find gaslift file: {gaslift_file}')
                 if os.path.isfile(gaslift_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusHydraulicsMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusHydraulicsMethods.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             self.load_hydraulics_methods()
         return self.__inputs
 
     @property
     def files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_hydraulics_methods(self):
+    def load_hydraulics_methods(self) -> None:
         # Read in hydraulics properties from Nexus hydraulics method files
         if self.__files is not None and len(self.__files) > 0:  # Check if hydraulics files exist
             for table_num in self.__files.keys():  # For each hydraulics property method
                 hydraulics_file = self.__files[table_num]
                 if hydraulics_file.location is None:
                     raise ValueError(f'Unable to find hydraulics file: {hydraulics_file}')
                 if os.path.isfile(hydraulics_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/equil_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/options_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/proc_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/proc_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/rock_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/separator_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/surface_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusKeywords/wells_keywords.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusKeywords/wells_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusNetwork.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusNetwork.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusPVTMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusPVTMethods.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             self.load_pvt_methods()
         return self.__inputs
 
     @property
     def files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_pvt_methods(self):
+    def load_pvt_methods(self) -> None:
         # Read in pvt properties from Nexus pvt method files
         if self.__files is not None and len(self.__files) > 0:  # Check if pvt files exist
             for table_num in self.__files.keys():  # For each pvt property method
                 pvt_file = self.__files[table_num]
                 if pvt_file.location is None:
                     raise ValueError(f'Unable to find pvt file: {pvt_file}')
                 if os.path.isfile(pvt_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusRelPermMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusRelPermMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             self.load_relperm_methods()
         return self.__inputs
 
     @property
     def files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_relperm_methods(self):
+    def load_relperm_methods(self) -> None:
         # Read in relperm properties from Nexus relperm method files
         if self.__files is not None and len(self.__files) > 0:  # Check if relperm files exist
             for table_num in self.__files.keys():  # For each relperm property method
                 relperm_file = self.__files[table_num]
                 if relperm_file.location is None:
                     raise ValueError(f'Unable to find relperm file: {relperm_file}')
                 if os.path.isfile(relperm_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusReporting.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusReporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     table_footer = 'ENDOUTPUT'
 
     def __init__(self, model: NexusSimulator, assume_loaded: bool = False) -> None:
         """Initialises the NexusReporting class.
 
         Args:
             model (NexusSimulator): The Nexus model to get the reporting information from.
+            assume_loaded(bool): Create the object assuming the file has already been loaded into memory.
         """
         super().__init__(model)
         self.__model: NexusSimulator = model
         self.__add_object_operations = AddObjectOperations(NexusOutputRequest, self.table_header, self.table_footer,
                                                            model)
         if assume_loaded:
             self.__load_status = True
@@ -70,23 +71,23 @@
     @property
     def array_output_contents(self) -> list[NexusOutputContents]:
         """Gets the contents requested to be output for the arrays."""
         if not self.__load_status:
             self.load_output_requests()
         return self.__array_output_contents
 
-    def add_map_properties_to_start_of_grid_file(self):
+    def add_map_properties_to_start_of_grid_file(self) -> None:
         """Adds 'map' statements to the start of the grid file to ensure standalone outputs all the required \
         properties. Writes out to the same structured grid file path provided.
 
         Raises:
             ValueError: if no structured grid file path is specified in the class instance
         """
         structured_grid_path = self.__model.structured_grid_path
-        if self.__model.structured_grid_path is None:
+        if structured_grid_path is None:
             raise ValueError("No file path given or found for structured grid file path. \
                 Please update structured grid file path")
         file = nfo.load_file_as_list(structured_grid_path)
 
         if not fo.value_in_file('MAPBINARY', file):
             new_file = ['MAPBINARY\n']
         else:
@@ -249,16 +250,21 @@
         """Adds an output request to the array output requests list.
 
         Args:
             output_request (NexusOutputRequest): The output request to add the model and associated in memory files.
         """
         if self.__model.model_files.runcontrol_file is None:
             raise ValueError("No file found for runcontrol file path.")
+
+        if output_request.date is None:
+            raise ValueError(f"No date on NexusOutputRequest object: {output_request}")
+
         file_as_list = self.__model.model_files.runcontrol_file.get_flat_list_str_file
         obj_props = output_request.to_dict(add_units=False)
+
         self.__add_object_operations.add_object_to_file(date=output_request.date,
                                                         file_as_list=file_as_list,
                                                         file_to_add_to=self.__model.model_files.runcontrol_file,
                                                         new_object=output_request,
                                                         object_properties=obj_props,
                                                         skip_reading_headers=True,
                                                         )
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusRockMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusRockMethods.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             self.load_rock_methods()
         return self.__inputs
 
     @property
     def files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_rock_methods(self):
+    def load_rock_methods(self) -> None:
         # Read in rock properties from Nexus rock method files
         if self.__files is not None and len(self.__files) > 0:  # Check if rock files exist
             for table_num in self.__files.keys():  # For each rock property method
                 rock_file = self.__files[table_num]
                 if rock_file.location is None:
                     raise ValueError(f'Unable to find rock file: {rock_file}')
                 if os.path.isfile(rock_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusSeparatorMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusSeparatorMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             self.load_separator_methods()
         return self.__inputs
 
     @property
     def files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_separator_methods(self):
+    def load_separator_methods(self) -> None:
         # Read in separator properties from Nexus separator method files
         if self.__files is not None and len(self.__files) > 0:  # Check if separator files exist
             for table_num in self.__files.keys():  # For each separator property method
                 separator_file = self.__files[table_num]
                 if separator_file.location is None:
                     raise ValueError(f'Unable to find separator file: {separator_file}')
                 if os.path.isfile(separator_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusSimulator.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusSimulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,23 @@
     def __init__(self, origin: Optional[str] = None, destination: Optional[str] = None,
                  root_name: Optional[str] = None, nexus_data_name: str = "data", write_times: bool = False,
                  manual_fcs_tidy_call: bool = False, lazy_loading: bool = True) -> None:
         """Nexus simulator class. Inherits from the Simulator super class.
 
         Args:
             origin (Optional[str], optional): file path to the fcs file. Defaults to None.
+            destination (Optional[str], optional): The location to move the model to.
             root_name (Optional[str], optional): Root file name of the fcs. Defaults to None.
             nexus_data_name (str, optional): Folder name for the nexus data files to be stored in. Defaults to "data".
             write_times (bool, optional): Sets whether the runcontrol file will expand the include files with time \
                 cards in. Defaults to True.
             manual_fcs_tidy_call (bool, optional): Determines whether fcs_tidy should be called - Currently not used. \
                 Defaults to False.
+            lazy_loading(bool): If set to True, parts of the model will only be loaded in when requested via \
+                properties on the object.
 
         Attributes:
             run_control_file_path (Optional[str]): file path to the run control file - derived from the fcs file
             __destination (Optional[str]): output path for the simulation. Currently not used.
             date_format (DateFormat): Enum value representing the date format.
             __original_fcs_file_path (str): Path to the original fcs file path supplied
             __new_fcs_file_path (str): Where the new fcs will be saved to
@@ -210,33 +213,34 @@
                 # if base_class_tuple and other_class_tuple both return empty tuple, that means both of them /
                 # have no network constraints or wells completions
                 raise ValueError("Both models have empty network constraints or wells completions. Unable to compare.")
             return self.network_wells_tuple() == other.network_wells_tuple()
         raise TypeError(f"Unable to compare {type(self)} with {other}. Ensure that {other} is of type NexusSimulator. "
                         f"{other} has {type(other)}")
 
-    def remove_temp_from_properties(self):
+    def remove_temp_from_properties(self) -> None:
         """Updates model values if the files are moved from a temp directory
         Replaces the first instance of temp/ in the file paths in the nexus simulation file paths.
 
         Raises:
             ValueError: if any of [__structured_grid_file_path, __new_fcs_file_path, __surface_file_path] are None.
         """
-        if self.model_files.structured_grid_file.location is None:
+        if self.model_files.structured_grid_file is None or self.model_files.structured_grid_file.location is None:
             raise ValueError(
                 "No structured_grid_file_path found, can't remove temporary properties from file path")
         if self.__new_fcs_file_path is None:
             raise ValueError(
                 "No __new_fcs_file_path found, can't remove temporary properties from file path")
-        if self.model_files.surface_files[1] is None or self.model_files.surface_files[1].location is None:
+        if self.model_files.surface_files is None or self.model_files.surface_files[1] is None \
+                or self.model_files.surface_files[1].location is None:
             raise ValueError(
                 "No __surface_file_path found, can't remove temporary properties from file path")
 
         self._origin = self._origin.replace('temp/', '', 1)
-        self.__root_name = self.__root_name.replace('temp/', '', 1)
+        self.__root_name = '' if self.root_name is None else self.root_name.replace('temp/', '', 1)
         self.model_files.structured_grid_file.location = \
             self.model_files.structured_grid_file.location.replace('temp/', '', 1)
         self.__new_fcs_file_path = self.__new_fcs_file_path.replace('temp/', '', 1)
         self.model_files.surface_files[1].location = self.model_files.surface_files[1].location.replace('temp/', '', 1)
 
     def get_simulation_status(self, from_startup: bool = False) -> Optional[str]:
         return self.logging.get_simulation_status(from_startup)
@@ -252,47 +256,47 @@
         return self._model_files
 
     @property
     def network(self) -> NexusNetwork:
         return self._network
 
     @property
-    def structured_grid_path(self):
+    def structured_grid_path(self) -> Optional[str]:
         """Returns the location of the structured grid file."""
-        return self.model_files.structured_grid_file.location
+        return None if self.model_files.structured_grid_file is None else self.model_files.structured_grid_file.location
 
     @property
-    def default_units(self):
+    def default_units(self) -> UnitSystem:
         """Returns the default units."""
         return self._default_units
 
     @property
-    def run_units(self):
+    def run_units(self) -> UnitSystem:
         """Returns the run units."""
         return self.__run_units
 
     @property
-    def new_fcs_name(self):
+    def new_fcs_name(self) -> Optional[str]:
         """Returns the new name for the FCS file without the fcs extension."""
         return self.__root_name
 
     @property
     def write_times(self) -> bool:
         return self.__write_times
 
     @property
-    def original_fcs_file_path(self):
+    def original_fcs_file_path(self) -> str:
         return self.__original_fcs_file_path
 
     @property
-    def root_name(self):
+    def root_name(self) -> Optional[str]:
         return self.__root_name
 
     @root_name.setter
-    def root_name(self, value: str) -> None:
+    def root_name(self, value: Optional[str]) -> None:
         """Returns the name of the fcs file without the .fcs extension.
 
         Returns:
             str: string of the fcs file without the .fcs extension.
         """
         if value is not None:
             rootname = value
@@ -648,15 +652,15 @@
                 file.append('\n' + token_line)
 
         new_file_str = "".join(file)
 
         with open(file_path, "w") as text_file:
             text_file.write(new_file_str)
 
-    def update_fcs_file_value(self, token: str, new_value: str, add_to_start: bool = False):
+    def update_fcs_file_value(self, token: str, new_value: str, add_to_start: bool = False) -> None:
         """Updates a value in the FCS file."""
         self.update_file_value(self.__new_fcs_file_path, token=token, new_value=new_value, add_to_start=add_to_start)
 
     @staticmethod
     def comment_out_file_value(token: str, file_path: str) -> None:
         """Comments out an uncommented line containing the specified token.
 
@@ -684,15 +688,15 @@
 
     def get_date_format(self) -> str:
         """Returns the date format being used by the model
         formats used: ('MM/DD/YYYY', 'DD/MM/YYYY').
         """
         return self._sim_controls.get_date_format(self.date_format)
 
-    def modify(self, operation: str, section: str, keyword: str, content: list[str]):
+    def modify(self, operation: str, section: str, keyword: str, content: list[str]) -> None:
         """Generic modify method to modify part of the input deck. \
         Operations are dependent on the section being modified.
 
         Args:
             operation (str): operation to perform on the section of the input deck (e.g. 'merge')
             section (str): file type from the input deck provided (e.g. RUNCONTROL)
             keyword (str): which keyword/token to find within the deck provided (e.g. TIME)
@@ -739,32 +743,32 @@
 
     def get_structured_grid_dict(self) -> dict[str, Any]:
         """Convert the structured grid info to a dictionary and pass it to the front end."""
         if self._grid is None:
             return {}
         return self._grid.to_dict()
 
-    def get_abs_structured_grid_path(self, filename: str):
+    def get_abs_structured_grid_path(self, filename: str) -> str:
         """Returns the absolute path to the Structured Grid file."""
         if self.model_files.structured_grid_file is None:
             raise ValueError(
                 f"No structured grid file found within simulator class: {self.model_files.structured_grid_file}")
         grid_path = self.model_files.structured_grid_file.location
         if grid_path is None:
             raise ValueError("No path found for structured grid file path. \
                 Please provide a path to the structured grid")
         return os.path.dirname(grid_path) + '/' + filename
 
-    def get_surface_file_path(self):
+    def get_surface_file_path(self) -> str:
         """Get the surface file path."""
         if self.model_files.surface_files is None or self.model_files.surface_files[1] is None:
             raise ValueError('No path found for surface file.')
         return self.model_files.surface_files[1].location
 
-    def load_network(self):
+    def load_network(self) -> None:
         """Populates nodes and connections from a surface file."""
         self._network.load()
 
     def write_out_case(self, new_file_path: str, new_include_file_location: str = 'include_files',
                        case_suffix: str = '') -> None:
         """Creates a new case of a simulator run by writing out the modified include files to a new file.
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusSolverParameters.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusSolverParameters.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusValveMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusValveMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             self.load_valve_methods()
         return self.__inputs
 
     @property
     def valve_files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_valve_methods(self):
+    def load_valve_methods(self) -> None:
         # Read in valve properties from Nexus valve method files
         if self.__files is not None and len(self.__files) > 0:  # Check if valve files exist
             for table_num in self.__files.keys():  # For each valve property method
                 valve_file = self.__files[table_num]
                 if valve_file.location is None:
                     raise ValueError(f'Unable to find valve file: {valve_file}')
                 if os.path.isfile(valve_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusWaterMethods.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusWaterMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             self.load_water_methods()
         return self.__inputs
 
     @property
     def files(self) -> dict[int, NexusFile]:
         return self.__files
 
-    def load_water_methods(self):
+    def load_water_methods(self) -> None:
         # Read in water properties from Nexus water method files
         if self.__files is not None and len(self.__files) > 0:  # Check if water files exist
             for table_num in self.__files.keys():  # For each water property method
                 water_file = self.__files[table_num]
                 if water_file.location is None:
                     raise ValueError(f'Unable to find water file: {water_file}')
                 if os.path.isfile(water_file.location):
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/NexusWells.py` & `ressimpy-2.2.0/ResSimpy/Nexus/NexusWells.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """A class for collecting all NexusWell objects in a NexusSimulator. Handles adding and removing completions
     as well as rescheduling wells. This is usually accessed through the model.wells property.
 
     Arguments:
         model (Simulator): NexusSimulator object that has the instance of wells on.
     """
     __model: NexusSimulator = field(compare=False, repr=False)
-    __date_format: DateFormat = field(repr=False)
+    __date_format: DateFormat = DateFormat.MM_DD_YYYY
     _wells: list[NexusWell] = field(default_factory=list)
 
     def __init__(self, model: NexusSimulator) -> None:
         """Initialises the NexusWells class.
 
         Args:
             model (NexusSimulator): The model object that contains this NexusWells instance.
@@ -56,14 +56,15 @@
 
     @property
     def start_date(self) -> str:
         return self.__model.start_date
 
     @property
     def date_format(self) -> DateFormat:
+        # If we haven't loaded in the wells file, load it in case date format is specified there.
         if not self._wells_loaded:
             self._load()
         return self.__date_format
 
     @property
     def table_header(self) -> str:
         return 'WELLSPEC'
@@ -159,21 +160,21 @@
                 raise ValueError('Please select one of the valid OperationEnum values: e.g. OperationEnum.ADD')
 
     def add_completion(self, well_name: str, completion_properties: dict[str, None | float | int | str],
                        preserve_previous_completions: bool = True, comments: Optional[str] = None) -> None:
         """Adds a completion to an existing wellspec file.
 
         Args:
-        ----
             well_name (str): well name to update
-            completion_properties (dict[str, float | int | str]: properties of the completion you want to update.
+            completion_properties (dict[str, float | int | str]): properties of the completion you want to update.
             Must contain date of the completion to be added.
             preserve_previous_completions (bool): if true a new perforation added on a TIME card without a \
             wellspec card for that well will preserve the previous completions from the closest TIME card in addition \
             to the new completion
+            comments (Optional[str]): Comments to add to the object line in the file.
         """
         basic_dict: dict[str, float | int | str | None] = {'name': well_name}
         _, completion_date = self.__add_object_operations.check_name_date(basic_dict | completion_properties)
         well = self.get(well_name)
         if well is None:
             # TODO could make this not raise an error and instead initialize a NexusWell and add it to NexusWells
             raise ValueError(
@@ -405,14 +406,15 @@
 
         Args:
             well_name (str): Name of the well with the completion to be modified.
             properties_to_modify (dict[str, None | float | int | str]): attributes to change to.
             completion_to_change (Optional[dict[str, None | float | int | str]]): properties of the existing completion.
             User must provide enough to uniquely identify the completion.
             completion_id (Optional[UUID]): If provided will match against a known UUID for the completion.
+            comments (Optional[str]): Comments to add to the object line in the file.
         """
         well = self.get(well_name)
         if well is None:
             raise ValueError(f'No well found with name: {well_name}')
 
         if completion_to_change is not None:
             completion = well.find_completion(completion_to_change)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/array_function_operations.py` & `ressimpy-2.2.0/ResSimpy/Nexus/array_function_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/load_wells.py` & `ressimpy-2.2.0/ResSimpy/Nexus/load_wells.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                model_date_format: DateFormat) -> tuple[Sequence[NexusWell], DateFormat]:
     """Loads a list of Nexus Well instances and populates it with the wells completions over time from a wells file.
 
     Args:
         nexus_file (NexusFile): NexusFile containing the wellspec files.
         start_date (str): starting date of the wellspec file as a string.
         default_units (UnitSystem): default units to use if no units are found.
+        parent_wells_instance (NexusWells): The NexusWells object this function will load the wells into.
         model_date_format (DateFormat): Date format specified in the FCS file.
 
     Raises:
         ValueError: If no value is found after a TIME card.
         ValueError: If no well name is found after a WELLSPEC keyword.
         ValueError: If no valid wells are found in the wellspec file.
 
@@ -248,14 +249,15 @@
                                       unit_system: UnitSystem,
                                       start_date: None | str = None,
                                       ) -> list[NexusCompletion]:
     """Loads a completion table in for a single WELLSPEC keyword. \
         Loads in the next available completions following a WELLSPEC keyword and a header line.
 
     Args:
+        nexus_file (NexusFile): The Nexus file containing the completions.
         header_index (int): index number of the header in the file as list parameter
         header_values (dict[str, Union[Optional[int], Optional[float], Optional[str]]]): dictionary of column \
             headings to populate from the table
         headers (list[str]): list of strings containing the headers from the wellspec table
         date (str): date to populate the completion class with.
         end_point_scaling_header_values (dict): dictionary containing the header values for thes special end point
         scaling columns.
@@ -413,14 +415,16 @@
     `WELLMOD well_name KH CON value`.
 
     Args:
         line (str): line to extract the wellmod from
         current_date (str): current date in the file
         unit_system (UnitSystem | None): Unit system enum
         wells_loaded (list[NexusWell]): list of wells loaded, used for determining the number of completions in the well
+        start_date (str): The model start date.
+        date_format (DateFormat): The date format.
     """
     keyword_mapping = NexusWellMod.get_keyword_mapping()
     next_value = nfo.get_next_value(0, [line], line)
     counter = 0
     prop: None | str = None
     method: None | str = None
     well_mod_dict: dict[str, None | float | int | str | list[float]] = \
@@ -471,24 +475,27 @@
                              line: str) -> int:
     """Returns the number of completions for a given well name.
 
     Args:
         well_name (str | None): name of the well to find the number of completions for
         current_date (str): current date in the file
         wells_loaded (list[NexusWell]): list of wells loaded, used for determining the number of completions in the well
+        current_iso_date (ISODateTime): The date of the completion in ISO format.
+        line (str): The line in the file.
 
     Returns:
         int: number of completions for a given well name.
     """
     if well_name is None:
         raise ValueError(f"No well name found for the wellmod in the wellspec file in line:\n{line}")
     number_completions = 0
     for well in wells_loaded:
         if well.well_name.upper() != well_name.upper():
             continue
 
-        completion_dates = [x.iso_date for x in well.completions if x.iso_date <= current_iso_date]
+        completion_dates = [x.iso_date for x in well.completions if x.iso_date is not None and x.iso_date
+                            <= current_iso_date]
         # get the most recent completions
         number_completions = len([x for x in completion_dates if x == max(completion_dates)])
         break
 
     return number_completions
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/logfile_operations.py` & `ressimpy-2.2.0/ResSimpy/Nexus/logfile_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,16 +153,16 @@
         Returns:
             Optional[str]: The path of the .log file from the simulation if found. If not found returns None.
         """
         folder_path = os.path.dirname(
             self.__model.original_fcs_file_path) if from_startup else os.path.dirname(self.__model.origin)
         files = os.listdir(folder_path)
         original_fcs_file_location = os.path.basename(self.__model.original_fcs_file_path)
-        log_file_name = os.path.splitext(original_fcs_file_location)[
-                            0] + ".log" if from_startup else self.__model.root_name + ".log"
+        log_file_name = os.path.splitext(original_fcs_file_location)[0] + ".log" if from_startup \
+            or self.__model.root_name is None else self.__model.root_name + ".log"
 
         if log_file_name in files:
             if from_startup:
                 file_location = folder_path
             else:
                 file_location = self.__model.destination if self.__model.destination is not None else folder_path
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/nexus_add_new_object_to_file.py` & `ressimpy-2.2.0/ResSimpy/Nexus/nexus_add_new_object_to_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/nexus_collect_tables.py` & `ressimpy-2.2.0/ResSimpy/Nexus/nexus_collect_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     Args:
     ----
     nexus_file (File): NexusFile representation of the file.
     table_object_map (dict[str, Storage_Object]): dictionary containing the name of the table as keys and \
                 the object type to store the data from each row into. Require objects to have a get_keyword_mapping \
                 function
     model: (NexusSimulator): main simulator object
+    start_date (Optional[str]): The model start date.
+    default_units (Optional[UnitSystem]): The default unit system the Nexus model is set to.
 
     Raises:
     ------
     TypeError: if the unit system found in the property check is not a valid enum UnitSystem.
 
     Returns:
     -------
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/nexus_constraint_operations.py` & `ressimpy-2.2.0/ResSimpy/Nexus/nexus_constraint_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         file_as_list (list[str]): file represented as a list of strings
         constraint (NexusConstraint): object to store the attributes extracted from each row.
         current_date (str): the current date in the table
         unit_system (UnitSystem): Unit system enum
         property_map (dict[str, tuple[str, type]]): Mapping of nexus keywords to attributes
         existing_constraints (dict[str, NexusConstraint]): all existing constraints from previous lines of the \
             surface file
+        nexus_file (File): The Nexus file containing the constraints.
+        start_line_index (int): The index of the line in the file to start loading from.
         network_names (Optional[list[str]]): list of names for all nodes, wells and connections in a nexus network.
             Used in deriving constraints from wildcards. Defaults to None
 
     Returns:
     -------
         dict[UUID, int]: dictionary of object locations derived from inline table.
     """
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/nexus_file_operations.py` & `ressimpy-2.2.0/ResSimpy/Nexus/nexus_file_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import re
 from enum import Enum
 from io import StringIO
 from string import Template
 from typing import Optional, Union, Any
 
+import numpy as np
 import pandas as pd
 
 from ResSimpy.Enums.UnitsEnum import UnitSystem, TemperatureUnits, SUnits
 from ResSimpy.FileOperations.file_operations import get_next_value, check_token, get_expected_token_value, \
     strip_file_of_comments, load_file_as_list
 from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 from ResSimpy.Nexus.NexusKeywords.nexus_keywords import VALID_NEXUS_KEYWORDS
@@ -82,15 +83,15 @@
         # If we are not on the first line, we can search the whole line
         first_line = False
 
     # Start of file reached, no values found
     return None
 
 
-def create_templated_file(template_location: str, substitutions: dict, output_file_name: str):
+def create_templated_file(template_location: str, substitutions: dict, output_file_name: str) -> None:
     """Creates a new text file at the requested destination substituting the supplied values.
 
     Args:
         template_location (str): path to the template file
         substitutions (dict): dictionary of substitutions to be made {variable: subsistuted_value,}
         output_file_name (str): path/name of the file to write out to
     """
@@ -225,15 +226,15 @@
     value = value.replace("\t", "")
     return value
 
 
 def check_for_and_populate_common_input_data(
         file_as_list: list[str],
         property_dict: dict[str,
-                            Union[str, int, float, Enum, list[str], pd.DataFrame,
+                            Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                   dict[str, Union[float, pd.DataFrame]]]]
 ) -> None:
     """Loop through lines of Nexus input file content looking for common input data, e.g.,
     units such as ENGLISH or METRIC, temperature units such as FAHR or CELSIUS, DATEFORMAT, etc.,
     as defined in Nexus manual. If any found, include in provided property_dict and return.
 
     Args:
@@ -247,15 +248,15 @@
         # Check for description
         check_property_in_line(line, property_dict, file_as_list)
 
 
 def check_property_in_line(
         line: str,
         property_dict: dict[str,
-                            Union[str, int, float, Enum, list[str], pd.DataFrame,
+                            Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                   dict[str, Union[float, pd.DataFrame]]]], file_as_list: list[str]) -> None:
     """Given a line of Nexus input file content looking for common input data, e.g.,
     units such as ENGLISH or METRIC, temperature units such as FAHR or CELSIUS, DATEFORMAT, etc.,
     as defined in Nexus manual. If any found, include in provided property_dict and return.
 
     Args:
     line (str): line to search for the common input data
@@ -456,21 +457,20 @@
                 if new_object_date is not None and new_object_date == current_date:
                     # otherwise just update the object inplace and don't add it to the return list
                     existing_constraint.update(keyword_store)
                     # add just the id back in to track the lines where it came from in the file
                     return_objects.append((existing_constraint.id, index))
                     continue
                 else:
-                    new_object = row_object(keyword_store)
+                    new_object = row_object(properties_dict=keyword_store, date=current_date, unit_system=unit_system)
             else:
-                new_object = row_object(keyword_store)
+                new_object = row_object(properties_dict=keyword_store, date=current_date, unit_system=unit_system)
         else:
-            new_object = row_object(keyword_store)
-        setattr(new_object, 'date', current_date)
-        setattr(new_object, 'unit_system', unit_system)
+            new_object = row_object(properties_dict=keyword_store, date=current_date, unit_system=unit_system)
+
         return_objects.append((new_object, index))
     return return_objects
 
 
 def check_list_tokens(list_tokens: list[str], line: str) -> Optional[str]:
     """Checks a list of tokens for whether it exists in a string and returns the token that matched.
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/nexus_load_well_list.py` & `ressimpy-2.2.0/ResSimpy/Nexus/nexus_load_well_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                     previous_well_lists: None | list[NexusWellList] = None,
                     table_start_index: int = 0) -> list[tuple[NexusWellList, int]]:
     """Loads a well list from a surface network file.
 
     Args:
         file_as_list (list[str]): The surface network file as a list of strings.
         current_date (None | str): The current date of the simulation.
-        previous_well_lists (None | list[tuple[NexusWellList, int]]):
+        previous_well_lists (None | list[tuple[NexusWellList, int]]): ??
         The list of tuples of already loaded in NexusWellLists with their starting index. Defaults to None.
         table_start_index (int): The starting index of the table. Defaults to 0.
 
     Returns:
         NexusWellList: A NexusWellList object containing the well list data.
     """
     if previous_well_lists is None:
@@ -55,14 +55,15 @@
                               previous_well_list: NexusWellList | None = None) -> NexusWellList:
     """Loads a well list from a table taken from a surface network file.
     Currently does not support Wildcards in welllists.
 
     Args:
         well_list_as_list_str (list[str]): The subsection of surface network file as a list of strings.
         current_date (str): The current date of the simulation.
+        well_list_name (str): The name of the well list.
         previous_well_list (NexusWellList | None): The previous well list. Defaults to None.
 
     Returns:
         NexusWellList: A NexusWellList object containing the well list data.
     """
     well_list = previous_well_list.wells.copy() if previous_well_list is not None else []
     operation: OperationEnum | None = None
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/nexus_modify_object_in_file.py` & `ressimpy-2.2.0/ResSimpy/Nexus/nexus_modify_object_in_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,24 @@
         Updates the properties with properties in the new_properties dictionary.
         Applies primarily to network based objects.
 
         Args:
             object_to_modify (dict[str, None | str | float | int]): dictionary containing attributes to match in the
             existing object set. Requires an implemented add, remove
             new_properties (dict[str, None | str | float | int]): properties to switch to in the new object
+            network (NexusNetwork): The network object containing the object to modify.
         """
         # TODO apply this to more of the network attributes through the Base Class
         network_attribute_name = self.object_to_modify._network_element_name
         name = object_to_modify.get('name', None)
         if name is None:
             raise ValueError(f'Name is required for modifying {network_attribute_name}, '
                              f'instead got {name}')
         name = str(name)
         network_element = network.find_network_element_with_dict(name, object_to_modify,
                                                                  network_attribute_name)
-        existing_properties = network_element.to_dict(include_nones=False)
+        existing_properties = network_element.to_dict(include_nones=False, units_as_string=False)
         # do the union of the two dicts
         existing_properties.update(new_properties)
 
         self.object_to_modify.remove(object_to_modify)
         self.object_to_modify.add(existing_properties)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/nexus_remove_object_from_file.py` & `ressimpy-2.2.0/ResSimpy/Nexus/nexus_remove_object_from_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/rel_perm_operations.py` & `ressimpy-2.2.0/ResSimpy/Nexus/rel_perm_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/runcontrol_operations.py` & `ressimpy-2.2.0/ResSimpy/Nexus/runcontrol_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,23 +66,23 @@
         self.__times: None | list[str] = None
         self.__date_format_string: str = ''
         self.__number_of_processors: None | int = None
         self.__grid_to_proc: None | GridToProc = None
         self.__solver_parameters: NexusSolverParameters = NexusSolverParameters(model)
 
     @property
-    def date_format_string(self):
+    def date_format_string(self) -> str:
         return self.__date_format_string
 
     @date_format_string.setter
     def date_format_string(self, value: str) -> None:
         self.__date_format_string = value
 
     @property
-    def times(self):
+    def times(self) -> list[str]:
         return self.__times if self.__times is not None else []
 
     @staticmethod
     def get_times(times_file: list[str]) -> list[str]:
         """Retrieves a list of TIMES from the supplied Runcontrol / Include file.
 
         Args:
@@ -285,15 +285,15 @@
         flat_list.append(stop_string)
         new_file_content.extend(flat_list)
         new_file_str = "".join(new_file_content)
 
         with open(filename, "w") as text_file:
             text_file.write(new_file_str)
 
-    def load_run_control_file(self):
+    def load_run_control_file(self) -> None:
         """Loads the run control information into the class instance. \
             If the write_times attribute is True then it expands out any INCLUDE files with the times found within
         Raises:
             ValueError: if the run_control_file attribute is None.
         """
         if self.__model.model_files.runcontrol_file is None:
             warnings.warn(f"Run control file path not found for {self.__model.model_files.location}")
@@ -335,15 +335,15 @@
             return
         for file in self.__model.model_files.runcontrol_file.include_locations:
             if self.__model.destination is not None:
                 self.remove_times_from_file(run_control_file_content, file)
 
         self.modify_times(content=times, operation='replace')
 
-    def modify_times(self, content: None | list[str] = None, operation: str = 'merge'):
+    def modify_times(self, content: None | list[str] = None, operation: str = 'merge') -> None:
         """Modifies the output times in the simulation.
 
         Args:
         ----
             content (list[str]], optional): The content to modify using the above operation, \
             represented as a list of strings with a new entry per line of the file. Defaults to None.
             operation (str, optional): operation to perform on the content provided (e.g. 'merge'). Defaults to 'merge'.
```

### Comparing `ressimpy-2.1.1/ResSimpy/Nexus/structured_grid_operations.py` & `ressimpy-2.2.0/ResSimpy/Nexus/structured_grid_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,15 @@
 
         Args:
         ----
             file_as_list (list[str]): a list of strings containing each line of the file as a new entry
             old_property (VariableEntry): property found in the original file to be replaced
             new_property (VariableEntry): new property to replace the old property with
             token_name (str): name of the token being replaced
+
         Returns:
             None: modifies the file_as_list with the new property
         """
 
         for line in file_as_list:
             old_token_modifier = f"{token_name} {old_property.modifier}"
             new_token_modifier = f"{token_name} {new_property.modifier}"
```

### Comparing `ressimpy-2.1.1/ResSimpy/Node.py` & `ressimpy-2.2.0/ResSimpy/Node.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Abstract base class for a node in a network."""
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
-from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Units.AttributeMappings.NetworkUnitMapping import NetworkUnits
 
 
 @dataclass(repr=False)
 class Node(DataObjectMixin, ABC):
     name: Optional[str] = None
     type: Optional[str] = None
     depth: Optional[float] = None
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
 
     @property
     def units(self) -> NetworkUnits:
         """Returns the attribute to unit map for the constraint."""
         return NetworkUnits(self.unit_system)
```

### Comparing `ressimpy-2.1.1/ResSimpy/NodeConnection.py` & `ressimpy-2.2.0/ResSimpy/NodeConnection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Base class object for storing data related to nodeconnections."""
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 from ResSimpy.DataObjectMixin import DataObjectMixin
-from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.Units.AttributeMappings.NetworkUnitMapping import NetworkUnits
 
 
 @dataclass(repr=False)
 class NodeConnection(DataObjectMixin, ABC):
     """Base class object for storing data related to nodeconnections."""
     name: Optional[str] = None
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
 
     node_in: Optional[str] = None
     node_out: Optional[str] = None
     con_type: Optional[str] = None
     depth: Optional[float] = None
 
     @property
```

### Comparing `ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py` & `ressimpy-2.2.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py` & `ressimpy-2.2.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py` & `ressimpy-2.2.0/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py` & `ressimpy-2.2.0/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/OpenGoSim/OpenGoSimSimulator.py` & `ressimpy-2.2.0/ResSimpy/OpenGoSim/OpenGoSimSimulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,9 +226,10 @@
         raise NotImplementedError("Not implemented for OGS yet")
 
     def write_out_new_model(self, new_location: str, new_model_name: str) -> None:
         """Writes out a new version of the model to the location supplied.
 
         Args:
         new_location (str): Path to write the contents of the model to.
+        new_model_name (str): The name for the model that will be created.
         """
         raise NotImplementedError("Not implemented for OGS yet")
```

### Comparing `ressimpy-2.1.1/ResSimpy/OperationsMixin.py` & `ressimpy-2.2.0/ResSimpy/OperationsMixin.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/RelPermEndPoint.py` & `ressimpy-2.2.0/ResSimpy/RelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Reporting.py` & `ressimpy-2.2.0/ResSimpy/Reporting.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Rock.py` & `ressimpy-2.2.0/ResSimpy/Rock.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from dataclasses import dataclass
 from abc import ABC
+from typing import Mapping
+
+from ResSimpy.DynamicProperty import DynamicProperty
 
 
 @dataclass(kw_only=True)
 class Rock(ABC):
     """The abstract base class for a collection of rock property inputs.
 
     Attributes:
         inputs (dict[int, DynamicProperty]): Collection of rock property inputs, as a dictionary.
     """
 
     @property
-    def inputs(self):
+    def inputs(self) -> Mapping[int, DynamicProperty]:
         """A Collection of rock property inputs, as a dictionary."""
         raise NotImplementedError("Implement this in the derived class")
 
-    def to_string(self):
+    def to_string(self) -> str:
         raise NotImplementedError('Implement this in the derived class.')
```

### Comparing `ressimpy-2.1.1/ResSimpy/Separator.py` & `ressimpy-2.2.0/ResSimpy/PVT.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from dataclasses import dataclass
 from abc import ABC
+from typing import Mapping
+
+from ResSimpy.DynamicProperty import DynamicProperty
 
 
 @dataclass(kw_only=True)
-class Separator(ABC):
-    """The abstract base class for a collection of separator property inputs.
+class PVT(ABC):
+    """The abstract base class for a collection of PVT inputs.
 
     Attributes:
-        inputs (dict[int, DynamicProperty]): Collection of separator property inputs, as a dictionary.
+        inputs (dict[int, DynamicProperty]): Collection of PVT inputs, as a dictionary.
     """
 
     @property
-    def inputs(self):
-        """A Collection of separator property inputs, as a dictionary."""
-        raise NotImplementedError("Implement this in the derived class.")
-
-    def to_string(self):
-        raise NotImplementedError('Implement this in the derived class.')
+    def inputs(self) -> Mapping[int, DynamicProperty]:
+        """A Collection of PVT inputs, as a dictionary."""
+        raise NotImplementedError("Implement this in the derived class")
```

### Comparing `ressimpy-2.1.1/ResSimpy/Simulator.py` & `ressimpy-2.2.0/ResSimpy/Simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,9 +156,10 @@
 
     @abstractmethod
     def write_out_new_model(self, new_location: str, new_model_name: str) -> None:
         """Writes out a new version of the model to the location supplied.
 
         Args:
         new_location (str): Path to write the contents of the model to.
+        new_model_name (str): The name for the model that will be created.
         """
         raise NotImplementedError("Implement this method on the derived class")
```

### Comparing `ressimpy-2.1.1/ResSimpy/SolverParameters.py` & `ressimpy-2.2.0/ResSimpy/SolverParameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @dataclass
 class SolverParameters(ABC):
     """Abstract base class for storing solver parameter objects and handle loading of these parameters."""
 
     __solver_parameters: Sequence[SolverParameter]
 
     @abstractmethod
-    def load(self):
+    def load(self) -> None:
         """Loads the solver parameters given to the simulator."""
         raise NotImplementedError("Implement this in the derived class.")
 
     @property
     @abstractmethod
     def solver_parameters(self) -> Sequence[SolverParameter]:
         return self.__solver_parameters
```

### Comparing `ressimpy-2.1.1/ResSimpy/Target.py` & `ressimpy-2.2.0/ResSimpy/Target.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from __future__ import annotations
-import uuid
 from abc import ABC
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from typing import Optional
 from ResSimpy.DataObjectMixin import DataObjectMixin
-from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.Units.AttributeMappings.NetworkUnitMapping import NetworkUnits
 
 
 @dataclass(repr=False)
 class Target(DataObjectMixin, ABC):
     name: Optional[str] = None
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
 
     control_quantity: Optional[str] = None
     control_conditions: Optional[str] = None
     control_connections: Optional[str] = None
     control_method: Optional[str] = None
     calculation_method: Optional[str] = None
     calculation_conditions: Optional[str] = None
@@ -28,13 +24,12 @@
     minimum_rate: Optional[str] = None
     minimum_rate_no_shut: Optional[float] = None
     guide_rate: Optional[str] = None
     max_change_pressure: Optional[float] = None
     rank_dt: Optional[float] = None
     control_type: Optional[str] = None
     calculation_type: Optional[str] = None
-    __id: uuid.UUID = field(default_factory=lambda: uuid.uuid4(), compare=False)
 
     @property
     def units(self) -> NetworkUnits:
         """Returns the attribute to unit map for the WellConnection."""
         return NetworkUnits(self.unit_system)
```

### Comparing `ressimpy-2.1.1/ResSimpy/Units/AttributeMapping.py` & `ressimpy-2.2.0/ResSimpy/Units/AttributeMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py` & `ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py` & `ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py` & `ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py` & `ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py`

 * *Files identical despite different names*

```diff
@@ -202,14 +202,15 @@
     """Unit types for the attributes of hydraulics, gaslift, valve, etc. methods."""
 
     def __init__(self, unit_system: None | UnitSystem, ratio_thousands: bool = True) -> None:
         """Initialises the HydraulicsUnits class.
 
         Args:
             unit_system (None | UnitSystem): unit system to get the unit from.
+            ratio_thousands (bool): ??
         """
         self.ratio_thousands = ratio_thousands
         super().__init__(unit_system=unit_system)
 
     attribute_map: Mapping[str, UnitDimension] = {
         'surface_oil_rate': SurfaceRatesLiquid(),  # For use in hyd & gaslift methods
         'surface_liquid_rate': SurfaceRatesLiquid(),
```

### Comparing `ressimpy-2.1.1/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py` & `ressimpy-2.2.0/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Units/Units.py` & `ressimpy-2.2.0/ResSimpy/Units/Units.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Utils/factory_methods.py` & `ressimpy-2.2.0/ResSimpy/Utils/factory_methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from enum import Enum
 from typing import TYPE_CHECKING, Union
 from uuid import UUID
 
+import numpy as np
 import pandas as pd
 
 if TYPE_CHECKING:  # pragma: no cover
     from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
     from ResSimpy.Nexus.DataModels.NexusWaterMethod import NexusWaterParams
     from ResSimpy.File import File
 
@@ -14,17 +15,18 @@
 # Factory methods for generating empty lists with typing
 def get_empty_list_str() -> list[str]:
     value: list[str] = []
     return value
 
 
 # Factory method for generating empty dictionary with typing
-def get_empty_dict_union() -> dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+def get_empty_dict_union() -> dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
                                    dict[str, Union[float, pd.DataFrame]]]]:
-    value: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] = {}
+    value: dict[str, Union[str, int, float, Enum, list[str], np.ndarray, pd.DataFrame,
+                           dict[str, Union[float, pd.DataFrame]]]] = {}
     return value
 
 
 # Factory method for generating empty dictionary for eos options
 def get_empty_eosopt_dict_union() -> \
         dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float], tuple[str, dict[str, float]], dict[
             str, pd.DataFrame]]]:
```

### Comparing `ressimpy-2.1.1/ResSimpy/Utils/invert_nexus_map.py` & `ressimpy-2.2.0/ResSimpy/Utils/invert_nexus_map.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Utils/obj_to_table_string.py` & `ressimpy-2.2.0/ResSimpy/Utils/obj_to_table_string.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Utils/to_dict_generic.py` & `ressimpy-2.2.0/ResSimpy/Utils/to_dict_generic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from typing import Any
 
 from ResSimpy.Enums.UnitsEnum import UnitSystem
 
 
 def to_dict(nexus_object: Any, keys_in_nexus_style: bool = False, add_date: bool = True, add_units: bool = True,
-            include_nones: bool = True) -> dict[str, None | str | int | float]:
+            include_nones: bool = True, units_as_string: bool = True) -> dict[str, None | str | int | float]:
     """Returns a dictionary of the attributes of a Nexus object. Requires a nexus mapping dictionary.
         Useful for creating dataframes of objects.
 
     Args:
     ----
         nexus_object (Any): Nexus object with a mapping dictionary defined
         keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the
             attribute name as stored by ressimpy
         add_date (bool): adds a date attribute if it exists
         add_units (bool): adds a units attribute if it exists.
-        include_nones (bool): If False filters the nones out of the dictionary. Defaults to True
+        include_nones (bool): If False filters the nones out of the dictionary. Defaults to True.
+        units_as_string (bool): If set to true, the unit system will be stored as a string in the dictionary.
+            Defaults to True.
 
     Returns:
     -------
         a dictionary keyed by attributes and values as the value of the attribute
     """
     mapping_dict = nexus_object.get_keyword_mapping()
     if keys_in_nexus_style:
@@ -38,15 +40,15 @@
         try:
             unit_sys = getattr(nexus_object, 'unit_system')
         except AttributeError:
             raise AttributeError(
                 'Unit system was requested from the object but does not have a unit system associated with it.'
                 f'Try setting add_units to False. Full contents of the object: {nexus_object}')
         if isinstance(unit_sys, UnitSystem):
-            result_dict['unit_system'] = unit_sys.value
+            result_dict['unit_system'] = unit_sys.value if units_as_string else unit_sys
 
     if hasattr(nexus_object, 'control_mode'):
         result_dict['control_mode'] = getattr(nexus_object, 'control_mode')
 
     if not include_nones:
         result_dict = {k: v for k, v in result_dict.items() if v is not None}
     return result_dict
```

### Comparing `ressimpy-2.1.1/ResSimpy/Well.py` & `ressimpy-2.2.0/ResSimpy/Well.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The abstract base class for all wells."""
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass
-from typing import Optional, Sequence, Union
+from typing import Optional, Sequence
 
 from ResSimpy.Completion import Completion
 from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.Enums.WellTypeEnum import WellType
 
 
 @dataclass
@@ -61,15 +61,15 @@
 
     @property
     def dates_of_completions(self) -> list[str]:
         """Returns a list of dates that the well was changed using a completion."""
 
         dates_changed: list[str] = []
         for completion in self._completions:
-            if completion.date not in dates_changed:
+            if completion.date not in dates_changed and completion.date is not None:
                 dates_changed.append(completion.date)
 
         return dates_changed
 
     @property
     def perforations(self) -> list[Completion]:
         """Returns a list of all of the perforations for the well."""
@@ -111,24 +111,27 @@
     Last Shut-in: {'N/A' if self.last_shutin is None else self.last_shutin.date}
     Dates Changed: {'N/A' if len(self.dates_of_completions) == 0 else printable_dates_of_completions}
     """
 
         return well_info
 
     @property
-    def open_and_shut_events(self) -> list[tuple[str, Union[int, tuple[float, float]]]]:
+    def open_and_shut_events(self) -> list[tuple[str, int | tuple[float, float]]]:
         """Returns a list of dates and values representing either the layer, or the depths of each perforation."""
-        events = []
+        events: list[tuple[str, int | tuple[float, float]]] = []
         using_k_values: Optional[bool] = None
 
         for completion in self._completions:
             is_perforation = completion.completion_is_perforation
             if not is_perforation:
                 continue
             if completion.k is not None and using_k_values is not False:
                 using_k_values = True
-                events.append((completion.date, completion.k))
-            elif completion.depth_to_top is not None and using_k_values is not True:
+                if completion.date is not None:
+                    events.append((completion.date, completion.k))
+            elif completion.depth_to_top is not None and using_k_values is not True \
+                    and completion.depth_to_bottom is not None:
                 using_k_values = False
-                events.append((completion.date, (completion.depth_to_top, completion.depth_to_bottom)))
+                if completion.date is not None:
+                    events.append((completion.date, (completion.depth_to_top, completion.depth_to_bottom)))
 
         return events
```

### Comparing `ressimpy-2.1.1/ResSimpy/WellConnection.py` & `ressimpy-2.2.0/ResSimpy/WellConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
-from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Units.AttributeMappings.NetworkUnitMapping import NetworkUnits
 
 
 @dataclass(repr=False)
 class WellConnection(DataObjectMixin, ABC):
     name: Optional[str] = None
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
 
     bhdepth: Optional[float] = None
     datum_depth: Optional[float] = None
     x_pos: Optional[float] = None
     y_pos: Optional[float] = None
     length: Optional[float] = None
     temperature: Optional[float] = None
```

### Comparing `ressimpy-2.1.1/ResSimpy/WellConnections.py` & `ressimpy-2.2.0/ResSimpy/WellConnections.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/WellLists.py` & `ressimpy-2.2.0/ResSimpy/WellLists.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/ResSimpy/Wellbore.py` & `ressimpy-2.2.0/ResSimpy/Wellbore.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from __future__ import annotations
 
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
-from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Units.AttributeMappings.NetworkUnitMapping import NetworkUnits
 
 
 @dataclass(repr=False)
 class Wellbore(DataObjectMixin, ABC):
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
     name: Optional[str] = None
     diameter: Optional[float] = None
     inner_diameter: Optional[float] = None
     roughness: Optional[float] = None
 
     @property
     def units(self) -> NetworkUnits:
```

### Comparing `ressimpy-2.1.1/ResSimpy/Wellhead.py` & `ressimpy-2.2.0/ResSimpy/Wellhead.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
 from ResSimpy.DataObjectMixin import DataObjectMixin
-from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.Units.AttributeMappings.NetworkUnitMapping import NetworkUnits
 
 
 @dataclass(repr=False)
 class Wellhead(DataObjectMixin, ABC):
     well: Optional[str] = None
     name: Optional[str] = None
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
     wellhead_type: Optional[str] = None
     depth: Optional[float] = None
     x_pos: Optional[float] = None
     y_pos: Optional[float] = None
 
     @property
     def units(self) -> NetworkUnits:
```

### Comparing `ressimpy-2.1.1/ResSimpy/Wells.py` & `ressimpy-2.2.0/ResSimpy/Wells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.1.1/pyproject.toml` & `ressimpy-2.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ResSimpy"
-version = "2.1.1" # Set at build time
+version = "2.2.0" # Set at build time
 description = "A Python library for working with Reservoir Simulator Models."
 authors = ["BP"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["ResSimpy", "Reservoir Engineering"]
 classifiers = [
     "Operating System :: OS Independent",
@@ -58,30 +58,28 @@
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.ruff]
 line-length = 120
 # Rule codes for ruff can be found at: https://beta.ruff.rs/docs/rules/
 select = ["E", "F", "W", "C90", "N",  "UP", "YTT", "ANN", "S", "BLE", "D", "PLE", "PLW", "RUF", "BLE", "ARG", "I",
     "COM", "C4", "PIE", "T20", "PYI", "TID", "INT", "ERA", "PD", "FLY", "NPY"] # To add later: PL, PLR
-ignore = ["UP007",  "ANN101", "N999", "UP035", "S105", "N802", "S106", "S107", "UP015", "ANN401", "ANN102", "D202",
+ignore = ["UP007",  "ANN101", "N999", "UP035", "S105", "N802", "S106", "S107", "UP015", "ANN401", "D202",
     "D105", "D203", "D213", "RUF010", "I001", "B028", "COM812", "PD901",
     # To fix later:
-   "ANN201", # Types
     "C901", # Complexity
-    "D102", "D100", "D103", "D101", "D205", "D401", "D417", "D104", "D106", # Docstrings
-    "FA100", # TODO need to remove references to Union, Optional, capital lettered typing (e.g. List)
+    "D102", "D100", "D103", "D101", "D205", "D401", "D104", "D106", # Docstrings
+    # TODO need to remove references to Union, Optional, capital lettered typing (e.g. List)
              # from typings module.
     ]
 exclude = ["./tests"]
 
 [tool.ruff.pydocstyle]
 # Use Google-style docstrings.
 convention = "google"
 
-
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 autoclasstoc = "*"
 sphinx_rtd_theme = "*"
 sphinx = "^7.2"
```

### Comparing `ressimpy-2.1.1/PKG-INFO` & `ressimpy-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResSimpy
-Version: 2.1.1
+Version: 2.2.0
 Summary: A Python library for working with Reservoir Simulator Models.
 License: Apache-2.0
 Keywords: ResSimpy,Reservoir Engineering
 Author: BP
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

