# Comparing `tmp/RFEM-1.7.0.tar.gz` & `tmp/RFEM-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RFEM-1.7.0.tar", last modified: Wed Apr 27 05:53:52 2022, max compression
+gzip compressed data, was "RFEM-1.8.0.tar", last modified: Wed May 18 08:53:58 2022, max compression
```

## Comparing `RFEM-1.7.0.tar` & `RFEM-1.8.0.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.829242 RFEM-1.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.821242 RFEM-1.7.0/Examples/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/Examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12491 2022-04-27 05:53:42.000000 RFEM-1.7.0/Examples/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     6440 2022-04-27 05:53:42.000000 RFEM-1.7.0/Examples/window.py
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2022-04-27 05:53:42.000000 RFEM-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5563 2022-04-27 05:53:52.829242 RFEM-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5102 2022-04-27 05:53:42.000000 RFEM-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.821242 RFEM-1.7.0/RFEM/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.825242 RFEM-1.7.0/RFEM/BasicObjects/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7317 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/bracing.py
--rw-r--r--   0 runner    (1001) docker     (116)     4482 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/frame.py
--rw-r--r--   0 runner    (1001) docker     (116)    16241 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/line.py
--rw-r--r--   0 runner    (1001) docker     (116)     4053 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/lineSet.py
--rw-r--r--   0 runner    (1001) docker     (116)     1207 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/material.py
--rw-r--r--   0 runner    (1001) docker     (116)   106668 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/member.py
--rw-r--r--   0 runner    (1001) docker     (116)     4271 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/memberSet.py
--rw-r--r--   0 runner    (1001) docker     (116)    15685 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/node.py
--rw-r--r--   0 runner    (1001) docker     (116)     1245 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/opening.py
--rw-r--r--   0 runner    (1001) docker     (116)     1374 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/section.py
--rw-r--r--   0 runner    (1001) docker     (116)     7278 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/solid.py
--rw-r--r--   0 runner    (1001) docker     (116)     4065 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/solidSet.py
--rw-r--r--   0 runner    (1001) docker     (116)    18361 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/surface.py
--rw-r--r--   0 runner    (1001) docker     (116)     4242 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/surfaceSet.py
--rw-r--r--   0 runner    (1001) docker     (116)    30640 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/BasicObjects/thickness.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.825242 RFEM-1.7.0/RFEM/ConcreteDesign/
--rw-r--r--   0 runner    (1001) docker     (116)     2230 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/ConcreteDesign/ConcreteServiceabilityConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (116)     2224 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/ConcreteDesign/ConcreteUltimateConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/ConcreteDesign/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.825242 RFEM-1.7.0/RFEM/Imperfections/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Imperfections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1249 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Imperfections/imperfectionCase.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.825242 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1753 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/designSituation.py
--rw-r--r--   0 runner    (1001) docker     (116)     5948 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/loadCase.py
--rw-r--r--   0 runner    (1001) docker     (116)     3319 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/loadCombination.py
--rw-r--r--   0 runner    (1001) docker     (116)     3458 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/modalAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1103 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/resultCombination.py
--rw-r--r--   0 runner    (1001) docker     (116)     3980 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/spectralAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (116)    21948 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/stabilityAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (116)    19300 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/LoadCasesAndCombinations/staticAnalysisSettings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.825242 RFEM-1.7.0/RFEM/Loads/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    38715 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/freeLoad.py
--rw-r--r--   0 runner    (1001) docker     (116)     1687 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/imposedLineDeformation.py
--rw-r--r--   0 runner    (1001) docker     (116)     1822 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/imposedNodalDeformation.py
--rw-r--r--   0 runner    (1001) docker     (116)    32286 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/lineLoad.py
--rw-r--r--   0 runner    (1001) docker     (116)    29774 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/linesetLoad.py
--rw-r--r--   0 runner    (1001) docker     (116)    98614 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/memberLoad.py
--rw-r--r--   0 runner    (1001) docker     (116)   111135 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/membersetload.py
--rw-r--r--   0 runner    (1001) docker     (116)    22296 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/nodalLoad.py
--rw-r--r--   0 runner    (1001) docker     (116)    10481 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/solidLoad.py
--rw-r--r--   0 runner    (1001) docker     (116)    10626 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/solidSetLoad.py
--rw-r--r--   0 runner    (1001) docker     (116)    25944 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/surfaceLoad.py
--rw-r--r--   0 runner    (1001) docker     (116)    26043 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/Loads/surfacesetload.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.825242 RFEM-1.7.0/RFEM/SpecialObjects/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/SpecialObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      869 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/SpecialObjects/enlargedColumnHead.py
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/SpecialObjects/intersection.py
--rw-r--r--   0 runner    (1001) docker     (116)      834 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/SpecialObjects/resultSection.py
--rw-r--r--   0 runner    (1001) docker     (116)     4667 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/SpecialObjects/rigidLink.py
--rw-r--r--   0 runner    (1001) docker     (116)      882 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/SpecialObjects/structureModification.py
--rw-r--r--   0 runner    (1001) docker     (116)      845 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/SpecialObjects/surfaceContact.py
--rw-r--r--   0 runner    (1001) docker     (116)      901 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/SpecialObjects/surfaceResultAdjustment.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.825242 RFEM-1.7.0/RFEM/TypesForLines/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForLines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForLines/lineHinge.py
--rw-r--r--   0 runner    (1001) docker     (116)     5571 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForLines/lineMeshRefinements.py
--rw-r--r--   0 runner    (1001) docker     (116)     3435 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForLines/lineSupport.py
--rw-r--r--   0 runner    (1001) docker     (116)     2420 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForLines/lineWeldedJoint.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.829242 RFEM-1.7.0/RFEM/TypesForMembers/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForMembers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4008 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForMembers/memberDefinableStiffness.py
--rw-r--r--   0 runner    (1001) docker     (116)      864 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForMembers/memberEccentricity.py
--rw-r--r--   0 runner    (1001) docker     (116)     2013 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForMembers/memberHinge.py
--rw-r--r--   0 runner    (1001) docker     (116)      864 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForMembers/memberNonlinearity.py
--rw-r--r--   0 runner    (1001) docker     (116)      940 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForMembers/memberResultIntermediatePoints.py
--rw-r--r--   0 runner    (1001) docker     (116)      924 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForMembers/memberStiffnessModification.py
--rw-r--r--   0 runner    (1001) docker     (116)      834 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForMembers/memberSupport.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.829242 RFEM-1.7.0/RFEM/TypesForNodes/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForNodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7239 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForNodes/nodalMeshRefinement.py
--rw-r--r--   0 runner    (1001) docker     (116)     4306 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForNodes/nodalSupport.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.829242 RFEM-1.7.0/RFEM/TypesForSolids/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSolids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3453 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSolids/solidContact.py
--rw-r--r--   0 runner    (1001) docker     (116)     1637 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSolids/solidGas.py
--rw-r--r--   0 runner    (1001) docker     (116)     1539 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSolids/solidMeshRefinement.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.829242 RFEM-1.7.0/RFEM/TypesForSpecialObjects/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSpecialObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      871 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSpecialObjects/surfaceContactType.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.829242 RFEM-1.7.0/RFEM/TypesForSurfaces/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSurfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3236 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSurfaces/surfaceEccentricity.py
--rw-r--r--   0 runner    (1001) docker     (116)     1578 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSurfaces/surfaceMeshRefinements.py
--rw-r--r--   0 runner    (1001) docker     (116)     4922 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSurfaces/surfaceStiffnessModification.py
--rw-r--r--   0 runner    (1001) docker     (116)     2201 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesForSurfaces/surfaceSupport.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.829242 RFEM-1.7.0/RFEM/TypesforConcreteDesign/
--rw-r--r--   0 runner    (1001) docker     (116)     8659 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesforConcreteDesign/ConcreteDurability.py
--rw-r--r--   0 runner    (1001) docker     (116)     6073 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesforConcreteDesign/ConcreteEffectiveLength.py
--rw-r--r--   0 runner    (1001) docker     (116)     2296 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesforConcreteDesign/ConcreteReinforcementDirections.py
--rw-r--r--   0 runner    (1001) docker     (116)    10708 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesforConcreteDesign/ConcreteSurfaceReinforcements.py
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/TypesforConcreteDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2546 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/baseSettings.py
--rw-r--r--   0 runner    (1001) docker     (116)       42 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/dataTypes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1330 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (116)    99974 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/enums.py
--rw-r--r--   0 runner    (1001) docker     (116)     3674 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/globalParameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    14656 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/initModel.py
--rw-r--r--   0 runner    (1001) docker     (116)     2633 2022-04-27 05:53:42.000000 RFEM-1.7.0/RFEM/suds_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-27 05:53:52.821242 RFEM-1.7.0/RFEM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5563 2022-04-27 05:53:52.000000 RFEM-1.7.0/RFEM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3564 2022-04-27 05:53:52.000000 RFEM-1.7.0/RFEM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:52.000000 RFEM-1.7.0/RFEM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-27 05:53:52.000000 RFEM-1.7.0/RFEM.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       55 2022-04-27 05:53:52.000000 RFEM-1.7.0/RFEM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-04-27 05:53:52.000000 RFEM-1.7.0/RFEM.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-04-27 05:53:52.829242 RFEM-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      882 2022-04-27 05:53:42.000000 RFEM-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.464519 RFEM-1.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.452518 RFEM-1.8.0/Examples/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/Examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12342 2022-05-18 08:53:48.000000 RFEM-1.8.0/Examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6440 2022-05-18 08:53:48.000000 RFEM-1.8.0/Examples/window.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1072 2022-05-18 08:53:48.000000 RFEM-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     5563 2022-05-18 08:53:58.464519 RFEM-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5102 2022-05-18 08:53:48.000000 RFEM-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.452518 RFEM-1.8.0/RFEM/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.456518 RFEM-1.8.0/RFEM/BasicObjects/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7317 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/bracing.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4482 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/frame.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16241 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/line.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4053 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/lineSet.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1207 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/material.py
+-rw-r--r--   0 runner    (1001) docker     (116)   106668 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/member.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4271 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/memberSet.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15685 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/node.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1245 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/opening.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1374 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/section.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7278 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/solid.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4065 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/solidSet.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18361 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/surface.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4242 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/surfaceSet.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30303 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/BasicObjects/thickness.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.456518 RFEM-1.8.0/RFEM/ConcreteDesign/
+-rw-r--r--   0 runner    (1001) docker     (116)     2230 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/ConcreteDesign/ConcreteServiceabilityConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2224 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/ConcreteDesign/ConcreteUltimateConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/ConcreteDesign/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.456518 RFEM-1.8.0/RFEM/Imperfections/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Imperfections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1249 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Imperfections/imperfectionCase.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.456518 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1753 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/designSituation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5948 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/loadCase.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3419 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/loadCombination.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3458 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/modalAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1103 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/resultCombination.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3980 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/spectralAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21948 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/stabilityAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19300 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/LoadCasesAndCombinations/staticAnalysisSettings.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.460518 RFEM-1.8.0/RFEM/Loads/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    38823 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/freeLoad.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1687 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/imposedLineDeformation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1822 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/imposedNodalDeformation.py
+-rw-r--r--   0 runner    (1001) docker     (116)    32366 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/lineLoad.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29854 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/linesetLoad.py
+-rw-r--r--   0 runner    (1001) docker     (116)    99082 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/memberLoad.py
+-rw-r--r--   0 runner    (1001) docker     (116)   111603 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/membersetload.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22296 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/nodalLoad.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10481 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/solidLoad.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10626 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/solidSetLoad.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25964 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/surfaceLoad.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26063 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/Loads/surfacesetload.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.460518 RFEM-1.8.0/RFEM/SpecialObjects/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/SpecialObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      869 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/SpecialObjects/enlargedColumnHead.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/SpecialObjects/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (116)      834 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/SpecialObjects/resultSection.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4667 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/SpecialObjects/rigidLink.py
+-rw-r--r--   0 runner    (1001) docker     (116)      882 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/SpecialObjects/structureModification.py
+-rw-r--r--   0 runner    (1001) docker     (116)      845 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/SpecialObjects/surfaceContact.py
+-rw-r--r--   0 runner    (1001) docker     (116)      901 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/SpecialObjects/surfaceResultAdjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.460518 RFEM-1.8.0/RFEM/TypesForLines/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForLines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1968 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForLines/lineHinge.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5571 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForLines/lineMeshRefinements.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3435 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForLines/lineSupport.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2436 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForLines/lineWeldedJoint.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.460518 RFEM-1.8.0/RFEM/TypesForMembers/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForMembers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4008 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForMembers/memberDefinableStiffness.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6215 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForMembers/memberEccentricity.py
+-rw-r--r--   0 runner    (1001) docker     (116)    32883 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForMembers/memberHinge.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2475 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForMembers/memberNonlinearity.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2289 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForMembers/memberResultIntermediatePoints.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6188 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForMembers/memberStiffnessModification.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2627 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForMembers/memberSupport.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4037 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForMembers/memberTransverseStiffeners.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.460518 RFEM-1.8.0/RFEM/TypesForNodes/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForNodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7239 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForNodes/nodalMeshRefinement.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4306 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForNodes/nodalSupport.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.460518 RFEM-1.8.0/RFEM/TypesForSolids/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSolids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3453 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSolids/solidContact.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1637 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSolids/solidGas.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1539 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSolids/solidMeshRefinement.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.460518 RFEM-1.8.0/RFEM/TypesForSpecialObjects/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSpecialObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      871 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSpecialObjects/surfaceContactType.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.460518 RFEM-1.8.0/RFEM/TypesForSurfaces/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSurfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3236 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSurfaces/surfaceEccentricity.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1578 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSurfaces/surfaceMeshRefinements.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4922 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSurfaces/surfaceStiffnessModification.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2201 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesForSurfaces/surfaceSupport.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.464519 RFEM-1.8.0/RFEM/TypesforConcreteDesign/
+-rw-r--r--   0 runner    (1001) docker     (116)     8659 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesforConcreteDesign/ConcreteDurability.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6073 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesforConcreteDesign/ConcreteEffectiveLength.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2296 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesforConcreteDesign/ConcreteReinforcementDirections.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10708 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesforConcreteDesign/ConcreteSurfaceReinforcements.py
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/TypesforConcreteDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2546 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/baseSettings.py
+-rw-r--r--   0 runner    (1001) docker     (116)       42 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/dataTypes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1330 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (116)   104815 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/enums.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3674 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/globalParameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14661 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/initModel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2633 2022-05-18 08:53:48.000000 RFEM-1.8.0/RFEM/suds_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-18 08:53:58.456518 RFEM-1.8.0/RFEM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5563 2022-05-18 08:53:58.000000 RFEM-1.8.0/RFEM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3615 2022-05-18 08:53:58.000000 RFEM-1.8.0/RFEM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:58.000000 RFEM-1.8.0/RFEM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-18 08:53:58.000000 RFEM-1.8.0/RFEM.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       55 2022-05-18 08:53:58.000000 RFEM-1.8.0/RFEM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2022-05-18 08:53:58.000000 RFEM-1.8.0/RFEM.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-05-18 08:53:58.464519 RFEM-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      882 2022-05-18 08:53:48.000000 RFEM-1.8.0/setup.py
```

### Comparing `RFEM-1.7.0/Examples/main.py` & `RFEM-1.8.0/Examples/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,16 @@
     Line(5, insertSpaces([k+5, k+6, k+10, k+9, k+5]))
     Line(6, insertSpaces([k+6, k+7, k+11, k+10, k+6]))
     Line(7, insertSpaces([k+7, k+8, k+12, k+11, k+7]))
     Line(8, insertSpaces([k+8, k+5, k+9, k+12, k+8]))
 
 # -------------------------------------------------------------
     # Member Hinges
