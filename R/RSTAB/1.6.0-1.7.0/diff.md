# Comparing `tmp/RSTAB-1.6.0.tar.gz` & `tmp/RSTAB-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RSTAB-1.6.0.tar", last modified: Fri May  5 08:23:37 2023, max compression
+gzip compressed data, was "RSTAB-1.7.0.tar", last modified: Mon May 29 07:00:46 2023, max compression
```

## Comparing `RSTAB-1.6.0.tar` & `RSTAB-1.7.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.901231 RSTAB-1.6.0/Examples/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/Examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-05-05 08:23:29.000000 RSTAB-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-05 08:23:29.000000 RSTAB-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-05-05 08:23:37.913231 RSTAB-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9988 2023-05-05 08:23:29.000000 RSTAB-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/BasicObjects/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/material.py
--rw-r--r--   0 runner    (1001) docker     (122)    89338 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/member.py
--rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/memberSet.py
--rw-r--r--   0 runner    (1001) docker     (122)    14897 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/node.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/section.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/Calculate/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Calculate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Calculate/optimizationSettings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/ConcreteDesign/
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ConcreteDesign/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/DynamicLoads/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/DynamicLoads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/DynamicLoads/responseSpectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/Imperfections/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Imperfections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20742 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Imperfections/imperfectionCase.py
--rw-r--r--   0 runner    (1001) docker     (122)     9351 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Imperfections/memberImperfection.py
--rw-r--r--   0 runner    (1001) docker     (122)     9275 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Imperfections/membersetImperfection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/ImportExport/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ImportExport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5650 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ImportExport/exports.py
--rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ImportExport/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8304 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/combinationWizard.py
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/designSituation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9427 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCase.py
--rw-r--r--   0 runner    (1001) docker     (122)   136467 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py
--rw-r--r--   0 runner    (1001) docker     (122)     3957 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCombination.py
--rw-r--r--   0 runner    (1001) docker     (122)    16722 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/resultCombination.py
--rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (122)    23114 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (122)    14699 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/Loads/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/imposedNodalDeformation.py
--rw-r--r--   0 runner    (1001) docker     (122)    99681 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/memberLoad.py
--rw-r--r--   0 runner    (1001) docker     (122)   113024 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/membersetload.py
--rw-r--r--   0 runner    (1001) docker     (122)    22037 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/nodalLoad.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/Reports/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32882 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/favicon32.png
--rw-r--r--   0 runner    (1001) docker     (122)    10352 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/html.py
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/htmlScript.js
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/htmlStyles.css
--rw-r--r--   0 runner    (1001) docker     (122)     2158 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/partsList.py
--rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/printoutReport.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/Results/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Results/designOverview.py
--rw-r--r--   0 runner    (1001) docker     (122)   174365 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Results/resultTables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/SpecialObjects/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SpecialObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SpecialObjects/nodalRelease.py
--rw-r--r--   0 runner    (1001) docker     (122)    10945 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SpecialObjects/structureModification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/SteelDesign/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SteelDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SteelDesign/steelServiceabilityConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SteelDesign/steelUltimateConfigurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/TimberDesign/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TimberDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TimberDesign/timberUltimateConfigurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/Tools/
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/GetObjectNumbersByType.py
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/ModelCheck.py
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/PlausibilityCheck.py
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/centreOfGravityAndObjectInfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/sectionDialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py
--rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py
--rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForMembers/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberDefinableStiffness.py
--rw-r--r--   0 runner    (1001) docker     (122)     6504 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberEccentricity.py
--rw-r--r--   0 runner    (1001) docker     (122)    33161 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberHinge.py
--rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberNonlinearity.py
--rw-r--r--   0 runner    (1001) docker     (122)     2629 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberResultIntermediatePoints.py
--rw-r--r--   0 runner    (1001) docker     (122)    11825 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberRotationalRestraint.py
--rw-r--r--   0 runner    (1001) docker     (122)    18158 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberShearPanel.py
--rw-r--r--   0 runner    (1001) docker     (122)     6297 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberStiffnessModification.py
--rw-r--r--   0 runner    (1001) docker     (122)     4100 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberSupport.py
--rw-r--r--   0 runner    (1001) docker     (122)     5685 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberTransverseStiffeners.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForNodes/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForNodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4332 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForNodes/nodalSupport.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForSpecialObjects/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSpecialObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    44487 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSpecialObjects/nodalReleaseType.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/
--rw-r--r--   0 runner    (1001) docker     (122)     5381 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10495 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py
--rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7941 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py
--rw-r--r--   0 runner    (1001) docker     (122)    11534 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberServiceClass.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/
--rw-r--r--   0 runner    (1001) docker     (122)     8964 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/ConcreteDurability.py
--rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2943 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/baseData.py
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/baseSettings.py
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/dataTypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)   124006 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     5007 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/globalParameter.py
--rw-r--r--   0 runner    (1001) docker     (122)    23148 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/initModel.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/suds_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4182 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 08:23:37.913231 RSTAB-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-05-05 08:23:29.000000 RSTAB-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.169124 RSTAB-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.149123 RSTAB-1.7.0/Examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/Examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-05-29 07:00:27.000000 RSTAB-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-29 07:00:27.000000 RSTAB-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-05-29 07:00:46.165123 RSTAB-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9988 2023-05-29 07:00:27.000000 RSTAB-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.149123 RSTAB-1.7.0/RSTAB/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.153123 RSTAB-1.7.0/RSTAB/BasicObjects/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/BasicObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/BasicObjects/material.py
+-rw-r--r--   0 runner    (1001) docker     (122)    89338 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/BasicObjects/member.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/BasicObjects/memberSet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14897 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/BasicObjects/node.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/BasicObjects/section.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.153123 RSTAB-1.7.0/RSTAB/Calculate/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Calculate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Calculate/optimizationSettings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.153123 RSTAB-1.7.0/RSTAB/ConcreteDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/ConcreteDesign/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.153123 RSTAB-1.7.0/RSTAB/DynamicLoads/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/DynamicLoads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6414 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/DynamicLoads/responseSpectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.153123 RSTAB-1.7.0/RSTAB/Imperfections/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Imperfections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20826 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Imperfections/imperfectionCase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9351 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Imperfections/memberImperfection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9275 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Imperfections/membersetImperfection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.157123 RSTAB-1.7.0/RSTAB/ImportExport/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/ImportExport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5650 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/ImportExport/exports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/ImportExport/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.157123 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8304 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/combinationWizard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/designSituation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9427 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/loadCase.py
+-rw-r--r--   0 runner    (1001) docker     (122)   136467 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3996 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/loadCombination.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16722 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/resultCombination.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4458 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23114 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14699 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.157123 RSTAB-1.7.0/RSTAB/Loads/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Loads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Loads/imposedNodalDeformation.py
+-rw-r--r--   0 runner    (1001) docker     (122)   100244 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Loads/memberLoad.py
+-rw-r--r--   0 runner    (1001) docker     (122)   113605 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Loads/membersetload.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22041 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Loads/nodalLoad.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.161123 RSTAB-1.7.0/RSTAB/Reports/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32882 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Reports/favicon32.png
+-rw-r--r--   0 runner    (1001) docker     (122)    10352 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Reports/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Reports/htmlScript.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Reports/htmlStyles.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2158 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Reports/partsList.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Reports/printoutReport.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.161123 RSTAB-1.7.0/RSTAB/Results/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Results/designOverview.py
+-rw-r--r--   0 runner    (1001) docker     (122)   187093 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Results/resultTables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.161123 RSTAB-1.7.0/RSTAB/SpecialObjects/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/SpecialObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/SpecialObjects/nodalRelease.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10945 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/SpecialObjects/structureModification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.161123 RSTAB-1.7.0/RSTAB/SteelDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/SteelDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/SteelDesign/steelServiceabilityConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/SteelDesign/steelUltimateConfigurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.161123 RSTAB-1.7.0/RSTAB/TimberDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TimberDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TimberDesign/timberUltimateConfigurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.161123 RSTAB-1.7.0/RSTAB/Tools/
+-rw-r--r--   0 runner    (1001) docker     (122)    19719 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Tools/GetObjectNumbersByType.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Tools/ModelCheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Tools/PlausibilityCheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Tools/centreOfGravityAndObjectInfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/Tools/sectionDialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.161123 RSTAB-1.7.0/RSTAB/TypesForAluminumDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForAluminumDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.165123 RSTAB-1.7.0/RSTAB/TypesForMembers/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberDefinableStiffness.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6504 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberEccentricity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33419 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberHinge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberNonlinearity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2629 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberResultIntermediatePoints.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12272 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberRotationalRestraint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16988 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberShearPanel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6297 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberStiffnessModification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberSupport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5724 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForMembers/memberTransverseStiffeners.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.165123 RSTAB-1.7.0/RSTAB/TypesForNodes/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForNodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4332 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForNodes/nodalSupport.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.165123 RSTAB-1.7.0/RSTAB/TypesForSpecialObjects/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForSpecialObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45059 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForSpecialObjects/nodalReleaseType.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.165123 RSTAB-1.7.0/RSTAB/TypesForSteelDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)     5342 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForSteelDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10573 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10822 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.165123 RSTAB-1.7.0/RSTAB/TypesForTimberDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForTimberDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8021 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11534 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesForTimberDesign/timberServiceClass.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.165123 RSTAB-1.7.0/RSTAB/TypesforConcreteDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesforConcreteDesign/ConcreteDurability.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/TypesforConcreteDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/baseData.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2811 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/baseSettings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/dataTypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)   118624 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5007 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/globalParameter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24001 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/initModel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-05-29 07:00:27.000000 RSTAB-1.7.0/RSTAB/suds_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 07:00:46.153123 RSTAB-1.7.0/RSTAB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-05-29 07:00:46.000000 RSTAB-1.7.0/RSTAB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4182 2023-05-29 07:00:46.000000 RSTAB-1.7.0/RSTAB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:46.000000 RSTAB-1.7.0/RSTAB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 07:00:46.000000 RSTAB-1.7.0/RSTAB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-29 07:00:46.000000 RSTAB-1.7.0/RSTAB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-29 07:00:46.000000 RSTAB-1.7.0/RSTAB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-29 07:00:46.169124 RSTAB-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-05-29 07:00:27.000000 RSTAB-1.7.0/setup.py
```

### Comparing `RSTAB-1.6.0/LICENSE` & `RSTAB-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/PKG-INFO` & `RSTAB-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RSTAB
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python Framework for RSTAB9 Web Services
 Home-page: https://github.com/Dlubal-Software/RSTAB_Python_Client
 Author: Dlubal Software
 Author-email: info@dlubal.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RSTAB Version: 1.6.0 Summary: Python Framework for