-    MemberHinge(1, "Local", inf, inf, inf,  inf, 0, inf, "Rotational Release My")
+    MemberHinge(1, "Local", rotational_release_mz=inf)
+
 
 # -------------------------------------------------------------
     # Members
 
     member = Member()
     # Frames
     i = 1
@@ -196,20 +197,14 @@
     NodalSupport(2, solid_support, NodalSupportType.HINGED, "Hinged support")
 
 # -------------------------------------------------------------
     # Solids
     Solid(1, "2 3 4 5 6 7", 2)
 
 # -------------------------------------------------------------
-    # Sets
-    LineSet()
-    MemberSet()
-    SurfaceSet()
-
-# -------------------------------------------------------------
     print('Load Cases/Loads...')
 
 # -------------------------------------------------------------
     # Static Analysis Settings
     StaticAnalysisSettings(1, "Linear calculation", StaticAnalysisType.GEOMETRICALLY_LINEAR)
 
 # -------------------------------------------------------------
```

### Comparing `RFEM-1.7.0/Examples/window.py` & `RFEM-1.8.0/Examples/window.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/LICENSE` & `RFEM-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/PKG-INFO` & `RFEM-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFEM
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python Framework for RFEM6 Web Services
 Home-page: https://github.com/Dlubal-Software/RFEM_Python_Client
 Author: Dlubal Software
 Author-email: info@dlubal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RFEM-1.7.0/README.md` & `RFEM-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/bracing.py` & `RFEM-1.8.0/RFEM/BasicObjects/bracing.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/frame.py` & `RFEM-1.8.0/RFEM/BasicObjects/frame.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/line.py` & `RFEM-1.8.0/RFEM/BasicObjects/line.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/lineSet.py` & `RFEM-1.8.0/RFEM/BasicObjects/lineSet.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/material.py` & `RFEM-1.8.0/RFEM/BasicObjects/material.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/member.py` & `RFEM-1.8.0/RFEM/BasicObjects/member.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/memberSet.py` & `RFEM-1.8.0/RFEM/BasicObjects/memberSet.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/node.py` & `RFEM-1.8.0/RFEM/BasicObjects/node.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/opening.py` & `RFEM-1.8.0/RFEM/BasicObjects/opening.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/section.py` & `RFEM-1.8.0/RFEM/BasicObjects/section.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/solid.py` & `RFEM-1.8.0/RFEM/BasicObjects/solid.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/solidSet.py` & `RFEM-1.8.0/RFEM/BasicObjects/solidSet.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/surface.py` & `RFEM-1.8.0/RFEM/BasicObjects/surface.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/surfaceSet.py` & `RFEM-1.8.0/RFEM/BasicObjects/surfaceSet.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/BasicObjects/thickness.py` & `RFEM-1.8.0/RFEM/BasicObjects/thickness.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,28 +368,27 @@
         # Add Thickness to client model
         model.clientModel.service.set_thickness(clientObject)
 
     @staticmethod
     def Layers(
                  no: int = 1,
                  name: str = None,
-                 layers = [[0, 1, 0.2, 0.0, '']],
+                 layers = [[0, 1, 0.2]],
                  comment: str = '',
                  params: dict = None,
                  model = Model):
 
         '''
         NOTE: Available only for Special Solution Add-on Multilayer Surfaces.
 
         Args:
             no (int): Thickness Tag
             name (str): Thickness Name
             material_no (int): Tag of Material assigned to Thickness
             properties (list): Nested List of Layer Properties
-                properties: [[thickness_type, material, thickness, rotation, comment], ...]
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
         '''
 
         # Check if Multilayer Surfaces Add-on is ON.
         if not GetAddonStatus(model.clientModel, AddOn.multilayer_surfaces_design_active):
             SetAddonStatus(model.clientModel, AddOn.multilayer_surfaces_design_active, True)
@@ -411,26 +410,20 @@
         # Thickness Type
         clientObject.type = ThicknessType.TYPE_LAYERS.name
 
         # Layers
         clientObject.layers_reference_table = model.clientModel.factory.create('ns0:thickness.layers_reference_table')
 
         for i,j in enumerate(layers):
-            tlrt = model.clientModel.factory.create('ns0:thickness_layers_reference_table')
-            tlrt.no = no
-            tlrt.layer_no = i+1
-            tlrt.layer_type = None
-            tlrt.thickness_type = layers[i][0]
-            tlrt.material = layers[i][1]
-            tlrt.thickness = layers[i][2]
-            tlrt.angle = layers[i][3] * (pi/180)
-            tlrt.connection_with_other_topological_elements = False
-            tlrt.comment = layers[i][4]
-            tlrt.specific_weight = 0
-            tlrt.weight = 0
+            tlrt = model.clientModel.factory.create('ns0:thickness_layers_reference_table_row')
+            tlrt.no = i+1
+            tlrt.row.layer_no = i+1
+            tlrt.row.thickness_type = layers[i][0]
+            tlrt.row.material = layers[i][1]
+            tlrt.row.thickness = layers[i][2]
 
             clientObject.layers_reference_table.thickness_layers_reference_table.append(tlrt)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
```

### Comparing `RFEM-1.7.0/RFEM/ConcreteDesign/ConcreteServiceabilityConfigurations.py` & `RFEM-1.8.0/RFEM/ConcreteDesign/ConcreteServiceabilityConfigurations.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/ConcreteDesign/ConcreteUltimateConfigurations.py` & `RFEM-1.8.0/RFEM/ConcreteDesign/ConcreteUltimateConfigurations.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/Imperfections/imperfectionCase.py` & `RFEM-1.8.0/RFEM/Imperfections/imperfectionCase.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/LoadCasesAndCombinations/designSituation.py` & `RFEM-1.8.0/RFEM/LoadCasesAndCombinations/designSituation.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/LoadCasesAndCombinations/loadCase.py` & `RFEM-1.8.0/RFEM/LoadCasesAndCombinations/loadCase.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/LoadCasesAndCombinations/loadCombination.py` & `RFEM-1.8.0/RFEM/LoadCasesAndCombinations/loadCombination.py`

 * *Files 24% similar despite different names*

```diff
@@ -60,39 +60,39 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Items
         clientObject.items = model.clientModel.factory.create('ns0:load_combination.items')
 
         for i,j in enumerate(combination_items):
-            mlvlp = model.clientModel.factory.create('ns0:load_combination_items')
+            mlvlp = model.clientModel.factory.create('ns0:load_combination_items_row')
             mlvlp.no = i+1
-            mlvlp.factor = combination_items[i][0]
-            mlvlp.load_case = combination_items[i][1]
-            mlvlp.action = combination_items[i][2]
-            mlvlp.is_leading = combination_items[i][3]
-            mlvlp.gamma=0
-            mlvlp.psi=0
-            mlvlp.xi=0
-            mlvlp.k_fi=0
-            mlvlp.c_esl=0
-            mlvlp.k_def=0
-            mlvlp.psi_0=0
-            mlvlp.psi_1=0
-            mlvlp.psi_2=0
-            mlvlp.fi=0
-            mlvlp.gamma_0=0
-            mlvlp.alfa=0
-            mlvlp.k_f=0
-            mlvlp.phi=0
-            mlvlp.rho=0
-            mlvlp.omega_0=0
-            mlvlp.gamma_l_1=0
-            mlvlp.k_creep=0
-            mlvlp.shift=0
-            mlvlp.amplitude_function_type = "CONSTANT"
+            mlvlp.row.factor = combination_items[i][0]
+            mlvlp.row.load_case = combination_items[i][1]
+            mlvlp.row.action = combination_items[i][2]
+            mlvlp.row.is_leading = combination_items[i][3]
+            mlvlp.row.gamma=0
+            mlvlp.row.psi=0
+            mlvlp.row.xi=0
+            mlvlp.row.k_fi=0
+            mlvlp.row.c_esl=0
+            mlvlp.row.k_def=0
+            mlvlp.row.psi_0=0
+            mlvlp.row.psi_1=0
+            mlvlp.row.psi_2=0
+            mlvlp.row.fi=0
+            mlvlp.row.gamma_0=0
+            mlvlp.row.alfa=0
+            mlvlp.row.k_f=0
+            mlvlp.row.phi=0
+            mlvlp.row.rho=0
+            mlvlp.row.omega_0=0
+            mlvlp.row.gamma_l_1=0
+            mlvlp.row.k_creep=0
+            mlvlp.row.shift=0
+            mlvlp.row.amplitude_function_type = "CONSTANT"
 
 
             clientObject.items.load_combination_items.append(mlvlp)
 
         # Add Load Combination to client model
         model.clientModel.service.set_load_combination(clientObject)
```

### Comparing `RFEM-1.7.0/RFEM/LoadCasesAndCombinations/modalAnalysisSettings.py` & `RFEM-1.8.0/RFEM/LoadCasesAndCombinations/modalAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/LoadCasesAndCombinations/resultCombination.py` & `RFEM-1.8.0/RFEM/LoadCasesAndCombinations/resultCombination.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/LoadCasesAndCombinations/spectralAnalysisSettings.py` & `RFEM-1.8.0/RFEM/LoadCasesAndCombinations/spectralAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/LoadCasesAndCombinations/stabilityAnalysisSettings.py` & `RFEM-1.8.0/RFEM/LoadCasesAndCombinations/stabilityAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/LoadCasesAndCombinations/staticAnalysisSettings.py` & `RFEM-1.8.0/RFEM/LoadCasesAndCombinations/staticAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/Loads/freeLoad.py` & `RFEM-1.8.0/RFEM/Loads/freeLoad.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,18 +274,18 @@
                 clientObject.load_location_first_y = load_location_parameter[1]
                 clientObject.load_location_second_x = load_location_parameter[2]
                 clientObject.load_location_second_y = load_location_parameter[3]
 
                 clientObject.load_varying_in_z_parameters = model.clientModel.factory.create('ns0:free_rectangular_load.load_varying_in_z_parameters')
                 varying_in_z = load_location_parameter[4]
                 for i,j in enumerate(varying_in_z):
-                    frllvp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_in_z_parameters')
+                    frllvp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_in_z_parameters_row')
                     frllvp.no = i+1
-                    frllvp.distance = varying_in_z[i][0]
-                    frllvp.factor = varying_in_z[i][1]
+                    frllvp.row.distance = varying_in_z[i][0]
+                    frllvp.row.factor = varying_in_z[i][1]
                     clientObject.load_varying_in_z_parameters.free_rectangular_load_load_varying_in_z_parameters.append(frllvp)
 
             elif load_distribution.name == 'LOAD_DISTRIBUTION_VARYING_ALONG_PERIMETER':
                 if len(load_location_parameter) != 8:
                     raise Exception('WARNING: The load location parameter for the designated location and distribution type needs to be of length 9. Kindly check list inputs for completeness and correctness.')
                 clientObject.load_location_first_x = load_location_parameter[0]
                 clientObject.load_location_first_y = load_location_parameter[1]
@@ -298,52 +298,52 @@
                 clientObject.axis_definition_p2_y = load_location_parameter[5][1]
                 clientObject.axis_definition_p2_z = load_location_parameter[5][2]
                 clientObject.axis_start_angle = load_location_parameter[6]
 
                 clientObject.load_varying_along_perimeter_parameters = model.clientModel.factory.create('ns0:free_rectangular_load.load_varying_along_perimeter_parameters')
                 varying_along_perimeter = load_location_parameter[7]
                 for i,j in enumerate(varying_along_perimeter):
-                    frllvapp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_along_perimeter_parameters')
+                    frllvapp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_along_perimeter_parameters_row')
                     frllvapp.no = i+1