+Metadata-Version: 2.1 Name: RSTAB Version: 1.7.0 Summary: Python Framework for
 RSTAB9 Web Services Home-page: https://github.com/Dlubal-Software/
 RSTAB_Python_Client Author: Dlubal Software Author-email: info@dlubal.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
 ****** [Dlubal_Software] Dlubal Software GmbH [![image](https://img.shields.io/
 twitter/follow/dlubal_en?style=social)](https://twitter.com/dlubal_en "Twitter
```

### Comparing `RSTAB-1.6.0/README.md` & `RSTAB-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/BasicObjects/material.py` & `RSTAB-1.7.0/RSTAB/BasicObjects/material.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/BasicObjects/member.py` & `RSTAB-1.7.0/RSTAB/BasicObjects/member.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/BasicObjects/memberSet.py` & `RSTAB-1.7.0/RSTAB/BasicObjects/memberSet.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/BasicObjects/node.py` & `RSTAB-1.7.0/RSTAB/BasicObjects/node.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/BasicObjects/section.py` & `RSTAB-1.7.0/RSTAB/BasicObjects/section.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py` & `RSTAB-1.7.0/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py` & `RSTAB-1.7.0/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/DynamicLoads/responseSpectrum.py` & `RSTAB-1.7.0/RSTAB/DynamicLoads/responseSpectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         clientObject.user_defined_response_spectrum = model.clientModel.factory.create('ns0:response_spectrum.user_defined_response_spectrum')
 
         if user_defined_spectrum:
             for i,j in enumerate(user_defined_spectrum):
                 rsp = model.clientModel.factory.create('ns0:response_spectrum_user_defined_response_spectrum_row')
                 rsp.no = i+1
                 rsp.row = model.clientModel.factory.create('ns0:response_spectrum_user_defined_response_spectrum')
+                clearAttributes(rsp.row)
                 rsp.row.period = user_defined_spectrum[i][0]
                 rsp.row.acceleration = user_defined_spectrum[i][1]
 
                 clientObject.user_defined_response_spectrum.response_spectrum_user_defined_response_spectrum.append(rsp)
 
         # comment
         clientObject.comment = comment
@@ -131,14 +132,15 @@
         # user defined spectrum
         clientObject.user_defined_response_spectrum = model.clientModel.factory.create('ns0:response_spectrum.user_defined_response_spectrum')
 
         for i,j in enumerate(user_defined_spectrum):
             rsp = model.clientModel.factory.create('ns0:response_spectrum_user_defined_response_spectrum_row')
             rsp.no = i+1
             rsp.row = model.clientModel.factory.create('ns0:response_spectrum_user_defined_response_spectrum')
+            clearAttributes(rsp.row)
             rsp.row.period = user_defined_spectrum[i][0]
             rsp.row.acceleration = user_defined_spectrum[i][1]
 
             clientObject.user_defined_response_spectrum.response_spectrum_user_defined_response_spectrum.append(rsp)
 
         # comment
         clientObject.comment = comment
```

### Comparing `RSTAB-1.6.0/RSTAB/Imperfections/imperfectionCase.py` & `RSTAB-1.7.0/RSTAB/Imperfections/imperfectionCase.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
         # Level Imperfections Table
         clientObject.level_imperfections = model.clientModel.factory.create('ns0:array_of_imperfection_case_level_imperfections')
 
         for i in level_imperfections:
             li_proto = model.clientModel.factory.create('ns0:imperfection_case_level_imperfections_row')
             li_proto.no = i['no']
             li_proto.row = model.clientModel.factory.create('ns0:imperfection_case_level_imperfections')
+            clearAttributes(li_proto.row)
             li_proto.row.level = i['level']
             li_proto.row.e_1 = i['e_1']
             li_proto.row.theta_1 = i['theta_1']
             li_proto.row.e_2 = i['e_2']
             li_proto.row.theta_2 = i['theta_2']
             li_proto.row.comment = i['comment']
 
@@ -458,14 +459,15 @@
         # Imperfection Case Items
         clientObject.imperfection_cases_items = model.clientModel.factory.create('ns0:array_of_imperfection_case_imperfection_cases_items')
 
         for i in imperfection_cases:
             li_proto = model.clientModel.factory.create('ns0:imperfection_case_imperfection_cases_items_row')
             li_proto.no = i['no']
             li_proto.row = model.clientModel.factory.create('ns0:imperfection_case_imperfection_cases_items')
+            clearAttributes(li_proto.row)
             li_proto.row.name = i['name']
             li_proto.row.factor = i['factor']
             li_proto.row.operator_type = i['operator_type']
             li_proto.row.comment = i['comment']
 
             clientObject.imperfection_cases_items.imperfection_case_imperfection_cases_items.append(li_proto)
```

### Comparing `RSTAB-1.6.0/RSTAB/Imperfections/memberImperfection.py` & `RSTAB-1.7.0/RSTAB/Imperfections/memberImperfection.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Imperfections/membersetImperfection.py` & `RSTAB-1.7.0/RSTAB/Imperfections/membersetImperfection.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/ImportExport/exports.py` & `RSTAB-1.7.0/RSTAB/ImportExport/exports.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/ImportExport/imports.py` & `RSTAB-1.7.0/RSTAB/ImportExport/imports.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/combinationWizard.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/combinationWizard.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/designSituation.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/designSituation.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCase.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/loadCase.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCombination.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/loadCombination.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         # Items
         clientObject.items = model.clientModel.factory.create('ns0:load_combination.items')
 
         for i,j in enumerate(combination_items):
             mlvlp = model.clientModel.factory.create('ns0:load_combination_items_row')
             mlvlp.no = i+1
             mlvlp.row = model.clientModel.factory.create('ns0:load_combination_items')
+            clearAttributes(mlvlp.row)
             mlvlp.row.factor = combination_items[i][0]
             mlvlp.row.load_case = combination_items[i][1]
             mlvlp.row.action = combination_items[i][2]
             mlvlp.row.is_leading = combination_items[i][3]
 
             clientObject.items.load_combination_items.append(mlvlp)
```

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/resultCombination.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/resultCombination.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,15 @@
             damping_for_cqc_rule (enum): Cqs Damping Rule Enumeration
             constant_d_for_each_mode (float): Constant d for Each Mode
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
         # Check if Spectral Add-on is active.
-        if not GetAddonStatus(model.clientModel, AddOn.spectral_active):
-            SetAddonStatus(model.clientModel, AddOn.spectral_active)
+        SetAddonStatus(model.clientModel, AddOn.spectral_active)
 
         # Client model | Surface
         clientObject = model.clientModel.factory.create('ns0:spectral_analysis_settings')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
```

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py` & `RSTAB-1.7.0/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Loads/imposedNodalDeformation.py` & `RSTAB-1.7.0/RSTAB/Loads/imposedNodalDeformation.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Loads/memberLoad.py` & `RSTAB-1.7.0/RSTAB/Loads/memberLoad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
-from RSTAB.enums import LoadDirectionType, MemberLoadType, MemberLoadDistribution, MemberLoadDirection, MemberLoadDirectionOrientation
+from RSTAB.enums import MemberLoadDirection, MemberLoadType, MemberLoadDistribution, MemberLoadDirection, MemberLoadDirectionOrientation
 from RSTAB.enums import MemberLoadEccentricityHorizontalAlignment, MemberLoadEccentricityVerticalAlignment, MemberLoadEccentricitySectionMiddle
 from RSTAB.enums import MemberLoadAxisDefinitionType, MemberLoadAxisDefinitionAxisOrientation, MemberLoadAxisDefinition
 
 class MemberLoad():
 
     def __init__(self,
                  no: int = 1,
                  load_case_no: int = 1,
                  members_no: str = '1',
-                 load_direction = LoadDirectionType.LOAD_DIRECTION_LOCAL_Z,
+                 load_direction = MemberLoadDirection.LOAD_DIRECTION_LOCAL_Z,
                  magnitude: float = 2000,
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Args:
             no (int): Load Tag
@@ -221,14 +221,15 @@
 
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
@@ -271,27 +272,29 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING_IN_Z":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
@@ -489,14 +492,15 @@
 
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
@@ -539,14 +543,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
@@ -769,14 +774,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
                 mlvlp.row.magnitude_t_c = load_parameter[i][1]
                 mlvlp.row.magnitude_delta_t = load_parameter[i][2]
                 mlvlp.row.magnitude_t_t = load_parameter[i][1]
                 mlvlp.row.magnitude_t_b = load_parameter[i][2]
 
@@ -929,14 +935,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
                 mlvlp.row.magnitude_t_c = load_parameter[i][1]
                 mlvlp.row.magnitude_delta_t = load_parameter[i][2]
                 mlvlp.row.magnitude_t_t = load_parameter[i][1]
                 mlvlp.row.magnitude_t_b = load_parameter[i][2]
 
@@ -1078,14 +1085,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
@@ -1288,14 +1296,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
@@ -1522,14 +1531,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_1 = load_parameter[0]
@@ -1579,14 +1589,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
@@ -1748,14 +1759,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_1 = load_parameter[0]
@@ -1805,14 +1817,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
```

### Comparing `RSTAB-1.6.0/RSTAB/Loads/membersetload.py` & `RSTAB-1.7.0/RSTAB/Loads/membersetload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
-from RSTAB.enums import MemberSetLoadType, LoadDirectionType, MemberSetLoadDistribution, MemberSetLoadDirection, MemberSetLoadDirectionOrientation
+from RSTAB.enums import MemberSetLoadType, MemberSetLoadDirection, MemberSetLoadDistribution, MemberSetLoadDirection, MemberSetLoadDirectionOrientation
 from RSTAB.enums import MemberSetLoadEccentricityHorizontalAlignment, MemberSetLoadEccentricityVerticalAlignment, MemberSetLoadEccentricitySectionMiddle
 from RSTAB.enums import MemberSetLoadAxisDefinitionType, MemberSetLoadAxisDefinitionAxisOrientation, MemberSetLoadAxisDefinition
 
 class MemberSetLoad():
 
     def __init__(self,
                  no: int = 1,
                  load_case_no: int = 1,
                  member_sets: str = '1',
-                 load_direction = LoadDirectionType.LOAD_DIRECTION_LOCAL_Z,
+                 load_direction = MemberSetLoadDirection.LOAD_DIRECTION_LOCAL_Z,
                  magnitude: float = 0.0,
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Args:
             no (int): Load Tag
@@ -237,14 +237,15 @@
                 clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
                 for i,j in enumerate(load_parameter):
                     if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                     mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                     mlvlp.no = i+1
                     mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                    clearAttributes(mlvlp.row)
                     mlvlp.row.distance = load_parameter[i][0]
                     mlvlp.row.magnitude = load_parameter[i][1]
 
                     clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
             elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
                 if len(load_parameter) == 6:
@@ -295,27 +296,29 @@
                 clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
                 for i,j in enumerate(load_parameter):
                     if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                     mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                     mlvlp.no = i+1
                     mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                    clearAttributes(mlvlp.row)
                     mlvlp.row.distance = load_parameter[i][0]
                     mlvlp.row.magnitude = load_parameter[i][1]
 
                     clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
             elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING_IN_Z":
                 clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
                 for i,j in enumerate(load_parameter):
                     if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                     mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                     mlvlp.no = i+1
                     mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                    clearAttributes(mlvlp.row)
                     mlvlp.row.distance = load_parameter[i][0]
                     mlvlp.row.magnitude = load_parameter[i][1]
 
                     clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
@@ -525,14 +528,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             if len(load_parameter) != 6:
@@ -581,14 +585,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
@@ -817,14 +822,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
                 mlvlp.row.magnitude_t_c = load_parameter[i][1]
                 mlvlp.row.magnitude_t_t = load_parameter[i][1]
                 mlvlp.row.magnitude_t_b = load_parameter[i][2]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
@@ -978,14 +984,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
                 mlvlp.row.magnitude_t_c = load_parameter[i][1]
                 mlvlp.row.magnitude_t_t = load_parameter[i][1]
                 mlvlp.row.magnitude_t_b = load_parameter[i][2]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
@@ -1131,14 +1138,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
@@ -1345,14 +1353,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
@@ -1580,14 +1589,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             if len(load_parameter) != 6:
@@ -1646,14 +1656,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
@@ -1818,14 +1829,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             if len(load_parameter) != 6:
@@ -1884,14 +1896,15 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
                 mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
```

### Comparing `RSTAB-1.6.0/RSTAB/Loads/nodalLoad.py` & `RSTAB-1.7.0/RSTAB/Loads/nodalLoad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
-from RSTAB.enums import LoadDirectionType, NodalLoadType, NodalLoadSpecificDirectionType
+from RSTAB.enums import NodalLoadDirection, NodalLoadType, NodalLoadSpecificDirectionType
 
 class NodalLoad():
 
     def __init__(self,
                  no: int = 1,
                  load_case_no: int = 1,
                  nodes_no: str= '1',
-                 load_direction= LoadDirectionType.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W,
+                 load_direction= NodalLoadDirection.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W,
                  magnitude: float = 0.0,
                  comment: str= '',
                  params: dict= None,
                  model = Model):
         """
         Args:
             no (int): Load Tag
@@ -63,15 +63,15 @@
         model.clientModel.service.set_nodal_load(load_case_no, clientObject)
 
     @staticmethod
     def Force(
               no: int= 1,
               load_case_no: int = 1,
               nodes_no: str= '1',
-              load_direction= LoadDirectionType.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W,
+              load_direction= NodalLoadDirection.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W,
               magnitude: float= 0.0,
               force_eccentricity: bool = False,
               specific_direction: bool = False,
               shifted_display: bool = False,
               comment: str= '',
               params: dict = None,
               model = Model):
@@ -206,15 +206,15 @@
         model.clientModel.service.set_nodal_load(load_case_no, clientObject)
 
     @staticmethod
     def Moment(
               no: int= 1,
               load_case_no: int= 1,
               nodes_no: str= '1',
-              load_direction= LoadDirectionType.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W,
+              load_direction= NodalLoadDirection.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W,
               moment_magnitude: float= 0.0,
               specific_direction: bool= False,
               shifted_display: bool= False,
               comment: str = '',
               params: dict = None,
               model = Model):
         """
```

### Comparing `RSTAB-1.6.0/RSTAB/Reports/favicon32.png` & `RSTAB-1.7.0/RSTAB/Reports/favicon32.png`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Reports/html.py` & `RSTAB-1.7.0/RSTAB/Reports/html.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Reports/htmlScript.js` & `RSTAB-1.7.0/RSTAB/Reports/htmlScript.js`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Reports/htmlStyles.css` & `RSTAB-1.7.0/RSTAB/Reports/htmlStyles.css`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Reports/partsList.py` & `RSTAB-1.7.0/RSTAB/Reports/partsList.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Reports/printoutReport.py` & `RSTAB-1.7.0/RSTAB/Reports/printoutReport.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Results/designOverview.py` & `RSTAB-1.7.0/RSTAB/Results/designOverview.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Results/resultTables.py` & `RSTAB-1.7.0/RSTAB/Results/resultTables.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from cmath import inf
 import enum
 from RSTAB.initModel import Model
 from RSTAB.enums import CaseObjectType
 from RSTAB.dataTypes import inf
 
 # We  can't extract lines with description: Extremes, Total, and Average. Those are language dependent.
 # To do it set_settings_program_language() has to be called before calculation and the program needs to be restarted.
@@ -137,2831 +136,2997 @@
 
 class ResultTables():
 
     @staticmethod
     def BuildingStoriesForcesInSpandrels(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_forces_in_spandrels(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_forces_in_spandrels(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def BuildingStoriesForcesInShearWalls(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_forces_in_shear_walls(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_forces_in_shear_walls(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def BuildingStoriesCentresMassRigidity(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_centres_mass_rigidity(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_centres_mass_rigidity(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def BuildingStoriesInterstoryDrifts(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_interstory_drifts(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_interstory_drifts(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def BuildingStoriesStoryActions(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_story_actions(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_building_stories_story_actions(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def CalculationDiagrams(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_calculation_diagrams(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_calculation_diagrams(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def CriticalLoadFactors(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_critical_load_factors(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_critical_load_factors(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def EfeectiveLengthsAndCriticalLoadsByEigenvector(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_efeective_lengths_and_critical_loads_by_eigenvector(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_efeective_lengths_and_critical_loads_by_eigenvector(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def EfeectiveLengthsAndCriticalLoadsByMember(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_efeective_lengths_and_critical_loads_by_member(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_efeective_lengths_and_critical_loads_by_member(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def EigenvectorsByMember(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_eigenvectors_by_member(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_eigenvectors_by_member(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def EigenvectorsByNode(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_eigenvectors_by_node(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_eigenvectors_by_node(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def EigenvectorsBySolid(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_eigenvectors_by_solid(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_eigenvectors_by_solid(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def EigenvectorsBySurface(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_eigenvectors_by_surface(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_eigenvectors_by_surface(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def Errors(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_errors(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_errors(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def LineHingesDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_line_hinges_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_line_hinges_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def LineHingesForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_line_hinges_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_line_hinges_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def LinesSlabWallConnections(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_lines_slab_wall_connections(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_lines_slab_wall_connections(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def LinesSupportForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_lines_support_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_lines_support_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersByEigenvector(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_by_eigenvector(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_by_eigenvector(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersContactForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_contact_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_contact_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersGlobalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_global_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_global_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersHingeDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_hinge_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_hinge_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersHingeForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_hinge_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_hinge_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersInternalForcesByMemberSet(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_internal_forces_by_member_set(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_internal_forces_by_member_set(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersInternalForcesBySection(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_internal_forces_by_section(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_internal_forces_by_section(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersLocalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_local_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_local_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def MembersStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_members_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisEffectiveModalMasses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_effective_modal_masses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_effective_modal_masses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisMassesInLocations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_masses_in_locations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_masses_in_locations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisMembersByModeShape(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_members_by_mode_shape(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_members_by_mode_shape(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisModeShapesByMember(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_mode_shapes_by_member(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_mode_shapes_by_member(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisModeShapesByNode(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_mode_shapes_by_node(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_mode_shapes_by_node(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisModeShapesBySolid(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_mode_shapes_by_solid(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_mode_shapes_by_solid(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisModeShapesBySurface(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_mode_shapes_by_surface(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_mode_shapes_by_surface(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisNaturalFrequencies(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_natural_frequencies(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_natural_frequencies(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisNodesByModeShape(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_nodes_by_mode_shape(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_nodes_by_mode_shape(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisParticipationFactors(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_participation_factors(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_participation_factors(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisSolidsByModeShape(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_solids_by_mode_shape(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_solids_by_mode_shape(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def ModalAnalysisSurfacesByModeShape(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_surfaces_by_mode_shape(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_modal_analysis_surfaces_by_mode_shape(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def NodesByEigenvector(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_nodes_by_eigenvector(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_nodes_by_eigenvector(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def NodesDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_nodes_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_nodes_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def NodesSupportForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_nodes_support_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_nodes_support_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsBasicPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_basic_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_basic_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsBasicStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_basic_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_basic_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsBasicTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_basic_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_basic_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsByEigenvector(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_by_eigenvector(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_by_eigenvector(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsEquivalentPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_equivalent_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_equivalent_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsEquivalentStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_equivalent_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_equivalent_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsEquivalentTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_equivalent_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_equivalent_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsGasQuantities(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_gas_quantities(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_gas_quantities(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsPrincipalPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_principal_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_principal_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsPrincipalStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_principal_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_principal_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SolidsPrincipalTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_principal_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_solids_principal_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisBuildingStoriesCentresMassRigidity(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_centres_mass_rigidity(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_centres_mass_rigidity(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisBuildingStoriesForcesInShearWalls(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_forces_in_shear_walls(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_forces_in_shear_walls(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisBuildingStoriesForcesInSpandrels(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_forces_in_spandrels(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_forces_in_spandrels(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisBuildingStoriesInterstoryDrifts(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_interstory_drifts(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_interstory_drifts(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisBuildingStoriesStoryActions(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_story_actions(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_building_stories_story_actions(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisLineHingesDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_line_hinges_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_line_hinges_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisLineHingesForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_line_hinges_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_line_hinges_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisLinesSlabWallConnections(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_lines_slab_wall_connections(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_lines_slab_wall_connections(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisLinesSupportForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_lines_support_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_lines_support_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisMembersContactForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_contact_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_contact_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisMembersGlobalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_global_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_global_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisMembersHingeDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_hinge_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_hinge_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisMembersHingeForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_hinge_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_hinge_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisMembersInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisMembersInternalForcesByMemberSet(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_internal_forces_by_member_set(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_internal_forces_by_member_set(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisMembersInternalForcesBySection(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_internal_forces_by_section(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_internal_forces_by_section(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisMembersLocalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_local_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_local_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisMembersStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_members_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisNodesDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_nodes_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_nodes_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisNodesPseudoAccelerations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_nodes_pseudo_accelerations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_nodes_pseudo_accelerations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisNodesPseudoVelocities(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_nodes_pseudo_velocities(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_nodes_pseudo_velocities(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisNodesSupportForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_nodes_support_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_nodes_support_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSolidsBasicStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_basic_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_basic_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSolidsBasicTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_basic_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_basic_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSolidsDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSolidsEquivalentStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_equivalent_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_equivalent_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSolidsEquivalentTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_equivalent_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_equivalent_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSolidsGasQuantities(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_gas_quantities(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_gas_quantities(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSolidsPrincipalStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_principal_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_principal_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSolidsPrincipalTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_principal_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_solids_principal_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSummary(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_summary(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_summary(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesBasicInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_basic_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_basic_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesBasicStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_basic_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_basic_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesBasicTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_basic_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_basic_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesContactStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_contact_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_contact_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesDesignInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_design_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_design_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesElasticStressComponents(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_elastic_stress_components(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_elastic_stress_components(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesEquivalentStressesBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_stresses_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_stresses_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesEquivalentStressesMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_stresses_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_stresses_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesEquivalentStressesRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_stresses_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_stresses_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesEquivalentStressesTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_stresses_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_stresses_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesEquivalentTotalStrainsBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_total_strains_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_total_strains_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesEquivalentTotalStrainsMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_total_strains_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_total_strains_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesEquivalentTotalStrainsRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_total_strains_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_total_strains_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesEquivalentTotalStrainsTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_total_strains_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_equivalent_total_strains_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesGlobalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_global_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_global_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesLocalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_local_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_local_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesMaximumTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_maximum_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_maximum_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesPrincipalInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_principal_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_principal_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesPrincipalStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_principal_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_principal_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SpectralAnalysisSurfacesPrincipalTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_principal_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_spectral_analysis_surfaces_principal_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisBuildingStoriesCentresMassRigidity(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_centres_mass_rigidity(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_centres_mass_rigidity(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisBuildingStoriesForcesInShearWalls(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_forces_in_shear_walls(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_forces_in_shear_walls(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisBuildingStoriesForcesInSpandrels(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_forces_in_spandrels(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_forces_in_spandrels(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisBuildingStoriesInterstoryDrifts(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_interstory_drifts(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_interstory_drifts(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisBuildingStoriesStoryActions(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_story_actions(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_building_stories_story_actions(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisCalculationDiagrams(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_calculation_diagrams(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_calculation_diagrams(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisLineHingesDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_line_hinges_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_line_hinges_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisLineHingesForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_line_hinges_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_line_hinges_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisLinesSlabWallConnections(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_lines_slab_wall_connections(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_lines_slab_wall_connections(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisLinesSupportForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_lines_support_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_lines_support_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisMembersContactForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_contact_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_contact_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisMembersGlobalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_global_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_global_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisMembersHingeDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_hinge_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_hinge_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisMembersHingeForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_hinge_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_hinge_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisMembersInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisMembersInternalForcesByMemberSet(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_internal_forces_by_member_set(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_internal_forces_by_member_set(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisMembersInternalForcesBySection(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_internal_forces_by_section(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_internal_forces_by_section(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisMembersLocalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_local_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_local_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisMembersStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_members_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisNodesDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_nodes_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_nodes_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisNodesSupportForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_nodes_support_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_nodes_support_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsBasicPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_basic_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_basic_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsBasicStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_basic_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_basic_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsBasicTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_basic_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_basic_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsEquivalentPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_equivalent_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_equivalent_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsEquivalentStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_equivalent_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_equivalent_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsEquivalentTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_equivalent_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_equivalent_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsGasQuantities(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_gas_quantities(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_gas_quantities(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsPrincipalPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_principal_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_principal_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsPrincipalStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_principal_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_principal_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSolidsPrincipalTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_principal_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_solids_principal_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSummary(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_summary(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_summary(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesBasicInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_basic_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_basic_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesBasicPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_basic_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_basic_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesBasicStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_basic_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_basic_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesBasicTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_basic_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_basic_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesContactStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_contact_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_contact_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesDesignInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_design_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_design_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesElasticStressComponents(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_elastic_stress_components(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_elastic_stress_components(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentPlasticStrainsBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_plastic_strains_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_plastic_strains_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentPlasticStrainsMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_plastic_strains_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_plastic_strains_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentPlasticStrainsRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_plastic_strains_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_plastic_strains_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentPlasticStrainsTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_plastic_strains_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_plastic_strains_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentStressesBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_stresses_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_stresses_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentStressesMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_stresses_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_stresses_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentStressesRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_stresses_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_stresses_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentStressesTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_stresses_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_stresses_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentTotalStrainsBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_total_strains_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_total_strains_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentTotalStrainsMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_total_strains_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_total_strains_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentTotalStrainsRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_total_strains_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_total_strains_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesEquivalentTotalStrainsTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_total_strains_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_equivalent_total_strains_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesGlobalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_global_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_global_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesLocalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_local_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_local_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesMaximumPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_maximum_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_maximum_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesMaximumTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_maximum_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_maximum_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesPrincipalInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_principal_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_principal_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesPrincipalPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_principal_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_principal_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesPrincipalStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_principal_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_principal_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def StabilityIncrementalAnalysisSurfacesPrincipalTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_principal_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_stability_incremental_analysis_surfaces_principal_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def Summary(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
         model = Model):
 
@@ -2975,1522 +3140,1611 @@
 
         return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_summary(loading_type.name, loading_no))
 
     @staticmethod
     def SurfacesBasicInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_basic_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_basic_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesBasicPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_basic_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_basic_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesBasicStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_basic_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_basic_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesBasicTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_basic_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_basic_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesByEigenvector(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_by_eigenvector(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_by_eigenvector(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesContactStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_contact_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_contact_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesDesignInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_design_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_design_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesElasticStressComponents(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_elastic_stress_components(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_elastic_stress_components(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentPlasticStrainsBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_plastic_strains_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_plastic_strains_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentPlasticStrainsMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_plastic_strains_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_plastic_strains_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentPlasticStrainsRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_plastic_strains_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_plastic_strains_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentPlasticStrainsTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_plastic_strains_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_plastic_strains_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentStressesBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_stresses_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_stresses_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentStressesMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_stresses_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_stresses_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentStressesRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_stresses_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_stresses_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentStressesTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_stresses_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_stresses_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentTotalStrainsBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_total_strains_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_total_strains_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentTotalStrainsMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_total_strains_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_total_strains_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentTotalStrainsRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_total_strains_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_total_strains_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesEquivalentTotalStrainsTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_total_strains_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_equivalent_total_strains_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesGlobalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_global_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_global_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesLocalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_local_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_local_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesMaximumPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_maximum_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_maximum_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesMaximumTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_maximum_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_maximum_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesPrincipalInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_principal_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_principal_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesPrincipalPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_principal_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_principal_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesPrincipalStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_principal_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_principal_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def SurfacesPrincipalTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_principal_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_surfaces_principal_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisBuildingStoriesCentresMassRigidity(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_centres_mass_rigidity(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_centres_mass_rigidity(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisBuildingStoriesForcesInShearWalls(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_forces_in_shear_walls(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_forces_in_shear_walls(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisBuildingStoriesForcesInSpandrels(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_forces_in_spandrels(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_forces_in_spandrels(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisBuildingStoriesInterstoryDrifts(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_interstory_drifts(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_interstory_drifts(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisBuildingStoriesStoryActions(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_story_actions(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_building_stories_story_actions(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisLineHingesDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_line_hinges_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_line_hinges_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisLineHingesForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_line_hinges_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_line_hinges_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisLinesSlabWallConnections(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_lines_slab_wall_connections(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_lines_slab_wall_connections(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisLinesSupportForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_lines_support_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_lines_support_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisMembersContactForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_contact_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_contact_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisMembersGlobalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_global_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_global_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisMembersHingeDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_hinge_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_hinge_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisMembersHingeForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_hinge_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_hinge_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisMembersInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisMembersInternalForcesByMemberSet(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_internal_forces_by_member_set(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_internal_forces_by_member_set(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisMembersInternalForcesBySection(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_internal_forces_by_section(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_internal_forces_by_section(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisMembersLocalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_local_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_local_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisMembersStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_members_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisNodesAccelerations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_nodes_accelerations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_nodes_accelerations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisNodesDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_nodes_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_nodes_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisNodesSupportForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_nodes_support_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_nodes_support_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisNodesVelocities(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_nodes_velocities(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_nodes_velocities(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsBasicPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_basic_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_basic_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsBasicStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_basic_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_basic_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsBasicTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_basic_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_basic_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsEquivalentPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_equivalent_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_equivalent_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsEquivalentStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_equivalent_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_equivalent_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsEquivalentTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_equivalent_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_equivalent_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsGasQuantities(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_gas_quantities(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_gas_quantities(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsPrincipalPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_principal_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_principal_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsPrincipalStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_principal_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_principal_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSolidsPrincipalTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_principal_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_solids_principal_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSummary(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_summary(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_summary(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesBasicInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_basic_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_basic_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesBasicPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_basic_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_basic_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesBasicStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_basic_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_basic_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesBasicTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_basic_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_basic_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesContactStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_contact_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_contact_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesDesignInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_design_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_design_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesElasticStressComponents(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_elastic_stress_components(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_elastic_stress_components(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentPlasticStrainsBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_plastic_strains_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_plastic_strains_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentPlasticStrainsMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_plastic_strains_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_plastic_strains_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentPlasticStrainsRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_plastic_strains_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_plastic_strains_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentPlasticStrainsTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_plastic_strains_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_plastic_strains_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentStressesBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_stresses_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_stresses_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentStressesMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_stresses_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_stresses_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentStressesRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_stresses_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_stresses_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentStressesTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_stresses_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_stresses_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentTotalStrainsBach(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_total_strains_bach(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_total_strains_bach(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentTotalStrainsMises(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_total_strains_mises(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_total_strains_mises(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentTotalStrainsRankine(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_total_strains_rankine(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_total_strains_rankine(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesEquivalentTotalStrainsTresca(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_total_strains_tresca(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_equivalent_total_strains_tresca(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesGlobalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_global_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_global_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesLocalDeformations(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_local_deformations(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_local_deformations(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesMaximumPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_maximum_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_maximum_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesMaximumTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_maximum_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_maximum_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesPrincipalInternalForces(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_principal_internal_forces(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_principal_internal_forces(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesPrincipalPlasticStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_principal_plastic_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_principal_plastic_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesPrincipalStresses(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_principal_stresses(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_principal_stresses(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def TimeHistoryAnalysisSurfacesPrincipalTotalStrains(
         loading_type: enum = CaseObjectType.E_OBJECT_TYPE_LOAD_CASE,
         loading_no: int = 1,
-        object_no: int = 1,
+        object_no: int = 0,
+        include_base: bool = False,
         model = Model):
 
         '''
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             object_no (int): Object number
             model (class, optional): Model instance
         '''
 
-        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_principal_total_strains(loading_type.name, loading_no, object_no))
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_time_history_analysis_surfaces_principal_total_strains(loading_type.name, loading_no, object_no), include_base)
 
     @staticmethod
     def HasAnyResults( model = Model):
 
         '''
          Args:
             model (class, optional): Model instance
```

### Comparing `RSTAB-1.6.0/RSTAB/SpecialObjects/nodalRelease.py` & `RSTAB-1.7.0/RSTAB/SpecialObjects/nodalRelease.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,28 @@
     def __init__(self,
                  no: int = 1,
                  nodes: str = '',
                  nodal_release_type: int = 1,
                  release_location = NodalReleaseReleaseLocation.RELEASE_LOCATION_ORIGIN,
                  released_members: str = '1',
                  deactivate_release: bool = False,
+                 name: str = '',
                  comment: str = '',
                  params: dict = None,
                  model = Model):
 
         '''
          Args:
             no (int): Nodal Release Tag
-            nodes (str): Nodes
-            nodal_release_type (int): Nodale Release Type
-            release_location (enums): Nodal Release Release Location
-            released_members (str): Released Members
-            deactivate_release (bool): Deactivate Release
+            nodes (str): Assigned Nodes
+            nodal_release_type (int): Nodale Release Type Number
+            release_location (enums): Nodal Release Release Location Enumeration
+            released_members (str): Assigned Released Members
+            deactivate_release (bool): Activate/Deactivate Nodal Release
+            name (str, optional): User Defined Nodal Release Name
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
         # Client model | Node
         clientObject = model.clientModel.factory.create('ns0:nodal_release')
 
@@ -39,26 +41,31 @@
 
         # Nodal Release Type
         clientObject.nodal_release_type = nodal_release_type
 
         # Released Members
         clientObject.released_members = ConvertToDlString(released_members)
 
-        # Nodal Release
+        # Nodal Release Location
         clientObject.release_location = release_location.name
 
         # Deactivate Release
         clientObject.deactivated = deactivate_release
 
+        # Nodal Release User defined name
+        if name:
+            clientObject.user_defined_name_enabled = True
+            clientObject.name = name
+
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add Node to client model
+        # Add Nodal Release to client model
         model.clientModel.service.set_nodal_release(clientObject)
```

### Comparing `RSTAB-1.6.0/RSTAB/SpecialObjects/structureModification.py` & `RSTAB-1.7.0/RSTAB/SpecialObjects/structureModification.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/SteelDesign/steelServiceabilityConfiguration.py` & `RSTAB-1.7.0/RSTAB/SteelDesign/steelServiceabilityConfiguration.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/SteelDesign/steelUltimateConfigurations.py` & `RSTAB-1.7.0/RSTAB/SteelDesign/steelUltimateConfigurations.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py` & `RSTAB-1.7.0/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             member_sets_no (str): Assign Configuration to Selected Member Sets
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # Client Model | Timber Design Service Limit State Configurations
-        clientObject = model.clientModel.factory.create('ns0:timber_design_uls_configuration')
+        clientObject = model.clientModel.factory.create('ns0:timber_design_sls_configuration')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # SLS Configuration No.
         clientObject.no = no
```

### Comparing `RSTAB-1.6.0/RSTAB/TimberDesign/timberUltimateConfigurations.py` & `RSTAB-1.7.0/RSTAB/TimberDesign/timberUltimateConfigurations.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Tools/ModelCheck.py` & `RSTAB-1.7.0/RSTAB/Tools/ModelCheck.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Tools/PlausibilityCheck.py` & `RSTAB-1.7.0/RSTAB/Tools/PlausibilityCheck.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Tools/centreOfGravityAndObjectInfo.py` & `RSTAB-1.7.0/RSTAB/Tools/centreOfGravityAndObjectInfo.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/Tools/sectionDialogue.py` & `RSTAB-1.7.0/RSTAB/Tools/sectionDialogue.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py` & `RSTAB-1.7.0/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py` & `RSTAB-1.7.0/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py` & `RSTAB-1.7.0/RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
         count = 0
         for comp in component:
             clientWeld = model.clientModel.factory.create('ns0:aluminum_member_transverse_weld_components_row')
             clientWeld.no = count+1
             count = count+1
             clientWeld.row = model.clientModel.factory.create('ns0:aluminum_member_transverse_weld_components')
+            clearAttributes(clientWeld.row)
             clientWeld.row.weld_type = comp['weld_type'].name
             clientWeld.row.position = comp['position']
             clientWeld.row.multiple = comp['multiple']
             clientWeld.row.multiple_number = comp['multiple_number']
             clientWeld.row.multiple_offset_definition_type = comp['multiple_offset_definition_type'].name
             clientWeld.row.multiple_offset = comp['multiple_offset']
             clientWeld.row.size = comp['size']
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberDefinableStiffness.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberDefinableStiffness.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberEccentricity.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberEccentricity.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberHinge.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberHinge.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 
             clientObject.diagram_along_x_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_along_x_table')
 
             for i,j in enumerate(translational_release_n_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_x_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_x_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.displacement = translational_release_n_nonlinearity[1][2][i][0]
                 mlvlp.row.force = translational_release_n_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = translational_release_n_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_along_x_table.member_hinge_diagram_along_x_table.append(mlvlp)
 
         elif translational_release_n_nonlinearity[0].name == "NONLINEARITY_TYPE_FRICTION_DIRECTION_1" \
@@ -202,14 +203,15 @@
 
             clientObject.diagram_along_y_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_along_y_table')
 
             for i,j in enumerate(translational_release_vy_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_y_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_y_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.displacement = translational_release_vy_nonlinearity[1][2][i][0]
                 mlvlp.row.force = translational_release_vy_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = translational_release_vy_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_along_y_table.member_hinge_diagram_along_y_table.append(mlvlp)
 
         elif translational_release_vy_nonlinearity[0].name == "NONLINEARITY_TYPE_FRICTION_DIRECTION_1" \
@@ -274,14 +276,15 @@
 
             clientObject.diagram_along_z_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_along_z_table')
 
             for i,j in enumerate(translational_release_vz_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_z_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_z_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.displacement = translational_release_vz_nonlinearity[1][2][i][0]
                 mlvlp.row.force = translational_release_vz_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = translational_release_vz_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_along_z_table.member_hinge_diagram_along_z_table.append(mlvlp)
 
         elif translational_release_vz_nonlinearity[0].name == "NONLINEARITY_TYPE_FRICTION_DIRECTION_1" \
@@ -346,14 +349,15 @@
 
             clientObject.diagram_around_x_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_around_x_table')
 
             for i,j in enumerate(rotational_release_mt_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_x_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_x_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.rotation = rotational_release_mt_nonlinearity[1][2][i][0]
                 mlvlp.row.moment = rotational_release_mt_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = rotational_release_mt_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_around_x_table.member_hinge_diagram_around_x_table.append(mlvlp)
 
         # Rotational Release My Nonlinearity
@@ -407,14 +411,15 @@
 
             clientObject.diagram_around_y_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_around_y_table')
 
             for i,j in enumerate(rotational_release_my_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_y_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_y_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.rotation = rotational_release_my_nonlinearity[1][2][i][0]
                 mlvlp.row.moment = rotational_release_my_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = rotational_release_my_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_around_y_table.member_hinge_diagram_around_y_table.append(mlvlp)
 
         # Rotational Release Mz Nonlinearity
@@ -468,14 +473,15 @@
 
             clientObject.diagram_around_z_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_around_z_table')
 
             for i,j in enumerate(rotational_release_mz_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_z_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_z_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.rotation = rotational_release_mz_nonlinearity[1][2][i][0]
                 mlvlp.row.moment = rotational_release_mz_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = rotational_release_mz_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_around_z_table.member_hinge_diagram_around_z_table.append(mlvlp)
 
         # Comment
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberNonlinearity.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberNonlinearity.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberResultIntermediatePoints.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberResultIntermediatePoints.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberRotationalRestraint.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberRotationalRestraint.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,73 +4,72 @@
 class MemberRotationalRestraint():
 
     def __init__(self) -> None:
         pass
 
     @staticmethod
     def Continuous(
-        no: int = 1,
-        name: str = '',
-        member_supports: str = '1',
-        sheeting_material: str = 'S235',
-        sheeting_name: str = 'Arval (-) 35/207 - 0.63 (b: 1) | DIN 18807 | Arval',
-        position_of_sheeting = MemberRotationalRestraintSheetingPosition.SHEETING_POSITION_POSITIVE,
-        continuous_beam_effect = MemberRotationalRestraintContinousBeamEffect.CONTINUOUS_BEAM_EFFECT_END_PANEL,
-        section_deformation_cdb: bool = True,
-        modulus_of_elasticity: float = 205000000000.0,
-        sheeting_thickness: float = 0.00063,
-        sheeting_moment_of_inertia: float = 7.5e-08,
-        sheeting_distance_of_ribs: float = 0.207,
-        width_of_sheeting_flange: float = 0.106,
-        spring_stiffness: float = 5200.0,
-        beam_spacing: float= 3.0,
-        comment: str = '',
-        params: dict = None):
+                no: int = 1,
+                name: str = '',
+                sheeting_material: str = 'S235',
+                sheeting_name: str = 'Arval (-) 35/207 - 0.63 (b: 1) | DIN 18807 | Arval',
+                position_of_sheeting = MemberRotationalRestraintSheetingPosition.SHEETING_POSITION_POSITIVE,
+                continuous_beam_effect = MemberRotationalRestraintContinousBeamEffect.CONTINUOUS_BEAM_EFFECT_END_PANEL,
+                section_deformation_cdb: bool = True,
+                modulus_of_elasticity: float = None,
+                sheeting_thickness: float = None,
+                sheeting_moment_of_inertia: float = None,
+                sheeting_distance_of_ribs: float = None,
+                width_of_sheeting_flange: float = None,
+                spring_stiffness: float = 5200.0,
+                beam_spacing: float= 3.0,
+                comment: str = '',
+                params: dict = None,
+                model = Model):
+
         """
         Args:
             no (int): Member Rotational Restraint Tag
-            name (str): Member Shear Panel Name
+            name (str): User Defined Member Rotational Restraint Name
                 if name == '':
-                    name = False (Automatic Name Assignment)
+                    user_defined_name_enabled = False (Automatic Name Assignment)
                 else:
-                    name = name
-            member_supports (str): Assigned Member Supports
+                    user_defined_name_enabled = True
+                    name = User Defined Name
             sheeting_material (str): Sheeting Material
-            sheeting_name (str): Sheeting Material
+            sheeting_name (str): Sheeting Name According to Library
             position_of_sheeting (enum): Position of Sheeting Enumeration
             continuous_beam_effect (enum): Continous Beam Effect Enumeration
             section_deformation_cdb (bool): Section Deformation Cdb Option
-            modulus_of_elasticity (float): Modulus of Elasticity
-            sheeting_thickness (float): Sheeting Thickness
-            sheeting_moment_of_inertia (float): Sheeting Moment of Inertia
-            sheeting_distance_of_ribs (float): Sheeting Distance of Ribs
-            width_of_sheeting_flange (float): Width of Sheeting Flange
+            modulus_of_elasticity (float, optional): Modulus of Elasticity
+            sheeting_thickness (float, optional): Sheeting Thickness
+            sheeting_moment_of_inertia (float, optional): Sheeting Moment of Inertia
+            sheeting_distance_of_ribs (float, optional): Sheeting Distance of Ribs
+            width_of_sheeting_flange (float, optional): Width of Sheeting Flange
             spring_stiffness (float): Spring Stiffness
             beam_spacing (float): Beam Spacing
             comment (str, optional): Comment
-            params (dict, optional): Parameters
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
 
         # Client Model | Member Rotational Restraint
-        clientObject = Model.clientModel.factory.create('ns0:member_rotational_restraint')
+        clientObject = model.clientModel.factory.create('ns0:member_rotational_restraint')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Member Rotational Restraint No.
         clientObject.no = no
 
         # Member Rotational Restraint User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
-        # Member Rotational Restraints Assigned Member Supports
-        clientObject.member_supports = ConvertToDlString(member_supports)
-
         # Member Rotational Restraint Definition Type
         clientObject.type = MemberRotationalRestraintType.TYPE_CONTINUOUS.name
 
         # Member Rotational Restraint Sheeting Material Name
         clientObject.material_name = sheeting_material
 
         # Member Rotational Restraint Sheeting Name
@@ -114,75 +113,74 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Member Rotational Restraint to client model
-        Model.clientModel.service.set_member_rotational_restraint(clientObject)
+        model.clientModel.service.set_member_rotational_restraint(clientObject)
 
     @staticmethod
     def Discrete(
-        no: int = 1,
-        name: str = '',
-        member_supports: str = '1',
-        section_material: str = 'S235',
-        section_name: str = 'CHC 60.3x3.2',
-        rotational_stifness: list = [MemberRotationalRestraintRotationalStiffness.ROTATIONAL_STIFFNESS_INFINITELY],
-        continous_beam_effect = MemberRotationalRestraintContinousBeamEffect.CONTINUOUS_BEAM_EFFECT_END_PANEL,
-        section_deformation_cdb: bool =  True,
-        modulus_of_elasticity: float = 205000000000.0,
-        section_moment_of_inertia: float = 2.35e-07,
-        purlin_spacing: float = 1.0,
-        beam_spacing: float = 3.0,
-        comment: str = '',
-        params: dict = None):
+                no: int = 1,
+                name: str = '',
+                section_material: str = 'S235',
+                section_name: str = 'CHC 60.3x3.2',
+                rotational_stifness: list = [MemberRotationalRestraintRotationalStiffness.ROTATIONAL_STIFFNESS_INFINITELY],
+                continous_beam_effect = MemberRotationalRestraintContinousBeamEffect.CONTINUOUS_BEAM_EFFECT_END_PANEL,
+                section_deformation_cdb: bool =  True,
+                modulus_of_elasticity: float = None,
+                section_moment_of_inertia: float = None,
+                purlin_spacing: float = 1.0,
+                beam_spacing: float = 3.0,
+                comment: str = '',
+                params: dict = None,
+                model = Model):
+
         """
         Args:
             no (int): Member Rotational Restraint Tag
-            name (str): Member Shear Panel Name
+            name (str): User Defined Member Rotational Restraint Name
                 if name == '':
-                    name = False (Automatic Name Assignment)
+                    user_defined_name_enabled = False (Automatic Name Assignment)
                 else:
-                    name = name
-            member_supports (str): Assigned Member Supports
+                    user_defined_name_enabled = True
+                    name = User Defined Name
             section_material (str): Section Material
             section_name (str): Section Name
             rotational_stifness (list): Rotational Stiffness
                 if rotational_stiffness[0] == MemberRotationalRestraintRotationalStiffness.ROTATIONAL_STIFFNESS_INFINITELY:
                     pass
                 elif rotational_stiffness[0] == MemberRotationalRestraintRotationalStiffness.ROTATIONAL_STIFFNESS_MANUALLY:
-                    rotational_stiffness[1] = rotational_stiffness_value
+                    rotational_stiffness[1] (float): Rotational Stiffness Value
             continous_beam_effect (enum): Continous Beam Effect Enumeration
             section_deformation_cdb (bool): Section Deformation Cdb Option
-            modulus_of_elasticity (float): Modulus of Elasticity
-            section_moment_of_inertia (float): Section Moment of Inertia
+            modulus_of_elasticity (float, optional): Modulus of Elasticity
+            section_moment_of_inertia (float, optional): Section Moment of Inertia
             purlin_spacing (float): Purlin Spacing
             beam_spacing (float): Beam Spacing
             comment (str, optional): Comment
-            params (dict, optional): Params
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
 
         # Client Model | Member Rotational Restraint
-        clientObject = Model.clientModel.factory.create('ns0:member_rotational_restraint')
+        clientObject = model.clientModel.factory.create('ns0:member_rotational_restraint')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Member Rotational Restraint No.
         clientObject.no = no
 
         # Member Rotational Restraint User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
-        # Member Rotational Restraints Assigned Member Supports
-        clientObject.member_supports = ConvertToDlString(member_supports)
-
         # Member Rotational Restraint Definition Type
         clientObject.type = MemberRotationalRestraintType.TYPE_DISCRETE.name
 
         # Member Rotational Restraint Section Material Name
         clientObject.material_name = section_material
 
         # Member Rotational Restraint Section Name
@@ -219,55 +217,54 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Member Rotational Restraint to client model
-        Model.clientModel.service.set_member_rotational_restraint(clientObject)
+        model.clientModel.service.set_member_rotational_restraint(clientObject)
 
     @staticmethod
     def Manually(
-        no: int = 1,
-        name: str = '',
-        member_supports: str = '1',
-        rotational_spring_stiffness: float = 3000.0,
-        comment: str = '',
-        params: dict = None):
+                no: int = 1,
+                name: str = '',
+                rotational_spring_stiffness: float = 3000.0,
+                comment: str = '',
+                params: dict = None,
+                model = Model):
+
         """
         Args:
             no (int): Member Rotational Restraint Tag
-            name (str): Member Shear Panel Name
+            name (str): User Defined Member Rotational Restraint Name
                 if name == '':
-                    name = False (Automatic Name Assignment)
+                    user_defined_name_enabled = False (Automatic Name Assignment)
                 else:
-                    name = name
-            member_supports (str): Assigned Member Supports
+                    user_defined_name_enabled = True
+                    name = User Defined Name
             rotational_spring_stiffness (float): Rotational Spring Stiffness
             comment (str, optional): Comment
-            params (dict, optional): Params
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
 
         # Client Model | Member Rotational Restraint
-        clientObject = Model.clientModel.factory.create('ns0:member_rotational_restraint')
+        clientObject = model.clientModel.factory.create('ns0:member_rotational_restraint')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Member Rotational Restraint No.
         clientObject.no = no
 
         # Member Rotational Restraint User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
-        # Member Rotational Restraints Assigned Member Supports
-        clientObject.member_supports = ConvertToDlString(member_supports)
-
         # Member Rotational Restraint Definition Type
         clientObject.type = MemberRotationalRestraintType.TYPE_MANUALLY.name
 
         # Member Rotational Restraint Total Rotational Spring Stiffness
         clientObject.total_rotational_spring_stiffness = rotational_spring_stiffness
 
         # Comment
@@ -278,8 +275,8 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Member Rotational Restraint to client model
-        Model.clientModel.service.set_member_rotational_restraint(clientObject)
+        model.clientModel.service.set_member_rotational_restraint(clientObject)
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberShearPanel.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberShearPanel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,69 @@
-from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
-from RSTAB.enums import MemberShearPanelDefinitionType, MemberShearPanelFasteningArrangement, MemberShearPanelPositionOnSection
+from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes
+from RSTAB.enums import MemberShearPanelDefinitionType, MemberShearPanelFasteningArrangement
 
 class MemberShearPanel():
 
     def __init__(self) -> None:
         pass
 
     @staticmethod
-    def TrapezodialSheeting(
-        no: int = 1,
-        name: str = '',
-        member_supports: str = '1',
-        position_on_section = MemberShearPanelPositionOnSection.POSITION_ON_UPPER_FLANGE,
-        girder_length_definition: list = [True],
-        sheeting_name: str = 'FI (+) 35/207 - 0.63 (b: 1) | DIN 18807 | Fischer Profil',
-        fastening_arrangement = MemberShearPanelFasteningArrangement.FASTENING_ARRANGEMENT_EVERY_RIB,
-        panel_length: float = 2.0,
-        beam_spacing: float = 1.0,
-        coefficient_k1: float = 0.0002,
-        coefficient_k2: float = 0.0123,
-        position_on_section_value: float = 1.0,
-        comment: str = '',
-        params: dict = None):
+    def TrapezodialSheeting(no: int = 1,
+                            name: str = '',
+                            girder_length_definition: list = [True],
+                            sheeting_name: str = 'FI (+) 35/207 - 0.63 (b: 1) | DIN 18807 | Fischer Profil',
+                            fastening_arrangement = MemberShearPanelFasteningArrangement.FASTENING_ARRANGEMENT_EVERY_RIB,
+                            panel_length: float = 2.0,
+                            beam_spacing: float = 1.0,
+                            coefficient_k1: float = None,
+                            coefficient_k2: float = None,
+                            comment: str = '',
+                            params: dict = None,
+                            model = Model):
+
         """
         Args:
             no (int): Member Shear Panel Tag
-            name (str): Member Shear Panel Name
+            name (str): User Defined Member Shear Panel Name
                 if name == '':
-                    name = False (Automatic Name Assignment)
+                    user_defined_name_enabled = False (Automatic Name Assignment)
                 else:
-                    name = name
-            member_supports (str): Assigned Member Supports
-            position_on_section (enum): Member Shear Panel Position Enumeration
+                    user_defined_name_enabled = True
+                    name = User Defined Name
             girder_length_definition (list): Girder Length Definition List
-                girder_length_definition[0] (boolean): Definition Option
-                girder_length_definition[1] (enum): Definition Type Enumeration
-            sheeting_name (str): Sheeting Name
+                girder_length_definition[0] (bool): Activate/Deactivate Automatically Girder Length
+                girder_length_definition[1] (float): Girder Length Value
+            sheeting_name (str): Sheeting Name According to Library
             fastening_arrangement (enum): Fastening Arrangement Enumeration
             panel_length (float): Panel Length
             beam_spacing (float): Beam Spacing
-            coefficient_k1 (float): Coefficient K1
-            coefficient_k2 (float): Coefficient K2
-            position_on_section_value (float): Position on Section Value
+            coefficient_k1 (float, optional): Coefficient K1
+            coefficient_k2 (float, optional): Coefficient K2
             comment (str, optional): Comment
-            params (dict, optional): Parameters
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
 
         # Client Model | Member Shear Panel
-        clientObject = Model.clientModel.factory.create('ns0:member_shear_panel')
+        clientObject = model.clientModel.factory.create('ns0:member_shear_panel')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Member Shear Panel No.
         clientObject.no = no
 
         # Member Shear Panel Definition Type
         clientObject.definition_type = MemberShearPanelDefinitionType.DEFINITION_TYPE_TRAPEZOIDAL_SHEETING.name
 
-        # Member Shear Panel Assigned Member Supports
-        clientObject.member_supports = ConvertToDlString(member_supports)
-
         # Member Shear Panel User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
-        # Member Shear Panel Position On Section
-        clientObject.position_on_section = position_on_section.name
-
-        if position_on_section == MemberShearPanelPositionOnSection.POSITION_DEFINE:
-            clientObject.position_on_section_value = position_on_section_value
-
         # Member Shear Panel Girder Length Definition
         if girder_length_definition[0]:
             clientObject.define_girder_length_automatically = True
         else:
             clientObject.define_girder_length_automatically = False
             clientObject.girder_length = girder_length_definition[1]
 
@@ -105,87 +93,78 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Member Shear Panel to client model
-        Model.clientModel.service.set_member_shear_panel(clientObject)
+        model.clientModel.service.set_member_shear_panel(clientObject)
 
     @staticmethod
-    def Bracing(
-        no: int = 1,
-        name: str = '',
-        member_supports: str = '1',
-        position_on_section = MemberShearPanelPositionOnSection.POSITION_ON_UPPER_FLANGE,
-        girder_length_definition: list = [True],
-        material_name: str = 'S235',
-        diagonal_section: str = 'CHC 60.3x4.0',
-        posts_section: str = 'CHC 76.1x4.0',
-        modulus_of_elasticity: float = 210000000000.0,
-        panel_length: float = 2.0,
-        beam_spacing: float = 1.0,
-        posts_spacing: float = 2.0,
-        number_of_bracings: int = 2,
-        diagonals_section_area: float = 0.001007,
-        posts_section_area: float = 0.0009,
-        position_on_section_value: float = 1.0,
-        comment: str = '',
-        params: dict = None):
+    def Bracing(no: int = 1,
+                name: str = '',
+                girder_length_definition: list = [True],
+                material_name: str = 'S235',
+                diagonal_section: str = 'CHC 60.3x4.0',
+                posts_section: str = 'CHC 76.1x4.0',
+                modulus_of_elasticity: float = None,
+                panel_length: float = 2.0,
+                beam_spacing: float = 1.0,
+                posts_spacing: float = 2.0,
+                number_of_bracings: int = 2,
+                diagonals_section_area: float = None,
+                posts_section_area: float = None,
+                comment: str = '',
+                params: dict = None,
+                model = Model):
+
         """
         Args:
             no (int): Member Shear Panel Tag
-            name (str): Member Shear Panel Name
+            name (str): User Defined Member Shear Panel Name
                 if name == '':
-                    name = False (Automatic Name Assignment)
+                    user_defined_name_enabled = False (Automatic Name Assignment)
                 else:
-                    name = name
-            member_supports (str): Assigned Member Supports
-            position_on_section (enum): Member Shear Panel Position Enumeration
+                    user_defined_name_enabled = True
+                    name = User Defined Name
+            girder_length_definition (list): Girder Length Definition List
+                girder_length_definition[0] (bool): Activate/Deactivate Automatically Girder Length
+                girder_length_definition[1] (float): Girder Length Value
             material_name (str): Material Name
             diagonal_section (str): Diagonal Section
             posts_section (str): Posts Section
-            modulus_of_elasticity (float): Modulus of Elasticity
+            modulus_of_elasticity (float, optional): Modulus of Elasticity
             panel_length (float): Panel Length
             beam_spacing (float): Beam Spacing
             posts_spacing (float): Posts Spacing
             number_of_bracings (int): Number of Bracings
-            diagonals_section_area (float): Diagonals Section Area
-            posts_section_area (float): Posts Section Area
-            position_on_section_value (float): Position of Section Value
+            diagonals_section_area (float, optional): Diagonals Section Area
+            posts_section_area (float, optional): Posts Section Area
             comment (str, optional): Comment
-            params (dict, optional): Params
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
 
         # Client Model | Member Shear Panel
-        clientObject = Model.clientModel.factory.create('ns0:member_shear_panel')
+        clientObject = model.clientModel.factory.create('ns0:member_shear_panel')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Member Shear Panel No.
         clientObject.no = no
 
         # Member Shear Panel Definition Type
         clientObject.definition_type = MemberShearPanelDefinitionType.DEFINITION_TYPE_BRACING.name
 
-        # Member Shear Panel Assigned Member Supports
-        clientObject.member_supports = ConvertToDlString(member_supports)
-
         # Member Shear Panel User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
-        # Member Shear Panel Position On Section
-        clientObject.position_on_section = position_on_section.name
-
-        if position_on_section == MemberShearPanelPositionOnSection.POSITION_DEFINE:
-            clientObject.position_on_section_value = position_on_section_value
-
         # Member Shear Panel Girder Length Definition
         if girder_length_definition[0]:
             clientObject.define_girder_length_automatically = True
         else:
             clientObject.define_girder_length_automatically = False
             clientObject.girder_length = girder_length_definition[1]
 
@@ -227,71 +206,60 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Member Shear Panel to client model
-        Model.clientModel.service.set_member_shear_panel(clientObject)
+        model.clientModel.service.set_member_shear_panel(clientObject)
 
     @staticmethod
-    def DefineSProv(
-        no: int = 1,
-        name: str = '',
-        member_supports: str = '1',
-        position_on_section = MemberShearPanelPositionOnSection.POSITION_ON_UPPER_FLANGE,
-        girder_length_definition: list = [True],
-        shear_panel_stiffness: float = 1000.0,
-        position_on_section_value: float = 1.0,
-        comment: str = '',
-        params: dict = None):
+    def DefineSProv(no: int = 1,
+                    name: str = '',
+                    girder_length_definition: list = [True],
+                    shear_panel_stiffness: float = 1000.0,
+                    comment: str = '',
+                    params: dict = None,
+                    model = Model):
+
         """
         Args:
             no (int): Member Shear Panel Tag
-            name (str): Member Shear Panel Name
+            name (str): User Defined Member Shear Panel Name
                 if name == '':
-                    name = False (Automatic Name Assignment)
+                    user_defined_name_enabled = False (Automatic Name Assignment)
                 else:
-                    name = name
-            member_supports (str): Assigned Member Supports
-            position_on_section (enum): Position on Section Enumeration
+                    user_defined_name_enabled = True
+                    name = User Defined Name
             girder_length_definition (list): Girder Length Definition List
-                girder_length_definition[0] (boolean): Definition Option
-                girder_length_definition[1] (enum): Definition Type Enumeration
+                girder_length_definition[0] (bool): Activate/Deactivate Automatically Girder Length
+                girder_length_definition[1] (float): Girder Length Value
             shear_panel_stiffness (float): Shear Panel Stiffness
-            position_on_section_value (float): Position on Section Value
             comment (str, optional): Comment
-            params (dict, optional): Parameters
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
+
         # Client Model | Member Shear Panel
-        clientObject = Model.clientModel.factory.create('ns0:member_shear_panel')
+        clientObject = model.clientModel.factory.create('ns0:member_shear_panel')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Member Shear Panel No.
         clientObject.no = no
 
         # Member Shear Panel Definition Type
         clientObject.definition_type = MemberShearPanelDefinitionType.DEFINITION_TYPE_DEFINE_S_PROV.name
 
-        # Member Shear Panel Assigned Member Supports
-        clientObject.member_supports = ConvertToDlString(member_supports)
-
         # Member Shear Panel User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
-        # Member Shear Panel Position On Section
-        clientObject.position_on_section = position_on_section.name
-
-        if position_on_section == MemberShearPanelPositionOnSection.POSITION_DEFINE:
-            clientObject.position_on_section_value = position_on_section_value
-
         # Member Shear Panel Stiffness
         clientObject.stiffness = shear_panel_stiffness
 
         # Member Shear Panel Girder Length Definition
         if girder_length_definition[0]:
             clientObject.define_girder_length_automatically = True
         else:
@@ -306,98 +274,87 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Member Shear Panel to client model
-        Model.clientModel.service.set_member_shear_panel(clientObject)
+        model.clientModel.service.set_member_shear_panel(clientObject)
 
     @staticmethod
     def TrapeziodalSheetingAndBracing(
-        no: int = 1,
-        name: str = '',
-        member_supports: str = '1',
-        position_on_section = MemberShearPanelPositionOnSection.POSITION_ON_UPPER_FLANGE,
-        sheeting_name: str = 'FI (+) 35/207 - 0.63 (b: 1) | DIN 18807 | Fischer Profil',
-        material_name: str = 'S235',
-        diagonals_section: str = 'CHC 60.3x3.2',
-        posts_section: str = 'CHC 76.1x4.0',
-        fastening_arrangement = MemberShearPanelFasteningArrangement.FASTENING_ARRANGEMENT_EVERY_RIB,
-        modulus_of_elasticity: float = 205000000000.0,
-        panel_length: float = 1.0,
-        girder_length_definition: list = [True],
-        beam_spacing: float = 2.0,
-        coefficient_k1: float = 0.0002,
-        coefficient_k2: float = 0.0104,
-        post_spacing: float = 3.0,
-        number_of_bracing: int = 2,
-        diagonals_section_area: float = 0.0005,
-        posts_section_area = 0.0009,
-        position_on_section_value = 1.0,
-        comment: str = '',
-        params: dict = None
-    ):
+                    no: int = 1,
+                    name: str = '',
+                    sheeting_name: str = 'FI (+) 35/207 - 0.63 (b: 1) | DIN 18807 | Fischer Profil',
+                    material_name: str = 'S235',
+                    diagonals_section: str = 'CHC 60.3x3.2',
+                    posts_section: str = 'CHC 76.1x4.0',
+                    fastening_arrangement = MemberShearPanelFasteningArrangement.FASTENING_ARRANGEMENT_EVERY_RIB,
+                    modulus_of_elasticity: float = None,
+                    panel_length: float = 1.0,
+                    girder_length_definition: list = [True],
+                    beam_spacing: float = 2.0,
+                    coefficient_k1: float = None,
+                    coefficient_k2: float = None,
+                    post_spacing: float = 3.0,
+                    number_of_bracing: int = 2,
+                    diagonals_section_area: float = None,
+                    posts_section_area: float = None,
+                    comment: str = '',
+                    params: dict = None,
+                    model = Model):
+
         """
         Args:
             no (int): Member Shear Panel Tag
-            name (str): Member Shear Panel Name
+            name (str): User Defined Member Shear Panel Name
                 if name == '':
-                    name = False (Automatic Name Assignment)
+                    user_defined_name_enabled = False (Automatic Name Assignment)
                 else:
-                    name = name
-            member_supports (str): Assigned Member Supports
-            position_on_section (enum): Position on Section Enumeration
-            sheeting_name (str): Sheeting Name
+                    user_defined_name_enabled = True
+                    name = User Defined Name
+            sheeting_name (str): Sheeting Name According to Library
             material_name (str): Material Name
             diagonals_section (str): Diagonals Section
             posts_section (str): Posts Section
             fastening_arrangement (enum): Fastening Arrangement Enumeration
-            modulus_of_elasticity (float): Modulus of Elasticity
+            modulus_of_elasticity (float, optional): Modulus of Elasticity
             panel_length (float): Panel Length
             girder_length_definition (list): Girder Length Definition List
-                girder_length_definition[0] (boolean): Definition Option
-                girder_length_definition[1] (enum): Definition Type Enumeration
+                girder_length_definition[0] (bool): Activate/Deactivate Automatically Girder Length
+                girder_length_definition[1] (float): Girder Length Value
             beam_spacing (float): Beam Spacing
-            coefficient_k1 (float): Coefficient K1
-            coefficient_k2 (float): Coefficient K2
+            coefficient_k1 (float, optional): Coefficient K1
+            coefficient_k2 (float, optional): Coefficient K2
             post_spacing (float): Posts Spacing
             number_of_bracing (int): Number of Bracings
-            diagonals_section_area (float): Diagonals Section Area
-            posts_section_area (float): Posts Section Area
-            position_on_section_value (float): Position on Section Value
+            diagonals_section_area (float, optional): Diagonals Section Area
+            posts_section_area (float, optional): Posts Section Area
             comment (str, optional): Comment
-            params (dict, optional): Parameters
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
+
         # Client Model | Member Shear Panel
-        clientObject = Model.clientModel.factory.create('ns0:member_shear_panel')
+        clientObject = model.clientModel.factory.create('ns0:member_shear_panel')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Member Shear Panel No.
         clientObject.no = no
 
         # Member Shear Panel Definition Type
         clientObject.definition_type = MemberShearPanelDefinitionType.DEFINITION_TYPE_TRAPEZOIDAL_SHEETING_AND_BRACING.name
 
-        # Member Shear Panel Assigned Member Supports
-        clientObject.member_supports = ConvertToDlString(member_supports)
-
         # Member Shear Panel User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
-        # Member Shear Panel Position On Section
-        clientObject.position_on_section = position_on_section.name
-
-        if position_on_section == MemberShearPanelPositionOnSection.POSITION_DEFINE:
-            clientObject.position_on_section_value = position_on_section_value
-
         # Member Shear Panel Sheeting Name
         clientObject.sheeting_name = sheeting_name
 
         # Member Shear Panel Material Name
         clientObject.material_name = material_name
 
         # Member Shear Panel Diagonals Section
@@ -449,8 +406,8 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Member Shear Panel to client model
-        Model.clientModel.service.set_member_shear_panel(clientObject)
+        model.clientModel.service.set_member_shear_panel(clientObject)
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberStiffnessModification.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberStiffnessModification.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberSupport.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberSupport.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 from RSTAB.enums import MemberSupportNonlinearity
 from RSTAB.initModel import Model, clearAttributes, ConvertToDlString, deleteEmptyAttributes
 from RSTAB.dataTypes import inf
 
 class MemberSupport():
+
     def __init__(self,
                  no: int = 1,
                  members: str = '',
                  spring_translation_x: float = 0.0,
                  spring_translation_y: float = 0.0,
                  spring_translation_z: list = [inf, MemberSupportNonlinearity.NONLINEARITY_NONE],
                  spring_rotation: float = 0.0,
                  spring_shear_x: float = 0.0,
                  spring_shear_y: float = 0.0,
                  spring_shear_z: float = 0.0,
-                 member_shear_panel: list = [False],
-                 member_rotational_restraint: list = [False],
+                 member_rotational_restraint: list = None,
                  comment: str = '',
                  params: dict = None,
                  model = Model):
+
         """
         Args:
             no (int): Member Support Tag
             members (str): Assigned Members
             spring_translation_x (float): Translational X Spring Constant
             spring_translation_y (float): Translational Y Spring Constant
             spring_translation_z (list): [Translational Z Spring Constant, Nonlinearity Type]
             spring_rotation (float): Rotational Spring Constant
             spring_shear_x (float): Shear X Spring Constant
             spring_shear_y (float): Shear Y Spring Constant
             spring_shear_z (float): Shear Z Spring Constant
-            member_shear_panel (list): Member Shear Panel Option
-                if member_shear_panel[0] == True:
-                    member_shear_panel[1] = Member Shear Panel Number
             member_rotational_restraint (list): Member Rotational Restraint Option
-                if member_rotational_restraint[0] == True:
-                    member_rotational_restraint[1] = Member Rotational Restraint Number
-                    member_rotational_restraint[2] = load_introduced_from_sheeting_to_beam
+                if member_rotational_restraint:
+                    member_rotational_restraint[0] (int): Member Rotational Restraint Number
+                    member_rotational_restraint[1] (float): Load Introduced from Sheeting to Beam
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # Client model | Member Support
         clientObject = model.clientModel.factory.create('ns0:member_support')
@@ -54,31 +52,24 @@
         clientObject.members = ConvertToDlString(members)
 
         # Spring Translation
         clientObject.spring_rotation = spring_rotation
         clientObject.spring_translation_x = spring_translation_x
         clientObject.spring_translation_y = spring_translation_y
         clientObject.spring_translation_z = spring_translation_z[0]
-        clientObject.nonlinearity = spring_translation_z[1].name
 
         # Spring Shear
         clientObject.spring_shear_x = spring_shear_x
         clientObject.spring_shear_y = spring_shear_y
         clientObject.spring_shear_z = spring_shear_z
 
-        # Member Shear Panel
-        clientObject.shear_panel_enabled = member_shear_panel[0]
-        if member_shear_panel[0]:
-            clientObject.member_shear_panel = member_shear_panel[1]
-
         # Member Rotational Restraint
-        clientObject.rotational_restraint_enabled = member_rotational_restraint[0]
-        if member_rotational_restraint[0]:
-            clientObject.member_rotational_restraint = member_rotational_restraint[1]
-            clientObject.load_introduced_from_sheeting_to_beam = member_rotational_restraint[2]
+        if member_rotational_restraint:
+            clientObject.member_rotational_restraint = member_rotational_restraint[0]
+            clientObject.load_introduced_from_sheeting_to_beam = member_rotational_restraint[1]
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForMembers/memberTransverseStiffeners.py` & `RSTAB-1.7.0/RSTAB/TypesForMembers/memberTransverseStiffeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         # Member Transverse Components
         clientObject.components = Model.clientModel.factory.create('ns0:member_transverse_stiffener.components')
 
         for i in components:
             mlvlp = Model.clientModel.factory.create('ns0:member_transverse_stiffener_components_row')
             mlvlp.no = i['no']
             mlvlp.row = Model.clientModel.factory.create('ns0:member_transverse_stiffener_components')
+            clearAttributes(mlvlp.row)
             mlvlp.row.stiffener_type = i['stiffener_type'].name
             mlvlp.row.position = i['position']
             mlvlp.row.position_type = i['position_type'].name
             mlvlp.row.multiple = i['multiple']
             mlvlp.row.multiple_number = i['multiple_number']
             mlvlp.row.multiple_offset_definition_type = i['multiple_offset_definition_type'].name
             mlvlp.row.multiple_offset = i['multiple_offset']
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForNodes/nodalSupport.py` & `RSTAB-1.7.0/RSTAB/TypesForNodes/nodalSupport.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForSpecialObjects/nodalReleaseType.py` & `RSTAB-1.7.0/RSTAB/TypesForSpecialObjects/nodalReleaseType.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes
 from RSTAB.enums import NodalReleaseTypePartialActivityAlong, NodalReleaseTypePartialActivityAround, NodalReleaseTypeLocalAxisSystemObjectType, NodalReleaseTypeReleaseNonlinearity
 from RSTAB.dataTypes import inf
 
 class NodalReleaseType():
+
     def __init__(self,
                  no: int = 1,
                  coordinate_system: str = "Local",
                  translational_release_n: float = inf,
                  translational_release_vy: float = inf,
                  translational_release_vz: float = inf,
                  rotational_release_mt: float = inf,
@@ -25,67 +26,68 @@
                  params: dict = None,
                  model = Model):
 
         '''
          Args:
             no (int): Nodal Release Type Tag
             coordinate_system (str/int): Coordinate System Selection
-            translational_release_n (float): Translational Spring Constant X
-            translational_release_vy (float): Translational Spring Constant Y
-            translational_release_vz (float): Translational Spring Constant Z
-            rotational_release_mt (float): Rotational Spring Constant X
-            rotational_release_my (float): Rotational Spring Constant Y
-            rotational_release_mz (float): Rotational Spring Constant Z
+            translational_release_n (float): Spring Constant for Translation Release along X Direction
+            translational_release_vy (float): Spring Constant for Translation Release along Y Direction
+            translational_release_vz (float): Spring Constant for Translation Release along Z Direction
+            rotational_release_mt (float): Spring Constant for Rotational Release around X Direction
+            rotational_release_my (float): Spring Constant for Rotational Release around Y Direction
+            rotational_release_mz (float): Spring Constant for Rotational Release around Z Direction
             translational_release_n_nonlinearity (list/list of lists): Nonlinearity Parameter for Translation Release along X Direction
             translational_release_vy_nonlinearity (list/list of lists): Nonlinearity Parameter for Translation Release along Y Direction
             translational_release_vz_nonlinearity (list/list of lists): Nonlinearity Parameter for Translation Release along Z Direction
                 for translational_release_n/vy/vz_nonlinearity[0] == NodalReleaseTypeReleaseNonlinearity.NONLINEARITY_TYPE_PARTIAL_ACTIVITY:
                     translational_release_n/vy/vz_nonlinearity = [nonlinearity type Partial_Activity, negative zone, positive zone]
                     for negative/positive zone[0] == NodalReleaseTypePartialActivityAlong.PARTIAL_ACTIVITY_TYPE_COMPLETE:
                         negative/positive zone = [negative/positive zone type, slippage]
                     for negative/positive zone[0] == NodalReleaseTypePartialActivityAlong.PARTIAL_ACTIVITY_TYPE_FIXED:
                         negative/positive zone = [negative/positive zone type, displacement, slippage]  (Note: Displacement must be greater than slippage)
                     for negative/positive zone[0] == NodalReleaseTypePartialActivityAlong.PARTIAL_ACTIVITY_TYPE_FAILURE_FROM_FORCE/PARTIAL_ACTIVITY_TYPE_YIELDING_FROM_FORCE:
                         negative/positive zone = [negative/positive zone type, force, slippage]
                 for translational_release_n/vy/vz_nonlinearity[0] == NodalReleaseTypeReleaseNonlinearity.NONLINEARITY_TYPE_DIAGRAM:
                     translational_release_n/vy/vz_nonlinearity = [nonlinearity type Diagram, [symmetric(bool), NodalReleaseTypeDiagram Enumeration(start), NodalReleaseTypeDiagram Enumeration(end)], [[displacement, force],...]]
+                for translational_release_n/vy/vz_nonlinearity[0] == NodalReleaseTypeReleaseNonlinearity.NONLINEARITY_TYPE_FRICTION_DIRECTION_1/NONLINEARITY_TYPE_FRICTION_DIRECTION_2/NONLINEARITY_TYPE_FRICTION_DIRECTION_1_2:
+                    translational_release_n/vy/vz_nonlinearity = [nonlinearity type Diagram, [friction coefficient(float)]]
+                for translational_release_n/vy/vz_nonlinearity[0] == NodalReleaseTypeReleaseNonlinearity.NONLINEARITY_TYPE_FRICTION_DIRECTION_1_PLUS_2:
+                    translational_release_n/vy/vz_nonlinearity = [nonlinearity type Diagram, [friction coefficient 1(float), friction coefficient 2(float)]]
             rotational_release_mt_nonlinearity (list/list of lists): Nonlinearity Parameter for Rotational Release around X Direction
             rotational_release_my_nonlinearity (list/list of lists): Nonlinearity Parameter for Rotational Release around Y Direction
             rotational_release_mz_nonlinearity (list/list of lists): Nonlinearity Parameter for Rotational Release around Z Direction
-                for rotational_release_mt/my/mz_nonlinearity[0] == NodalReleaseTypePartialActivityAround.NONLINEARITY_TYPE_PARTIAL_ACTIVITY:
+                for rotational_release_mt/my/mz_nonlinearity[0] == NodalReleaseTypeReleaseNonlinearity.NONLINEARITY_TYPE_PARTIAL_ACTIVITY:
                     rotational_release_mt/my/mz_nonlinearity = [nonlinearity type Partial_Activity, negative zone, positive zone]
                     for negative/positive zone[0] == NodalReleaseTypePartialActivityAround.PARTIAL_ACTIVITY_TYPE_COMPLETE:
                         negative/positive zone = [negative/positive zone type, slippage]
                     for negative/positive zone[0] == NodalReleaseTypePartialActivityAround.PARTIAL_ACTIVITY_TYPE_FIXED:
                         negative/positive zone = [negative/positive zone type, rotation, slippage]
                     for negative/positive zone[0] == NodalReleaseTypePartialActivityAround.PARTIAL_ACTIVITY_TYPE_FAILURE_FROM_MOMENT/PARTIAL_ACTIVITY_TYPE_YIELDING_FROM_MOMENT:
                         negative/positive zone = [negative/positive zone type, moment, slippage]
-                for rotational_release_mt/my/mz_nonlinearity[0] == NodalReleaseTypePartialActivityAround.NONLINEARITY_TYPE_DIAGRAM:
+                for rotational_release_mt/my/mz_nonlinearity[0] == NodalReleaseTypeReleaseNonlinearity.NONLINEARITY_TYPE_DIAGRAM:
                     rotational_release_mt/my/mz_nonlinearity = [nonlinearity type Diagram, [symmetric(bool), NodalReleaseTypeDiagram Enumeration(start), NodalReleaseTypeDiagram Enumeration(end)], [[rotation, moment],...]]
-                for rotational_release_mt/my/mz_nonlinearity[0] == NodalReleaseTypePartialActivityAround.NONLINEARITY_TYPE_FORCE_MOMENT_DIAGRAM:
-                    rotational_release_mt/my/mz_nonlinearity = [nonlinearity type Force_Moment_Diagram, [symmetric(bool), NodalReleaseTypeReleaseNonlinearity Enumeration(end), NodalReleaseTypeReleaseNonlinearity Enumeration],
-                                                             [[force, max_moment, min_moment(if not symetric)],...]]
             local_axis_system (enum): Nodal Release Local Axis System Enumeration
-            local_axis_system_reference_object (int): Nodal Release Local Axis System Reference Object Enumeration
-            name (str): User Defined Name
+            local_axis_system_reference_object (int): Nodal Release Local Axis System Reference Object Number
+            name (str, optional): User Defined Nodal Release Type Name
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
 
-        # Client model | Node
+        # Client model | Nodal Release Type
         clientObject = model.clientModel.factory.create('ns0:nodal_release_type')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        # Node No.
+        # Nodal Release Type No.
         clientObject.no = no
 
-        # Nodal Release Typ
+        # Nodal Release Type
         clientObject.coordinate_system = coordinate_system
 
          # Translational Release/Spring [N/m] N
         clientObject.axial_release_n = translational_release_n
 
         # Translational Release/Spring [N/m] Vy
         clientObject.axial_release_vy = translational_release_vy
@@ -249,14 +251,15 @@
 
             clientObject.diagram_along_y_table = Model.clientModel.factory.create('ns0:nodal_release_type.diagram_along_y_table')
 
             for i,j in enumerate(translational_release_vy_nonlinearity[2]):
                 mlvlp = Model.clientModel.factory.create('ns0:nodal_release_type_diagram_along_y_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:nodal_release_type_diagram_along_y_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.displacement = translational_release_vy_nonlinearity[2][i][0]
                 mlvlp.row.force = translational_release_vy_nonlinearity[2][i][1]
 
                 clientObject.diagram_along_y_table.nodal_release_type_diagram_along_y_table.append(mlvlp)
 
         elif translational_release_vy_nonlinearity[0] == NodalReleaseTypeReleaseNonlinearity.NONLINEARITY_TYPE_FRICTION_DIRECTION_1 \
         or translational_release_vy_nonlinearity[0] == NodalReleaseTypeReleaseNonlinearity.NONLINEARITY_TYPE_FRICTION_DIRECTION_2 \
@@ -418,14 +421,15 @@
 
             clientObject.diagram_around_x_table = Model.clientModel.factory.create('ns0:nodal_release_type.diagram_around_x_table')
 
             for i,j in enumerate(rotational_release_mt_nonlinearity[2]):
                 mlvlp = Model.clientModel.factory.create('ns0:nodal_release_type_diagram_around_x_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:nodal_release_type_diagram_around_x_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.rotation = rotational_release_mt_nonlinearity[2][i][0]
                 mlvlp.row.moment = rotational_release_mt_nonlinearity[2][i][1]
 
                 clientObject.diagram_around_x_table.nodal_release_type_diagram_around_x_table.append(mlvlp)
 
         else:
             raise TypeError('Incorrect Nodal Release Nonlinearity Type')
@@ -492,14 +496,15 @@
 
             clientObject.diagram_around_y_table = Model.clientModel.factory.create('ns0:nodal_release_type.diagram_around_y_table')
 
             for i,j in enumerate(rotational_release_my_nonlinearity[2]):
                 mlvlp = Model.clientModel.factory.create('ns0:nodal_release_type_diagram_around_y_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:nodal_release_type_diagram_around_y_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.rotation = rotational_release_my_nonlinearity[2][i][0]
                 mlvlp.row.moment = rotational_release_my_nonlinearity[2][i][1]
 
                 clientObject.diagram_around_y_table.nodal_release_type_diagram_around_y_table.append(mlvlp)
 
         else:
             raise TypeError('Incorrect Nodal Release Nonlinearity Type')
@@ -566,29 +571,30 @@
 
             clientObject.diagram_around_z_table = Model.clientModel.factory.create('ns0:nodal_release_type.diagram_around_z_table')
 
             for i,j in enumerate(rotational_release_mz_nonlinearity[2]):
                 mlvlp = Model.clientModel.factory.create('ns0:nodal_release_type_diagram_around_z_table_row')
                 mlvlp.no = i+1
                 mlvlp.row = Model.clientModel.factory.create('ns0:nodal_release_type_diagram_around_z_table')
+                clearAttributes(mlvlp.row)
                 mlvlp.row.rotation = rotational_release_mz_nonlinearity[2][i][0]
                 mlvlp.row.moment = rotational_release_mz_nonlinearity[2][i][1]
 
                 clientObject.diagram_around_z_table.nodal_release_type_diagram_around_z_table.append(mlvlp)
 
         else:
             raise TypeError('Incorrect Nodal Release Nonlinearity Type')
 
         # Nodal Release Local Axis System Object Type
         clientObject.local_axis_system_object_type = local_axis_system.name
 
         # Nodal Release Local Axis System Reference Object
         clientObject.local_axis_system_reference_object = local_axis_system_reference_object
 
-        # Line Release Type User defined name
+        # Nodal Release Type User defined name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
         # Comment
         clientObject.comment = comment
 
@@ -596,9 +602,9 @@
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add Node to client model
+        # Add Nodal Release Type to client model
         model.clientModel.service.set_nodal_release_type(clientObject)
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py` & `RSTAB-1.7.0/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
                  members: str = '1',
                  member_sets: str = '',
                  components: list = [
                     [SteelMemberLocalSectionReductionType.REDUCTION_COMPONENT_TYPE_DESIGN_PARAMETERS, 1.0, False,\
                      FastenerDefinitionType.DEFINITION_TYPE_ABSOLUTE, 0.5, 2,\
                      MultipleOffsetDefinitionType.OFFSET_DEFINITION_TYPE_ABSOLUTE, 1.0]
                                     ],
-                 user_defined_name: str = '',
+                 name: str = '',
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Args:
             no (int): Member Local Section Reduction Tag
             members (str): Assigned Members
@@ -55,17 +55,17 @@
         # Local Section Reduction Assigned Members
         clientObject.members = ConvertToDlString(members)
 
         # Local Section Reduction Assigned Member Sets
         clientObject.member_sets = ConvertToDlString(member_sets)
 
         # Local Section Reduction User defined Name
-        if user_defined_name:
+        if name:
             clientObject.user_defined_name_enabled = True
-            clientObject.name = user_defined_name
+            clientObject.name = name
 
         # Local Section Reduction Components
         clientObject.components = model.clientModel.factory.create('ns0:array_of_steel_member_local_section_reduction_components')
 
         for i,j in enumerate(components):
             smlsr = model.clientModel.factory.create('ns0:steel_member_local_section_reduction_components_row')
             smlsr.no = i+1
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py` & `RSTAB-1.7.0/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         # Boundary Conditions Nodal Supports
         clientObject.nodal_supports = model.clientModel.factory.create('ns0:steel_boundary_conditions.nodal_supports')
 
         for i,j in enumerate(nodal_supports):
             mlvlp = model.clientModel.factory.create('ns0:steel_boundary_conditions_nodal_supports_row')
             mlvlp.no = i+1
             mlvlp.row = model.clientModel.factory.create('ns0:steel_boundary_conditions_nodal_supports')
+            clearAttributes(mlvlp.row)
             mlvlp.row.node_seq_no = nodal_supports[i][0]
             mlvlp.row.support_type = nodal_supports[i][1].name
             mlvlp.row.support_in_x = nodal_supports[i][2]
             mlvlp.row.support_in_y = nodal_supports[i][3]
             mlvlp.row.support_in_z = nodal_supports[i][4]
             mlvlp.row.restraint_about_x = nodal_supports[i][5]
             mlvlp.row.restraint_about_y = nodal_supports[i][6]
@@ -142,14 +143,15 @@
         # Boundary Conditions Member Hinges
         clientObject.member_hinges = model.clientModel.factory.create('ns0:steel_boundary_conditions.member_hinges')
 
         for i,j in enumerate(member_hinges):
             mlvlp = model.clientModel.factory.create('ns0:steel_boundary_conditions_member_hinges_row')
             mlvlp.no = i+1
             mlvlp.row = model.clientModel.factory.create('ns0:steel_boundary_conditions_member_hinges')
+            clearAttributes(mlvlp.row)
             mlvlp.row.node_seq_no = member_hinges[i][0]
             mlvlp.row.release_in_x = member_hinges[i][1]
             mlvlp.row.release_in_y = member_hinges[i][2]
             mlvlp.row.release_in_z = member_hinges[i][3]
             mlvlp.row.release_about_x = member_hinges[i][4]
             mlvlp.row.release_about_y = member_hinges[i][5]
             mlvlp.row.release_about_z = member_hinges[i][6]
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py` & `RSTAB-1.7.0/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
         # Effective Lengths Nodal Supports
         clientObject.nodal_supports = model.clientModel.factory.create('ns0:array_of_steel_effective_lengths_nodal_supports')
 
         for i,j in enumerate(nodal_supports):
             mlvlp = model.clientModel.factory.create('ns0:steel_effective_lengths_nodal_supports_row')
             mlvlp.no = i+1
             mlvlp.row = model.clientModel.factory.create('ns0:steel_effective_lengths_nodal_supports')
+            clearAttributes(mlvlp.row)
             mlvlp.row.support_type = nodal_supports[i][0].name
             mlvlp.row.support_in_z = nodal_supports[i][1]
             mlvlp.row.support_spring_in_y = nodal_supports[i][2]
             mlvlp.row.eccentricity_type = nodal_supports[i][3].name
             mlvlp.row.eccentricity_ez = nodal_supports[i][4]
             mlvlp.row.restraint_spring_about_x = nodal_supports[i][5]
             mlvlp.row.restraint_spring_about_z = nodal_supports[i][6]
@@ -144,14 +145,15 @@
         # Effective Lengths Factors
         clientObject.factors = model.clientModel.factory.create('ns0:array_of_steel_effective_lengths_factors')
 
         for i,j in enumerate(factors):
             mlvlp_f = model.clientModel.factory.create('ns0:steel_effective_lengths_factors_row')
             mlvlp_f.no = i+1
             mlvlp_f.row = model.clientModel.factory.create('ns0:steel_effective_lengths_factors')
+            clearAttributes(mlvlp_f.row)
             mlvlp_f.row.flexural_buckling_u = factors[i][0]
             mlvlp_f.row.flexural_buckling_v = factors[i][1]
             mlvlp_f.row.flexural_buckling_y = factors[i][2]
             mlvlp_f.row.flexural_buckling_z = factors[i][3]
             mlvlp_f.row.torsional_buckling = factors[i][4]
             mlvlp_f.row.lateral_torsional_buckling = factors[i][5]
             mlvlp_f.row.lateral_torsional_buckling_top = factors[i][6]
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py` & `RSTAB-1.7.0/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         # Effective Lengths Nodal Supports
         clientObject.nodal_supports = model.clientModel.factory.create('ns0:array_of_timber_effective_lengths_nodal_supports')
 
         for i,j in enumerate(nodal_supports):
             mlvlp = model.clientModel.factory.create('ns0:timber_effective_lengths_nodal_supports_row')
             mlvlp.no = i+1
             mlvlp.row = model.clientModel.factory.create('ns0:timber_effective_lengths_nodal_supports')
+            clearAttributes(mlvlp.row)
             mlvlp.row.support_type = nodal_supports[i][0].name
             mlvlp.row.support_in_z = nodal_supports[i][1]
             mlvlp.row.eccentricity_type = nodal_supports[i][2].name
             mlvlp.row.support_in_y_type = nodal_supports[i][3].name
             mlvlp.row.restraint_about_x_type = nodal_supports[i][4].name
             mlvlp.row.nodes = ConvertToDlString(nodal_supports[i][5])
 
@@ -117,14 +118,15 @@
         # Effective Lengths Factors
         clientObject.factors = model.clientModel.factory.create('ns0:array_of_timber_effective_lengths_factors')
 
         for i,j in enumerate(factors):
             mlvlp_f = model.clientModel.factory.create('ns0:timber_effective_lengths_factors_row')
             mlvlp_f.no = i+1
             mlvlp_f.row = model.clientModel.factory.create('ns0:timber_effective_lengths_factors')
+            clearAttributes(mlvlp_f.row)
             mlvlp_f.row.flexural_buckling_u = factors[i][0]
             mlvlp_f.row.flexural_buckling_v = factors[i][1]
             mlvlp_f.row.lateral_torsional_buckling = factors[i][2]
 
             clientObject.factors.timber_effective_lengths_factors.append(mlvlp_f)
 
         # Effective Lengths Fire Design
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py` & `RSTAB-1.7.0/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberServiceClass.py` & `RSTAB-1.7.0/RSTAB/TypesForTimberDesign/timberServiceClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,31 @@
     def __init__(self,
                 no: int = 1,
                 name: str = '',
                 members: str = '',
                 member_sets: str = '',
                 service_class = TimberServiceClassServiceClass.TIMBER_SERVICE_CLASS_TYPE_1,
                 comment: str = '',
-                params: dict = None):
+                params: dict = None,
+                model = Model):
+
         """
         Args:
             no (int): Timber Service Class Tag
             name (str): User Defined Timber Service Class Name
             members (str): Assigned Members
             member_sets (str): Assigned Member Sets
             service_class (enum): Timber Service Class Service Class
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RFEM Class, optional): Model to be edited
         """
 
          # Client Model | Types For Timber Design Service Class
-        clientObject = Model.clientModel.factory.create('ns0:timber_service_class')
+        clientObject = model.clientModel.factory.create('ns0:timber_service_class')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Member Service Class
         clientObject.no = no
 
@@ -52,8 +55,8 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Service Class to client model
-        Model.clientModel.service.set_timber_service_class(clientObject)
+        model.clientModel.service.set_timber_service_class(clientObject)
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/ConcreteDurability.py` & `RSTAB-1.7.0/RSTAB/TypesforConcreteDesign/ConcreteDurability.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 class ConcreteDurability():
     def __init__(self,
                 no: int = 1,
                 name: str = "XC 1",
                 members_no: str = "1",
                 member_sets_no: str = "1",
-                surfaces_no: str = "1",
                 exposure_classes_reinforcement: list = [True, False, False, False],
                 exposure_classes_reinforcement_types: list = None,
                 exposure_classes_concrete: list = [False, False, False],
                 exposure_classes_concrete_types: list = None,
                 structural_class: list = [DurabilityStructuralClassType.STANDARD, False, False, False, False],
                 stainless_steel_reduction: list = [False],
                 additional_protection_reduction: list = [False],
@@ -21,15 +20,14 @@
                 model = Model):
         """
         Args:
             no (int): Concrete Durability Tag
             name (str): User Defined Name
             members_no (str): Assigned Members
             member_sets_no (str): Assigned Member Sets
-            surfaces_no (str): Assigned Surfaces
             exposure_classes_reinforcement (list): Exposure Classes Reinforcement Parameters
             exposure_classes_reinforcement_types (list of enum): Exposure Classes Reinforcement Type List of Enumeration
             exposure_classes_concrete (list): Exposure Classes Concrete Parameters
             exposure_classes_concrete_types (list of enum): Exposure Classes Concrete Type List of Enumeration
             structural_class (list): Structural Class Parameters
             stainless_steel_reduction (list): Stainless Steel Reduction Parameters
             additional_protection_reduction (list): Additional Protection Reduction
@@ -55,17 +53,14 @@
 
         # Assigned Members
         clientObject.members = ConvertToDlString(members_no)
 
         # Assigned Member Sets
         clientObject.member_sets = ConvertToDlString(member_sets_no)
 
-        # Assigned Surfaces
-        clientObject.surfaces = ConvertToDlString(surfaces_no)
-
         # Exposure Classes for Reinforcement
         clientObject.no_risk_of_corrosion_or_attack_enabled = exposure_classes_reinforcement[0]
         clientObject.corrosion_induced_by_carbonation_enabled = exposure_classes_reinforcement[1]
         clientObject.corrosion_induced_by_chlorides_enabled = exposure_classes_reinforcement[2]
         clientObject.corrosion_induced_by_chlorides_from_sea_water_enabled = exposure_classes_reinforcement[3]
 
         if all(exposure_classes_reinforcement):
```

### Comparing `RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py` & `RSTAB-1.7.0/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
         # Nodal Supports
         clientObject.nodal_supports = model.clientModel.factory.create('ns0:array_of_concrete_effective_lengths_nodal_supports')
         for i in range(len(nodal_supports)):
             mlvlp = model.clientModel.factory.create('ns0:concrete_effective_lengths_nodal_supports_row')
             mlvlp.no = i+1
             mlvlp.row = model.clientModel.factory.create('ns0:concrete_effective_lengths_nodal_supports')
+            clearAttributes(mlvlp.row)
             mlvlp.row.support_type = nodal_supports[i][0].name
             mlvlp.row.support_in_z = nodal_supports[i][1]
             mlvlp.row.eccentricity_type = nodal_supports[i][2].name
             mlvlp.row.support_in_y_type = nodal_supports[i][3].name
             mlvlp.row.restraint_about_x_type = nodal_supports[i][4].name
             mlvlp.row.restraint_about_z_type = nodal_supports[i][5].name
             mlvlp.row.restraint_warping_type = nodal_supports[i][6].name
```

### Comparing `RSTAB-1.6.0/RSTAB/baseData.py` & `RSTAB-1.7.0/RSTAB/baseData.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from RSTAB.initModel import Model
+from RSTAB.initModel import Model, clearAttributes
 from RSTAB.enums import ModelType
 
 class ModelParameters():
 
     def __init__(self,
                  model_parameters: list = None,
                  model = Model):
@@ -19,14 +19,15 @@
 
         # Add Model Parameters
 
         for i,j in enumerate(model_parameters):
             mp = Model.clientModel.factory.create('ns0:model_parameters_row')
             mp.no = i+3
             mp.row = Model.clientModel.factory.create('ns0:model_parameters')
+            clearAttributes(mp.row)
             mp.row.name = model_parameters[i][0]
             mp.row.description_1 = model_parameters[i][1]
             mp.row.description_2 = model_parameters[i][2]
 
             clientObject.model_parameters.append(mp)
 
         # Add Base Data Model Parameters to client model
@@ -51,14 +52,15 @@
         # Add Model Parameters
 
         for i,j in enumerate(model_parameters_location):
             mpl = Model.clientModel.factory.create('ns0:model_parameters_location_row')
             mpl.no = i+1
             mpl.description = str(i+1)
             mpl.row = Model.clientModel.factory.create('ns0:model_parameters_location')
+            clearAttributes(mpl.row)
             mpl.row.location_row_type = model_parameters_location[i][0].name
             mpl.row.name = model_parameters_location[i][1]
             mpl.row.value = model_parameters_location[i][2]
             mpl.row.unit_group = model_parameters_location[i][3]
 
             clientObject.model_parameters_location.append(mpl)
```

### Comparing `RSTAB-1.6.0/RSTAB/baseSettings.py` & `RSTAB-1.7.0/RSTAB/baseSettings.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,26 @@
     def __init__(self,
                 gravitational_acceleration: int = 10,
                 global_axes_orientation = GlobalAxesOrientationType.E_GLOBAL_AXES_ORIENTATION_ZDOWN,
                 local_axes_orientation = LocalAxesOrientationType.E_LOCAL_AXES_ORIENTATION_ZDOWN,
                 tolerances: list = [0.0005, 0.0005, 0.0005, 0.0005],
                 member_representatives: bool = False,
                 member_set_representatives: bool = False,
+                params: dict = None,
                 model = Model):
         """
         Args:
             gravitational_acceleration (int): Gravitational Acceleration (m/sn2)
             global_axes_orientation (enum): Global Axes Orientation Enumeration
             local_axes_orientation (Enum): Local Axes Orientation Enumeration
             tolerances (list): Tolerances List
                 tolerances = [tolerance_for_nodes, tolerance_for_lines, tolerance_for_surfaces_and_planes, tolerance_for_directions]
             member_representatives (bool): Member Representatives
             member_set_representatives (bool): Member Set Representatives
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
         # Client model | Get Model Settings
         clientObject = model.clientModel.service.get_model_settings_and_options()
 
         # Gravitational Acceleration
         clientObject.gravitational_acceleration = gravitational_acceleration
@@ -44,9 +46,14 @@
 
         # Member Representatives
         clientObject.member_representatives_active = member_representatives
 
         # Member Set Representatives
         clientObject.member_set_representatives_active = member_set_representatives
 
+        # Adding optional parameters via dictionary
+        if params:
+            for key in params:
+                clientObject[key] = params[key]
+
         # Add Base Data Settings to client model
         model.clientModel.service.set_model_settings_and_options(clientObject)
```

### Comparing `RSTAB-1.6.0/RSTAB/dependencies.py` & `RSTAB-1.7.0/RSTAB/dependencies.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/enums.py` & `RSTAB-1.7.0/RSTAB/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,14 @@
 class NodalSupportType(Enum):
     '''
     Nodal Support Type
     '''
     FIXED, HINGED, ROLLER, ROLLER_IN_X, ROLLER_IN_Y, ROLLER_IN_Z, FREE = range(7)
 
 
-class LineSupportType(Enum):
-    '''
-    Nodal Support Type
-    '''
-    FIXED, HINGED, SLIDING_IN_X_AND_Y, SLIDING_IN_X, SLIDING_IN_Y, SLIDING_IN_Z, FREE = range(7)
-
-
-class LineWeldedJointType(Enum):
-    """
-    Line Welded Joint Type | Enum
-    """
-    BUTT_JOINT, CORNER_JOINT, LAP_JOINT, TEE_JOINT = range(4)
-
-
 class WeldType(Enum):
     """
     Welded Type | Enum
     """
     WELD_BEVEL_AND_FILLET, WELD_DOUBLE_BEVEL, WELD_DOUBLE_FILLET, WELD_DOUBLE_J,\
     WELD_DOUBLE_SQUARE, WELD_DOUBLE_U, WELD_DOUBLE_V, WELD_J_AND_FILLET, WELD_SINGLE_BEVEL,\
     WELD_SINGLE_FILLET, WELD_SINGLE_J, WELD_SINGLE_SQUARE, WELD_SINGLE_U, WELD_SINGLE_V, WELD_V_AND_FILLET = range(15)
@@ -57,21 +43,14 @@
 class WeldLongitudalArrangement(Enum):
     """
     Weld Longitudat Arrangement Type | Enum
     """
     CHAIN_INTERMITTENT, CONTINUOUS, STAGGERED_INTERMITTENT = range(3)
 
 
-class LineMeshRefinementsType(Enum):
-    """
-    Line Mesh Refinements Type | Enum
-    """
-    TYPE_LENGTH, TYPE_ELEMENTS, TYPE_GRADUAL = range(3)
-
-
 class StaticAnalysisType(Enum):
     '''
     Static Analysis Type
     '''
     GEOMETRICALLY_LINEAR, LARGE_DEFORMATIONS, LARGE_DEFORMATIONS_POSTRCRITICAL, SECOND_ORDER_P_DELTA = range(4)
 
 
@@ -101,17 +80,17 @@
     '''
     Analysis Type
     '''
     ANALYSIS_TYPE_CREEP_AND_SHRINKAGE, ANALYSIS_TYPE_CUTTING_PATTERN, ANALYSIS_TYPE_MODAL, ANALYSIS_TYPE_RESPONSE_SPECTRUM,\
     ANALYSIS_TYPE_STATIC, ANALYSIS_TYPE_TIME_DEPENDENT, ANALYSIS_TYPE_TIME_HISTORY, ANALYSIS_TYPE_WIND_SIMULATION = range(8)
 
 
-class LoadDirectionType(Enum):
+class NodalLoadDirection(Enum):
     '''
-    Load Direction Type
+    Nodal Load Direction
     '''
     LOAD_DIRECTION_GLOBAL_X_OR_USER_DEFINED_U, LOAD_DIRECTION_GLOBAL_Y_OR_USER_DEFINED_V, LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W,\
     LOAD_DIRECTION_LOCAL_X, LOAD_DIRECTION_LOCAL_Y, LOAD_DIRECTION_LOCAL_Z = range(6)
 
 
 class MemberLoadDirection(Enum):
     '''
@@ -149,96 +128,14 @@
     Member Hinge Axial Release
     '''
     NONLINEARITY_TYPE_DIAGRAM, NONLINEARITY_TYPE_FAILURE_ALL_IF_NEGATIVE, NONLINEARITY_TYPE_FAILURE_ALL_IF_POSITIVE,\
     NONLINEARITY_TYPE_FAILURE_IF_NEGATIVE, NONLINEARITY_TYPE_FAILURE_IF_POSITIVE, NONLINEARITY_TYPE_FRICTION_DIRECTION_1,\
     NONLINEARITY_TYPE_FRICTION_DIRECTION_1_2, NONLINEARITY_TYPE_FRICTION_DIRECTION_1_PLUS_2, NONLINEARITY_TYPE_FRICTION_DIRECTION_2,\
     NONLINEARITY_TYPE_NONE, NONLINEARITY_TYPE_PARTIAL_ACTIVITY, NONLINEARITY_TYPE_STIFFNESS_DIAGRAM = range(12)
 
-
-class LineLoadType(Enum):
-    '''
-    Line Load Type
-    '''
-    E_TYPE_MASS, LOAD_TYPE_FORCE, LOAD_TYPE_MOMENT = range(3)
-
-
-class LineSetLoadType(Enum):
-    '''
-    Lineset Load Type
-    '''
-    E_TYPE_MASS, LOAD_TYPE_FORCE, LOAD_TYPE_MOMENT = range(3)
-
-
-class LineLoadDistribution(Enum):
-    '''
-    Line Load Distribution
-    '''
-    LOAD_DISTRIBUTION_CONCENTRATED_1, LOAD_DISTRIBUTION_CONCENTRATED_2, LOAD_DISTRIBUTION_CONCENTRATED_2x2,\
-    LOAD_DISTRIBUTION_CONCENTRATED_N, LOAD_DISTRIBUTION_CONCENTRATED_VARYING, LOAD_DISTRIBUTION_PARABOLIC,\
-    LOAD_DISTRIBUTION_TAPERED, LOAD_DISTRIBUTION_TRAPEZOIDAL, LOAD_DISTRIBUTION_UNIFORM, LOAD_DISTRIBUTION_UNIFORM_TOTAL,\
-    LOAD_DISTRIBUTION_VARYING = range(11)
-
-
-class LineSetLoadDistribution(Enum):
-    '''
-    Line Load Distribution
-    '''
-    LOAD_DISTRIBUTION_CONCENTRATED_1, LOAD_DISTRIBUTION_CONCENTRATED_2, LOAD_DISTRIBUTION_CONCENTRATED_2x2,\
-    LOAD_DISTRIBUTION_CONCENTRATED_N, LOAD_DISTRIBUTION_CONCENTRATED_VARYING, LOAD_DISTRIBUTION_PARABOLIC,\
-    LOAD_DISTRIBUTION_TAPERED, LOAD_DISTRIBUTION_TRAPEZOIDAL, LOAD_DISTRIBUTION_UNIFORM, LOAD_DISTRIBUTION_UNIFORM_TOTAL,\
-    LOAD_DISTRIBUTION_VARYING = range(11)
-
-
-class SurfaceGeometry(Enum):
-    '''
-    Geometry Type
-    '''
-    GEOMETRY_PLANE, GEOMETRY_QUADRANGLE, GEOMETRY_NURBS, GEOMETRY_ROTATED, GEOMETRY_PIPE = range(5)
-
-
-class SurfaceType(Enum):
-    '''
-    Stiffness Type
-    '''
-    TYPE_LOAD_TRANSFER, TYPE_MEMBRANE, TYPE_RIGID, TYPE_STANDARD, TYPE_WITHOUT_MEMBRANE_TENSION, TYPE_WITHOUT_THICKNESS = range(6)
-
-
-class SurfaceLoadDistribution(Enum):
-    '''
-    Surface Load Distribution
-    '''
-    LOAD_DISTRIBUTION_LINEAR, LOAD_DISTRIBUTION_LINEAR_IN_X, LOAD_DISTRIBUTION_LINEAR_IN_Y, LOAD_DISTRIBUTION_LINEAR_IN_Z,\
-    LOAD_DISTRIBUTION_RADIAL, LOAD_DISTRIBUTION_UNIFORM, LOAD_DISTRIBUTION_VARYING_IN_Z = range(7)
-
-
-class SurfaceLoadDirection(Enum):
-    '''
-    Surface Load Direction | Enum
-    '''
-    LOAD_DIRECTION_GLOBAL_X_OR_USER_DEFINED_U_PROJECTED, LOAD_DIRECTION_GLOBAL_X_OR_USER_DEFINED_U_TRUE,\
-    LOAD_DIRECTION_GLOBAL_Y_OR_USER_DEFINED_V_PROJECTED, LOAD_DIRECTION_GLOBAL_Y_OR_USER_DEFINED_V_TRUE,\
-    LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_PROJECTED, LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_TRUE,\
-    LOAD_DIRECTION_LOCAL_X, LOAD_DIRECTION_LOCAL_Y, LOAD_DIRECTION_LOCAL_Z = range(9)
-
-
-class SurfaceLoadType(Enum):
-    '''
-    Surface Load Type | Enum
-    '''
-    LOAD_TYPE_AXIAL_STRAIN, LOAD_TYPE_FORCE, LOAD_TYPE_FORM_FINDING, LOAD_TYPE_MASS, LOAD_TYPE_PRECAMBER,\
-    LOAD_TYPE_ROTARY_MOTION, LOAD_TYPE_TEMPERATURE = range(7)
-
-
-class SurfaceLoadDistributionDirection(Enum):
-    '''
-    Surface Load Distribution Direction
-    '''
-    LOAD_TRANSFER_DIRECTION_IN_BOTH, LOAD_TRANSFER_DIRECTION_IN_X, LOAD_TRANSFER_DIRECTION_IN_Y = range(3)
-
-
 class SetType(Enum):
     '''
     Line, Member, Surface, and Solid Set Type
     '''
     SET_TYPE_CONTINUOUS, SET_TYPE_GROUP = range(2)
 
 
@@ -316,34 +213,14 @@
 
 
 class ThicknessOrthotropyType(Enum):
     BIDIRECTIONAL_RIBBED_PLATE, COUPLING, EFFECTIVE_THICKNESS, GRILLAGE, \
     HOLLOW_CORE_SLAB, TRAPEZOIDAL_SHEET, UNIDIRECTIONAL_RIBBED_PLATE = range(7)
 
 
-class LineLoadDirection(Enum):
-    '''
-    Line Load Direction
-    '''
-    LOAD_DIRECTION_GLOBAL_X_OR_USER_DEFINED_U_PROJECTED, LOAD_DIRECTION_GLOBAL_X_OR_USER_DEFINED_U_TRUE,\
-    LOAD_DIRECTION_GLOBAL_Y_OR_USER_DEFINED_V_PROJECTED, LOAD_DIRECTION_GLOBAL_Y_OR_USER_DEFINED_V_TRUE,\
-    LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_PROJECTED, LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_TRUE,\
-    LOAD_DIRECTION_LOCAL_X, LOAD_DIRECTION_LOCAL_Y, LOAD_DIRECTION_LOCAL_Z = range(9)
-
-
-class LineSetLoadDirection(Enum):
-    '''
-    Lineset Load Direction
-    '''
-    LOAD_DIRECTION_GLOBAL_X_OR_USER_DEFINED_U_PROJECTED, LOAD_DIRECTION_GLOBAL_X_OR_USER_DEFINED_U_TRUE,\
-    LOAD_DIRECTION_GLOBAL_Y_OR_USER_DEFINED_V_PROJECTED, LOAD_DIRECTION_GLOBAL_Y_OR_USER_DEFINED_V_TRUE,\
-    LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_PROJECTED, LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_TRUE,\
-    LOAD_DIRECTION_LOCAL_X, LOAD_DIRECTION_LOCAL_Y, LOAD_DIRECTION_LOCAL_Z = range(9)
-
-
 class MemberLoadEccentricityHorizontalAlignment(Enum):
     '''
     Member Load Eccentricity Horizontal Alignment
     '''
 
     ALIGN_LEFT, ALIGN_MIDDLE, ALIGN_NONE, ALIGN_TOP = range(4)
 
@@ -463,21 +340,14 @@
 class NodeReferenceType(Enum):
     '''
     Node Reference Type| Enum
     '''
     REFERENCE_TYPE_L, REFERENCE_TYPE_XY, REFERENCE_TYPE_XZ, REFERENCE_TYPE_YZ = range(4)
 
 
-class LineArcAlphaAdjustmentTarget(Enum):
-    '''
-    Line Arc Alpha Adjustment Target | Enum
-    '''
-    ALPHA_ADJUSTMENT_TARGET_ARC_CONTROL_POINT, ALPHA_ADJUSTMENT_TARGET_BEGINNING_OF_ARC, ALPHA_ADJUSTMENT_TARGET_END_OF_ARC = range(3)
-
-
 class MemberSetLoadType(Enum):
     '''
     Member Set Load Load Type
     '''
     E_TYPE_MASS, LOAD_TYPE_AXIAL_DISPLACEMENT, LOAD_TYPE_AXIAL_STRAIN, LOAD_TYPE_DISPLACEMENT, \
     LOAD_TYPE_FORCE, LOAD_TYPE_FORM_FINDING, LOAD_TYPE_INITIAL_PRESTRESS, LOAD_TYPE_MOMENT, \
     LOAD_TYPE_PIPE_CONTENT_FULL, LOAD_TYPE_PIPE_CONTENT_PARTIAL, LOAD_TYPE_PIPE_INTERNAL_PRESSURE, \
@@ -694,32 +564,14 @@
 class FreeConcentratedLoadLoadType(Enum):
     '''
     Free Concentrated Load Load Type | Enum
     '''
     LOAD_TYPE_FORCE, LOAD_TYPE_MOMENT = range(2)
 
 
-class FreeLineLoadLoadDirection(Enum):
-    '''
-    Free Line Load Load Direction | Enum
-    '''
-    LOAD_DIRECTION_GLOBAL_X_PROJECTED, LOAD_DIRECTION_GLOBAL_X_TRUE, LOAD_DIRECTION_GLOBAL_Y_PROJECTED, \
-    LOAD_DIRECTION_GLOBAL_Y_TRUE, LOAD_DIRECTION_GLOBAL_Z_PROJECTED, LOAD_DIRECTION_GLOBAL_Z_TRUE, \
-    LOAD_DIRECTION_LOCAL_X, LOAD_DIRECTION_LOCAL_Y, LOAD_DIRECTION_LOCAL_Z, LOAD_DIRECTION_USER_DEFINED_U_PROJECTED, \
-    LOAD_DIRECTION_USER_DEFINED_U_TRUE, LOAD_DIRECTION_USER_DEFINED_V_PROJECTED, LOAD_DIRECTION_USER_DEFINED_V_TRUE, \
-    LOAD_DIRECTION_USER_DEFINED_W_PROJECTED, LOAD_DIRECTION_USER_DEFINED_W_TRUE = range(15)
-
-
-class FreeLineLoadLoadDistribution(Enum):
-    '''
-    Free Line Load Load Distribution | Enum
-    '''
-    LOAD_DISTRIBUTION_LINEAR, LOAD_DISTRIBUTION_UNIFORM = range(2)
-
-
 class FreeRectangularLoadLoadDirection(Enum):
     '''
     Free Rectangular Load Load Direction | Enum
     '''
     LOAD_DIRECTION_GLOBAL_X_PROJECTED, LOAD_DIRECTION_GLOBAL_X_TRUE, LOAD_DIRECTION_GLOBAL_Y_PROJECTED, \
     LOAD_DIRECTION_GLOBAL_Y_TRUE, LOAD_DIRECTION_GLOBAL_Z_PROJECTED, LOAD_DIRECTION_GLOBAL_Z_TRUE, \
     LOAD_DIRECTION_LOCAL_X, LOAD_DIRECTION_LOCAL_Y, LOAD_DIRECTION_LOCAL_Z, LOAD_DIRECTION_USER_DEFINED_U_PROJECTED, \
@@ -862,47 +714,33 @@
     Stability Analysis Settings Stopping Of Load Increasing Result | Enum
     '''
     RESULT_TYPE_DISPLACEMENT_U, RESULT_TYPE_DISPLACEMENT_U_X, RESULT_TYPE_DISPLACEMENT_U_Y, \
     RESULT_TYPE_DISPLACEMENT_U_Z, RESULT_TYPE_ROTATION_PHI, RESULT_TYPE_ROTATION_PHI_X, \
     RESULT_TYPE_ROTATION_PHI_Y, RESULT_TYPE_ROTATION_PHI_Z = range(8)
 
 
-class LineType(Enum):
-    '''
-    Line Type
-    '''
-    TYPE_ARC, TYPE_CIRCLE, TYPE_CUT_VIA_SECTION, TYPE_CUT_VIA_TWO_LINES, TYPE_ELLIPTICAL_ARC, TYPE_ELLIPSE, TYPE_NURBS, TYPE_PARABOLA, TYPE_POLYLINE, TYPE_SPLINE = range(10)
-
-
 class ObjectTypes(Enum):
     '''
     Object Types
     '''
-    E_OBJECT_TYPE_ACTION, E_OBJECT_TYPE_ACTION_COMBINATION, E_OBJECT_TYPE_ALUMINUM_EFFECTIVE_LENGTHS, E_OBJECT_TYPE_ALUMINUM_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_ALUMINUM_MEMBER_TRANSVERSE_WELD, E_OBJECT_TYPE_BOREHOLE, \
-    E_OBJECT_TYPE_BUILDING_STORY, E_OBJECT_TYPE_CLIPPING_BOX, E_OBJECT_TYPE_CLIPPING_PLANE, E_OBJECT_TYPE_COMBINATION_WIZARD, E_OBJECT_TYPE_CONSTRUCTION_STAGE,  \
-    E_OBJECT_TYPE_COORDINATE_SYSTEM, E_OBJECT_TYPE_DESIGN_SITUATION, E_OBJECT_TYPE_DESIGN_SUPPORT, E_OBJECT_TYPE_DIMENSION, E_OBJECT_TYPE_DXF_FILE_MODEL_OBJECT,  \
-    E_OBJECT_TYPE_DXF_MODEL_OBJECT, E_OBJECT_TYPE_FREE_CIRCULAR_LOAD, E_OBJECT_TYPE_FREE_CONCENTRATED_LOAD, E_OBJECT_TYPE_FREE_LINE_LOAD, E_OBJECT_TYPE_FREE_POLYGON_LOAD,  \
-    E_OBJECT_TYPE_FREE_RECTANGULAR_LOAD, E_OBJECT_TYPE_GLOBAL_PARAMETER, E_OBJECT_TYPE_IMPERFECTION_CASE, E_OBJECT_TYPE_IMPOSED_LINE_DEFORMATION, E_OBJECT_TYPE_IMPOSED_NODAL_DEFORMATION, \
-    E_OBJECT_TYPE_INTERSECTION, E_OBJECT_TYPE_LINE, E_OBJECT_TYPE_LINE_GRID, E_OBJECT_TYPE_LINE_HINGE, E_OBJECT_TYPE_LINE_LOAD, E_OBJECT_TYPE_LINE_MESH_REFINEMENT, E_OBJECT_TYPE_LINE_SET, \
-    E_OBJECT_TYPE_LINE_SET_LOAD, E_OBJECT_TYPE_LINE_SUPPORT, E_OBJECT_TYPE_LINE_WELDED_JOINT, E_OBJECT_TYPE_LOAD_CASE, E_OBJECT_TYPE_LOAD_COMBINATION, E_OBJECT_TYPE_MATERIAL, \
-    E_OBJECT_TYPE_MEMBER, E_OBJECT_TYPE_MEMBER_DEFINABLE_STIFFNESS, E_OBJECT_TYPE_MEMBER_ECCENTRICITY, E_OBJECT_TYPE_MEMBER_HINGE, E_OBJECT_TYPE_MEMBER_IMPERFECTION, E_OBJECT_TYPE_MEMBER_LOAD, \
-    E_OBJECT_TYPE_MEMBER_NONLINEARITY, E_OBJECT_TYPE_MEMBER_REPRESENTATIVE, E_OBJECT_TYPE_MEMBER_RESULT_INTERMEDIATE_POINT, E_OBJECT_TYPE_MEMBER_SET, E_OBJECT_TYPE_MEMBER_SET_IMPERFECTION, \
-    E_OBJECT_TYPE_MEMBER_SET_LOAD, E_OBJECT_TYPE_MEMBER_SET_REPRESENTATIVE, E_OBJECT_TYPE_MEMBER_STIFFNESS_MODIFICATION, E_OBJECT_TYPE_MEMBER_SUPPORT, E_OBJECT_TYPE_MEMBER_TRANSVERSE_STIFFENER, \
-    E_OBJECT_TYPE_MODAL_ANALYSIS_SETTINGS, E_OBJECT_TYPE_NODAL_LOAD, E_OBJECT_TYPE_NODAL_MESH_REFINEMENT, E_OBJECT_TYPE_NODAL_SUPPORT, E_OBJECT_TYPE_NODE, E_OBJECT_TYPE_NOTE, \
-    E_OBJECT_TYPE_OBJECT_SNAP, E_OBJECT_TYPE_OPENING, E_OBJECT_TYPE_OPENING_LOAD, E_OBJECT_TYPE_PUNCHING_REINFORCEMENT, E_OBJECT_TYPE_RELATIONSHIP_BETWEEN_LOAD_CASES, \
-    E_OBJECT_TYPE_RESULT_COMBINATION, E_OBJECT_TYPE_RESULT_SECTION, E_OBJECT_TYPE_RIGID_LINK, E_OBJECT_TYPE_SECTION, E_OBJECT_TYPE_SOIL_MASSIF, E_OBJECT_TYPE_SOLID, E_OBJECT_TYPE_SOLID_CONTACTS, \
-    E_OBJECT_TYPE_SOLID_GAS, E_OBJECT_TYPE_SOLID_LOAD, E_OBJECT_TYPE_SOLID_MESH_REFINEMENT, E_OBJECT_TYPE_SOLID_SET, E_OBJECT_TYPE_SOLID_SET_LOAD, E_OBJECT_TYPE_SPECTRAL_ANALYSIS_SETTINGS, \
-    E_OBJECT_TYPE_STABILITY_ANALYSIS_SETTINGS, E_OBJECT_TYPE_STATIC_ANALYSIS_SETTINGS, E_OBJECT_TYPE_STEEL_BOUNDARY_CONDITIONS, E_OBJECT_TYPE_STEEL_EFFECTIVE_LENGTHS, \
-    E_OBJECT_TYPE_STEEL_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_STRUCTURE_MODIFICATION, \
-    E_OBJECT_TYPE_SURFACE, E_OBJECT_TYPE_SURFACES_CONTACT, E_OBJECT_TYPE_SURFACES_CONTACT_TYPE, E_OBJECT_TYPE_SURFACE_ECCENTRICITY, E_OBJECT_TYPE_SURFACE_IMPERFECTION, E_OBJECT_TYPE_SURFACE_LOAD, \
-    E_OBJECT_TYPE_SURFACE_MESH_REFINEMENT, E_OBJECT_TYPE_SURFACE_RESULTS_ADJUSTMENT, E_OBJECT_TYPE_SURFACE_SET, E_OBJECT_TYPE_SURFACE_SET_IMPERFECTION, E_OBJECT_TYPE_SURFACE_SET_LOAD, \
-    E_OBJECT_TYPE_SURFACE_STIFFNESS_MODIFICATION, E_OBJECT_TYPE_SURFACE_SUPPORT, E_OBJECT_TYPE_TERRAIN, E_OBJECT_TYPE_THICKNESS, E_OBJECT_TYPE_TIMBER_EFFECTIVE_LENGTHS, \
-    E_OBJECT_TYPE_TIMBER_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_TIMBER_MOISTURE_CLASS, \
-    E_OBJECT_TYPE_TIMBER_SERVICE_CLASS, E_OBJECT_TYPE_TIMBER_SERVICE_CONDITIONS, E_OBJECT_TYPE_VISUAL_OBJECT, E_OBJECT_TYPE_WIND_PROFILE, E_OBJECT_TYPE_WIND_SIMULATION, E_OBJECT_TYPE_WIND_SIMULATION_ANALYSIS_SETTINGS,\
-    E_OBJECT_TYPE_RESPONSE_SPECTRUM, E_OBJECT_TYPE_MEMBER_ROTATIONAL_RESTRAINT, E_OBJECT_TYPE_MEMBER_SHEAR_PANEL = range(112)
+    E_OBJECT_TYPE_ACCELEROGRAM, E_OBJECT_TYPE_ACTION, E_OBJECT_TYPE_ACTION_COMBINATION, E_OBJECT_TYPE_ALUMINUM_DESIGN_SLS_CONFIGURATION, E_OBJECT_TYPE_ALUMINUM_DESIGN_ULS_CONFIGURATION, E_OBJECT_TYPE_ALUMINUM_EFFECTIVE_LENGTHS, \
+    E_OBJECT_TYPE_ALUMINUM_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_ALUMINUM_MEMBER_TRANSVERSE_WELD, E_OBJECT_TYPE_CALCULATION_DIAGRAM, E_OBJECT_TYPE_CLIPPING_BOX, E_OBJECT_TYPE_CLIPPING_PLANE, E_OBJECT_TYPE_COMBINATION_WIZARD, \
+    E_OBJECT_TYPE_CONCRETE_DESIGN_SLS_CONFIGURATION, E_OBJECT_TYPE_CONCRETE_DESIGN_ULS_CONFIGURATION, E_OBJECT_TYPE_CONCRETE_DURABILITY, E_OBJECT_TYPE_CONCRETE_EFFECTIVE_LENGTHS, E_OBJECT_TYPE_COORDINATE_SYSTEM, \
+    E_OBJECT_TYPE_DESIGN_SITUATION, E_OBJECT_TYPE_DESIGN_SUPPORT, E_OBJECT_TYPE_DIMENSION, E_OBJECT_TYPE_DXF_FILE_MODEL_OBJECT, E_OBJECT_TYPE_DXF_MODEL_OBJECT, E_OBJECT_TYPE_GLOBAL_PARAMETER, E_OBJECT_TYPE_IMPERFECTION_CASE, \
+    E_OBJECT_TYPE_IMPOSED_NODAL_DEFORMATION, E_OBJECT_TYPE_LINE_GRID, E_OBJECT_TYPE_LOAD_CASE, E_OBJECT_TYPE_LOAD_COMBINATION, E_OBJECT_TYPE_MATERIAL, E_OBJECT_TYPE_MEMBER, E_OBJECT_TYPE_MEMBER_DEFINABLE_STIFFNESS, \
+    E_OBJECT_TYPE_MEMBER_ECCENTRICITY, E_OBJECT_TYPE_MEMBER_HINGE, E_OBJECT_TYPE_MEMBER_IMPERFECTION, E_OBJECT_TYPE_MEMBER_LOAD, E_OBJECT_TYPE_MEMBER_NONLINEARITY, E_OBJECT_TYPE_MEMBER_OPENINGS, E_OBJECT_TYPE_MEMBER_REPRESENTATIVE, \
+    E_OBJECT_TYPE_MEMBER_RESULT_INTERMEDIATE_POINT, E_OBJECT_TYPE_MEMBER_ROTATIONAL_RESTRAINT, E_OBJECT_TYPE_MEMBER_SET, E_OBJECT_TYPE_MEMBER_SET_IMPERFECTION, E_OBJECT_TYPE_MEMBER_SET_LOAD, E_OBJECT_TYPE_MEMBER_SET_REPRESENTATIVE, \
+    E_OBJECT_TYPE_MEMBER_SHEAR_PANEL, E_OBJECT_TYPE_MEMBER_STIFFNESS_MODIFICATION, E_OBJECT_TYPE_MEMBER_SUPPORT, E_OBJECT_TYPE_MEMBER_TRANSVERSE_STIFFENER, E_OBJECT_TYPE_MODAL_ANALYSIS_SETTINGS, E_OBJECT_TYPE_NODAL_LOAD, \
+    E_OBJECT_TYPE_NODAL_RELEASE, E_OBJECT_TYPE_NODAL_RELEASE_TYPE, E_OBJECT_TYPE_NODAL_SUPPORT, E_OBJECT_TYPE_NODE, E_OBJECT_TYPE_NOTE, E_OBJECT_TYPE_OBJECT_SNAP, E_OBJECT_TYPE_OPTIMIZATION_SETTINGS, E_OBJECT_TYPE_RELATIONSHIP_BETWEEN_LOAD_CASES, \
+    E_OBJECT_TYPE_RESPONSE_SPECTRUM, E_OBJECT_TYPE_RESULT_COMBINATION, E_OBJECT_TYPE_SECTION, E_OBJECT_TYPE_SPECTRAL_ANALYSIS_SETTINGS, E_OBJECT_TYPE_STABILITY_ANALYSIS_SETTINGS, E_OBJECT_TYPE_STATIC_ANALYSIS_SETTINGS, \
+    E_OBJECT_TYPE_STEEL_BOUNDARY_CONDITIONS, E_OBJECT_TYPE_STEEL_DESIGN_FR_CONFIGURATION, E_OBJECT_TYPE_STEEL_DESIGN_SEISMIC_CONFIGURATION, E_OBJECT_TYPE_STEEL_DESIGN_SLS_CONFIGURATION, E_OBJECT_TYPE_STEEL_DESIGN_ULS_CONFIGURATION, \
+    E_OBJECT_TYPE_STEEL_EFFECTIVE_LENGTHS, E_OBJECT_TYPE_STEEL_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_STRUCTURE_MODIFICATION, E_OBJECT_TYPE_TERRAIN, E_OBJECT_TYPE_TIMBER_DESIGN_FR_CONFIGURATION, \
+    E_OBJECT_TYPE_TIMBER_DESIGN_SLS_CONFIGURATION, E_OBJECT_TYPE_TIMBER_DESIGN_ULS_CONFIGURATION, E_OBJECT_TYPE_TIMBER_EFFECTIVE_LENGTHS, E_OBJECT_TYPE_TIMBER_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_TIMBER_MOISTURE_CLASS, \
+    E_OBJECT_TYPE_TIMBER_SERVICE_CLASS, E_OBJECT_TYPE_TIMBER_SERVICE_CONDITIONS, E_OBJECT_TYPE_VISUAL_OBJECT = range(82)
+
 
 class export_to_ifc_axis_rotation_sequence_type(Enum):
     '''
     Export to IFC Axis Rotation Sequence Type
     '''
     XYZ, XZY, YXZ, YZX, ZXY, ZYX = range(6)
 
@@ -979,15 +817,15 @@
     CANTILEVERS_TYPE_HORIZONTAL, CANTILEVERS_TYPE_OFFSET, CANTILEVERS_TYPE_PARALLEL, CANTILEVERS_TYPE_TAPER = range(4)
 
 
 class MemberRotationSpecificationType(Enum):
     ''''
     Member Rotation Specification Type
     '''
-    COORDINATE_SYSTEM_ROTATION_VIA_ANGLE, COORDINATE_SYSTEM_ROTATION_VIA_HELP_NODE, COORDINATE_SYSTEM_ROTATION_VIA_INSIDE_NODE, COORDINATE_SYSTEM_ROTATION_VIA_SURFACE = range(4)
+    COORDINATE_SYSTEM_ROTATION_VIA_ANGLE, COORDINATE_SYSTEM_ROTATION_VIA_HELP_NODE = range(2)
 
 
 class MemberRotationPlaneType(Enum):
     '''
     Member Rotation Plane Type
     '''
     ROTATION_PLANE_XY, ROTATION_PLANE_XZ = range(2)
@@ -1504,28 +1342,27 @@
 class ImperfectionCaseAssignmentType(Enum):
     '''
     Imperfection Case, Static Deformation Type, Magnitude Assignment Type
     '''
     MAGNITUDE_ASSIGNMENT_SPECIFIC_NODE, MAGNITUDE_ASSIGNMENT_LOCATION_WITH_LARGEST_DISPLACEMENT = range(2)
 
 
-class OptimizeOnType(Enum):
+class OptimizerType(Enum):
     '''
-    Optimization Settings Optimize On Type
+    Optimization Settings
     '''
-    E_OPTIMIZE_ON_TYPE_MIN_WHOLE_WEIGHT, E_OPTIMIZE_ON_TYPE_MIN_VECTORIAL_DISPLACEMENT, E_OPTIMIZE_ON_TYPE_MIN_MEMBER_DEFORMATION, \
-    E_OPTIMIZE_ON_TYPE_MIN_SURFACE_DEFORMATION, E_OPTIMIZE_ON_TYPE_MIN_COST, E_OPTIMIZE_ON_TYPE_MIN_CO2_EMISSIONS = range(6)
+    ALL_MUTATIONS, PARTICLE_SWARM, RANDOM_MUTATIONS = range(3)
 
 
-class Optimizer(Enum):
+class OptimizationTargetValueType(Enum):
     '''
-    Optimization Settings Optimizer
+    Optimization Settings
     '''
-    E_OPTIMIZER_TYPE_ALL_MUTATIONS, E_OPTIMIZER_TYPE_PERCENTS_OF_RANDOM_MUTATIONS, E_OPTIMIZER_TYPE_PARTICLE_SWARM = range(3)
-
+    MAX_GLOBAL_PARAMETER, MIN_CO2_EMISSIONS, MIN_COST, MIN_GLOBAL_PARAMETER, MIN_MEMBER_DEFORMATION, MIN_NODAL_DEFORMATION, \
+    MIN_SURFACE_DEFORMATION, MIN_TOTAL_WEIGHT, MIN_VECTORIAL_DISPLACEMENT = range(9)
 
 class SurfacesShapeOfFiniteElements(Enum):
     '''
     Surfaces Shape of Finite Elements
     '''
     E_SHAPE_OF_FINITE_ELEMENTS_FOR_SURFACES__TRIANGLES_AND_QUADRANGLES, E_SHAPE_OF_FINITE_ELEMENTS_FOR_SURFACES__QUADRANGLES_ONLY, \
         E_SHAPE_OF_FINITE_ELEMENTS_FOR_SURFACES__TRIANGLES_ONLY = range(3)
@@ -1660,20 +1497,14 @@
 
 class DirectionType(Enum):
     '''
     Timber Member Local Section Reduction Direction Type
     '''
     E_DIRECTION_DEPTH_NEGATIVE, E_DIRECTION_DEPTH_POSITIVE, E_DIRECTION_WIDTH_NEGATIVE, E_DIRECTION_WIDTH_POSITIVE = range(4)
 
-class PositionOnSection(Enum):
-    '''
-    Timber Member Shear Panel Position On Section
-    '''
-    POSITION_DEFINE, POSITION_IN_CENTROID, POSITION_ON_LOWER_FLANGE, POSITION_ON_UPPER_FLANGE = range(4)
-
 class TimberServiceClassServiceClass(Enum):
     '''
     Timber Service Class Service Classs
     '''
     TIMBER_SERVICE_CLASS_TYPE_1, TIMBER_SERVICE_CLASS_TYPE_2, TIMBER_SERVICE_CLASS_TYPE_3 = range(3)
 
 class AluminumEffectiveLengthsDeterminationMcrEurope(Enum):
@@ -2269,65 +2100,28 @@
 class RotationalReleaseNonlinearity(Enum):
     '''
     Rotational Release Nonlinearity Enumeration
     '''
     NONLINEARITY_TYPE_NONE, NONLINEARITY_TYPE_FAILURE_IF_NEGATIVE, NONLINEARITY_TYPE_FAILURE_IF_POSITIVE, \
     NONLINEARITY_TYPE_DIAGRAM, NONLINEARITY_TYPE_PARTIAL_ACTIVITY, NONLINEARITY_TYPE_FORCE_MOMENT_DIAGRAM = range(6)
 
-class LineReleaseLocalAxisSystem(Enum):
-    '''
-    Line Release Local Axis System Enumeration
-    '''
-    LOCAL_AXIS_SYSTEM_TYPE_ORIGINAL_LINE, LOCAL_AXIS_SYSTEM_TYPE_MEMBER_ON_ORIGINAL_LINE, \
-    LOCAL_AXIS_SYSTEM_TYPE_Z_AXIS_PERPENDICULAR_TO_SURFACE, E_LOCAL_AXIS_SYSTEM_TYPE_HELP_NODE= range(4)
-
-class LocalAxisSystemObjectInPlane(Enum):
-    '''
-    Line Release Local Axis System Object In Plane Enumeration
-    '''
-    LOCAL_AXIS_SYSTEM_IN_PLANE_XY, LOCAL_AXIS_SYSTEM_IN_PLANE_XZ = range(2)
-
 class PartialActivityAlongType(Enum):
     '''
     Partial Activity Along Type Enumeration
     '''
     PARTIAL_ACTIVITY_TYPE_COMPLETE, PARTIAL_ACTIVITY_TYPE_FIXED, PARTIAL_ACTIVITY_TYPE_FAILURE_FROM_FORCE, \
     PARTIAL_ACTIVITY_TYPE_YIELDING_FROM_FORCE, PARTIAL_ACTIVITY_TYPE_INEFFECTIVNESS = range(5)
 
 class PartialActivityAroundType(Enum):
     '''
     Partial Activity Around Type Enumeration
     '''
     PARTIAL_ACTIVITY_TYPE_COMPLETE, PARTIAL_ACTIVITY_TYPE_FIXED, PARTIAL_ACTIVITY_TYPE_FAILURE_FROM_MOMENT, \
     PARTIAL_ACTIVITY_TYPE_YIELDING_FROM_MOMENT, PARTIAL_ACTIVITY_TYPE_INEFFECTIVNESS = range(5)
 
-class LineReleaseDiagram(Enum):
-    '''
-    Line Release Diagram Type Enumeration
-    '''
-    DIAGRAM_ENDING_TYPE_CONTINUOUS, DIAGRAM_ENDING_TYPE_FAILURE, DIAGRAM_ENDING_TYPE_STOP, DIAGRAM_ENDING_TYPE_YIELDING = range(4)
-
-class LineReleaseForceMomentDiagram(Enum):
-    '''
-    Line Release Force Moment Diagram Enumeration
-    '''
-    FORCE_MOMENT_DIAGRAM_ENDING_TYPE_CONTINUOUS, FORCE_MOMENT_DIAGRAM_ENDING_TYPE_FAILURE, FORCE_MOMENT_DIAGRAM_ENDING_TYPE_YIELDING = range(3)
-
-class LineReleaseForceMomentDepend(Enum):
-    '''
-    Line Release Force Moment Depend Enumeration
-    '''
-    FORCE_MOMENT_DIAGRAM_DEPENDS_ON_N, FORCE_MOMENT_DIAGRAM_DEPENDS_ON_VY, FORCE_MOMENT_DIAGRAM_DEPENDS_ON_VZ = range(3)
-
-class LineReleaseReleaseLocation(Enum):
-    '''
-    Line Release Release Location Enumeration
-    '''
-    RELEASE_LOCATION_ORIGIN, RELEASE_LOCATION_RELEASED = range(2)
-
 class LoadWizardType(Enum):
     ''''
     Types of Loading Wizards
     '''
     GENERATE_LOAD_COMBINATIONS, GENERATE_RESULT_COMBINATIONS = range(2)
 
 class InitialStateDefintionType(Enum):
@@ -2465,7 +2259,65 @@
     REFERENCE_TYPE_L, REFERENCE_TYPE_XY, REFERENCE_TYPE_XZ, REFERENCE_TYPE_YZ = range(4)
 
 class NoteSurfaceReferenceType(Enum):
     '''
     Note Surface Reference Type Enumeration
     '''
     OFFSET_TYPE_XY, OFFSET_TYPE_XZ, OFFSET_TYPE_YZ = range(3)
+
+class OperatorType(Enum):
+    '''
+    Operator Type
+    '''
+    OPERATOR_AND, OPERATOR_NONE, OPERATOR_OR = range(3)
+
+class ResultCombinationType(Enum):
+    '''
+    Result Combination Combination Type
+    '''
+    COMBINATION_TYPE_ENVELOPE_PERMANENT, COMBINATION_TYPE_ENVELOPE_TRANSIENT, COMBINATION_TYPE_GENERAL, COMBINATION_TYPE_SUPERPOSITION = range(4)
+
+class ActionLoadType(Enum):
+    '''
+    Action Load Type
+    '''
+    LOAD_TYPE_PERMANENT, LOAD_TYPE_TRANSIENT = range(2)
+
+class ResultCombinationExtremeValueSign(Enum):
+    '''
+    Result Combination SRSS Extreme Value Sign
+    '''
+    EXTREME_VALUE_SIGN_ACCORDING_TO_LC_CO, EXTREME_VALUE_SIGN_NEGATIVE, EXTREME_VALUE_SIGN_POSITIVE, EXTREME_VALUE_SIGN_POSITIVE_OR_NEGATIVE = range(4)
+
+class CaseObjectSubResultType(Enum):
+    '''
+    Case Object Sub Result Type
+    '''
+    SUB_RESULT_INCREMENTAL_ALL, SUB_RESULT_INCREMENTAL_FINAL_STATE, SUB_RESULT_INCREMENTAL_SUB_RESULT_ID, SUB_RESULT_SPECTRAL_ANALYSIS_ABSOLUTE_SUM, SUB_RESULT_SPECTRAL_ANALYSIS_DIRECTION_X, \
+    SUB_RESULT_SPECTRAL_ANALYSIS_DIRECTION_X_WITH_MODE_SHAPE, SUB_RESULT_SPECTRAL_ANALYSIS_DIRECTION_Y, SUB_RESULT_SPECTRAL_ANALYSIS_DIRECTION_Y_WITH_MODE_SHAPE, SUB_RESULT_SPECTRAL_ANALYSIS_DIRECTION_Z, \
+    SUB_RESULT_SPECTRAL_ANALYSIS_DIRECTION_Z_WITH_MODE_SHAPE, SUB_RESULT_SPECTRAL_ANALYSIS_SCALED_SUMS_ENVELOPE, SUB_RESULT_SPECTRAL_ANALYSIS_SCALED_SUM_FULL_X, SUB_RESULT_SPECTRAL_ANALYSIS_SCALED_SUM_FULL_Y, \
+    SUB_RESULT_SPECTRAL_ANALYSIS_SCALED_SUM_FULL_Z, SUB_RESULT_SPECTRAL_ANALYSIS_SRSS = range(15)
+
+class TimberMoistureClassType(Enum):
+    '''
+    Timber Moisture Class
+    '''
+    TIMBER_MOISTURE_CLASS_TYPE_1, TIMBER_MOISTURE_CLASS_TYPE_2, TIMBER_MOISTURE_CLASS_TYPE_3 = range(3)
+
+class TimberServiceConditionsMoistureType(Enum):
+    '''
+    Timber Service Conditions Moisture Service Condition
+    '''
+    TIMBER_MOISTURE_SERVICE_CONDITION_TYPE_DRY, TIMBER_MOISTURE_SERVICE_CONDITION_TYPE_MOIST, TIMBER_MOISTURE_SERVICE_CONDITION_TYPE_VERY_DRY, TIMBER_MOISTURE_SERVICE_CONDITION_TYPE_WET = range(4)
+
+class TimberServiceConditionsTemperatureType(Enum):
+    '''
+    Timber Service Conditions Temperature
+    '''
+    TEMPERATURE_TYPE_EQUAL_TO_50, TEMPERATURE_TYPE_LESS_OR_EQUAL_100, TEMPERATURE_TYPE_LESS_OR_EQUAL_35, TEMPERATURE_TYPE_RANGE_100_125, TEMPERATURE_TYPE_RANGE_125_150, TEMPERATURE_TYPE_RANGE_35_50, \
+    TEMPERATURE_TYPE_TEMPERATURE_ZONE_1, TEMPERATURE_TYPE_TEMPERATURE_ZONE_2, TEMPERATURE_TYPE_TEMPERATURE_ZONE_3 = range(9)
+
+class TimberServiceConditionsTreatmentType(Enum):
+    '''
+    Timber Service Conditions Treatment
+    '''
+    TREATMENT_TYPE_FIRE_RETARDANT, TREATMENT_TYPE_NONE, TREATMENT_TYPE_PRESERVATIVE = range(3)
```

### Comparing `RSTAB-1.6.0/RSTAB/formula.py` & `RSTAB-1.7.0/RSTAB/formula.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/globalParameter.py` & `RSTAB-1.7.0/RSTAB/globalParameter.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB/initModel.py` & `RSTAB-1.7.0/RSTAB/initModel.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import socket
 import requests
 from suds.client import Client
 from RSTAB.enums import ObjectTypes, ModelType, AddOn
 from RSTAB.suds_requests import RequestsTransport
 from suds.cache import DocumentCache
 from tempfile import gettempdir
+import time
 
 # Connect to server
 # Check server port range set in "Program Options & Settings"
 # By default range is set between 8081 ... 8089
 print('Connecting to server...')
 
 # local machine url format: 'http://127.0.0.1'
@@ -31,17 +32,26 @@
 else:
     print('Error: Port '+urlAndPort+' is not open.')
     print('Please check:')
     print('- If you have started RSTAB application at the remote destination correctly.')
     a_socket.close()
     sys.exit()
 
+# Delete cached WSDL older than 1 day to reflect newer version of RFEM
+cacheLoc = os.path.join(gettempdir(), 'WSDL')
+currentTime = time.time()
+if os.path.exists(cacheLoc):
+    for file in os.listdir(cacheLoc):
+        filePath = os.path.join(cacheLoc, file)
+        if (currentTime - os.path.getmtime(filePath)) > 86400:
+            os.remove(filePath)
+
 # Check for issues locally and remotely
 try:
-    ca = DocumentCache(location=os.path.join(gettempdir(), 'WSDL'))
+    ca = DocumentCache(location=cacheLoc)
     client = Client(urlAndPort+'/wsdl', location = urlAndPort, cache=ca)
 except:
     print('Error: Connection to server failed!')
     print('Please check:')
     print('- If you have started RSTAB application')
     print('- If all RSTAB dialogs are closed')
     print('- If server port range is set correctly')
@@ -104,59 +114,56 @@
                 cModel.service.delete_all()
 
             # Requested new model, model with given name DOESN'T exist yet
             else:
                 modelPath = ''
                 # Requested new model, model with given name was NOT connected yet but file with the same name was opened
                 if model_name in modelLst:
-                    id = modelLst.index(model_name)
+                    id = 0
+                    for i,j in enumerate(modelLst):
+                        if modelLst[i] == model_name:
+                            id = i
                     modelPath =  client.service.get_model(id)
                 else:
                     modelPath =  client.service.new_model(original_model_name)
                 modelPort = modelPath[-5:-1]
                 modelUrlPort = url+':'+modelPort
                 modelCompletePath = modelUrlPort+'/wsdl'
 
-                if self.clientModelDct:
-                    cModel = Client(modelCompletePath, location = modelUrlPort, cache=ca)
-                else:
-                    session = requests.Session()
-                    adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
-                    session.mount('http://', adapter)
-                    trans = RequestsTransport(session)
+                session = requests.Session()
+                adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
+                session.mount('http://', adapter)
+                trans = RequestsTransport(session)
 
-                    cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort, cache=ca)
+                cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort, cache=ca)
 
                 self.clientModelDct[model_name] = cModel
 
         else:
             # Requested model which was already connected
-            assert model_name in self.clientModelDct or model_name in modelLst, 'WARNING: '+model_name +'is not connected neither opened in RSTAB.'
+            assert model_name in self.clientModelDct or model_name in modelLst, 'WARNING: '+model_name +' is not connected neither opened in RFEM.'
 
             if model_name in self.clientModelDct:
                 cModel = self.clientModelDct[model_name]
             elif model_name in modelLst:
                 id = 0
                 for i,j in enumerate(modelLst):
                     if modelLst[i] == model_name:
                         id = i
                 modelPath =  client.service.get_model(id)
                 modelPort = modelPath[-5:-1]
                 modelUrlPort = url+':'+modelPort
                 modelCompletePath = modelUrlPort+'/wsdl'
 
-                if self.clientModelDct:
-                    cModel = Client(modelCompletePath, location = modelUrlPort, cache=ca)
-                else:
-                    session = requests.Session()
-                    adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
-                    session.mount('http://', adapter)
-                    trans = RequestsTransport(session)
+                session = requests.Session()
+                adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
+                session.mount('http://', adapter)
+                trans = RequestsTransport(session)
 
-                    cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort, cache=ca)
+                cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort, cache=ca)
 
                 self.clientModelDct[model_name] = cModel
             else:
                 print('Model name "'+model_name+'" is not created in RSTAB. Consider changing new_model parameter in Model class from False to True.')
                 sys.exit()
 
             if delete:
@@ -199,38 +206,57 @@
                 else:
                     self.clientModel = None
 
 def clearAttributes(obj):
     '''
     Clears object attributes.
     Sets all attributes to None.
+    Use it whenever you create new (sub)object.
 
     Args:
         obj: object to clear
     '''
 
     # iterator
     it = iter(obj)
     for i in it:
         obj[i[0]] = None
+
     return obj
 
 def deleteEmptyAttributes(obj):
     '''
     Delete all attributes that are None for better performance.
 
     Args:
         obj: object to clear
     '''
+    it = [] # iterator
+    try:
+        it = iter(obj)
+    except:
+        ValueError('WARNING: Object feeded to deleteEmptyAttributes function is not iterable. It is type: '+str(type(obj)+'.'))
 
-    # iterator
-    it = iter(obj)
     for i in it:
-        if obj[i[0]] is None:
+        if isinstance(i, str) or isinstance(i, int) or isinstance(i, float) or isinstance(i, bool):
+            continue
+        if len(i) > 2:
+            i = deleteEmptyAttributes(i)
+        elif i[1] is None or i[1] == "":
             delattr(obj, i[0])
+        elif isinstance(i[1], str) or isinstance(i[1], int) or isinstance(i[1], float) or isinstance(i[1], bool):
+            pass
+        else:
+            if isinstance(i, tuple):
+                i = list(i)
+                i[1] = deleteEmptyAttributes(i[1])
+                i = tuple(i)
+            else:
+                i[1] = deleteEmptyAttributes(i[1])
+
     return obj
 
 def openFile(model_path):
     '''
     Open file with a name.
     This routine primarily adds client instance into
     Model.clientModelLst which manages all connections to the models.
@@ -262,31 +288,30 @@
         Model.__delete__(Model, index_or_name)
         client.service.close_model(index_or_name, save_changes)
 
     elif isinstance(index_or_name, str):
         if '.rs9' in index_or_name:
             index_or_name = index_or_name[:-4]
 
-        modelLs = client.service.get_model_list()
+        modelLs = client.service.get_model_list().name
         Model.__delete__(Model, index_or_name)
-        client.service.close_model(modelLs.name.index(index_or_name), save_changes)
+        client.service.close_model(modelLs.index(index_or_name), save_changes)
     else:
         assert False, 'Parameter index_or_name must be int or string.'
 
 def closeAllModels(save_changes = False):
     '''
     Function that closes all opened models in reverse order.
 
     Args:
         save_changes (bool): Enable/Disable Save Changes Option
     '''
-    modelLs = client.service.get_model_list()
-    if modelLs:
-        for j in reversed(modelLs.name):
-            closeModel(j, save_changes)
+    modelLs = client.service.get_model_list().name
+    for j in reversed(modelLs):
+        closeModel(j, save_changes)
 
 def saveFile(model_path):
     '''
     This function saves a model in a .rs9 file.
 
     Args:
         index_or_name : Model Index or Name to be Close
@@ -574,15 +599,14 @@
             ModelType.E_MODEL_TYPE_3D
         model (RSTAB Class, optional): Model to be edited
     '''
 
     model.clientModel.service.set_model_type(model_type.name)
 
 def GetModelType(model = Model):
-
     '''
     The method returns a string of the current model type.
 
     Args:
         model (RSTAB Class): Model Instance
     '''
```

### Comparing `RSTAB-1.6.0/RSTAB/suds_requests.py` & `RSTAB-1.7.0/RSTAB/suds_requests.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/RSTAB.egg-info/PKG-INFO` & `RSTAB-1.7.0/RSTAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RSTAB
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python Framework for RSTAB9 Web Services
 Home-page: https://github.com/Dlubal-Software/RSTAB_Python_Client
 Author: Dlubal Software
 Author-email: info@dlubal.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RSTAB Version: 1.6.0 Summary: Python Framework for
+Metadata-Version: 2.1 Name: RSTAB Version: 1.7.0 Summary: Python Framework for
 RSTAB9 Web Services Home-page: https://github.com/Dlubal-Software/
 RSTAB_Python_Client Author: Dlubal Software Author-email: info@dlubal.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
 ****** [Dlubal_Software] Dlubal Software GmbH [![image](https://img.shields.io/
 twitter/follow/dlubal_en?style=social)](https://twitter.com/dlubal_en "Twitter
```

### Comparing `RSTAB-1.6.0/RSTAB.egg-info/SOURCES.txt` & `RSTAB-1.7.0/RSTAB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RSTAB-1.6.0/setup.py` & `RSTAB-1.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent
 readme = (here/"README.md").read_text(encoding="utf-8")
 
 setup(
     name='RSTAB',
-    version='1.06.0',
+    version='1.07.0',
     description='Python Framework for RSTAB9 Web Services',
     long_description=readme,
     long_description_content_type = "text/markdown",
     url="https://github.com/Dlubal-Software/RSTAB_Python_Client",
     author="Dlubal Software",
     author_email="info@dlubal.com",
     license="MIT",
```