-                    frllvapp.alpha = varying_along_perimeter[i][0] * (pi/180)
-                    frllvapp.factor = varying_along_perimeter[i][1]
+                    frllvapp.row.alpha = varying_along_perimeter[i][0] * (pi/180)
+                    frllvapp.row.factor = varying_along_perimeter[i][1]
                     clientObject.load_varying_along_perimeter_parameters.free_rectangular_load_load_varying_along_perimeter_parameters.append(frllvapp)
 
             elif load_distribution.name == 'LOAD_DISTRIBUTION_VARYING_IN_Z_AND_ALONG_PERIMETER':
                 if len(load_location_parameter) != 9:
                     raise Exception('WARNING: The load location parameter for the designated location and distribution type needs to be of length 9. Kindly check list inputs for completeness and correctness.')
                 clientObject.load_location_first_x = load_location_parameter[0]
                 clientObject.load_location_first_y = load_location_parameter[1]
                 clientObject.load_location_second_x = load_location_parameter[2]
                 clientObject.load_location_second_y = load_location_parameter[3]
 
                 clientObject.load_varying_in_z_parameters = model.clientModel.factory.create('ns0:free_rectangular_load.load_varying_in_z_parameters')
                 varying_in_z = load_location_parameter[4]
                 for i,j in enumerate(varying_in_z):
-                    frllvp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_in_z_parameters')
+                    frllvp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_in_z_parameters_row')
                     frllvp.no = i+1
-                    frllvp.distance = varying_in_z[i][0]
-                    frllvp.factor = varying_in_z[i][1]
+                    frllvp.row.distance = varying_in_z[i][0]
+                    frllvp.row.factor = varying_in_z[i][1]
                     clientObject.load_varying_in_z_parameters.free_rectangular_load_load_varying_in_z_parameters.append(frllvp)
 
                 clientObject.axis_definition_p1_x = load_location_parameter[5][0]
                 clientObject.axis_definition_p1_y = load_location_parameter[5][1]
                 clientObject.axis_definition_p1_z = load_location_parameter[5][2]
                 clientObject.axis_definition_p2_x = load_location_parameter[6][0]
                 clientObject.axis_definition_p2_y = load_location_parameter[6][1]
                 clientObject.axis_definition_p2_z = load_location_parameter[6][2]
                 clientObject.axis_start_angle = load_location_parameter[7]
 
                 clientObject.load_varying_along_perimeter_parameters = model.clientModel.factory.create('ns0:free_rectangular_load.load_varying_along_perimeter_parameters')
                 varying_along_perimeter = load_location_parameter[8]
                 for i,j in enumerate(varying_along_perimeter):
-                    frllvapp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_along_perimeter_parameters')
+                    frllvapp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_along_perimeter_parameters_row')
                     frllvapp.no = i+1
-                    frllvapp.alpha = varying_along_perimeter[i][0] * (pi/180)
-                    frllvapp.factor = varying_along_perimeter[i][1]
+                    frllvapp.row.alpha = varying_along_perimeter[i][0] * (pi/180)
+                    frllvapp.row.factor = varying_along_perimeter[i][1]
                     clientObject.load_varying_along_perimeter_parameters.free_rectangular_load_load_varying_along_perimeter_parameters.append(frllvapp)
 
         elif load_location.name == 'LOAD_LOCATION_RECTANGLE_CENTER_AND_SIDES':
 
             if load_distribution.name == 'LOAD_DISTRIBUTION_UNIFORM' or load_distribution.name == 'LOAD_DISTRIBUTION_LINEAR_FIRST' or load_distribution.name == 'LOAD_DISTRIBUTION_LINEAR_SECOND':
                 if len(load_location_parameter) != 5:
                     raise Exception('WARNING: The load location parameter for the designated location and distribution type needs to be of length 5. Kindly check list inputs for completeness and correctness.')
@@ -360,18 +360,18 @@
                 clientObject.load_location_center_y = load_location_parameter[1]
                 clientObject.load_location_center_side_a = load_location_parameter[2]
                 clientObject.load_location_center_side_b = load_location_parameter[3]
 
                 clientObject.load_varying_in_z_parameters = model.clientModel.factory.create('ns0:free_rectangular_load.load_varying_in_z_parameters')
                 varying_in_z = load_location_parameter[4]
                 for i,j in enumerate(varying_in_z):
-                    frllvp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_in_z_parameters')
+                    frllvp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_in_z_parameters_row')
                     frllvp.no = i+1
-                    frllvp.distance = varying_in_z[i][0]
-                    frllvp.factor = varying_in_z[i][1]
+                    frllvp.row.distance = varying_in_z[i][0]
+                    frllvp.row.factor = varying_in_z[i][1]
                     clientObject.load_varying_in_z_parameters.free_rectangular_load_load_varying_in_z_parameters.append(frllvp)
 
             elif load_distribution.name == 'LOAD_DISTRIBUTION_VARYING_ALONG_PERIMETER':
                 if len(load_location_parameter) != 8:
                     raise Exception('WARNING: The load location parameter for the designated location and distribution type needs to be of length 9. Kindly check list inputs for completeness and correctness.')
                 clientObject.load_location_center_x = load_location_parameter[0]
                 clientObject.load_location_center_y = load_location_parameter[1]
@@ -384,52 +384,52 @@
                 clientObject.axis_definition_p2_y = load_location_parameter[5][1]
                 clientObject.axis_definition_p2_z = load_location_parameter[5][2]
                 clientObject.axis_start_angle = load_location_parameter[6]
 
                 clientObject.load_varying_along_perimeter_parameters = model.clientModel.factory.create('ns0:free_rectangular_load.load_varying_along_perimeter_parameters')
                 varying_along_perimeter = load_location_parameter[7]
                 for i,j in enumerate(varying_along_perimeter):
-                    frllvapp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_along_perimeter_parameters')
+                    frllvapp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_along_perimeter_parameters_row')
                     frllvapp.no = i+1
-                    frllvapp.alpha = varying_along_perimeter[i][0] * (pi/180)
-                    frllvapp.factor = varying_along_perimeter[i][1]
+                    frllvapp.row.alpha = varying_along_perimeter[i][0] * (pi/180)
+                    frllvapp.row.factor = varying_along_perimeter[i][1]
                     clientObject.load_varying_along_perimeter_parameters.free_rectangular_load_load_varying_along_perimeter_parameters.append(frllvapp)
 
             elif load_distribution.name == 'LOAD_DISTRIBUTION_VARYING_IN_Z_AND_ALONG_PERIMETER':
                 if len(load_location_parameter) != 9:
                     raise Exception('WARNING: The load location parameter for the designated location and distribution type needs to be of length 9. Kindly check list inputs for completeness and correctness.')
                 clientObject.load_location_center_x = load_location_parameter[0]
                 clientObject.load_location_center_y = load_location_parameter[1]
                 clientObject.load_location_center_side_a = load_location_parameter[2]
                 clientObject.load_location_center_side_b = load_location_parameter[3]
 
                 clientObject.load_varying_in_z_parameters = model.clientModel.factory.create('ns0:free_rectangular_load.load_varying_in_z_parameters')
                 varying_in_z = load_location_parameter[4]
                 for i,j in enumerate(varying_in_z):
-                    frllvp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_in_z_parameters')
+                    frllvp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_in_z_parameters_row')
                     frllvp.no = i+1
-                    frllvp.distance = varying_in_z[i][0]
-                    frllvp.factor = varying_in_z[i][1]
+                    frllvp.row.distance = varying_in_z[i][0]
+                    frllvp.row.factor = varying_in_z[i][1]
                     clientObject.load_varying_in_z_parameters.free_rectangular_load_load_varying_in_z_parameters.append(frllvp)
 
                 clientObject.axis_definition_p1_x = load_location_parameter[5][0]
                 clientObject.axis_definition_p1_y = load_location_parameter[5][1]
                 clientObject.axis_definition_p1_z = load_location_parameter[5][2]
                 clientObject.axis_definition_p2_x = load_location_parameter[6][0]
                 clientObject.axis_definition_p2_y = load_location_parameter[6][1]
                 clientObject.axis_definition_p2_z = load_location_parameter[6][2]
                 clientObject.axis_start_angle = load_location_parameter[7]
 
                 clientObject.load_varying_along_perimeter_parameters = model.clientModel.factory.create('ns0:free_rectangular_load.load_varying_along_perimeter_parameters')
                 varying_along_perimeter = load_location_parameter[8]
                 for i,j in enumerate(varying_along_perimeter):
-                    frllvapp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_along_perimeter_parameters')
+                    frllvapp = model.clientModel.factory.create('ns0:free_rectangular_load_load_varying_along_perimeter_parameters_row')
                     frllvapp.no = i+1
-                    frllvapp.alpha = varying_along_perimeter[i][0] * (pi/180)
-                    frllvapp.factor = varying_along_perimeter[i][1]
+                    frllvapp.row.alpha = varying_along_perimeter[i][0] * (pi/180)
+                    frllvapp.row.factor = varying_along_perimeter[i][1]
                     clientObject.load_varying_along_perimeter_parameters.free_rectangular_load_load_varying_along_perimeter_parameters.append(frllvapp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -585,18 +585,18 @@
 
         # Load Direction
         clientObject.load_direction = load_direction.name
 
         # Load Location
         clientObject.load_location = model.clientModel.factory.create('ns0:free_polygon_load.load_location')
         for i,j in enumerate(load_location):
-            fplld = model.clientModel.factory.create('ns0:free_polygon_load_load_location')
+            fplld = model.clientModel.factory.create('ns0:free_polygon_load_load_location_row')
             fplld.no = i+1
-            fplld.first_coordinate = load_location[i][0]
-            fplld.second_coordinate = load_location[i][1]
+            fplld.row.first_coordinate = load_location[i][0]
+            fplld.row.second_coordinate = load_location[i][1]
             clientObject.load_location.free_polygon_load_load_location.append(fplld)
 
         # Load Parameter
         if load_distribution.name == 'LOAD_DISTRIBUTION_UNIFORM':
             if len(load_parameter) != 1:
                 raise Exception('WARNING: The load parameter needs to be of length 1. Kindly check list inputs for completeness and correctness.')
             clientObject.magnitude_uniform = load_parameter[0]
```

### Comparing `RFEM-1.7.0/RFEM/Loads/imposedLineDeformation.py` & `RFEM-1.8.0/RFEM/Loads/imposedLineDeformation.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/Loads/imposedNodalDeformation.py` & `RFEM-1.8.0/RFEM/Loads/imposedNodalDeformation.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/Loads/lineLoad.py` & `RFEM-1.8.0/RFEM/Loads/lineLoad.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,20 +223,20 @@
                 print("WARNING: LineLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:line_load.varying_load_parameters')
 
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise Exception('WARNING: The load parameter sub-lists need to be of length 3. Kindly check sub-list inputs for completeness and correctness.')
-                mlvlp = model.clientModel.factory.create('ns0:line_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:line_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
 
                 clientObject.varying_load_parameters.line_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             if len(load_parameter) != 6:
                 raise Exception('WARNING: The load parameter needs to be of length 6. Kindly check list inputs for completeness and correctness.')
             if not isinstance(load_parameter[0], bool) or not isinstance(load_parameter[1], bool):
@@ -289,20 +289,20 @@
             except:
                 print("WARNING: LineLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:line_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise Exception('WARNING: The load parameter sub-lists need to be of length 3. Kindly check sub-list inputs for completeness and correctness.')
-                mlvlp = model.clientModel.factory.create('ns0:line_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:line_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
 
                 clientObject.varying_load_parameters.line_load_varying_load_parameters.append(mlvlp)
 
         # Line Load Direction
         clientObject.load_direction = load_direction.name
 
         # Reference to List of Lines
@@ -476,20 +476,20 @@
                 print("WARNING: LineLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:line_load.varying_load_parameters')
 
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise Exception('WARNING: The load parameter sub-lists need to be of length 3. Kindly check sub-list inputs for completeness and correctness.')
-                mlvlp = model.clientModel.factory.create('ns0:line_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:line_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
 
                 clientObject.varying_load_parameters.line_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             if len(load_parameter) != 6:
                 raise Exception('WARNING: The load parameter needs to be of length 6. Kindly check list inputs for completeness and correctness.')
             if not isinstance(load_parameter[0], bool) or not isinstance(load_parameter[1], bool):
@@ -542,20 +542,20 @@
             except:
                 print("WARNING: LineLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:line_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise Exception('WARNING: The load parameter sub-lists need to be of length 3. Kindly check sub-list inputs for completeness and correctness.')
-                mlvlp = model.clientModel.factory.create('ns0:line_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:line_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
 
                 clientObject.varying_load_parameters.line_load_varying_load_parameters.append(mlvlp)
 
         # Line Load Direction
         clientObject.load_direction = load_direction.name
 
         #Reference to List of Lines
```

### Comparing `RFEM-1.7.0/RFEM/Loads/linesetLoad.py` & `RFEM-1.8.0/RFEM/Loads/linesetLoad.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,20 +197,20 @@
                 print("WARNING: LineLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = Model.clientModel.factory.create('ns0:line_load.varying_load_parameters')
 
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise Exception('WARNING: The load parameter sub-lists need to be of length 3. Kindly check sub-list inputs for completeness and correctness.')
-                mlvlp = Model.clientModel.factory.create('ns0:line_set_load_varying_load_parameters')
+                mlvlp = Model.clientModel.factory.create('ns0:line_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
 
                 clientObject.varying_load_parameters.line_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             if len(load_parameter) != 6:
                 raise Exception('WARNING: The load parameter needs to be of length 6. Kindly check list inputs for completeness and correctness.')
             if not isinstance(load_parameter[0], bool) or not isinstance(load_parameter[1], bool):
@@ -263,20 +263,20 @@
             except:
                 print("WARNING: LineLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = Model.clientModel.factory.create('ns0:line_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise Exception('WARNING: The load parameter sub-lists need to be of length 3. Kindly check sub-list inputs for completeness and correctness.')
-                mlvlp = Model.clientModel.factory.create('ns0:line_set_load_varying_load_parameters')
+                mlvlp = Model.clientModel.factory.create('ns0:line_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
 
                 clientObject.varying_load_parameters.line_set_load_varying_load_parameters.append(mlvlp)
 
         # Line Load Direction
         clientObject.load_direction = load_direction.name
 
         # Reference to List of Lines
@@ -428,20 +428,20 @@
                 print("WARNING: LineLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = Model.clientModel.factory.create('ns0:line_load.varying_load_parameters')
 
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise Exception('WARNING: The load parameter sub-lists need to be of length 3. Kindly check sub-list inputs for completeness and correctness.')
-                mlvlp = Model.clientModel.factory.create('ns0:line_set_load_varying_load_parameters')
+                mlvlp = Model.clientModel.factory.create('ns0:line_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
 
                 clientObject.varying_load_parameters.line_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             if len(load_parameter) != 6:
                 raise Exception('WARNING: The load parameter needs to be of length 6. Kindly check list inputs for completeness and correctness.')
             if not isinstance(load_parameter[0], bool) or not isinstance(load_parameter[1], bool):
@@ -494,20 +494,20 @@
             except:
                 print("WARNING: LineLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = Model.clientModel.factory.create('ns0:line_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise Exception('WARNING: The load parameter sub-lists need to be of length 3. Kindly check sub-list inputs for completeness and correctness.')
-                mlvlp = Model.clientModel.factory.create('ns0:line_set_load_varying_load_parameters')
+                mlvlp = Model.clientModel.factory.create('ns0:line_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
 
                 clientObject.varying_load_parameters.line_set_load_varying_load_parameters.append(mlvlp)
 
         # Lineset Load Direction
         clientObject.load_direction = load_direction.name
 
         # Reference to List of Lines
```

### Comparing `RFEM-1.7.0/RFEM/Loads/memberLoad.py` & `RFEM-1.8.0/RFEM/Loads/memberLoad.py`

 * *Files 7% similar despite different names*

```diff
@@ -215,24 +215,24 @@
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
 
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
             clientObject.distance_b_is_defined_as_relative = load_parameter[1]
             clientObject.magnitude_1 = load_parameter[2]
@@ -273,45 +273,45 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING_IN_Z":
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
         #Reference to List of Members
@@ -503,24 +503,24 @@
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
 
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
             clientObject.distance_b_is_defined_as_relative = load_parameter[1]
             clientObject.magnitude_1 = load_parameter[2]
@@ -561,24 +561,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
         #Reference to List of Members
@@ -791,24 +791,24 @@
             try:
                 len(load_parameter[0])==4
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = load_parameter[i][2]
-                mlvlp.magnitude_delta_t = load_parameter[i][3]
-                mlvlp.magnitude_t_t = load_parameter[i][2]
-                mlvlp.magnitude_t_b = load_parameter[i][3]
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = load_parameter[i][2]
+                mlvlp.row.magnitude_delta_t = load_parameter[i][3]
+                mlvlp.row.magnitude_t_t = load_parameter[i][2]
+                mlvlp.row.magnitude_t_b = load_parameter[i][3]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
@@ -951,24 +951,24 @@
             try:
                 len(load_parameter[0])==4
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = load_parameter[i][2]
-                mlvlp.magnitude_delta_t = load_parameter[i][3]
-                mlvlp.magnitude_t_t = load_parameter[i][2]
-                mlvlp.magnitude_t_b = load_parameter[i][3]
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = load_parameter[i][2]
+                mlvlp.row.magnitude_delta_t = load_parameter[i][3]
+                mlvlp.row.magnitude_t_t = load_parameter[i][2]
+                mlvlp.row.magnitude_t_b = load_parameter[i][3]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
@@ -1100,24 +1100,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
@@ -1310,24 +1310,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
@@ -1544,24 +1544,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
 
@@ -1609,24 +1609,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
@@ -1782,24 +1782,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
 
@@ -1847,24 +1847,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
```

### Comparing `RFEM-1.7.0/RFEM/Loads/membersetload.py` & `RFEM-1.8.0/RFEM/Loads/membersetload.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,24 +235,24 @@
                     len(load_parameter[0])==3
                 except:
                     print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
                 clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
 
                 for i,j in enumerate(load_parameter):
-                    mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                    mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                     mlvlp.no = i+1
-                    mlvlp.distance = load_parameter[i][0]
-                    mlvlp.delta_distance = load_parameter[i][1]
-                    mlvlp.magnitude = load_parameter[i][2]
-                    mlvlp.note = None
-                    mlvlp.magnitude_t_c = 0.0
-                    mlvlp.magnitude_delta_t = 0.0
-                    mlvlp.magnitude_t_t = 0.0
-                    mlvlp.magnitude_t_b = 0.0
+                    mlvlp.row.distance = load_parameter[i][0]
+                    mlvlp.row.delta_distance = load_parameter[i][1]
+                    mlvlp.row.magnitude = load_parameter[i][2]
+                    mlvlp.row.note = None
+                    mlvlp.row.magnitude_t_c = 0.0
+                    mlvlp.row.magnitude_delta_t = 0.0
+                    mlvlp.row.magnitude_t_t = 0.0
+                    mlvlp.row.magnitude_t_b = 0.0
 
                     clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
             elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
                 if len(load_parameter) == 6:
                     clientObject.distance_a_is_defined_as_relative = load_parameter[0]
                     clientObject.distance_b_is_defined_as_relative = load_parameter[1]
@@ -301,45 +301,45 @@
                 try:
                     len(load_parameter[0])==3
                 except:
                     print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
                 clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
                 for i,j in enumerate(load_parameter):
-                    mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                    mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                     mlvlp.no = i+1
-                    mlvlp.distance = load_parameter[i][0]
-                    mlvlp.delta_distance = load_parameter[i][1]
-                    mlvlp.magnitude = load_parameter[i][2]
-                    mlvlp.note = None
-                    mlvlp.magnitude_t_c = 0.0
-                    mlvlp.magnitude_delta_t = 0.0
-                    mlvlp.magnitude_t_t = 0.0
-                    mlvlp.magnitude_t_b = 0.0
+                    mlvlp.row.distance = load_parameter[i][0]
+                    mlvlp.row.delta_distance = load_parameter[i][1]
+                    mlvlp.row.magnitude = load_parameter[i][2]
+                    mlvlp.row.note = None
+                    mlvlp.row.magnitude_t_c = 0.0
+                    mlvlp.row.magnitude_delta_t = 0.0
+                    mlvlp.row.magnitude_t_t = 0.0
+                    mlvlp.row.magnitude_t_b = 0.0
 
                     clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
             elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING_IN_Z":
                 try:
                     len(load_parameter[0])==3
                 except:
                     print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
                 clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
                 for i,j in enumerate(load_parameter):
-                    mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                    mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                     mlvlp.no = i+1
-                    mlvlp.distance = load_parameter[i][0]
-                    mlvlp.delta_distance = load_parameter[i][1]
-                    mlvlp.magnitude = load_parameter[i][2]
-                    mlvlp.note = None
-                    mlvlp.magnitude_t_c = 0.0
-                    mlvlp.magnitude_delta_t = 0.0
-                    mlvlp.magnitude_t_t = 0.0
-                    mlvlp.magnitude_t_b = 0.0
+                    mlvlp.row.distance = load_parameter[i][0]
+                    mlvlp.row.delta_distance = load_parameter[i][1]
+                    mlvlp.row.magnitude = load_parameter[i][2]
+                    mlvlp.row.note = None
+                    mlvlp.row.magnitude_t_c = 0.0
+                    mlvlp.row.magnitude_delta_t = 0.0
+                    mlvlp.row.magnitude_t_t = 0.0
+                    mlvlp.row.magnitude_t_b = 0.0
 
                     clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
         #Force Eccentiricity
@@ -555,24 +555,24 @@
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
 
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             try:
                 len(load_parameter)==6
             except:
@@ -625,24 +625,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
         # Comment
@@ -870,24 +870,24 @@
             try:
                 len(load_parameter[0])==4
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = load_parameter[i][2]
-                mlvlp.magnitude_delta_t = load_parameter[i][3]
-                mlvlp.magnitude_t_t = load_parameter[i][2]
-                mlvlp.magnitude_t_b = load_parameter[i][3]
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = load_parameter[i][2]
+                mlvlp.row.magnitude_delta_t = load_parameter[i][3]
+                mlvlp.row.magnitude_t_t = load_parameter[i][2]
+                mlvlp.row.magnitude_t_b = load_parameter[i][3]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -1041,24 +1041,24 @@
             try:
                 len(load_parameter[0])==4
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = load_parameter[i][2]
-                mlvlp.magnitude_delta_t = load_parameter[i][3]
-                mlvlp.magnitude_t_t = load_parameter[i][2]
-                mlvlp.magnitude_t_b = load_parameter[i][3]
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = load_parameter[i][2]
+                mlvlp.row.magnitude_delta_t = load_parameter[i][3]
+                mlvlp.row.magnitude_t_t = load_parameter[i][2]
+                mlvlp.row.magnitude_t_b = load_parameter[i][3]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -1201,24 +1201,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -1421,24 +1421,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -1667,24 +1667,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             try:
                 len(load_parameter)==6
             except:
@@ -1747,24 +1747,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -1934,24 +1934,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             try:
                 len(load_parameter) ==  6
             except:
@@ -2014,24 +2014,24 @@
             try:
                 len(load_parameter[0])==3
             except:
                 print("WARNING: MemberSetLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
-                mlvlp.magnitude_t_c = 0.0
-                mlvlp.magnitude_delta_t = 0.0
-                mlvlp.magnitude_t_t = 0.0
-                mlvlp.magnitude_t_b = 0.0
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
+                mlvlp.row.magnitude_t_c = 0.0
+                mlvlp.row.magnitude_delta_t = 0.0
+                mlvlp.row.magnitude_t_t = 0.0
+                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
```

### Comparing `RFEM-1.7.0/RFEM/Loads/nodalLoad.py` & `RFEM-1.8.0/RFEM/Loads/nodalLoad.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/Loads/solidLoad.py` & `RFEM-1.8.0/RFEM/Loads/solidLoad.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/Loads/solidSetLoad.py` & `RFEM-1.8.0/RFEM/Loads/solidSetLoad.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/Loads/surfaceLoad.py` & `RFEM-1.8.0/RFEM/Loads/surfaceLoad.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,20 +163,20 @@
                 clientObject.axis_definition_p1_y = load_parameter[6][1]
                 clientObject.axis_definition_p1_z = load_parameter[6][2]
 
         elif load_distribution == SurfaceLoadDistribution.LOAD_DISTRIBUTION_VARYING_IN_Z:
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:surface_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:surface_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:surface_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
                 clientObject.varying_load_parameters.surface_load_varying_load_parameters.append(mlvlp)
                 clientObject.varying_load_parameters_sorted = True
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
```

### Comparing `RFEM-1.7.0/RFEM/Loads/surfacesetload.py` & `RFEM-1.8.0/RFEM/Loads/surfacesetload.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,20 +163,20 @@
                 clientObject.axis_definition_p1_y = load_parameter[6][1]
                 clientObject.axis_definition_p1_z = load_parameter[6][2]
 
         elif load_distribution == SurfaceSetLoadDistribution.LOAD_DISTRIBUTION_VARYING_IN_Z:
 
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:surface_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                mlvlp = model.clientModel.factory.create('ns0:surface_set_load_varying_load_parameters')
+                mlvlp = model.clientModel.factory.create('ns0:surface_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
-                mlvlp.distance = load_parameter[i][0]
-                mlvlp.delta_distance = load_parameter[i][1]
-                mlvlp.magnitude = load_parameter[i][2]
-                mlvlp.note = None
+                mlvlp.row.distance = load_parameter[i][0]
+                mlvlp.row.delta_distance = load_parameter[i][1]
+                mlvlp.row.magnitude = load_parameter[i][2]
+                mlvlp.row.note = None
                 clientObject.varying_load_parameters.surface_set_load_varying_load_parameters.append(mlvlp)
                 clientObject.varying_load_parameters_sorted = True
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
```

### Comparing `RFEM-1.7.0/RFEM/SpecialObjects/enlargedColumnHead.py` & `RFEM-1.8.0/RFEM/SpecialObjects/enlargedColumnHead.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/SpecialObjects/intersection.py` & `RFEM-1.8.0/RFEM/SpecialObjects/intersection.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/SpecialObjects/resultSection.py` & `RFEM-1.8.0/RFEM/SpecialObjects/resultSection.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/SpecialObjects/rigidLink.py` & `RFEM-1.8.0/RFEM/SpecialObjects/rigidLink.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/SpecialObjects/structureModification.py` & `RFEM-1.8.0/RFEM/SpecialObjects/structureModification.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/SpecialObjects/surfaceContact.py` & `RFEM-1.8.0/RFEM/SpecialObjects/surfaceContact.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/SpecialObjects/surfaceResultAdjustment.py` & `RFEM-1.8.0/RFEM/SpecialObjects/surfaceResultAdjustment.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForLines/lineHinge.py` & `RFEM-1.8.0/RFEM/TypesForLines/lineHinge.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForLines/lineMeshRefinements.py` & `RFEM-1.8.0/RFEM/TypesForLines/lineMeshRefinements.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForLines/lineSupport.py` & `RFEM-1.8.0/RFEM/TypesForLines/lineSupport.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForLines/lineWeldedJoint.py` & `RFEM-1.8.0/RFEM/TypesForLines/lineWeldedJoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 
         iLines = ConvertStrToListOfInt(lines)
         iSurfaces = ConvertStrToListOfInt(surfaces)
 
         for i in iLines:
             line = model.clientModel.service.get_line(i)
             line.has_line_welds = True
-            clientWeld = model.clientModel.factory.create('ns0:line_line_weld_assignment')
+            clientWeld = model.clientModel.factory.create('ns0:line_line_weld_assignment_row')
             clientWeld.no = i
-            clientWeld.weld = no
-            clientWeld.surface1 = iSurfaces[0]
-            clientWeld.surface2 = iSurfaces[1]
+            clientWeld.row.weld = no
+            clientWeld.row.surface1 = iSurfaces[0]
+            clientWeld.row.surface2 = iSurfaces[1]
             if len(iSurfaces) == 3:
                 clientWeld.surface3 = iSurfaces[2]
             line.line_weld_assignment = model.clientModel.factory.create('ns0:array_of_line_line_weld_assignment')
             line.line_weld_assignment.line_line_weld_assignment.append(clientWeld)
             model.clientModel.service.set_line(line)
```

### Comparing `RFEM-1.7.0/RFEM/TypesForMembers/memberDefinableStiffness.py` & `RFEM-1.8.0/RFEM/TypesForMembers/memberDefinableStiffness.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForMembers/memberEccentricity.py` & `RFEM-1.8.0/RFEM/TypesForSpecialObjects/surfaceContactType.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from RFEM.initModel import Model, clearAtributes
 
-class MemberEccentricity():
+class SurfaceContactType():
     def __init__(self,
                  no: int = 1,
                  comment: str = '',
                  params: dict = None,
                  model = Model):
 
-        # Client model | Member Eccentricity
-        clientObject = model.clientModel.factory.create('ns0:member_eccentricity')
+        # Client model | Surface Contact Type
+        clientObject = model.clientModel.factory.create('ns0:surfaces_contact_type')
 
         # Clears object atributes | Sets all atributes to None
         clearAtributes(clientObject)
 
-        # Member Eccentricity No.
+        # Surface Contact Type No.
         clientObject.no = no
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
-        # Add Member Eccentricity to client model
-        model.clientModel.service.set_member_eccentricity(clientObject)
+        # Add Surface Contact Type to client model
+        model.clientModel.service.set_surfaces_contact_type(clientObject)
```

### Comparing `RFEM-1.7.0/RFEM/TypesForNodes/nodalMeshRefinement.py` & `RFEM-1.8.0/RFEM/TypesForNodes/nodalMeshRefinement.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForNodes/nodalSupport.py` & `RFEM-1.8.0/RFEM/TypesForNodes/nodalSupport.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForSolids/solidContact.py` & `RFEM-1.8.0/RFEM/TypesForSolids/solidContact.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForSolids/solidGas.py` & `RFEM-1.8.0/RFEM/TypesForSolids/solidGas.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForSolids/solidMeshRefinement.py` & `RFEM-1.8.0/RFEM/TypesForSolids/solidMeshRefinement.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForSurfaces/surfaceEccentricity.py` & `RFEM-1.8.0/RFEM/TypesForSurfaces/surfaceEccentricity.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForSurfaces/surfaceMeshRefinements.py` & `RFEM-1.8.0/RFEM/TypesForSurfaces/surfaceMeshRefinements.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForSurfaces/surfaceStiffnessModification.py` & `RFEM-1.8.0/RFEM/TypesForSurfaces/surfaceStiffnessModification.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesForSurfaces/surfaceSupport.py` & `RFEM-1.8.0/RFEM/TypesForSurfaces/surfaceSupport.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesforConcreteDesign/ConcreteDurability.py` & `RFEM-1.8.0/RFEM/TypesforConcreteDesign/ConcreteDurability.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesforConcreteDesign/ConcreteEffectiveLength.py` & `RFEM-1.8.0/RFEM/TypesforConcreteDesign/ConcreteEffectiveLength.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesforConcreteDesign/ConcreteReinforcementDirections.py` & `RFEM-1.8.0/RFEM/TypesforConcreteDesign/ConcreteReinforcementDirections.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/TypesforConcreteDesign/ConcreteSurfaceReinforcements.py` & `RFEM-1.8.0/RFEM/TypesforConcreteDesign/ConcreteSurfaceReinforcements.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/baseSettings.py` & `RFEM-1.8.0/RFEM/baseSettings.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/dependencies.py` & `RFEM-1.8.0/RFEM/dependencies.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/enums.py` & `RFEM-1.8.0/RFEM/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -1938,7 +1938,122 @@
         DESIGN_SITUATION_TYPE_TYPE_1_ACCIDENTAL_PSI_1_1, DESIGN_SITUATION_TYPE_TYPE_1_ACCIDENTAL_PSI_2_1, DESIGN_SITUATION_TYPE_TYPE_1_FUNDAMENTAL, DESIGN_SITUATION_TYPE_TYPE_2_ACCIDENTAL_PSI_1_1, DESIGN_SITUATION_TYPE_TYPE_2_ACCIDENTAL_PSI_2_1, DESIGN_SITUATION_TYPE_TYPE_2_FUNDAMENTAL, DESIGN_SITUATION_TYPE_TYPE_3_ACCIDENTAL_PSI_1_1, \
         DESIGN_SITUATION_TYPE_TYPE_3_ACCIDENTAL_PSI_2_1, DESIGN_SITUATION_TYPE_TYPE_3_FUNDAMENTAL, DESIGN_SITUATION_TYPE_ULS_ACCIDENTAL_GB_50068, DESIGN_SITUATION_TYPE_ULS_ACCIDENTAL_STORAGE, DESIGN_SITUATION_TYPE_ULS_ALL_VARIABLE_ACTIONS_STORAGE, DESIGN_SITUATION_TYPE_ULS_CSA_A23_3, DESIGN_SITUATION_TYPE_ULS_EXCEPTIONAL, \
         DESIGN_SITUATION_TYPE_ULS_FUNDAMENTAL_EARTHQUAKE_GB_50011, DESIGN_SITUATION_TYPE_ULS_FUNDAMENTAL_GB_50068, DESIGN_SITUATION_TYPE_ULS_LOAD_CASE_1, DESIGN_SITUATION_TYPE_ULS_LOAD_CASE_2, DESIGN_SITUATION_TYPE_ULS_LOAD_CASE_3, DESIGN_SITUATION_TYPE_ULS_LOAD_CASE_4, DESIGN_SITUATION_TYPE_ULS_NORMAL, \
         DESIGN_SITUATION_TYPE_ULS_ONE_VARIABLE_ACTION_STORAGE, DESIGN_SITUATION_TYPE_ULS_SNIP_BASIC, DESIGN_SITUATION_TYPE_ULS_SNIP_SPECIAL, DESIGN_SITUATION_TYPE_ULS_SP63_13330, DESIGN_SITUATION_TYPE_ULS_SPECIAL, DESIGN_SITUATION_TYPE_ULS_STABILITY_AS_NZS, DESIGN_SITUATION_TYPE_ULS_STRENGTH_AS_NZS, DESIGN_SITUATION_TYPE_ULS_STRENGTH_FIRE_NZS, \
         DESIGN_SITUATION_TYPE_ULS_STR_GEO_PERMANENT_AND_TRANSIENT, DESIGN_SITUATION_TYPE_ULTIMATE_LIMIT_STATE, DESIGN_SITUATION_TYPE_ULTIMATE_LIMIT_STATE_1, DESIGN_SITUATION_TYPE_ULTIMATE_LIMIT_STATE_2, DESIGN_SITUATION_TYPE_ULTIMATE_LIMIT_STATE_3, DESIGN_SITUATION_TYPE_ULTIMATE_LIMIT_STATE_4, DESIGN_SITUATION_TYPE_ULTIMATE_LIMIT_STATE_5, \
         DESIGN_SITUATION_TYPE_UPL_ACCIDENTAL_PSI_1_1, DESIGN_SITUATION_TYPE_UPL_ACCIDENTAL_PSI_2_1, DESIGN_SITUATION_TYPE_UPL_PERMANENT_AND_TRANSIENT, DESIGN_SITUATION_TYPE_UPL_SEISMIC = range(
             387)
+
+class MemberEccentricityHorizontalSectionAlignment(Enum):
+    '''
+    Member Eccentricity Horizontal Section Alignment
+    '''
+    ALIGN_LEFT, ALIGN_MIDDLE, ALIGN_RIGHT = range(3)
+
+class MemberEccentricitySpecificationType(Enum):
+    '''
+    Member Eccentricity Specification Type
+    '''
+    TYPE_ABSOLUTE, TYPE_RELATIVE, TYPE_RELATIVE_AND_ABSOLUTE = range(3)
+
+class MemberEccentricityTransverseOffsetType(Enum):
+    '''
+    Member Eccentricity Transverse Offset Reference Type
+    '''
+    TRANSVERSE_OFFSET_TYPE_FROM_MEMBER_SECTION, TRANSVERSE_OFFSET_TYPE_FROM_SURFACE_THICKNESS, TRANSVERSE_OFFSET_TYPE_NONE = range(3)
+
+class MemberEccentricityTransverseOffsetHorizontalAlignment(Enum):
+    '''
+    Member Eccentricity Transverse Offset Horizontal Alignment
+    '''
+    ALIGN_LEFT, ALIGN_MIDDLE, ALIGN_RIGHT = range(3)
+
+class MemberEccentricityTransverseOffsetVerticalAlignment(Enum):
+    '''
+    Member Eccentricity Transverse Vertical Alignment
+    '''
+    ALIGN_BOTTOM, ALIGN_MIDDLE, ALIGN_TOP = range(3)
+
+class MemberEccentricityVerticalSectionAlignment(Enum):
+    '''
+    Member Eccentricity Vertical Section Alignment
+    '''
+    ALIGN_BOTTOM, ALIGN_MIDDLE, ALIGN_TOP = range(3)
+
+class MemberHingeNonlineartiy(Enum):
+    '''
+    Member Hinge Nonlineartiy
+    '''
+    NONLINEARITY_TYPE_DIAGRAM, NONLINEARITY_TYPE_FAILURE_ALL_IF_NEGATIVE, NONLINEARITY_TYPE_FAILURE_ALL_IF_POSITIVE, NONLINEARITY_TYPE_FAILURE_IF_NEGATIVE, \
+    NONLINEARITY_TYPE_FAILURE_IF_POSITIVE, NONLINEARITY_TYPE_FORCE_MOMENT_DIAGRAM, NONLINEARITY_TYPE_FRICTION_DIRECTION_1, NONLINEARITY_TYPE_FRICTION_DIRECTION_1_2, \
+    NONLINEARITY_TYPE_FRICTION_DIRECTION_1_PLUS_2, NONLINEARITY_TYPE_FRICTION_DIRECTION_2, NONLINEARITY_TYPE_NONE, NONLINEARITY_TYPE_PARTIAL_ACTIVITY, \
+    NONLINEARITY_TYPE_PLASTIC_BILINEAR, NONLINEARITY_TYPE_PLASTIC_DIAGRAM, NONLINEARITY_TYPE_PLASTIC_FEMA_356_ELASTIC, NONLINEARITY_TYPE_PLASTIC_FEMA_356_RIGID, \
+    NONLINEARITY_TYPE_STIFFNESS_DIAGRAM = range(17)
+
+class MemberHingeDiagramType(Enum):
+    '''
+    Member Hinge Diagram Type
+    '''
+    DIAGRAM_ENDING_TYPE_CONTINUOUS, DIAGRAM_ENDING_TYPE_STOP, DIAGRAM_ENDING_TYPE_TEARING, DIAGRAM_ENDING_TYPE_YIELDING = range(4)
+
+class MemberHingePartialActivityType(Enum):
+    '''
+    Member Hinge Partial Activity Type
+    '''
+    PARTIAL_ACTIVITY_TYPE_COMPLETE, PARTIAL_ACTIVITY_TYPE_FIXED, PARTIAL_ACTIVITY_TYPE_INEFFECTIVNESS, PARTIAL_ACTIVITY_TYPE_TEARING, PARTIAL_ACTIVITY_TYPE_YIELDING = range(5)
+
+class MemberNonlinearityType(Enum):
+    '''
+    Member Nonlinearity Type
+    '''
+    TYPE_FAILURE_IF_COMPRESSION, TYPE_FAILURE_IF_COMPRESSION_WITH_SLIPPAGE, TYPE_FAILURE_IF_TENSION, TYPE_FAILURE_IF_TENSION_WITH_SLIPPAGE, \
+    TYPE_SLIPPAGE, TYPE_TEARING, TYPE_TEARING_IF_COMPRESSION, TYPE_TEARING_IF_TENSION, TYPE_YIELDING, TYPE_YIELDING_IF_COMPRESSION, TYPE_YIELDING_IF_TENSION = range(11)
+
+class MemberStiffnessModificationType(Enum):
+    '''
+    Member Stiffness Modification Type
+    '''
+    TYPE_CONCRETE_STRUCTURES_ACI, TYPE_CONCRETE_STRUCTURES_CSA, TYPE_PARTIAL_STIFFNESSES_FACTORS, TYPE_STEEL_STRUCTURES, TYPE_STEEL_STRUCTURES_CSA, TYPE_TOTAL_STIFFNESSES_FACTORS = range(6)
+
+class MemberStiffnessModificationSteelTaub(Enum):
+    '''
+    Member Stiffness Modification Steel Structure tau_b Determination
+    '''
+    ITERATIVE, SET_TO_1 = range(2)
+
+class MemberStiffnessModificationSteelDesignMethod(Enum):
+    '''
+    Member Stiffness Modification Steel Structure Design Method
+    '''
+    ASD, LRFD = range(2)
+
+class MemberStiffnessModificationConcreteComponentType(Enum):
+    '''
+    Member Stiffness Modification Concrete Structure Component Type
+    '''
+    COMPONENT_TYPE_BEAMS, COMPONENT_TYPE_COLUMNS = range(2)
+
+class MemberSupportNonlinearity(Enum):
+    '''
+    Member Support Nonlinearity
+    '''
+    NONLINEARITY_FAILURE_IF_NEGATIVE_CONTACT_STRESS_Z, NONLINEARITY_FAILURE_IF_POSITIVE_CONTACT_STRESS_Z, NONLINEARITY_NONE = range(3)
+
+class MemberTransverseStiffenerType(Enum):
+    '''
+    Member Transverse Stiffeners Stiffener Type
+    '''
+    STIFFENER_COMPONENT_TYPE_ANGLE, STIFFENER_COMPONENT_TYPE_CHANNEL_SECTION, STIFFENER_COMPONENT_TYPE_CONNECTING_COLUMN_END, \
+    STIFFENER_COMPONENT_TYPE_CONNECTING_COLUMN_START, STIFFENER_COMPONENT_TYPE_END_PLATE_END, STIFFENER_COMPONENT_TYPE_END_PLATE_START, \
+    STIFFENER_COMPONENT_TYPE_FLAT,STIFFENER_COMPONENT_TYPE_WARPING_RESTRAINT = range(8)
+
+class MemberTransverseStiffenerPosition(Enum):
+    '''
+    Member Transverse Stiffener Position Type
+    '''
+    STIFFENER_COMPONENT_POSITION_DOUBLE_SIDED, STIFFENER_COMPONENT_POSITION_SINGLE_SIDED_LEFT, STIFFENER_COMPONENT_POSITION_SINGLE_SIDED_RIGHT = range(3)
+
+class MemberTransverseStiffenerOffsetType(Enum):
+    '''
+    Member Transverse Stiffener Multiple Offset Definition Type
+    '''
+    OFFSET_DEFINITION_TYPE_ABSOLUTE, OFFSET_DEFINITION_TYPE_RELATIVE = range(2)
```

### Comparing `RFEM-1.7.0/RFEM/globalParameter.py` & `RFEM-1.8.0/RFEM/globalParameter.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM/initModel.py` & `RFEM-1.8.0/RFEM/initModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     for i in it:
         obj[i[0]] = None
     return obj
 
 def closeModel(index_or_name, save_changes = False):
     """
     Close any model with index or name. Be sure to close the first created
-    model last (2,1, and then 0). It carries whole session.
+    model last (2,1, and then 0). 0 index carries whole session.
     """
     if isinstance(index_or_name, int):
         client.service.close_model(index_or_name, save_changes)
         Model.__delete__(Model, index_or_name)
     elif isinstance(index_or_name, str):
         modelLs = client.service.get_model_list()
         for i,j in enumerate(modelLs.name):
```

### Comparing `RFEM-1.7.0/RFEM/suds_requests.py` & `RFEM-1.8.0/RFEM/suds_requests.py`

 * *Files identical despite different names*

### Comparing `RFEM-1.7.0/RFEM.egg-info/PKG-INFO` & `RFEM-1.8.0/RFEM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFEM
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python Framework for RFEM6 Web Services
 Home-page: https://github.com/Dlubal-Software/RFEM_Python_Client
 Author: Dlubal Software
 Author-email: info@dlubal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RFEM-1.7.0/RFEM.egg-info/SOURCES.txt` & `RFEM-1.8.0/RFEM.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 RFEM/TypesForMembers/memberDefinableStiffness.py
 RFEM/TypesForMembers/memberEccentricity.py
 RFEM/TypesForMembers/memberHinge.py
 RFEM/TypesForMembers/memberNonlinearity.py
 RFEM/TypesForMembers/memberResultIntermediatePoints.py
 RFEM/TypesForMembers/memberStiffnessModification.py
 RFEM/TypesForMembers/memberSupport.py
+RFEM/TypesForMembers/memberTransverseStiffeners.py
 RFEM/TypesForNodes/__init__.py
 RFEM/TypesForNodes/nodalMeshRefinement.py
 RFEM/TypesForNodes/nodalSupport.py
 RFEM/TypesForSolids/__init__.py
 RFEM/TypesForSolids/solidContact.py
 RFEM/TypesForSolids/solidGas.py
 RFEM/TypesForSolids/solidMeshRefinement.py
```

### Comparing `RFEM-1.7.0/setup.py` & `RFEM-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent
 readme = (here/"README.md").read_text()
 
 setup(
     name='RFEM',
-    version='1.7.0',
+    version='1.8.0',
     description='Python Framework for RFEM6 Web Services',
     long_description=readme,
     long_description_content_type = "text/markdown",
     url="https://github.com/Dlubal-Software/RFEM_Python_Client",
     author="Dlubal Software",
     author_email="info@dlubal.com",
     license="MIT",
```

