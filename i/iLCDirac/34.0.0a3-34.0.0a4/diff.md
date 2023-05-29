# Comparing `tmp/iLCDirac-34.0.0a3.tar.gz` & `tmp/iLCDirac-34.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iLCDirac-34.0.0a3.tar", last modified: Tue Dec 13 11:40:29 2022, max compression
+gzip compressed data, was "iLCDirac-34.0.0a4.tar", last modified: Mon May 29 13:18:57 2023, max compression
```

## Comparing `iLCDirac-34.0.0a3.tar` & `iLCDirac-34.0.0a4.tar`

### file list

```diff
@@ -1,466 +1,472 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.891514 iLCDirac-34.0.0a3/
--rw-rw-rw-   0 root         (0) root         (0)    32452 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1124 2022-12-13 11:40:29.892514 iLCDirac-34.0.0a3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      241 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      361 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)    79850 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/release.notes
--rw-rw-rw-   0 root         (0) root         (0)    27449 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/releases.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4370 2022-12-13 11:40:29.893514 iLCDirac-34.0.0a3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      276 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.794515 iLCDirac-34.0.0a3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.796515 iLCDirac-34.0.0a3/src/ILCDIRAC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.797515 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.798515 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    10978 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.798515 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     6343 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.799515 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)    36181 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    44494 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py
--rw-rw-rw-   0 root         (0) root         (0)     5951 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3971 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/TODO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.800515 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/
--rw-rw-rw-   0 root         (0) root         (0)    14462 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     2255 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py
--rw-rw-rw-   0 root         (0) root         (0)    51085 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)     9201 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.801515 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.804515 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/
--rw-rw-rw-   0 root         (0) root         (0)     3152 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1811 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig
--rw-rw-rw-   0 root         (0) root         (0)     2388 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     3967 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py
--rw-rw-rw-   0 root         (0) root         (0)     4968 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Helper_Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3579 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.805515 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/
--rw-rw-rw-   0 root         (0) root         (0)     1765 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt
--rw-rw-rw-   0 root         (0) root         (0)     3928 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml
--rw-rw-rw-   0 root         (0) root         (0)     1484 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)    12301 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/dev_create_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.805515 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.813515 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     3755 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py
--rw-rw-rw-   0 root         (0) root         (0)    14847 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/Configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    18781 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/DetectOS.py
--rw-rw-rw-   0 root         (0) root         (0)     4861 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/FileUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     9749 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py
--rw-rw-rw-   0 root         (0) root         (0)     2767 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py
--rw-rw-rw-   0 root         (0) root         (0)     4110 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/GeneratorModels.py
--rw-rw-rw-   0 root         (0) root         (0)    17917 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/HTML.py
--rw-rw-rw-   0 root         (0) root         (0)     6866 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/InputDataResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     4246 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5318 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/InstalledFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/JobPathResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     7040 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/MarlinXML.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/OverlayFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2856 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/PrepareLibs.py
--rw-rw-rw-   0 root         (0) root         (0)    32172 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     7483 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/ProcessList.py
--rw-rw-rw-   0 root         (0) root         (0)    11004 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/ProductionData.py
--rw-rw-rw-   0 root         (0) root         (0)     3993 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/RemoveSoft.py
--rw-rw-rw-   0 root         (0) root         (0)     2690 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/ResolveSE.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/Splitting.py
--rw-rw-rw-   0 root         (0) root         (0)    21977 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/TARsoft.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/WasteCPU.py
--rw-rw-rw-   0 root         (0) root         (0)    41912 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/WhizardOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1100 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6604 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.819515 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6226 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py
--rw-rw-rw-   0 root         (0) root         (0)    31722 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    23878 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py
--rw-rw-rw-   0 root         (0) root         (0)    17273 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py
--rw-rw-rw-   0 root         (0) root         (0)    16707 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py
--rw-rw-rw-   0 root         (0) root         (0)     4872 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py
--rw-rw-rw-   0 root         (0) root         (0)    10164 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     7506 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)    18959 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py
--rw-rw-rw-   0 root         (0) root         (0)    26585 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py
--rw-rw-rw-   0 root         (0) root         (0)    83044 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py
--rw-rw-rw-   0 root         (0) root         (0)    14816 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py
--rw-rw-rw-   0 root         (0) root         (0)     6220 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    11294 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py
--rw-rw-rw-   0 root         (0) root         (0)     9475 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py
--rw-rw-rw-   0 root         (0) root         (0)    72966 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py
--rw-rw-rw-   0 root         (0) root         (0)     3214 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py
--rw-rw-rw-   0 root         (0) root         (0)    26730 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.822515 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     3224 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     6151 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     6706 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     3200 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     2307 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh
--rwxrwxrwx   0 root         (0) root         (0)     9197 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac-architecture
--rw-rw-rw-   0 root         (0) root         (0)    15857 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py
--rw-rw-rw-   0 root         (0) root         (0)    10543 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py
--rw-rw-rw-   0 root         (0) root         (0)     9819 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py
--rw-rw-rw-   0 root         (0) root         (0)    16436 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py
--rw-rw-rw-   0 root         (0) root         (0)     1573 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.822515 iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.823515 iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/Agent/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.823515 iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/
--rw-rw-rw-   0 root         (0) root         (0)     5544 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.823515 iLCDirac-34.0.0a3/src/ILCDIRAC/FrameworkSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.824515 iLCDirac-34.0.0a3/src/ILCDIRAC/FrameworkSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       11 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/FrameworkSystem/ConfigTemplate.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/FrameworkSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.824515 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.825515 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    25777 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     9996 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     5395 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.825515 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     1934 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.827515 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/
--rw-rw-rw-   0 root         (0) root         (0)    35437 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    14308 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py
--rw-rw-rw-   0 root         (0) root         (0)    19604 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py
--rw-rw-rw-   0 root         (0) root         (0)    13782 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py
--rw-rw-rw-   0 root         (0) root         (0)    31158 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py
--rw-rw-rw-   0 root         (0) root         (0)     7554 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2889 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.828515 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     5456 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py
--rw-rw-rw-   0 root         (0) root         (0)     6462 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py
--rw-rw-rw-   0 root         (0) root         (0)     3204 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.831515 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49237 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py
--rw-rw-rw-   0 root         (0) root         (0)    45899 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py
--rw-rw-rw-   0 root         (0) root         (0)     3366 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    12482 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py
--rw-rw-rw-   0 root         (0) root         (0)     7314 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py
--rwxrwxrwx   0 root         (0) root         (0)     9954 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py
--rw-rw-rw-   0 root         (0) root         (0)     4673 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    16641 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     3536 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    12116 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.831515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.831515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/
--rw-rw-rw-   0 root         (0) root         (0)    13658 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/DiracILC.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.791515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.832515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/
--rw-rw-rw-   0 root         (0) root         (0)       77 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/alias.properties
--rw-rw-rw-   0 root         (0) root         (0)     1890 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py
--rw-rw-rw-   0 root         (0) root         (0)     9474 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml
--rw-rw-rw-   0 root         (0) root         (0)    10942 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.833515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/
--rw-rw-rw-   0 root         (0) root         (0)     1202 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.843515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/default.mac
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/defaultClicCrossingAngle.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      323 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      327 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      326 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_10gev_theta5-175.mac
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.843515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/
--rw-rw-rw-   0 root         (0) root         (0)     8759 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.846515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/
--rw-rw-rw-   0 root         (0) root         (0)    27099 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.854514 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/
--rw-rw-rw-   0 root         (0) root         (0)     3135 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     3757 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py
--rw-rw-rw-   0 root         (0) root         (0)    10462 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py
--rw-rw-rw-   0 root         (0) root         (0)    35946 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py
--rw-rw-rw-   0 root         (0) root         (0)     9311 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py
--rw-rw-rw-   0 root         (0) root         (0)     6521 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     3885 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)     6140 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py
--rw-rw-rw-   0 root         (0) root         (0)    10161 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py
--rw-rw-rw-   0 root         (0) root         (0)     8281 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py
--rw-rw-rw-   0 root         (0) root         (0)    16303 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     3918 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)     3312 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py
--rw-rw-rw-   0 root         (0) root         (0)     2090 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py
--rw-rw-rw-   0 root         (0) root         (0)     2461 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py
--rw-rw-rw-   0 root         (0) root         (0)     3752 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6174 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py
--rw-rw-rw-   0 root         (0) root         (0)     6089 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py
--rw-rw-rw-   0 root         (0) root         (0)     5479 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6957 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py
--rw-rw-rw-   0 root         (0) root         (0)    17277 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12788 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py
--rw-rw-rw-   0 root         (0) root         (0)     4441 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py
--rw-rw-rw-   0 root         (0) root         (0)     4876 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.856515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/
--rw-rw-rw-   0 root         (0) root         (0)     2831 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py
--rw-rw-rw-   0 root         (0) root         (0)     2665 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py
--rw-rw-rw-   0 root         (0) root         (0)    19613 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py
--rw-rw-rw-   0 root         (0) root         (0)    22228 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py
--rw-rw-rw-   0 root         (0) root         (0)     2834 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py
--rw-rw-rw-   0 root         (0) root         (0)     4247 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py
--rw-rw-rw-   0 root         (0) root         (0)     9857 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    24484 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py
--rw-rw-rw-   0 root         (0) root         (0)    26292 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py
--rw-rw-rw-   0 root         (0) root         (0)    15111 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py
--rw-rw-rw-   0 root         (0) root         (0)    37308 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.857514 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/
--rw-rw-rw-   0 root         (0) root         (0)    27996 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    29727 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py
--rwxrwxrwx   0 root         (0) root         (0)    35679 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py
--rw-rw-rw-   0 root         (0) root         (0)    13124 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    12330 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.865514 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/
--rw-rw-rw-   0 root         (0) root         (0)     7876 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2878 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py
--rw-rw-rw-   0 root         (0) root         (0)    18299 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py
--rw-rw-rw-   0 root         (0) root         (0)    41414 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py
--rw-rw-rw-   0 root         (0) root         (0)     5930 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     4218 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)    13745 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py
--rw-rw-rw-   0 root         (0) root         (0)     7579 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py
--rw-rw-rw-   0 root         (0) root         (0)    12305 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py
--rw-rw-rw-   0 root         (0) root         (0)     8309 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py
--rw-rw-rw-   0 root         (0) root         (0)     6492 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py
--rw-rw-rw-   0 root         (0) root         (0)    14537 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     4767 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)    65340 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py
--rw-rw-rw-   0 root         (0) root         (0)     4830 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     4798 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6232 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py
--rw-rw-rw-   0 root         (0) root         (0)     7551 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py
--rw-rw-rw-   0 root         (0) root         (0)     5077 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6829 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     4763 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py
--rw-rw-rw-   0 root         (0) root         (0)    22726 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py
--rw-rw-rw-   0 root         (0) root         (0)    20865 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py
--rw-rw-rw-   0 root         (0) root         (0)    13044 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py
--rw-rw-rw-   0 root         (0) root         (0)     4169 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9860 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.865514 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Test/
--rw-rw-rw-   0 root         (0) root         (0)    20440 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.865514 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Tests/
--rw-rw-rw-   0 root         (0) root         (0)     2622 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.866515 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     4727 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py
--rw-rw-rw-   0 root         (0) root         (0)    15312 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.868514 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2968 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7808 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py
--rw-rw-rw-   0 root         (0) root         (0)     3538 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3088 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py
--rw-rw-rw-   0 root         (0) root         (0)     2396 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py
--rwxrwxrwx   0 root         (0) root         (0)     3724 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.868514 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.868514 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     2638 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.869515 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     1399 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.869515 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/DB/
--rw-rw-rw-   0 root         (0) root         (0)     6376 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.870514 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/DB/Test/
--rw-rw-rw-   0 root         (0) root         (0)     9281 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.870514 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)     2462 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.870514 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.880514 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/
--rw-rw-rw-   0 root         (0) root         (0)     4515 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py
--rw-rw-rw-   0 root         (0) root         (0)     5524 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py
--rw-rw-rw-   0 root         (0) root         (0)    23026 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     5789 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py
--rw-rw-rw-   0 root         (0) root         (0)     3146 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    16673 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/DummyModule.py
--rw-rw-rw-   0 root         (0) root         (0)     6809 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py
--rw-rw-rw-   0 root         (0) root         (0)    19926 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     8224 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)     4454 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)     6156 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     6801 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5057 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     8078 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)    13096 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18950 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    31351 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)    26082 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5266 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/MoveInFC.py
--rw-rw-rw-   0 root         (0) root         (0)    33871 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     7960 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)     8182 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5743 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ReportErrors.py
--rw-rw-rw-   0 root         (0) root         (0)     5915 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5740 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    11639 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4044 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py
--rw-rw-rw-   0 root         (0) root         (0)     9340 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/StdHepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     3020 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.886514 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/
--rw-rw-rw-   0 root         (0) root         (0)     2304 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py
--rw-rw-rw-   0 root         (0) root         (0)    14814 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)    44092 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py
--rw-rw-rw-   0 root         (0) root         (0)    28578 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    10005 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    45397 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    43848 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)    41500 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)    10867 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py
--rw-rw-rw-   0 root         (0) root         (0)     8844 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    28021 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py
--rw-rw-rw-   0 root         (0) root         (0)    19461 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py
--rw-rw-rw-   0 root         (0) root         (0)    14457 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)    12973 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py
--rw-rw-rw-   0 root         (0) root         (0)    10007 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    32143 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py
--rw-rw-rw-   0 root         (0) root         (0)    14235 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    67243 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    86486 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py
--rw-rw-rw-   0 root         (0) root         (0)     6505 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    17704 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py
--rw-rw-rw-   0 root         (0) root         (0)    15076 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    17792 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py
--rw-rw-rw-   0 root         (0) root         (0)     9795 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    22938 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.887514 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     3265 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4526 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Utilities/RootMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.887514 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.888514 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    24455 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.888514 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)    15894 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.889514 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Executor/
--rw-rw-rw-   0 root         (0) root         (0)     5646 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.889514 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Tests/
--rw-rw-rw-   0 root         (0) root         (0)    13587 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py
--rw-rw-rw-   0 root         (0) root         (0)    31624 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     3345 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-13 11:40:08.000000 iLCDirac-34.0.0a3/src/ILCDIRAC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 11:40:29.891514 iLCDirac-34.0.0a3/src/iLCDirac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1124 2022-12-13 11:40:29.000000 iLCDirac-34.0.0a3/src/iLCDirac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24161 2022-12-13 11:40:29.000000 iLCDirac-34.0.0a3/src/iLCDirac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 11:40:29.000000 iLCDirac-34.0.0a3/src/iLCDirac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2121 2022-12-13 11:40:29.000000 iLCDirac-34.0.0a3/src/iLCDirac.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 11:40:28.000000 iLCDirac-34.0.0a3/src/iLCDirac.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      279 2022-12-13 11:40:29.000000 iLCDirac-34.0.0a3/src/iLCDirac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-12-13 11:40:29.000000 iLCDirac-34.0.0a3/src/iLCDirac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.331254 iLCDirac-34.0.0a4/
+-rw-rw-rw-   0 root         (0) root         (0)    32452 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-05-29 13:18:57.332254 iLCDirac-34.0.0a4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)    82539 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/release.notes
+-rw-rw-rw-   0 root         (0) root         (0)    27753 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/releases.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2023-05-29 13:18:57.333254 iLCDirac-34.0.0a4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.223255 iLCDirac-34.0.0a4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.226255 iLCDirac-34.0.0a4/src/ILCDIRAC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.227254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.227254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    10978 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.228254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.229254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)    36181 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    44494 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py
+-rw-rw-rw-   0 root         (0) root         (0)     5951 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/TODO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.230255 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/
+-rw-rw-rw-   0 root         (0) root         (0)    14462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    51085 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9201 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.232254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.235254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     3152 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     3967 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py
+-rw-rw-rw-   0 root         (0) root         (0)     4968 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Helper_Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.235254 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3928 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12301 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/dev_create_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.236254 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.243254 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     3755 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py
+-rw-rw-rw-   0 root         (0) root         (0)    15006 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    18781 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/DetectOS.py
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FileUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9749 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2767 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py
+-rw-rw-rw-   0 root         (0) root         (0)     4110 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/GeneratorModels.py
+-rw-rw-rw-   0 root         (0) root         (0)    17917 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/HTML.py
+-rw-rw-rw-   0 root         (0) root         (0)     6866 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InputDataResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5506 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InstalledFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/JobPathResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     7040 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/MarlinXML.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/OverlayFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/PrepareLibs.py
+-rw-rw-rw-   0 root         (0) root         (0)    34638 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     7483 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ProcessList.py
+-rw-rw-rw-   0 root         (0) root         (0)    11004 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ProductionData.py
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/RemoveSoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ResolveSE.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Splitting.py
+-rw-rw-rw-   0 root         (0) root         (0)    21977 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/TARsoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/WasteCPU.py
+-rw-rw-rw-   0 root         (0) root         (0)    41912 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/WhizardOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6604 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.250254 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py
+-rw-rw-rw-   0 root         (0) root         (0)    31722 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    23878 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py
+-rw-rw-rw-   0 root         (0) root         (0)    17273 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16707 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py
+-rw-rw-rw-   0 root         (0) root         (0)    10164 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18959 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py
+-rw-rw-rw-   0 root         (0) root         (0)    26585 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py
+-rw-rw-rw-   0 root         (0) root         (0)    84519 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)    14816 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py
+-rw-rw-rw-   0 root         (0) root         (0)     6220 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    11294 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py
+-rw-rw-rw-   0 root         (0) root         (0)     9475 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py
+-rw-rw-rw-   0 root         (0) root         (0)    72966 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py
+-rw-rw-rw-   0 root         (0) root         (0)    26730 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.254254 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3224 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     6151 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     6706 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3200 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2307 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh
+-rwxrwxrwx   0 root         (0) root         (0)     9197 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac-architecture
+-rw-rw-rw-   0 root         (0) root         (0)    15857 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py
+-rw-rw-rw-   0 root         (0) root         (0)    10543 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     9819 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    16436 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.254254 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.254254 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.255254 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/
+-rw-rw-rw-   0 root         (0) root         (0)     5544 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.255254 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.255254 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/ConfigTemplate.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.256254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.257254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    25777 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     9996 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     5395 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.257254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.259254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)    35437 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    14308 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)    19604 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13782 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    30921 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7554 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.260254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     5456 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.264254 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49360 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py
+-rw-rw-rw-   0 root         (0) root         (0)    48013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6228 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12482 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     7314 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py
+-rwxrwxrwx   0 root         (0) root         (0)     9954 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py
+-rw-rw-rw-   0 root         (0) root         (0)     4673 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    16641 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12116 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.264254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.264254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/
+-rw-rw-rw-   0 root         (0) root         (0)    13833 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/DiracILC.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.219255 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.265254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/alias.properties
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py
+-rw-rw-rw-   0 root         (0) root         (0)     9474 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml
+-rw-rw-rw-   0 root         (0) root         (0)    10942 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.266254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.277254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/default.mac
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/defaultClicCrossingAngle.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_10gev_theta5-175.mac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.278254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/
+-rw-rw-rw-   0 root         (0) root         (0)     8759 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.280254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/
+-rw-rw-rw-   0 root         (0) root         (0)    27099 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.288254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py
+-rw-rw-rw-   0 root         (0) root         (0)     9579 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py
+-rw-rw-rw-   0 root         (0) root         (0)    35946 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py
+-rw-rw-rw-   0 root         (0) root         (0)    12520 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6521 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6140 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py
+-rw-rw-rw-   0 root         (0) root         (0)    10161 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8281 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py
+-rw-rw-rw-   0 root         (0) root         (0)    16303 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     3918 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py
+-rw-rw-rw-   0 root         (0) root         (0)     2090 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py
+-rw-rw-rw-   0 root         (0) root         (0)     3752 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)     5479 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6957 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py
+-rw-rw-rw-   0 root         (0) root         (0)    17277 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12788 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py
+-rw-rw-rw-   0 root         (0) root         (0)     4984 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.290254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py
+-rw-rw-rw-   0 root         (0) root         (0)     2665 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    19613 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py
+-rw-rw-rw-   0 root         (0) root         (0)    22228 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4247 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py
+-rw-rw-rw-   0 root         (0) root         (0)     9857 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    24484 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py
+-rw-rw-rw-   0 root         (0) root         (0)    26292 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py
+-rw-rw-rw-   0 root         (0) root         (0)    15111 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3097 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)    40172 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.291254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/
+-rw-rw-rw-   0 root         (0) root         (0)    27996 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    29727 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py
+-rwxrwxrwx   0 root         (0) root         (0)    35679 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py
+-rw-rw-rw-   0 root         (0) root         (0)    13124 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    12330 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.300254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7876 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18299 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py
+-rw-rw-rw-   0 root         (0) root         (0)    15439 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py
+-rw-rw-rw-   0 root         (0) root         (0)    41414 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15264 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     4218 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    13745 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py
+-rw-rw-rw-   0 root         (0) root         (0)     7579 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py
+-rw-rw-rw-   0 root         (0) root         (0)    12305 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py
+-rw-rw-rw-   0 root         (0) root         (0)     8309 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6492 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py
+-rw-rw-rw-   0 root         (0) root         (0)    14537 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     4767 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)    71676 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4798 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py
+-rw-rw-rw-   0 root         (0) root         (0)     7551 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6829 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     4763 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py
+-rw-rw-rw-   0 root         (0) root         (0)    22726 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py
+-rw-rw-rw-   0 root         (0) root         (0)    20865 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13044 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4169 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9860 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.300254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Test/
+-rw-rw-rw-   0 root         (0) root         (0)    20190 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.300254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.301254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15312 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.303254 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2968 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7808 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py
+-rw-rw-rw-   0 root         (0) root         (0)     3538 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     2636 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2396 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     3724 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.304254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.304254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.305254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.305254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/
+-rw-rw-rw-   0 root         (0) root         (0)     6376 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.306254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/Test/
+-rw-rw-rw-   0 root         (0) root         (0)     9281 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.306254 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.306254 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.318254 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/
+-rw-rw-rw-   0 root         (0) root         (0)     4515 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py
+-rw-rw-rw-   0 root         (0) root         (0)    23026 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5789 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py
+-rw-rw-rw-   0 root         (0) root         (0)     3146 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    16673 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8009 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DummyModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     6809 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)    19926 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8774 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     4454 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6156 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     6801 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5057 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8078 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)    13096 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18950 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    31351 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    26082 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5266 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MoveInFC.py
+-rw-rw-rw-   0 root         (0) root         (0)    33871 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     7960 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8182 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5743 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ReportErrors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5915 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5740 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    11639 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4044 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9340 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     3020 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.325254 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)    14814 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)    44092 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    18662 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)    28578 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    20599 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)    10005 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    45397 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    43848 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    41500 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)    10867 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8844 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    28021 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)    19461 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)    14457 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)    12973 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    10007 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    32143 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py
+-rw-rw-rw-   0 root         (0) root         (0)    14235 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    67243 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    86847 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py
+-rw-rw-rw-   0 root         (0) root         (0)     6505 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    17704 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    15076 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    17792 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py
+-rw-rw-rw-   0 root         (0) root         (0)     9795 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    22938 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.326254 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     3265 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/RootMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.327254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.327254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    24455 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.328254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)    15894 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.329254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.329254 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13587 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    31624 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3345 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2023-05-29 13:18:33.000000 iLCDirac-34.0.0a4/src/ILCDIRAC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:18:57.331254 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24527 2023-05-29 13:18:57.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      279 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-29 13:18:56.000000 iLCDirac-34.0.0a4/src/iLCDirac.egg-info/top_level.txt
```

### Comparing `iLCDirac-34.0.0a3/LICENSE` & `iLCDirac-34.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/PKG-INFO` & `iLCDirac-34.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iLCDirac
-Version: 34.0.0a3
+Version: 34.0.0a4
 Summary: iLCDirac is the iLC/CLIC/FCC extension of DIRAC
 Home-page: https://gitlab.cern.ch/clicdp/ilcdirac/ilcdirac.git
 Maintainer: Andre Sailer
 Maintainer-email: ilcdirac-support@cern.ch
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://its.cern.ch/jira/browse/ILCDIRAC
 Project-URL: Documentation, https://ilcdirac-doc.web.cern.ch/
```

### Comparing `iLCDirac-34.0.0a3/release.notes` & `iLCDirac-34.0.0a4/release.notes`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,95 @@
+[v34r0]
+Release date: 2023-05-26
+
+*Core
+
+NEW: Depend on DIRAC version 7.3
+NEW: Python3 only
+NEW: (!430) Implementation of the Delphes Application interface.
+NEW: (!430) Addition of some functionalities to the Gaudi Application interface.
+NEW: (!430) Correct paths for storing FCC simulations outputs.
+FIX: (!421) client installation: corrected (a typo in) the URL of the configuration service, fixes problems during dirac-configure.
+
+[v32r0p3]
+Release date: 2021-11-18
+
+*Core
+NEW: Based on Dirac v7r2p34
+CHANGE: (!401) resolvePathsAndNames: fixes when ProductionOutputData contains a semicolon
+CHANGE: (!401) resolvePathsAndNames: be more lenient in terms of file extensions, anything outputfile with a dot in it should work now
+CHANGE: (!402) UploadOutputData: make it more configurable with Operations/Productions/ExtensionToFiletypes parameter
+NEW: (!382) dirac-ilc-add-cvmfs-software: also add detectors from FCCDetectors to the CS
+
+*Interfaces
+
+CHANGE: (!401) ProductionJob: add some treatment for FCC production creation
+
+*Workflow
+
+CHANGE: (!401) KKMC: Add treatment for ProductionOutputData
+CHANGE: (!401) KKMC: If production outputdata changes the outputfile name, keep a copy of the original filename
+CHANGE: (!402) KKMC: always copy outputfile to events.lhe
+CHANGE: (!403) Also run injectJobIndex when running jobs in mode=local, for testing
+FIX: (!403) Fix the use of %n to inject the job index at an arbitrary location
+FIX: (!397) Allow running GaudiApplication when not setting a detectorModel
+
+
+[v32r0p2]
+Release date: 2021-08-17
+
+*ILCTransformationSystem
+
+FIX: (!393) Fix setting the input data query for created transformations
+CHANGE: (!393) ``ProductionJob.createProduction`` now returns the transformation object in the return S_OK
+
+
+[v32r0p1]
+Release date: 2021-08-06
+
+*Interfaces
+
+NEW: (!386) New application, ``GaudiApp``, to run, for example, the Key4hep ``k4run``
+
+*Workflow
+
+FIX: (!387) Fix for ``GenericApplication`` when no setup script is set, fixes ILCDIRAC-971
+FIX: (!388) ``ModuleBase`` Fix exception in redirectLogOutput when program output contains Unicode characters., Fixes ILCDIRAC-972
+
+[v32r0]
+Release date: 2021-07-28
+
+*Core
+
+NEW: Based on Dirac v7r2p16
+
+*ILCTransformationSystem
+
+CHANGE: (!376) Use the changed way of creating and retrieving InputDataQuery
+CHANGE: (!380) The DataRecoveryAgent and related tools have been moved to DIRAC
+
+*Interfaces
+
+CHANGE: (!376) Remove the ``ProductionJob.applyInputDataQuery`` function.
+
+[v31r0p1]
+Release date: 2021-04-14
+
+*Core
+
+NEW: Based on Dirac v7r1p36
+
+*Docs
+
+FIX: (!374) Fix commands for installing iLCDirac client
+
+*Interfaces
+
+NEW: (!373) GenericApplication: Added possibility to source shell script
+
 [v31r0]
 Release date: 2021-03-23
 
 *Core
 
 NEW: Based on Dirac v7r1p34
```

### Comparing `iLCDirac-34.0.0a3/releases.cfg` & `iLCDirac-34.0.0a4/releases.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,34 @@
 
 Sources
 {
   ILCDIRAC = https://gitlab.cern.ch/CLICdp/iLCDirac/ILCDIRAC.git
 }
 Releases
 {
+  v32r0p3
+  {
+    Modules = ILCDIRAC:v32r0p3
+    Depends = DIRAC:v7r2p34
+  }
+  v32r0p2
+  {
+    Modules = ILCDIRAC:v32r0p2
+    Depends = DIRAC:v7r2p16
+  }
+  v32r0p1
+  {
+    Modules = ILCDIRAC:v32r0p1
+    Depends = DIRAC:v7r2p16
+  }
+  v32r0
+  {
+    Modules = ILCDIRAC:v32r0
+    Depends = DIRAC:v7r2p16
+  }
   v31r0
   {
     Modules = ILCDIRAC:v31r0
     Depends = DIRAC:v7r1p34
   }
   v29r2p6
   {
```

### Comparing `iLCDirac-34.0.0a3/setup.cfg` & `iLCDirac-34.0.0a4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [options]
 python_requires = >=3.9
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	DIRAC == 7.3.34
+	DIRAC == 7.3.36
 	requests
 	six
 zip_safe = False
 include_package_data = True
 
 [options.package_data]
 * = ConfigTemplate.cfg, *.sql
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Client/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Service/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/TODO` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/TODO`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Test/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Test/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/CalibrationSystem/dev_create_events.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/CalibrationSystem/dev_create_events.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,14 +382,21 @@
 
   :param str platform: platform
   :param app: tuple off application name and version
   :type app: ``tuple``
   :returns: S_OK of tuple of path and environmen stript
   """
   name, version = app
+
+  software_redirections = {'delphesapp': 'gaudiapp',
+                          }
+  if name in software_redirections:
+    name = software_redirections[name]
+
+
   csPath = "/AvailableTarBalls/%s/%s/%s" % (platform, name, version)
   cvmfspath = Operations().getValue(csPath + "/CVMFSPath", "")
   envScript = Operations().getValue(csPath + "/CVMFSEnvScript", "")
   if cvmfspath and os.path.exists(cvmfspath):
     return S_OK((cvmfspath, envScript))
   message = "Package %s version %s not found natively on cvmfs," % (name, version)
   LOG.info(message + " will try to use shared area instead: " + str(Operations().getOptionsDict(csPath)))
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/Configuration.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Configuration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/DetectOS.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/DetectOS.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/FileUtils.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FileUtils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/GeneratorModels.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/GeneratorModels.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/HTML.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/HTML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/InputDataResolution.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/InstalledFiles.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/InstalledFiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,20 @@
            "sidloi3_trackingStrategies.xml",
            "sidloi3_trackingStrategies_default.xml",
            "ild_00.gear",
            "ild_00_steering.xml",
            "ild_00.steer",
            "cuts_quarks_1400.txt", "cuts_taus_1400.txt",
            "cuts_h_gammaZ_1400.txt", "cuts_h_gammagamma_1400.txt",
-           "cuts_h_mumu_3000.txt", ]
+           "cuts_h_mumu_3000.txt", 
+           "delphes_card_IDEA.tcl", "edm4hep_output_config.tcl",
+           "geant_fullsim_fccee_lar_pgun.py", 
+           "k4simdelphesalg_pythia.py",
+           "pythia.py",
+           ]
   if myfile in files:
     return S_OK()
   elif configversion is None or platform is None:
     return S_ERROR("File %s is not available locally nor in the software installation." % myfile)
   else:
     return _checkInCVMFS(myfile, platform, configversion)
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/JobPathResolution.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/JobPathResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/MarlinXML.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/MarlinXML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/OverlayFiles.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/OverlayFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/PrepareLibs.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/PrepareLibs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -814,7 +814,54 @@
           if collection and subparam.attrib['name'] == 'MCCollectionName':
             com = Comment('Collections to analyse changed')
             param.insert(0, com)
             subparam.text = collection
 
   tree.write(outputxml)
   return S_OK()
+
+def preparePythia8Card(pythia8CardContent, NumberOfEvents, randomSeed, pythia8Card=None):
+  """Make the pythiacard file, using the string read in input. Edit it with the correct parameters of the task."""
+  
+  lines = pythia8CardContent.splitlines(keepends=True)
+
+  for i, line in enumerate(lines):
+    if line.lstrip().startswith('Beams:LHEF'):
+      LOG.info('Field `Beams:LHEF` found in your pythia card, Assuming it is a pythia card for reading LHE.')
+      card = 'reader'
+      break
+    elif line.replace(" ", "").startswith('Beams:eCM'):
+      LOG.info('Field `Beams:eCM` found in your pythia card, Assuming it is a pythia card for generating new events.')
+      card = 'generator'
+      break
+  else:
+    LOG.error('Pythia card with unusual content: neither `Beams:LHEF` nor `Beams:eCM` fields present. Please check the content of your card.')
+    return S_ERROR('Pythia card with unusual content: neither `Beams:LHEF` nor `Beams:eCM` fields present. Please check the content of your card.')
+  
+  modifiedEventNumber = False
+  for i, line in enumerate(lines):
+    if line.lstrip().startswith('Main:numberOfEvents'):
+      lines[i] = f'Main:numberOfEvents = {NumberOfEvents}'+' '*(13-len(str(NumberOfEvents)))+'! number of events to generate\n'
+      modifiedEventNumber = True
+  if not modifiedEventNumber:
+    LOG.error('Not found any line in the pythia card for setting the number of events')
+    return S_ERROR('Not found any line in the pythia card for setting the number of events')
+  
+  modifiedEventNumber = False
+  for i, line in enumerate(lines):
+    # setting seed instructions: https://pythia.org/latest-manual/RandomNumberSeed.html
+    if line.lstrip().startswith('Random:setSeed'): 
+      lines[i] = f'Random:setSeed = on\n'
+      lines.insert(i+1, f'Random:seed = {randomSeed}\n')
+      modifiedEventNumber = True
+  if not modifiedEventNumber:
+    if card == 'reader':
+      LOG.info('Not found any line for setting the seed in your pythia card. That is fine, since your card appears to be a LHE reader.')
+    elif card == 'generator':
+      LOG.info('Not found any line for setting the seed in your pythia card. Your card appears to be used for generation: I will add two lines for setting the seed by myself in the pythia card.')
+      lines.insert(0, f'Random:seed = {randomSeed}\n')
+      lines.insert(0, f'Random:setSeed = on\n')
+    
+  if pythia8Card:
+    with open(pythia8Card, 'w') as f:
+      f.writelines(lines)    
+  return S_OK()
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/ProcessList.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ProcessList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/ProductionData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ProductionData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/RemoveSoft.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/RemoveSoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/ResolveSE.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/ResolveSE.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/Splitting.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Splitting.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/TARsoft.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/TARsoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/Utilities.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/WasteCPU.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/WasteCPU.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/WhizardOptions.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/WhizardOptions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import unittest
 import os
 import filecmp
 import copy
 import collections
 import xml.etree.ElementTree as ET
 from mock import mock_open, patch, MagicMock as Mock
+from parameterized import parameterized
 
 from DIRAC import S_OK, S_ERROR
 from ILCDIRAC.Core.Utilities import PrepareOptionFiles
 from ILCDIRAC.Core.Utilities.PrepareOptionFiles import prepareMacFile
 from Tests.Utilities.FileUtils import FileUtil
 from Tests.Utilities.GeneralUtils import assertEqualsXml, \
     assertEqualsImproved, assertDiracFailsWith, assertDiracSucceeds, \
@@ -1345,14 +1346,38 @@
       expected_element.text = 'inputslcio'
       assertEqualsXml(current_tree.findall('global/parameter')[-1],
                       expected_element, self)
       expected_tuples = [('default.xml', 'w')]
       FileUtil.checkFileInteractions(self, mo, expected_tuples, expected,
                                       handles)
 
+  @parameterized.expand([('ciao\n', 'Pythia card with unusual content: neither `Beams:LHEF` nor `Beams:eCM` fields present. Please check the content of your card.'),
+                         ('Beams:LHEF\n', 'Not found any line in the pythia card for setting the number of events'),
+                         ('Beams:LHEF\nMain:numberOfEvents', None),
+                         ('Beams:LHEF\nMain:numberOfEvents\nRandom:setSeed', None),
+                         ('Beams:eCM\n', 'Not found any line in the pythia card for setting the number of events'),
+                         ('Beams:eCM\nMain:numberOfEvents', None),
+                         ('Beams:eCM\nMain:numberOfEvents\nRandom:setSeed', None)])
+  def test_preparePythia8Card(self, cardcontent, outmessage):
+    randomSeed = 12345
+    pythia8CardContent = cardcontent
+    pythia8Card = 'pythia8Card'
+    NumberOfEvents = 1234000
+    res = PrepareOptionFiles.preparePythia8Card(pythia8CardContent, NumberOfEvents, randomSeed, pythia8Card)
+    if outmessage:
+      self.assertEqual(outmessage, res['Message'])
+    else:
+      self.assertEqual(outmessage, res['Value'])
+
+  def test_preparePythia8Card_nofilename(self):
+    randomSeed = 12345
+    pythia8CardContent = 'Beams:eCM\nMain:numberOfEvents\nRandom:setSeed'
+    NumberOfEvents = 1234000
+    res = PrepareOptionFiles.preparePythia8Card(pythia8CardContent, NumberOfEvents, randomSeed)
+    self.assertEqual(None, res['Value'])
 
 def createXMLTreeForXML(flag=0):
   """Creates a XML Tree to test prepareXMLFile()"""
   root = ET.Element("root")
   ex = ET.SubElement(root, 'execute')
   ET.SubElement(ex, 'processor', name='MYOVERLAYTIMING', type='OverlayTiming')
   ET.SubElement(ex, 'processor', name='BGoverlAY', type='Overlay')
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac-architecture` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac-architecture`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/DataManagementSystem/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/DataManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/FrameworkSystem/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/FrameworkSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
               }
     for opName, value in opsDict.items():
       if args[0].endswith(opName):
         return value
     assert args[0] == opsDict
     return None
   theOps = Mock(name='OpsMock')
-  theOps.getValue = mockOpsConfig
+  theOps.getValue = Mock(side_effect=mockOpsConfig)
   return theOps
 
 
 @pytest.fixture
 def pMockMod():
   """Return Module for ProductionJob."""
   pMockMod = Mock()
@@ -122,15 +122,15 @@
 def theChain(opsMock):
   """Return production chain fixture."""
   params = Mock()
   params.additionalName = ''
   params.dryRun = True
   with patch("ILCDIRAC.ILCTransformationSystem.scripts.dirac_clic_make_productions.CLICDetProdChain.loadParameters",
              new=Mock()), \
-       patch("DIRAC.ConfigurationSystem.Client.Helpers.Operations.Operations",
+       patch("ILCDIRAC.ILCTransformationSystem.scripts.dirac_clic_make_productions.Operations",
              new=Mock(return_value=opsMock)):
     chain = theScript.CLICDetProdChain(params)
 
   return chain
 
 
 @pytest.fixture
@@ -277,44 +277,40 @@
   assert isinstance(ret, Marlin)
   assert ret.detectortype == 'myDetectorModel'
   assert ret.steeringFile == 'clicReconstruction.xml'
   assert theChain.cliRecoOption == '--Config.Tracking=Tracked'
   assert ret.extraCLIArguments == '--Config.Tracking=Tracked'
 
 
-def test_createWhizard2Application(theChain, aTask, cpMock, opsMock):
+def test_createWhizard2Application(theChain, aTask, cpMock):
   """Test creating the whizard2 application."""
   from ILCDIRAC.Interfaces.API.NewInterface.Applications import Whizard2
 
   parameter = Mock(name="ParameterMock")
   parameter.whizard2SinFile = 'filename'
   parameter.dumpConfigFile = False
-  with patch(SCP, new=Mock(return_value=cpMock)), \
-       patch("DIRAC.ConfigurationSystem.Client.Helpers.Operations.Operations",
-             new=Mock(return_value=opsMock)):
+  with patch(SCP, new=Mock(return_value=cpMock)):
     theChain.loadParameters(parameter)
 
   aTask.meta = {'ProdID': '123', 'EvtType': 'process', 'Energy': '555', 'Machine': 'clic'}
   aTask.eventsPerJob = 100
   aTask.genFile = 'sinFile'
 
   ret = theChain.createWhizard2Application(aTask)
   assert isinstance(ret, Whizard2)
   assert ret.version == 'myWhizardVersion'
 
 
-def test_createDDSimApplication(theChain, aTask, cpMock, opsMock):
+def test_createDDSimApplication(theChain, aTask, cpMock):
   """Test creating the ddsim application."""
   from ILCDIRAC.Interfaces.API.NewInterface.Applications import DDSim
   parameter = Mock()
   parameter.prodConfigFilename = 'filename'
   parameter.dumpConfigFile = False
-  with patch(SCP, new=Mock(return_value=cpMock)), \
-       patch("DIRAC.ConfigurationSystem.Client.Helpers.Operations.Operations",
-             new=Mock(return_value=opsMock)):
+  with patch(SCP, new=Mock(return_value=cpMock)):
     theChain.loadParameters(parameter)
 
   ret = theChain.createDDSimApplication(aTask)
   assert isinstance(ret, DDSim)
   assert ret.steeringFile == 'clic_steer.py'
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,20 @@
                      'detectorModel',
                      'softwareVersion',
                      'overlayEvents',
                      'overlayEventType',
                      ]
 
 
+def Operations(vo=None):
+  """Load Operations class after initialisation, and allow mocking."""
+  from DIRAC.ConfigurationSystem.Client.Helpers.Operations import Operations
+  return Operations(vo=vo)
+
+
 class _Params(object):
   """Parameter Object."""
 
   def __init__(self):
     self.prodConfigFilename = None
     self.dumpConfigFile = False
     self.dryRun = True
@@ -362,15 +368,14 @@
       """load flags values from configfile."""
       self.__splitStringToOptions(config, self._prodTypes, 'ProdTypes', prefix='_')
       self.__splitStringToOptions(config, self._moveTypes, 'MoveTypes', prefix='_')
       self._moves = config.getboolean(PP, 'move')
 
   def __init__(self, params=None, group='ilc_prod'):
 
-    from DIRAC.ConfigurationSystem.Client.Helpers.Operations import Operations
     self._ops = Operations(vo='ilc')
 
     self._machine = {'ilc_prod': 'clic',
                      'fcc_prod': 'fccee',
                      }[group]
 
     self.overlayEventType = {'ilc_prod': 'gghad',
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 from ILCDIRAC.Core.Utilities.Utilities import listify, lowerFirst
 from ILCDIRAC.ILCTransformationSystem.Utilities.Utilities import Task
 import six
 from six.moves import zip_longest
 
 PRODUCTION_PARAMETERS = 'Production Parameters'
 PP = PRODUCTION_PARAMETERS
-APPLICATION_LIST = ['Marlin', 'DDSim', 'Overlay', 'Whizard2', 'KKMC']
+APPLICATION_LIST = ['Marlin', 'DDSim', 'Overlay', 'Whizard2', 'KKMC', 'delphesapp', 'gaudiapp']
 LIST_ATTRIBUTES = ['ignoreMetadata',
                    'generatorSteeringFile',
                    'energies',
                    'eventsPerJobs',
                    'numberOfTasks',
                    'processes',
                    'prodIDs',
@@ -196,16 +196,21 @@
                      'MoveGroupSize',
                      'prodGroup',
                      'machine',
                      'detectorModel',
                      'softwareVersion',
                      'overlayEvents',
                      'overlayEventType',
+                     'campaign',
+                     'datatype',
+                     'processingAfterGen',
                      ]
 
+BOOL_ATTRIBUTES = [
+                   ]
 
 class _Params(object):
   """Parameter Object."""
 
   def __init__(self):
     self.prodConfigFilename = None
     self.dumpConfigFile = False
@@ -371,15 +376,15 @@
 
     def loadFlags(self, config):
       """load flags values from configfile."""
       self.__splitStringToOptions(config, self._prodTypes, 'ProdTypes', prefix='_')
       self.__splitStringToOptions(config, self._moveTypes, 'MoveTypes', prefix='_')
       self._moves = config.getboolean(PP, 'move')
 
-  def __init__(self, params=None, group='ilc_prod'):
+  def __init__(self, params=None, group='fcc_prod'):
 
     from DIRAC.ConfigurationSystem.Client.Helpers.Operations import Operations
     self._ops = Operations(group=group)
 
     self.machine = {'ilc_prod': 'clic',
                     'fcc_prod': 'fccee',
                     }[group]
@@ -415,16 +420,20 @@
 
     self.overlayEvents = ''
 
     self.cliRecoOption = ''
     self.cliReco = ''
 
     self.generatorApplication = 'whizard2'
-    self.generatorVersion = None
+    self.generatorVersion = 'key4hep-latest'
     self.generatorSteeringFile = []
+    self.processingAfterGen = ''
+
+    self.datatype = ''
+    self.campaign = ''
 
     self.simApplication = 'ddsim'
     self.simVersion = None
     self.simSteeringFile = 'clic_steer.py'
 
     self.recoApplication = 'Marlin'
     self.recoVersion = None
@@ -443,15 +452,15 @@
 
   @property
   def basepath(self):
     """Return the basepath"""
     if not self._basepath:
       prodPath = os.path.join('/Production', self.machine.upper())
       self._basepath = self._ops.getValue(os.path.join(prodPath, 'BasePath'))
-    return self._basepath
+    return os.path.join(self._basepath, self.campaign) + '/'
   
   def meta(self, prodID, process, energy):
     """return meta data dictionary, always new."""
     metaD = {'ProdID': str(prodID),
              'EvtType': process,
              'Energy': self.metaEnergy(energy),
              'Machine': self.machine,
@@ -460,27 +469,31 @@
       metaD.pop(key)
     return metaD
 
   def loadParameters(self, parameter):
     """Load parameters from config file."""
     if parameter.prodConfigFilename is not None:
       defaultValueDict = vars(self)
+      defaultValueDict = {key: str(value) for key, value in defaultValueDict.items()}
       self._flags.updateDictWithFlags(defaultValueDict)
       # we are passing all instance attributes as the default dict so generally we do not have to check
       # if an option exists, also options are case insensitive and stored in lowercase
       config = six.moves.configparser.SafeConfigParser(defaults=defaultValueDict, dict_type=dict)
       config.read(parameter.prodConfigFilename)
       self._flags.loadFlags(config)
 
       for attribute in LIST_ATTRIBUTES:
         setattr(self, attribute, listify(config.get(PP, attribute)))
 
       for attribute in STRING_ATTRIBUTES:
         setattr(self, lowerFirst(attribute), config.get(PP, attribute))
 
+      for attribute in BOOL_ATTRIBUTES:
+        setattr(self, lowerFirst(attribute), config.get(PP, attribute).lower() in ('true',))
+
       # this parameter is deprecated and not part of the instance attributes so we need to check for existence
       if config.has_option(PP, 'clicConfig'):
         gLogger.warn('"clicConfig" parameter is deprected, please dump a new steering file!')
         self.configVersion = config.get(PP, 'clicConfig')
 
       # attribute and option names differ, special treatment
       self.cliRecoOption = config.get(PP, 'cliReco')
@@ -498,14 +511,15 @@
       self.prodIDs = [int(pID.strip()) for pID in self.prodIDs if pID.strip()]
       self.prodIDs = self.prodIDs if self.prodIDs else [1 for _ in self.energies]
 
       # if one of the lists only has size 1 and there is a longer list we extend
       # the list to the maximum size assuming the values are re-used
       maxLength = 0
       parameterLists = [self.processes, self.energies, self.eventsPerJobs, self.generatorSteeringFile]
+      
       for parList in parameterLists:
         maxLength = len(parList) if len(parList) > maxLength else maxLength
       for parList in parameterLists:
         if len(parList) == 1 and maxLength > 1:
           parList.extend([parList[0]] * (maxLength - 1))
 
       if not (self.processes and self.energies and self.eventsPerJobs) and self.prodIDs:
@@ -598,14 +612,18 @@
 prodGroup = %(prodGroup)s
 detectorModel = %(detectorModel)s
 softwareVersion = %(softwareVersion)s
 
 generatorApplication = %(generatorApplication)s
 generatorVersion = %(generatorVersion)s
 generatorSteeringFile = %(generatorSteeringFile)s
+processingAfterGen = %(processingAfterGen)s
+
+datatype = %(datatype)s
+campaign = %(campaign)s
 
 simApplication = %(simApplication)s
 simVersion = %(simVersion)s
 simSteeringFile = %(simSteeringFile)s
 
 recoApplication = %(recoApplication)s
 recoVersion = %(recoVersion)s
@@ -654,63 +672,89 @@
     if isinstance(energy, six.string_types):
       return energy
     energy = ("%1.2f" % energy).rstrip('0').rstrip('.')
     return energy
 
   def createGeneratorApplication(self, task):
     """Create the selected generator application."""
-
     genApp =  {'kkmc': self.createKKMCApplication,
+               'whizard2': self.createWhizard2Application,
+               'delphesapp': self.createDelphesApplication,
+               'gaudiapp': self.createGaudiApplication,
              }[self.generatorApplication.lower()](task)
     if task.datatype:
       genApp.datatype = task.datatype
     return genApp
 
-
   def createSimulationApplication(self, task):
     """Create the selected Simulation application."""
 
     return {'genericapp': self.createGenericApplication,
             }[self.simApplication.lower()](task)
 
+  def createWhizard2Application(self, task):
+    """create Whizard2 Application."""
+    from ILCDIRAC.Interfaces.API.NewInterface.Applications import Whizard2
+    whiz = Whizard2()
+    whiz.setVersion(self.generatorVersion)
+    whiz.setNumberOfEvents(task.eventsPerJob)
+    whiz.setSinFile(task.genFile)
+    whiz.setEvtType(task.meta['EvtType'])
+    whiz.setEnergy(task.meta['Energy'])
+    whiz.datatype = 'lhef'
+    self._setApplicationOptions('Whizard2', whiz, task.applicationOptions)
+    return whiz
+
   def createKKMCApplication(self, task):
     """create KKMCee Application."""
     from ILCDIRAC.Interfaces.API.NewInterface.Applications import KKMC
-
     kkmcee = KKMC()
     kkmcee.setVersion(self.generatorVersion)
+    kkmcee.setNumberOfEvents(task.eventsPerJob)
     if task.genFile:
       kkmcee.setConfigFile(task.genFile)
-    kkmcee.setEvtType(''.join(task.meta['EvtType'][:len(task.meta['EvtType']) / 2]).capitalize())
-    kkmcee.setNumberOfEvents(task.eventsPerJob)
+    kkmcee.setEvtType(''.join(task.meta['EvtType'][:len(task.meta['EvtType']) // 2]).capitalize())
     kkmcee.setEnergy(task.meta['Energy'])
+    kkmcee.datatype = 'lhef'
     self._setApplicationOptions('KKMC', kkmcee, task.applicationOptions)
-    task.datatype = 'lhef'
-    task.generator = 'kkmcee'
     return kkmcee
+  
+  def createDelphesApplication(self, task):
+    """create Delphes Application."""
+    from ILCDIRAC.Interfaces.API.NewInterface.Applications import DelphesApp
+    delphes = DelphesApp()
+    delphes.setVersion(self.generatorVersion)
+    delphes.setPythia8Card(task.genFile)
+    delphes.setNumberOfEvents(task.eventsPerJob)
+    delphes.setEnergy(task.meta['Energy'])
+    delphes.detector = self.detectorModel
+    delphes.datatype = 'delphes'
+    self._setApplicationOptions('delphesapp', delphes, task.applicationOptions)
+    return delphes
 
-  def createGenericApplication(self, task):
-    """Create GenericApplication."""
+  def createGaudiApplication(self, task):
+    """create Gaudi Application."""
     from ILCDIRAC.Interfaces.API.NewInterface.Applications import GaudiApp
+    gaudi = GaudiApp()
+    gaudi.setVersion(self.generatorVersion)
+    gaudi.setNumberOfEvents(task.eventsPerJob)
+    gaudi.setEnergy(task.meta['Energy'])
+    gaudi.detector = self.detectorModel
+    if self.datatype:
+      gaudi.datatype = self.datatype
+    if self.datatype == 'delphes':
+      gaudi.setPythia8Card(task.genFile)
+    else:
+      gaudi.setKeepRecFile(True)
+    self._setApplicationOptions('gaudiapp', gaudi, task.applicationOptions)
+    return gaudi
 
-    ga = GaudiApp()
-    ga.setVersion('key4hep-latest')  # FIXME: task.gaSetupScript
-    ga.setExecutable("DelphesPythia8_EDM4HEP")  # FIXME task.gaScript
-    ga.setInputFileFlag('')
-    # FIXME this should be configurable
-    ga.setOutputFileFlag("delphes_card_IDEA.tcl edm4hep_output_config.tcl Pythia_LHEinput.cmd")
-    # task.gaArguments
-    # ga.setEvtType(task.meta['EvtType'])
-    ga.setNumberOfEvents(task.eventsPerJob)
-    ga.setEnergy(task.meta['Energy'])
-    ga._extension = 'root'
-    ga.datatype = 'delphes'
-    self._setApplicationOptions('GA', ga, task.applicationOptions)
-
-    return ga
+  def createGenericApplication(self, task):
+    """Create GenericApplication: not implemented"""
+    pass
 
   def createGenerationProduction(self, task):
     """Create generation production."""
     prodName = task.getProdName(self.machine, 'gen', self.additionalName)
     parameterDict = task.parameterDict
     nbTasks = task.nbTasks
     gLogger.notice("*" * 80 + "\nCreating generation production: %s " % prodName)
@@ -722,31 +766,35 @@
     # this might modify task
     genApp = self.createGeneratorApplication(task)
     if task.generator:
       genProd.generator = task.generator
     res = genProd.append(genApp)
     if not res['OK']:
       raise RuntimeError("Error creating generation production: %s" % res['Message'])
-
-    if True:  # delphes after the KKMC task
-      gaApp = self.createGenericApplication(task)
-      gaApp.detector = 'IDEA'
-      gaApp.datatype = 'delphes'
-      res = genProd.append(gaApp)
+    if self.processingAfterGen:
+      processingapp = {'delphes': self.createDelphesApplication,
+                       'gaudi': self.createGaudiApplication,
+                       }[self.processingAfterGen](task)
+      res = genProd.append(processingapp)
       if not res['OK']:
         raise RuntimeError("Error creating generation production: %s" % res['Message'])
-
+        
     genProd.addFinalization(True, True, True, True)
     if not prodName:
       raise RuntimeError("Error creating generation production: prodName empty")
     genProd.setDescription(prodName)
     res = genProd.createProduction()
     if not res['OK']:
       raise RuntimeError("Error creating generation production: %s" % res['Message'])
 
+    for finalPath in genProd.finalpaths:
+      if 'lhef' in finalPath:
+        genProd.specialFinalMetaData.setdefault(finalPath, {})['SWPackages'] = \
+          ';'.join(pkg for pkg in genProd.prodparameters["SWPackages"].split(';') if 'kkmc' in pkg.lower())
+
     # genProd.addMetadataToFinalFiles({'BeamParticle1': parameterDict['pname1'],
     #                                  'BeamParticle2': parameterDict['pname2'],
     #                                  'EPA_B1': parameterDict['epa_b1'],
     #                                  'EPA_B2': parameterDict['epa_b2'],
     #                                 }
     #                                )
 
@@ -1114,16 +1162,16 @@
   CLIP.registerSwitches()
   Script.parseCommandLine()
   from ILCDIRAC.Core.Utilities.CheckAndGetProdProxy import checkOrGetGroupProxy
   CHECKGROUP = checkOrGetGroupProxy(['ilc_prod', 'fcc_prod'])
   if CHECKGROUP['OK']:
     pass
   elif CLIP.dryRun:
-    gLogger.notice('Did not find correct group, dryRun enabled, assuming "ilc_prod"')
-    CHECKGROUP = S_OK('ilc_prod')
+    gLogger.notice('Did not find correct group, dryRun enabled, assuming "fcc_prod"')
+    CHECKGROUP = S_OK('fcc_prod')
   else:
     exit(1)
   try:
     CHAIN = FCCDetProdChain(params=CLIP, group=CHECKGROUP['Value'])
     CHAIN.createAllTransformations()
   except (AttributeError, RuntimeError) as excp:
     if str(excp) != '':
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/DiracILC.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/DiracILC.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,20 @@
     """Check availability of application in CS.
 
     :param str platform: System platform
     :param str appName: Application name
     :param str appVersion: Application version
     :return: :func:`~DIRAC.Core.Utilities.ReturnValues.S_OK` or :func:`~DIRAC.Core.Utilities.ReturnValues.S_ERROR`
     """
+
+    software_redirections = {'delphesapp': 'gaudiapp',
+                            }
+    if appName in software_redirections:
+      appName = software_redirections[appName]
+
     csPathTarBall = "/AvailableTarBalls/%s/%s/%s/TarBall" % (platform, appName, appVersion)
     csPathCVMFS = "/AvailableTarBalls/%s/%s/%s/CVMFSPath" % (platform, appName, appVersion)
 
     LOG.debug("Checking for software version in " + csPathTarBall)
     app_version = self.ops.getValue(csPathTarBall, '')
 
     LOG.debug("Checking for software version in " + csPathCVMFS)
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,51 +24,60 @@
 #
 """Gaudi Application to run applications based on Gaudi.
 
 .. versionadded:: v32r0p1
 
 Usage:
 
->>> ga.setVersion('key4hep_nightly')
->>> ga.setExecutable('k4run')
->>> ga.setSteeringFile('geant_fullsim_fccee_lar_pgun.py')
->>> ga.setDetectorModel("DetFCCeeIDEA-LAr")
->>> ga.setArguments("--GenAlg.MomentumRangeParticleGun.MomentumMin 1000 "
->>>                 "--GenAlg.MomentumRangeParticleGun.MomentumMax 1000 "
->>>                 "--GenAlg.MomentumRangeParticleGun.PdgCodes 11")
->>> ga.setOutputFile("output.root")
+>>> ga = GaudiApp()
+>>> ga.setVersion('key4hep-latest')
+>>> ga.setExecutable("k4run")
+>>> ga.setSteeringFile('k4simdelphesalg_pythia.py')
+>>> ga.setPythia8Card('p8_ee_ggqq_ecm91.cmd')
+>>> ga.setExtraCLIArguments("--GenAlg.PythiaInterface.pythiacard pythia8card.cmd --k4SimDelphesAlg.DelphesCard delphes_card_IDEA.tcl --k4SimDelphesAlg.DelphesOutputSettings edm4hep_output_config.tcl")
+>>> ga.setEnergy(91.2)
+>>> ga.setNumberOfEvents(50)
+>>> ga.setOutputFile('output.root')
 
 """
 from __future__ import absolute_import
 import types
 import os
 
 from ILCDIRAC.Interfaces.API.NewInterface.LCApplication import LCApplication
 from ILCDIRAC.Core.Utilities.InstalledFiles import Exists
 from ILCDIRAC.Interfaces.Utilities.DDInterfaceMixin import DDInterfaceMixin
 from DIRAC import S_OK, S_ERROR, gLogger
 from DIRAC.Core.Workflow.Parameter import Parameter
 from DIRAC.ConfigurationSystem.Client.Helpers.Operations import Operations
 import six
+from ILCDIRAC.Core.Utilities.PrepareOptionFiles import preparePythia8Card
 
 LOG = gLogger.getSubLogger(__name__)
 __RCSID__ = "$Id$"
 
 
 class GaudiApp(DDInterfaceMixin, LCApplication):
   """GaudiApp Application Class."""
 
   def __init__(self, paramdict=None):
     self.startFrom = 0
     self.randomSeed = -1
+    self.randomSeedFlag = ''
     self.detectorModel = ''
     self.executableName = 'k4run'
     self.inputFileFlag = '--EventDataSvc.inputs'
     self.outputFileFlag = '--out.filename'
     self.detectorModelFlag = '--GeoSvc.detectors'
+    self.pythia8CardContent = ''
+    self.outputDstPath = ''
+    self.outputDstFile = ''
+    self.outputRecPath = ''
+    self.outputRecFile = ''
+    self.keepRecFile = None
     super(GaudiApp, self).__init__(paramdict)
     # Those 5 need to come after default constructor
     self._modulename = 'GaudiAppModule'
     self._moduledescription = 'Module to run GaudiApp'
     self.appname = 'gaudiapp'
     self._ops = Operations()
 
@@ -100,14 +109,22 @@
 
     :param str args: Arguments to pass to the command call
     """
     self._checkArgs({'args': (str,)})
     self.extraCLIArguments = args
     return S_OK()
 
+  def setRandomSeedFlag(self, randomSeedFlag):
+    """ Optional: Define seed for some of the k4run steering files.
+
+    :param str randomSeedFlag: set the seed
+    """
+    self._checkArgs({'randomSeedFlag': (str,)})
+    self.randomSeedFlag = randomSeedFlag
+
   def setInputFileFlag(self, inputFileFlag):
     """ Optional: Define inputTypeFlag for k4run input files.
 
     :param str inputFileFlag: type of event files (LCIO, EventDataSvc)
     """
     self._checkArgs({'inputFileFlag': (str,)})
     self.inputFileFlag = inputFileFlag
@@ -134,22 +151,77 @@
     """Define from where GaudiApp starts to read in the input file.
 
     :param int startfrom: from where GaudiApp starts to read the input file
     """
     self._checkArgs({'startfrom': int})
     self.startFrom = startfrom
 
-  def setExecutable(self, executableName):
+  def setExecutableName(self, executableName):
     """Set the executable.
 
     :param str executableName: Name of the gaudi executable program. Default ``k4Run``
     """
     self._checkArgs({'executableName': (str,)})
     self.executableName = executableName
 
+  def setPythia8Card(self, pythia8CardPath):
+    """Set the pythia8 card.
+
+    :param str pythia8CardPath: Name of the Pythia8 configuration file path.
+    """
+    self._checkArgs({'pythia8CardPath': (str,)})
+    if not os.path.isfile(pythia8CardPath):
+      return self._reportError('Pythia8 configuration file does not exist!')
+    self.pythia8CardContent = open(pythia8CardPath).read()
+    return S_OK()
+    
+  def setKeepRecFile(self, val):
+    """Set the ``keepRecFile`` flag.
+
+    Only relevant for ProductionJobs
+
+    :param bool val: If ``False`` REC file is not stored
+    """
+    self._checkArgs({'val': bool})
+    self.keepRecFile = val
+    
+  def setOutputRecFile(self, outputRecFile, path=None):
+    """Optional: Define output rec file for Gaudi. Used only in production
+    context. Use :func:`UserJob.setOutputData
+    <ILCDIRAC.Interfaces.API.NewInterface.UserJob.UserJob.setOutputData>` if you
+    want to keep the file on the grid.
+
+    :param str outputRecFile: output rec file for Gaudi
+    :param str path: Path where to store the file.
+
+    """
+    self._checkArgs({'outputRecFile': (str,)})
+    self.outputRecFile = outputRecFile
+    self.prodparameters[self.outputRecFile] = {}
+    self.prodparameters[self.outputRecFile]['datatype'] = 'rec'
+    if path:
+      self.outputRecPath = path
+
+  def setOutputSimFile(self, outputSimFile, path=None):
+    """Optional: Define output sim file for Gaudi.  Used only in production
+    context. Use :func:`UserJob.setOutputData
+    <ILCDIRAC.Interfaces.API.NewInterface.UserJob.UserJob.setOutputData>` if you
+    want to keep the file on the grid.
+
+    :param str outputDstFile: output sim file for Gaudi
+    :param str path: Path where to store the file.
+
+    """
+    self._checkArgs({'outputSimFile': (str,)})
+    self.outputSimFile = outputSimFile
+    self.prodparameters[self.outputSimFile] = {}
+    self.prodparameters[self.outputSimFile]['datatype'] = 'sim'
+    if path:
+      self.outputSimPath = path
+
   def _userjobmodules(self, stepdefinition):
     res1 = self._setApplicationModuleAndParameters(stepdefinition)
     res2 = self._setUserJobFinalization(stepdefinition)
     if not res1["OK"] or not res2["OK"]:
       return S_ERROR('userjobmodules failed')
     return S_OK()
 
@@ -189,48 +261,59 @@
     if self._jobtype != 'User':
       self._listofoutput.append({"outputFile": "@{OutputFile}", "outputPath": "@{OutputPath}",
                                  "outputDataSE": '@{OutputSE}'})
 
       self.prodparameters['detectorType'] = self.detectortype
       self.prodparameters['slic_detectormodel'] = self.detectorModel
 
+    if self.pythia8CardContent:
+      res = preparePythia8Card(self.pythia8CardContent, 0, self.randomSeed)
+      if not res['OK']:
+        return res
+
     if not self.startFrom:
       LOG.verbose('No startFrom defined for GaudiApp : start from the beginning')
 
     return S_OK()
 
   def _applicationModule(self):
 
     md1 = self._createModuleDefinition()
     md1.addParameter(Parameter("randomSeed", 0, "int", "", "", False, False,
                                "Random seed for the generator"))
+    md1.addParameter(Parameter("randomSeedFlag", "", "string", "", "", False, False,
+                               "Flag that forces the random seed to be set (e.g. --SimG4Svc.seedValue)"))
     md1.addParameter(Parameter("executableName", "", "string", "", "", False, False,
                                "Name of the executable"))
     md1.addParameter(Parameter("startFrom", 0, "int", "", "", False, False,
                                "From where GaudiApp starts to read the input file"))
     md1.addParameter(Parameter("detectorModel", "", "string", "", "", False, False,
                                "Detecor model for simulation"))
     md1.addParameter(Parameter("inputFileFlag", "", "string", "", "", False, False,
                                "Flag that define the type flag for input files (lcio, eventdatasvc, ..)"))
+    md1.addParameter(Parameter("pythia8CardContent", "", "string", "", "", False, False,
+                               "Flag that contains the pythia8 card"))   
     md1.addParameter(Parameter("outputFileFlag", "", "string", "", "", False, False,
                                "Flag that defines the output file flag (e.g. PodioOutput)"))
     md1.addParameter(Parameter("detectorModelFlag", "", "string", "", "", False, False,
                                "Flag that defines the detector model file flag (e.g. GeoSvc)"))
     md1.addParameter(Parameter("debug", False, "bool", "", "", False, False, "debug mode"))
     return md1
 
   def _applicationModuleValues(self, moduleinstance):
 
     moduleinstance.setValue("randomSeed", self.randomSeed)
+    moduleinstance.setValue("randomSeedFlag", self.randomSeedFlag)
     moduleinstance.setValue("executableName", self.executableName)
     moduleinstance.setValue("startFrom", self.startFrom)
     moduleinstance.setValue("detectorModel", self.detectorModel)
     moduleinstance.setValue("inputFileFlag", self.inputFileFlag)
     moduleinstance.setValue("outputFileFlag", self.outputFileFlag)
     moduleinstance.setValue("detectorModelFlag", self.detectorModelFlag)
+    moduleinstance.setValue("pythia8CardContent", self.pythia8CardContent)
     moduleinstance.setValue("debug", self.debug)
 
   def _checkWorkflowConsistency(self):
     return self._checkRequiredApp()
 
   def _resolveLinkedStepParameters(self, stepinstance):
     if isinstance(self._linkedidx, six.integer_types):
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 __all__ = ['GenericApplication', 'GetSRMFile', '_Root', 'RootScript', 'RootMacro',
            'Whizard', 'Pythia', 'PostGenSelection', 'StdhepCut', 'StdhepCutJava',
            'Mokka', 'SLIC', 'OverlayInput', 'Marlin', 'LCSIM', 'SLICPandora',
            'CheckCollections', 'SLCIOConcatenate', 'SLCIOSplit', 'StdHepSplit',
            'Tomato', 'CheckWNs', 'DDSim', 'Fcc', 'FccSw', 'FccAnalysis', 'Whizard2',
            'KKMC',
            'GaudiApp',
+           'DelphesApp',
            ]
 
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.GenericApplication import GenericApplication
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.GetSRMFile import GetSRMFile
 from ILCDIRAC.Interfaces.API.NewInterface.Applications._Root import _Root
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.RootScript import RootScript
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.RootMacro import RootMacro
@@ -92,7 +93,8 @@
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.DDSim import DDSim
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.Fcc import Fcc
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.Fcc import FccSw
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.Fcc import FccAnalysis
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.Whizard2 import Whizard2
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.KKMC import KKMC
 from ILCDIRAC.Interfaces.API.NewInterface.Applications.GaudiApp import GaudiApp
+from ILCDIRAC.Interfaces.API.NewInterface.Applications.DelphesApp import DelphesApp
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     self.generator = None
 
     self.finalpaths = []
     self.finalMetaDict = defaultdict(dict)
     self.prodMetaDict = {}
     self.finalMetaDictNonSearch = {}
     self.metadict_external = {}
+    self.specialFinalMetaData = {}
     self.outputStorage = ''
 
     self.proxyinfo = getProxyInfo()
     self.vo = getVOForGroup(self.proxyinfo.get('Value', {}).get('group', 'ilc_user'))
 
     self.inputdataquery = False
     self.inputBKSelection = {}
@@ -547,22 +548,22 @@
 
     if 'extraCLIArguments' in self.prodparameters:
       info.append('- ExtraCLIArguments %s' % self.prodparameters['extraCLIArguments'])
 
     # as this is the very last call all applications are registered, so all software packages are known
     # add them the the metadata registration
     for finalpath in self.finalpaths:
-      if finalpath not in self.finalMetaDictNonSearch:
-        self.finalMetaDictNonSearch[finalpath] = {}
       if "SWPackages" in self.prodparameters:
-        self.finalMetaDictNonSearch[finalpath]["SWPackages"] = self.prodparameters["SWPackages"]
+        self.finalMetaDictNonSearch.setdefault(finalpath, {})["SWPackages"] = self.prodparameters["SWPackages"]
 
       if self.metadict_external:
         self.finalMetaDictNonSearch[finalpath].update(self.metadict_external)
 
+    self.finalMetaDictNonSearch.update(self.specialFinalMetaData)
+
     info.append('- Registered metadata: ')
     for path, metadata in sorted(self.finalMetaDict.items()):
       info.append('    %s = %s' % (path, metadata))
     info.append('- Registered non searchable metadata: ')
     for path, metadata in sorted(self.finalMetaDictNonSearch.items()):
       info.append('    %s = %s' % (path, metadata))
 
@@ -751,15 +752,15 @@
       self.prodparameters['Process'] = self.evttype
 
     if not self.outputStorage:
       return S_ERROR("You need to specify the Output storage element")
 
     curpackage = "%s.%s" % (application.appname, application.version)
     if "SWPackages" in self.prodparameters:
-      if not self.prodparameters["SWPackages"].count(curpackage):
+      if curpackage not in self.prodparameters["SWPackages"]:
         self.prodparameters["SWPackages"] += ";%s" % (curpackage)
     else:
       self.prodparameters["SWPackages"] = "%s" % (curpackage)
 
     if not application.accountInProduction:
       res = self._updateProdParameters(application)
       if not res['OK']:
@@ -788,19 +789,48 @@
       self.finalMetaDict[self.basepath + energypath] = {"Energy": str(self.energy)}
 
     currentPathList = [self.basepath, energypath, evttypepath]
     path = os.path.join(*currentPathList)
     self.finalMetaDict[path] = {"EvtType": self.evttype}
     if self.generator:
       self.prodparameters['Generator'] = self.generator
-      currentPathList.append(self.generator)
-      generatorPath = os.path.join(*currentPathList)
-      self.finalMetaDict[generatorPath] = {'Generator': self.generator}
+      if self.vo != 'fcc': # for fcc we no longer include the generator inside the file path
+        currentPathList.append(self.generator)
+        generatorPath = os.path.join(*currentPathList)
+        self.finalMetaDict[generatorPath] = {'Generator': self.generator}
+
+    # comment of Lorenzo Valentini, 12-05-2023
+    # In fcc we have a particular use of Gaudi. Its application is defined with the functions setOutputSimFile/setOutputRecFile.
+    # However, it is sometimes used for other tasks, for which we don't want it to use the file path of the sim/rec transformations.
+    # Up to now, seems like whenever we will be using sim/rec transformations we won't have to define the datatype, which we use to discriminate the two cases.
+    
+    # comment of Lorenzo Valentini, 12-05-2023
+    # this is the case of a (maybe Gaudi) application used for sim/rec transformations: no datatype defined, and we check the presence of setOutputSimFile
+    if hasattr(application, "setOutputSimFile") and not application.willBeCut and self.vo == 'fcc' and not application.datatype: 
+      detPath = os.path.join(path, application.detector)
+      self.finalMetaDict[detPath] = {"DetectorType": application.detector}
+      if application.keepRecFile:
+        path = os.path.join(detPath, 'rec')
+        self.finalMetaDict[path] = {'Datatype': 'rec'}
+        fname = self.basename + '_rec.slcio'
+        application.setOutputRecFile(fname, path)
+        LOG.notice('Will store the files under', path)
+        self.finalpaths.append(path)
+      path = os.path.join(detPath, 'sim')
+      self.finalMetaDict[path] = {'Datatype': 'sim'}
+      fname = self.basename + '_dst.slcio'
+      application.setOutputSimFile(fname, path)
+      LOG.notice('Will store the files under', path)
+      self.finalpaths.append(path)
 
-    if hasattr(application, "setOutputRecFile") and not application.willBeCut:
+    # comment of Lorenzo Valentini, 12-05-2023
+    # this is the case of a (maybe Gaudi) application used for dst/rec transformations: no datatype defined, and we check the presence of setOutputRecFile. It would make more sense to just check for setOutputDstFile,
+    # but we wanted to keep it backward compatibile with the ilc simulations.
+    # In the case of fcc, we check for the absence of datatype.
+    elif hasattr(application, "setOutputRecFile") and not application.willBeCut and (self.vo != 'fcc' or (self.vo == 'fcc' and not application.datatype)):
       detPath = os.path.join(path, application.detectortype)
       self.finalMetaDict[detPath] = {'DetectorType': application.detectortype}
       if application.keepRecFile:
         path = os.path.join(detPath, 'REC')
         self.finalMetaDict[path] = {'Datatype': 'REC'}
         fname = self.basename + '_rec.slcio'
         application.setOutputRecFile(fname, path)
@@ -809,42 +839,44 @@
       path = os.path.join(detPath, 'DST')
       self.finalMetaDict[path] = {'Datatype': 'DST'}
       fname = self.basename + '_dst.slcio'
       application.setOutputDstFile(fname, path)
       LOG.notice('Will store the files under', path)
       self.finalpaths.append(path)
 
+    # comment of Lorenzo Valentini, 12-05-2023
+    # this is the case of an application with a single outputfile. It works in the same way for both fcc and ilc. 
     elif hasattr(application, "outputFile") and hasattr(application, 'datatype') and not application.outputFile and not application.willBeCut:
       LOG.notice('Adding output meta data for %s' % type(application))
       path = os.path.join(*currentPathList)
 
       if not application.datatype and self.datatype:
         application.datatype = self.datatype
 
-      # for fcc datatype comes before detctor model
-      if self.vo == 'fcc':
-        path = os.path.join(path, application.datatype)
-        self.finalMetaDict[path] = {'Datatype': application.datatype}
-
+      # comment of Lorenzo Valentini, 12-05-2023
+      # here we are adding detector and detectortype to the path, if they are defined. For fcc, we usually set the detector using the attribute application.detector.
+      # Anyway, seems like for ilc we wanted to "be ready" for both cases (detector, detectortype), so I did something similar for fcc.
+      # The code for ilc is not modified, to keep it backward compatible. However seems like in that case we would add to the path both detector and detectortype.
+      # For fcc we don't need to see the detector in the path two times, so I added a check to avoid that.
       if hasattr(application, "detectortype"):
         if application.detectortype:
           path = os.path.join(path, application.detectortype)
           self.finalMetaDict[path] = {"DetectorType": application.detectortype}
         elif self.detector:
           path = os.path.join(path, self.detector)
           self.finalMetaDict[path] = {"DetectorType": self.detector}
       if hasattr(application, "detector"):
-        if application.detector:
+        if application.detector and self.vo != 'fcc':
           path = os.path.join(path, application.detector)
           self.finalMetaDict[path] = {"DetectorType": application.detector}
-
-      # datatype comes after detctor model
-      if self.vo != 'fcc':
-        path = os.path.join(path, application.datatype)
-        self.finalMetaDict[path] = {'Datatype': application.datatype}
+        if application.detector and self.vo == 'fcc' and not application.detectortype:
+          path = os.path.join(path, application.detector)
+          self.finalMetaDict[path] = {"DetectorType": application.detector}
+      path = os.path.join(path, application.datatype)
+      self.finalMetaDict[path] = {'Datatype': application.datatype}
 
       LOG.notice('Will store the files under', '%s' % path)
       self.finalpaths.append(path)
       extension = getattr(application, '_extension', 'stdhep')
       if application.datatype in ['SIM', 'REC']:
         extension = 'slcio'
       fname = self.basename + "_%s" % (application.datatype.lower()) + "." + extension
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py`

 * *Files 5% similar despite different names*

```diff
@@ -733,20 +733,20 @@
     self.myapp.setOutputSE.return_value = S_ERROR('setOSE_error')
     assertDiracFailsWith(self.prodJob.append(self.myapp), 'setOSE_error', self)
     self.myapp.setOutputSE.return_value = S_OK(True)
     self.prodJob.evttype = 'mytype/'
     self.myapp.willBeCut = False
     with patch('%s.hasattr' % MODULE_NAME, new=Mock(return_value=True), create=True):
       self.assertTrue(self.prodJob.append(self.myapp))
-    with patch('%s.hasattr' % MODULE_NAME, new=Mock(side_effect=[True, False, True, True, True, True]), create=True):
+    with patch('%s.hasattr' % MODULE_NAME, new=Mock(side_effect=[True, False, False, True, True, True, True]), create=True):
       self.myapp.outputFile = False
       self.myapp.willBeCut = False
       self.myapp.detectortype = 'mydetector'
       assertDiracSucceeds(self.prodJob.append(self.myapp), self)
-    with patch('%s.hasattr' % MODULE_NAME, new=Mock(side_effect=[True, False, True, True, True, True]), create=True):
+    with patch('%s.hasattr' % MODULE_NAME, new=Mock(side_effect=[True, False, False, True, True, True, True]), create=True):
       my_dict = self.prodJob.prodparameters
 
       def getitem(name):
         return my_dict[name]
 
       def setitem(name, val):
         my_dict[name] = val
@@ -773,14 +773,15 @@
         'detectortype': False,
         'detector': False,
         'eventType': True,
         'outputFile': True,
         'datatype': True,
         'setOutputRecFile': False,
         'setOutputDstFile': False,
+        'setOutputSimFile': False,
         }
     self.assertIn(args[1], opsDict)
     return opsDict[args[1]]
 
   def hasAttrMocks_2(self, *args, **kwargs):  # pylint: disable=unused-argument
     """mock the operations getConfig calls."""
     print("arguments", args, kwargs)
@@ -790,14 +791,15 @@
         'detectortype': True,
         'detector': False,
         'eventType': True,
         'outputFile': True,
         'datatype': True,
         'setOutputRecFile': False,
         'setOutputDstFile': False,
+        'setOutputSimFile': False,
         }
     self.assertIn(args[1], opsDict)
     return opsDict[args[1]]
 
   def test_jobSpecificParams_detector_and_datatype(self):
     self.myapp.setOutputSE.return_value = S_OK(True)
     self.prodJob.evttype = ''
@@ -813,36 +815,156 @@
 
     hasAttrMock = Mock()
     hasAttrMock.side_effect = self.hasAttrMocks_2
     with patch('%s.hasattr' % MODULE_NAME, new=hasAttrMock, create=True):
       self.myapp.detectortype = 'application_detectortype'
       assertDiracSucceeds(self.prodJob.append(self.myapp), self)
 
-  @parameterized.expand([(True, ['/vo/prod/250gev/fake/awesome/REC', '/vo/prod/250gev/fake/awesome/DST']),
-                         (False, ['/vo/prod/250gev/fake/awesome/DST'])])
-  def test_jobSpecificParams_rec_and_dst(self, keep, finalPaths):
-    """Test if disabling rec file works."""
+  @parameterized.expand([(True, "ilc", None, 'awesome', 'awesome', ['/vo/prod/250gev/fake/awesome/REC', '/vo/prod/250gev/fake/awesome/DST']),
+                         (True, "ilc", None, None, 'awesome', ['/vo/prod/250gev/fake/awesome/REC', '/vo/prod/250gev/fake/awesome/DST']),
+                         (False, "ilc", None, 'awesome', 'awesome', ['/vo/prod/250gev/fake/awesome/DST']),
+                         (False, "ilc", "delphes", 'awesome', 'awesome', ['/vo/prod/250gev/fake/awesome/DST']),
+                         (True, "fcc", None, 'awesome', 'awesome', ['/vo/prod/250gev/fake/awesome/REC', '/vo/prod/250gev/fake/awesome/DST']),
+                         (False, "fcc", None, 'awesome', 'awesome', ['/vo/prod/250gev/fake/awesome/DST']),
+                         (False, "fcc", "delphes", 'awesome', 'awesome', ['/vo/prod/250gev/fake/awesome/delphes']),
+                         (False, "fcc", "delphes", 'awesome', None, ['/vo/prod/250gev/fake/awesome/delphes']),
+                         (False, "fcc", "delphes", None, 'awesome', ['/vo/prod/250gev/fake/awesome/delphes']),
+                         ])
+  def test_jobSpecificParams_rec_and_dst(self, keep, vo, datatype, detector, detectortype, finalPaths):
+    """Testing different combinations of vo, transformation, detector, datatype"""
     self.myapp.setOutputSE.return_value = S_OK(True)
     self.prodJob.evttype = ''
     self.prodJob.basepath = '/vo/prod/'
     self.prodJob.basename = 'basename'
+    self.prodJob.generator = 'whatever'
+    self.prodJob.vo = vo
+    self.myapp.detector = detector
+    self.myapp.datatype = datatype
     self.myapp.eventType = 'fake'
-    self.myapp.detectortype = 'awesome'
+    self.myapp.detectortype = detectortype
     self.myapp.willBeCut = False
     self.myapp.outputFile = False
     self.myapp.extraCLIArguments = ''
     self.myapp.keepRecFile = keep
     self.myapp.setOutputRecFile = Mock(name='RecFile')
     self.myapp.setOutputDstFile = Mock(name='DstFile')
+    del self.myapp.setOutputSimFile
+    with patch('%s.ProductionJob._updateProdParameters' % MODULE_NAME, new=Mock(return_value=S_OK())):
+      assertDiracSucceeds(self.prodJob.append(self.myapp), self)
+    if vo != 'fcc':
+      if keep:
+        self.myapp.setOutputRecFile.assert_called_once()
+      else:
+        self.myapp.setOutputRecFile.assert_not_called()
+      self.myapp.setOutputDstFile.assert_called_once()
+    elif not datatype:
+      if keep:
+        self.myapp.setOutputRecFile.assert_called_once()
+      else:
+        self.myapp.setOutputRecFile.assert_not_called()
+      self.myapp.setOutputDstFile.assert_called_once()
+    else:
+      self.myapp.setOutputRecFile.assert_not_called()
+      self.myapp.setOutputDstFile.assert_not_called()
+
+    assert self.prodJob.finalpaths == finalPaths
+
+  @parameterized.expand([(True, "fcc", None, 'awesome', 'awesome', ['/vo/prod/250gev/fake/awesome/rec', '/vo/prod/250gev/fake/awesome/sim']),
+                         (True, "fcc", None, 'awesome', None, ['/vo/prod/250gev/fake/awesome/rec', '/vo/prod/250gev/fake/awesome/sim']),
+                         (False, "fcc", None, 'awesome', 'awesome', ['/vo/prod/250gev/fake/awesome/sim']),
+                         (False, "fcc", "delphes", 'awesome', 'awesome', ['/vo/prod/250gev/fake/awesome/delphes']),
+                         (False, "fcc", "delphes", 'awesome', None, ['/vo/prod/250gev/fake/awesome/delphes']),
+                         (False, "fcc", "delphes", None, 'awesome', ['/vo/prod/250gev/fake/awesome/delphes']),
+                         ])
+  def test_jobSpecificParams_rec_and_sim(self, keep, vo, datatype, detector, detectortype, finalPaths):
+    """Testing different combinations of vo, transformation, detector, datatype"""
+    self.myapp.setOutputSE.return_value = S_OK(True)
+    self.prodJob.evttype = ''
+    self.prodJob.basepath = '/vo/prod/'
+    self.prodJob.basename = 'basename'
+    self.prodJob.generator = 'whatever'
+    self.prodJob.vo = vo
+    self.myapp.detector = detector
+    self.myapp.datatype = datatype
+    self.myapp.eventType = 'fake'
+    self.myapp.detectortype = detectortype
+    self.myapp.willBeCut = False
+    self.myapp.outputFile = False
+    self.myapp.extraCLIArguments = ''
+    self.myapp.keepRecFile = keep
+    self.myapp.setOutputRecFile = Mock(name='RecFile')
+    self.myapp.setOutputSimFile = Mock(name='SimFile')
+    del self.myapp.setOutputDstFile
     with patch('%s.ProductionJob._updateProdParameters' % MODULE_NAME, new=Mock(return_value=S_OK())):
       assertDiracSucceeds(self.prodJob.append(self.myapp), self)
-    if keep:
-      self.myapp.setOutputRecFile.assert_called_once()
+    if not datatype:
+      if keep:
+        self.myapp.setOutputRecFile.assert_called_once()
+      else:
+        self.myapp.setOutputRecFile.assert_not_called()
+      self.myapp.setOutputSimFile.assert_called_once()
     else:
       self.myapp.setOutputRecFile.assert_not_called()
+      self.myapp.setOutputSimFile.assert_not_called()
+
+    assert self.prodJob.finalpaths == finalPaths
+
+
+  @parameterized.expand([('detector', 'detectortype', ['/vo/prod/250gev/fake/generator/detectortype/detector/datatype']),
+                         ])
+  def test_jobSpecificParams_rec_and_dst__2(self, detector, detectortype, finalPaths):
+    """Testing different combinations of vo, transformation, detector, datatype"""
+    self.myapp.setOutputSE.return_value = S_OK(True)
+    self.prodJob.evttype = ''
+    self.prodJob.basepath = '/vo/prod/'
+    self.prodJob.basename = 'basename'
+    self.prodJob.generator = 'generator'
+    self.prodJob.vo = "ilc"
+    self.myapp.detector = detector
+    self.myapp.datatype = "datatype"
+    self.myapp.eventType = 'fake'
+    self.myapp.detectortype = detectortype
+    self.myapp.willBeCut = False
+    self.myapp.outputFile = False
+    self.myapp.extraCLIArguments = ''
+    self.myapp.keepRecFile = False
+    del self.myapp.setOutputRecFile
+    with patch('%s.ProductionJob._updateProdParameters' % MODULE_NAME, new=Mock(return_value=S_OK())):
+      assertDiracSucceeds(self.prodJob.append(self.myapp), self)
+    assert self.prodJob.finalpaths == finalPaths
+
+
+  @parameterized.expand([(250, 250, ['/vo/prod/250gev/fake/awesome/DST']),
+                         (250, None, ['/vo/prod/250gev/fake/awesome/DST']),
+                         (None, 250, ['/vo/prod/250gev/fake/awesome/DST']),
+                         ])
+  def test_jobSpecificParams_energyandevents(self, selfenergy, appenergy, finalPaths):
+    """Testing different combinations of energies and paths"""
+    self.myapp.setOutputSE.return_value = S_OK(True)
+    self.prodJob.evttype = ''
+    self.prodJob.basepath = '/vo/prod/'
+    self.prodJob.basename = 'basename'
+    self.prodJob.generator = 'whatever'
+    self.prodJob.vo = "ilc"
+    self.prodJob.energy = selfenergy
+    self.prodJob.slicesize = 2
+    self.myapp.energy = appenergy
+    self.myapp.numberOfEvents = 1
+    self.myapp.detector = 'awesome'
+    self.myapp.eventType = 'fake'
+    self.myapp.detectortype = 'awesome'
+    self.myapp.willBeCut = False
+    self.myapp.outputFile = False
+    self.myapp.extraCLIArguments = ''
+    self.myapp.keepRecFile = False
+    self.myapp.setOutputRecFile = Mock(name='RecFile')
+    self.myapp.setOutputDstFile = Mock(name='DstFile')
+    with patch('%s.ProductionJob._updateProdParameters' % MODULE_NAME, new=Mock(return_value=S_OK())):
+      assertDiracSucceeds(self.prodJob.append(self.myapp), self)
+    self.myapp.setOutputRecFile.assert_not_called()
     self.myapp.setOutputDstFile.assert_called_once()
     assert self.prodJob.finalpaths == finalPaths
 
   def test_setters_1(self):
     import random
     self.prodJob.setDryRun(True)
     assertEqualsImproved(self.prodJob.dryrun, True, self)
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,37 +42,29 @@
 
 
 class DiracILCTestCase(unittest.TestCase):
   """Base class for the DiracILC test cases."""
 
   def setUp(self):
     """set up the objects."""
-    ops_mock = Mock()
-    mocked_modules = {'DIRAC.ConfigurationSystem.Client.Helpers.Operations': ops_mock}
-    self.module_patcher = patch.dict(sys.modules, mocked_modules)
-    self.module_patcher.start()
     from ILCDIRAC.Interfaces.API.DiracILC import DiracILC
     self.dilc = DiracILC()
 
     def setOptions(*args):
       if 'SingleReplicaSEs' in args[0]:
         return ['SE']
       if 'Minimum' in args[0]:
         return 1
       if args[0].endswith('PreferredSEs'):
         return ['Awesome-Tape-SE']
 
     ops_mock = Mock()
-    ops_mock.getValue = Mock()
-    ops_mock.getValue.side_effect = setOptions
+    ops_mock.getValue = Mock(side_effect=setOptions)
     self.dilc.ops = ops_mock
 
-  def tearDown(self):
-    self.module_patcher.stop()
-
   def test_getprocesslist(self):
     with patch('%s.gConfig.getValue' % MODULE_NAME, new=Mock(return_value='some_gconf_testval')) as conf_mock, \
         patch('%s.ProcessList' % MODULE_NAME, new=Mock()) as pl_mock:
       res = self.dilc.getProcessList()
       pl_mock.assert_called_once_with('some_gconf_testval')
       assertEqualsImproved(res, pl_mock(), self)
       conf_mock.assert_called_once_with('/LocalSite/ProcessListPath', '')
@@ -357,15 +349,15 @@
         return ['Awesome-Disk-SE']
       if 'Minimum' in args[0]:
         return 2
       if args[0].endswith('PreferredSEs'):
         return ['Awesome-Tape-SE']
 
     ops_mock = Mock()
-    ops_mock.getValue = setOptions
+    ops_mock.getValue = Mock(side_effect=setOptions)
     self.dilc.ops = ops_mock
 
     with patch('%s.DiracILC.getReplicas' % MODULE_NAME, new=Mock(return_value=S_OK(ret_dict))) as replica_mock:
       assertDiracFailsWith(self.dilc.checkInputSandboxLFNs(job_mock), 'Not enough replicas', self)
       replica_mock.assert_called_once_with(['/some/file.txt'])
 
   def test_checkinputsb_goodRepl(self):
@@ -378,13 +370,13 @@
         return ['Awesome-Disk-SE']
       if 'Minimum' in args[0]:
         return 2
       if args[0].endswith('PreferredSEs'):
         return ['Awesome-Tape-SE']
 
     ops_mock = Mock()
-    ops_mock.getValue = setOptions
+    ops_mock.getValue = Mock(side_effect=setOptions)
     self.dilc.ops = ops_mock
 
     with patch('%s.DiracILC.getReplicas' % MODULE_NAME, new=Mock(return_value=S_OK(ret_dict))) as replica_mock:
       assertDiracSucceeds(self.dilc.checkInputSandboxLFNs(job_mock), self)
       replica_mock.assert_called_once_with(['/some/file.txt'])
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/API/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/API/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/Utilities/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Agent/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Client/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/DB/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/Service/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/OverlaySystem/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/OverlaySystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Calibration.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/CheckCollections.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/DummyModule.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/DummyModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 from DIRAC.Core.Utilities.Subprocess import shellCall
 from DIRAC import S_OK, S_ERROR, gLogger
 from ILCDIRAC.Core.Utilities.CombinedSoftwareInstallation import getEnvironmentScript
 from ILCDIRAC.Core.Utilities.resolvePathsAndNames import resolveIFpaths, getProdFilename
 from ILCDIRAC.Workflow.Modules.ModuleBase import ModuleBase
 from ILCDIRAC.Workflow.Utilities.DD4hepMixin import DD4hepMixin
+from ILCDIRAC.Core.Utilities.PrepareOptionFiles import preparePythia8Card
 
 
 __RCSID__ = '$Id$'
 LOG = gLogger.getSubLogger(__name__)
 
 
 class GaudiAppModule(DD4hepMixin, ModuleBase):
@@ -47,19 +48,22 @@
     self.enable = True
     self.STEP_NUMBER = ''
     self.result = S_ERROR()
     self.applicationName = 'gaudiapp'
     self.executableName = ''
     self.startFrom = 0
     self.randomSeed = -1
+    self.randomSeedFlag = ''
     self.inputFileFlag = ''
     self.outputFileFlag = ''
     self.compactFile = ''
     self.detectorModel = ''
     self.detectorModelFlag = '--GeoSvc.detectors'
+    self.pythia8CardContent = ''
+    self.pythia8Card = 'pythia8card.cmd'
     self.eventstring = ['+++ Initializing event']  # FIXME
 
   def applicationSpecificInputs(self):
     """Resolve all input variables for the module here.
 
     :return: S_OK()
     """
@@ -82,17 +86,18 @@
         self.InputFile.append(files)
         LOG.info('Found input files', self.InputFile)
     return S_OK('Parameters resolved')
 
   def runIt(self):
     """Execute the following:
 
-    - find the detector model xml, using CS query to obtain the path
-    - prepare the steering file and command line parameters
-    - run GaudiApp on this steering file and catch the exit status
+    - if necessary find the detector model xml, using CS query to obtain the path
+    - if necessary prepare the pythia card
+    - prepare the run script using the input parameters
+    - run GaudiApp on the steering eventually using the prepared pythia card and/or the input files
 
     :returns: :func:`~DIRAC.Core.Utilities.ReturnValues.S_OK`, :func:`~DIRAC.Core.Utilities.ReturnValues.S_ERROR`
     """
     self.result = S_OK()
     if not self.platform:
       self.result = S_ERROR('No ILC platform selected')
     elif not self.applicationLog:
@@ -142,14 +147,17 @@
 
     if self.NumberOfEvents:
       cmd.append("-n %s" % self.NumberOfEvents)
 
     if self.compactFile:
       cmd.append("%s %s" % (self.detectorModelFlag, self.compactFile))
 
+    if self.randomSeedFlag:
+      cmd.append("%s %s" % (self.randomSeedFlag, self.randomSeed))
+
     cmd.append("%s %s" % (self.outputFileFlag, self.OutputFile))
 
     scriptName = 'GaudiApp_%s_Run_%s.sh' % (self.applicationVersion, self.STEP_NUMBER)
     if os.path.exists(scriptName):
       os.remove(scriptName)
     script = []
     script.append('#!/bin/bash')
@@ -178,14 +186,19 @@
 
     with open(scriptName, 'w') as scriptFile:
       scriptFile.write("\n".join(script))
 
     if os.path.exists(self.applicationLog):
       os.remove(self.applicationLog)
 
+    if self.pythia8CardContent:
+      res = preparePythia8Card(self.pythia8CardContent, self.NumberOfEvents, self.randomSeed, self.pythia8Card)
+      if not res['OK']:
+        return res
+    
     os.chmod(scriptName, 0o755)
     comm = 'bash "./%s"' % scriptName
     self.setApplicationStatus('GaudiApp %s step %s' % (self.applicationVersion, self.STEP_NUMBER))
     self.stdError = ''
     self.result = shellCall(0, comm, callbackFunction=self.redirectLogOutput, bufferLimit=20971520)
     resultTuple = self.result['Value']
     if not os.path.exists(self.applicationLog):
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ModuleBase.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ModuleBase.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/MoveInFC.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/MoveInFC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/OverlayInput.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/ReportErrors.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/ReportErrors.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/StdHepCut.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,25 @@
   """Remove files after run."""
   try:
     shutil.rmtree(tempdir)
   except OSError:
     pass
 
 
+def getFileReportMock():
+  fr_mock = Mock()
+  fr_mock.getFiles.return_value = {
+    "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0000.stdhep": "ApplicationCrash",
+    "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0001.stdhep": "ARG"}
+  fr_mock.setFileStatus.return_value = {'OK': True, 'Value': ''}
+  fr_mock.commit.return_value = {'OK': True, 'Value': ''}
+  fr_mock.generateRequest.return_value = {'OK': True, 'Value': ''}
+  return fr_mock
+
+
 class ModulesTestCase (unittest.TestCase):
   """ILCDirac version of Workflow module tests."""
 
   @patch("%s.ModuleBase.getProxyInfoAsString" % MODULE_NAME, new=Mock(return_value=S_OK()))
   @patch("DIRAC.Core.Security.ProxyInfo.getProxyInfoAsString", new=Mock(return_value=S_OK()))
   @patch("%s.ModuleBase.Operations" % MODULE_NAME, new=Mock())
   @patch("%s.UploadLogFile.StorageElement" % MODULE_NAME, new=Mock(return_value=S_OK()))
@@ -98,22 +109,14 @@
     self.jr_mock = Mock()
     self.jr_mock.setApplicationStatus.return_value = {'OK': True, 'Value': ''}
     self.jr_mock.generateRequest.return_value = {'OK': True, 'Value': 'pippo'}
     self.jr_mock.setJobParameter.return_value = {'OK': True, 'Value': 'pippo'}
     self.jr_mock.generateForwardDISET.return_value = {'OK': True, 'Value': 'pippo'}
 #    self.jr_mock.setJobApplicationStatus.return_value = {'OK': True, 'Value': 'pippo'}
 
-    self.fr_mock = Mock()
-    self.fr_mock.getFiles.return_value = {
-        "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0000.stdhep": "ApplicationCrash",
-        "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0001.stdhep": "ARG"}
-    self.fr_mock.setFileStatus.return_value = {'OK': True, 'Value': ''}
-    self.fr_mock.commit.return_value = {'OK': True, 'Value': ''}
-    self.fr_mock.generateRequest.return_value = {'OK': True, 'Value': ''}
-
     self.rm_mock = Mock()
     self.rm_mock.getReplicas.return_value = {'OK': True, 'Value': {'Successful': {'pippo': 'metadataPippo'},
                                                                    'Failed': None}}
     self.rm_mock.getCatalogFileMetadata.return_value = {'OK': True, 'Value': {'Successful': {'pippo': 'metadataPippo'},
                                                                               'Failed': None}}
     self.rm_mock.removeFile.return_value = {'OK': True, 'Value': {'Failed': False}}
     self.rm_mock.putStorageDirectory.return_value = {'OK': True, 'Value': {'Failed': False}}
@@ -142,15 +145,15 @@
                         'outputDataFileMask': '',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'numberOfEvents': '100',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'runNumber': 'Unknown',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
                         'JOB_ID': str(self.prod_job_id),
                         'configName': 'aConfigName',
                         'configVersion': 'aConfigVersion',
@@ -158,15 +161,15 @@
                         'jobType': 'merge',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'numberOfEvents': '100',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'runNumber': 'Unknown',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
                         'JOB_ID': str(self.prod_job_id),
                         'configName': 'aConfigName',
@@ -175,15 +178,15 @@
                         'jobType': 'merge',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'numberOfEvents': '100',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'LogTargetPath': 'someOtherDir',
                         'runNumber': 'Unknown',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
                         'JOB_ID': str(self.prod_job_id),
@@ -193,15 +196,15 @@
                         'jobType': 'merge',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'numberOfEvents': '100',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'LogTargetPath': 'someOtherDir',
                         'runNumber': 'Unknown',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
                         'JOB_ID': str(self.prod_job_id),
@@ -210,30 +213,30 @@
                         'outputDataFileMask': '',
                         'jobType': 'reco',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'runNumber': 'Unknown',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
                         'JOB_ID': str(self.prod_job_id),
                         'configName': 'aConfigName',
                         'configVersion': 'aConfigVersion',
                         'outputDataFileMask': '',
                         'jobType': 'reco',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'runNumber': 'Unknown',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
                         'JOB_ID': str(self.prod_job_id),
                         'configName': 'aConfigName',
@@ -241,15 +244,15 @@
                         'outputDataFileMask': '',
                         'jobType': 'reco',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'LogTargetPath': 'someOtherDir',
                         'runNumber': 'Unknown',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
                         'JOB_ID': str(self.prod_job_id),
@@ -258,15 +261,15 @@
                         'outputDataFileMask': '',
                         'jobType': 'reco',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'LogTargetPath': 'someOtherDir',
                         'runNumber': 'Unknown',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
                         'JOB_ID': str(self.prod_job_id),
@@ -275,15 +278,15 @@
                         'outputDataFileMask': '',
                         'jobType': 'reco',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'LogTargetPath': 'someOtherDir',
                         'runNumber': 'Unknown',
                         'InputData': '',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
@@ -293,15 +296,15 @@
                         'outputDataFileMask': '',
                         'jobType': 'reco',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'LogTargetPath': 'someOtherDir',
                         'runNumber': 'Unknown',
                         'InputData': 'foo;bar',
                         'appSteps': ['someApp_1']},
                        {'PRODUCTION_ID': str(self.prod_id),
@@ -311,15 +314,15 @@
                         'outputDataFileMask': '',
                         'jobType': 'reco',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'LogTargetPath': 'someOtherDir',
                         'runNumber': 'Unknown',
                         'InputData': 'foo;bar',
                         'ParametricInputData': '',
                         'appSteps': ['someApp_1']},
@@ -330,15 +333,15 @@
                         'outputDataFileMask': '',
                         'jobType': 'reco',
                         'BookkeepingLFNs': 'aa',
                         'ProductionOutputData': 'ProductionOutputData',
                         'JobReport': self.jr_mock,
                         'Request': self.rc_mock,
                         'AccountingReport': self.ar_mock,
-                        'FileReport': self.fr_mock,
+                        'FileReport': getFileReportMock(),
                         'SystemConfig': 'sys_config',
                         'LogFilePath': 'someDir',
                         'LogTargetPath': 'someOtherDir',
                         'runNumber': 'Unknown',
                         'InputData': 'foo;bar',
                         'ParametricInputData': 'pid1;pid2;pid3',
                         'appSteps': ['someApp_1']},
@@ -390,15 +393,15 @@
     self.step_number = '321'
     self.step_id = '%s_%s_%s' % (self.prod_id, self.prod_job_id, self.step_number)
 
     self.mbase = ModuleBase()
     self.mbase.rm = self.rm_mock
     self.mbase.request = self.rc_mock
     self.mbase.jobReport = self.jr_mock
-    self.mbase.fileReport = self.fr_mock
+    self.mbase.fileReport = getFileReportMock()
     self.mbase.workflow_commons = self.wf_commons[0]
     self.mbase.workflow_commons['LogFilePath'] = "/ilc/user/s/sailer/test/dummy/folder"
     self.mbase.workflow_commons['Platform'] = "x86_64-slc5-gcc43-opt"
     self.mbase.log = gLogger.getSubLogger("ModuleBaseTest")
     self.mbase.log.showHeaders(True)
     self.mbase.ignoreapperrors = False
     self.uod = UploadOutputData()
@@ -1078,15 +1081,15 @@
     self.frq.applicationSpecificInputs()
     self.assertFalse(self.frq.enable)
 
   def test_ASI_AllVariables(self):
     """applicationSpecificInputs: checks if all variables have been properly set after this call...."""
     gLogger.setLevel("ERROR")
     self.frq = FailoverRequest()
-    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=self.fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
+    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=getFileReportMock(), PRODUCTION_ID=43321, JOB_ID=12345)
     os.environ['JOBID'] = "12345"
     self.frq.applicationSpecificInputs()
     del os.environ['JOBID']
     self.assertTrue(self.frq.jobReport and self.frq.fileReport
                      and self.frq.productionID and self.frq.prodJobID and self.frq.enable)
 
   def test_ASI_NoVariables(self):
@@ -1102,118 +1105,126 @@
 
   def test_Exe_Disabled(self):
     """execute: is disabled........................................................................."""
     gLogger.setLevel("ERROR")
     self.frq = FailoverRequest()
     self.frq._getJobReporter = Mock(return_value=self.jr_mock)
     self.frq.log = gLogger.getSubLogger("Frq-Exe-Disabled")
-    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=self.fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
+    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=getFileReportMock(), PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.enable = False
     self.frq.workflow_commons = dict()
     res = self.frq.execute()
     self.assertIn("Module is disabled", res['Value'])
 
   def test_Exe_WFFail(self):
     """execute: WF Failed..........................................................................."""
     gLogger.setLevel("ERROR")
     self.frq = FailoverRequest()
     self.frq.log = gLogger.getSubLogger("Frq-Exe-Fail")
     self.frq.applicationSpecificInputs = Mock(return_value=S_OK())
     self.jr_mock.generateForwardDISET = Mock(return_value=S_ERROR("EKKE"))
     self.frq.enable = True
     self.frq.jobID = 12345
-    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=self.fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
+    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=getFileReportMock(), PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.workflowStatus = S_ERROR()
     res = self.frq.execute()
     self.assertFalse(res['OK'])
 
   def test_Exe_RIV_Failes(self):
     """execute: WF Failed..........................................................................."""
     gLogger.setLevel("ERROR")
     self.frq = FailoverRequest()
+    fr_mock = getFileReportMock()
+    self.frq.fileReport = fr_mock
     self.frq.log = gLogger.getSubLogger("Frq-Exe-Fail")
     self.frq.resolveInputVariables = Mock(return_value=S_ERROR("EKKE: no input variables"))
     self.frq.applicationSpecificInputs = Mock(return_value=S_OK())
     self.jr_mock.generateForwardDISET = Mock(return_value=S_ERROR("EKKE"))
     self.frq.enable = True
     self.frq.jobID = 12345
-    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=self.fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
+    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.workflowStatus = S_ERROR()
     res = self.frq.execute()
     self.assertFalse(res['OK'])
 
   def test_Exe_Success(self):
     """execute: succeeds............................................................................"""
     gLogger.setLevel("ERROR")
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       self.frq = FailoverRequest()
+    fr_mock = getFileReportMock()
+    self.frq.fileReport = fr_mock
     self.frq.log = gLogger.getSubLogger("Frq-Exe-Succeed")
     self.frq.applicationSpecificInputs = Mock(return_value=S_OK())
+    self.frq.productionID = 43321
     self.frq.jobID = 12345
-    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=self.fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
+    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.workflow_commons['Request'] = self.rc_mock
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       res = self.frq.execute()
     self.assertTrue(res['OK'])
 
   def test_Exe_Success_input(self):
     """execute: succeeds inputdata.................................................................."""
     gLogger.setLevel("ERROR")
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       self.frq = FailoverRequest()
-    self.frq.fileReport = self.fr_mock
+    fr_mock = getFileReportMock()
+    self.frq.fileReport = fr_mock
     self.frq.log = gLogger.getSubLogger("Frq-Exe-Succeed")
     self.frq.InputData = ["/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0000.stdhep"]
     self.frq.productionID = 43321
     self.frq.applicationSpecificInputs = Mock(return_value=S_OK())
     self.frq.jobID = 12345
-    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=self.fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
+    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.workflow_commons['Request'] = self.rc_mock
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       res = self.frq.execute()
     self.assertTrue(res['OK'])
 
   def test_Exe_Success_input_no(self):
     """execute: succeeds inputdata.................................................................."""
     gLogger.setLevel("ERROR")
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       self.frq = FailoverRequest()
-    self.frq.fileReport = self.fr_mock
+    fr_mock = getFileReportMock()
+    self.frq.fileReport = fr_mock
     self.frq.log = gLogger.getSubLogger("Frq-Exe-Succeed")
     self.frq.InputData = ["/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0000.stdhep",
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0001.stdhep",
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0002.stdhep",
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0003.stdhep",
                          ]
     self.frq.productionID = 43321
     self.frq.applicationSpecificInputs = Mock(return_value=S_OK())
     self.frq.jobID = 12345
-    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=self.fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
+    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.workflow_commons['Request'] = self.rc_mock
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       res = self.frq.execute()
     self.assertTrue(res['OK'])
 
   def test_Exe_statusFalse(self):
     """execute: workflowStatus not OK..............................................................."""
     gLogger.setLevel("ERROR")
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       self.frq = FailoverRequest()
-    self.frq.fileReport = self.fr_mock
+    fr_mock = getFileReportMock()
+    self.frq.fileReport = fr_mock
     self.frq.log = gLogger.getSubLogger("Frq-Exe-Succeed")
     self.frq.InputData = ["/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0000.stdhep",
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0001.stdhep",
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0002.stdhep",
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0003.stdhep",
                          ]
     self.frq.productionID = 43321
     self.frq.applicationSpecificInputs = Mock(return_value=S_OK())
     self.frq.jobID = 12345
     self.frq.workflowStatus['OK'] = False
-    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=self.fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
+    self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.workflow_commons['Request'] = self.rc_mock
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       res = self.frq.execute()
     self.assertTrue(not res['OK'])
 
   def test_Exe_statusFalse_diset_err(self):
     """execute: workflowStatus not OK diset error..................................................."""
@@ -1227,15 +1238,15 @@
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0003.stdhep",
                          ]
     self.frq.productionID = 43321
     self.frq.applicationSpecificInputs = Mock(return_value=S_OK())
     self.frq.jobID = 12345
     self.frq.workflowStatus['OK'] = False
     self.frq.jobType = "NotSplit"
-    fr_mock = Mock(self.fr_mock)
+    fr_mock = getFileReportMock()
     fr_mock.commit.return_value = S_ERROR()
     fr_mock.generateForwardDISET = Mock(return_value=S_ERROR("EKKE"))
     self.frq.fileReport = fr_mock
     self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.workflow_commons['Request'] = self.rc_mock
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       res = self.frq.execute()
@@ -1252,15 +1263,15 @@
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0002.stdhep",
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0003.stdhep",
                          ]
     self.frq.productionID = 43321
     self.frq.applicationSpecificInputs = Mock(return_value=S_OK())
     self.frq.jobID = 12345
     self.frq.workflowStatus['OK'] = False
-    fr_mock = Mock(self.fr_mock)
+    fr_mock = getFileReportMock()
     fr_mock.commit.return_value = S_ERROR()
     fr_mock.generateForwardDISET = Mock(return_value=S_OK(None))
     self.frq.fileReport = fr_mock
     self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.workflow_commons['Request'] = self.rc_mock
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       res = self.frq.execute()
@@ -1278,15 +1289,15 @@
                           "/ilc/prod/clic/1.4tev/h_nunu/GEN/00004191/000/h_nunu_gen_4191_0003.stdhep",
                          ]
     self.frq.productionID = 43321
     self.frq.applicationSpecificInputs = Mock(return_value=S_OK())
     self.frq.jobID = 12345
     self.frq.generateFailoverFile = Mock(return_value=S_ERROR("No can do"))
     self.frq.workflowStatus['OK'] = False
-    fr_mock = Mock(self.fr_mock)
+    fr_mock = getFileReportMock()
     fr_mock.commit.return_value = S_ERROR()
     fr_mock.generateForwardDISET = Mock(return_value=S_OK(None))
     self.frq.fileReport = fr_mock
     self.frq.workflow_commons = dict(JobReport=self.jr_mock, FileReport=fr_mock, PRODUCTION_ID=43321, JOB_ID=12345)
     self.frq.workflow_commons['Request'] = self.rc_mock
     with patch("%s.ModuleBase.RequestValidator" % MODULE_NAME, Mock()):
       res = self.frq.execute()
@@ -1313,15 +1324,15 @@
     """execute: test if setRegistrationRequest succeeds ............................................"""
     # setup the filedict from getFileMetaData and pass that to setRegistrationRequest
     gLogger.setLevel("ERROR")
     self.uod = UploadOutputData()
     self.uod.prodOutputLFNs = ['/ilc/user/s/sailer/test3.stdhep']
     self.uod.jobReport = Mock()
     self.uod.jobReport.generateForwardDISET.return_value = S_ERROR("No JobRep")
-    self.uod.fileReport = self.fr_mock
+    self.uod.fileReport = getFileReportMock()
     self.uod.workflow_commons = dict(Enable=True, PRODUCTION_ID=43321, JOB_ID=12345)
 
     candidateFiles = {'test3.stdhep': {'lfn': '/ilc/user/s/sailer/test3.stdhep', 'workflowSE': 'CERN-DIP-4'}}
     self.uod.getCandidateFiles = Mock(return_value=S_OK())
     res = self.uod.getFileMetadata(candidateFiles)
     fileDict = res['Value']
     self.uod.getFileMetadata = Mock(return_value=res)
@@ -1381,15 +1392,15 @@
     self.uod.applicationSpecificInputs()
     self.assertFalse(self.uod.enable)
 
   def test_ASI_AllVariables(self):
     """UOD.applicationSpecificInputs: checks if all variables have been properly set after this call"""
     gLogger.setLevel("ERROR")
     self.uod = UploadOutputData()
-    self.uod.workflow_commons = dict(JobReport=self.jr_mock, FileReport=self.fr_mock, PRODUCTION_ID=43321,
+    self.uod.workflow_commons = dict(JobReport=self.jr_mock, FileReport=getFileReportMock(), PRODUCTION_ID=43321,
                                       JOB_ID=12345,
                                       outputList=[{'outputFile': 'myFile_gen.stdhep'},
                                                     {'outputFile': 'myFile_dst.slcio'},
                                                     {'outputFile': 'myFile_sim.slcio'},
                                                     {'outputFile': 'myFile_rec.slcio'},
                                                     {'outputFile': 'myFile_unk.slcio'}
                                                    ],
```

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Modules/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Modules/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Utilities/RootMixin.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/RootMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/Utilities/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/Workflow/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/Workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/WorkloadManagementSystem/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/WorkloadManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a3/src/ILCDIRAC/__init__.py` & `iLCDirac-34.0.0a4/src/ILCDIRAC/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,12 +61,12 @@
 
 def extension_metadata():
   """Extension metadata for ILCDIRAC bootstrap."""
   return {
       "primary_extension": True,
       "priority": 100,
       "setups": {
-          "ILC-Production": "dips://voilcdiraconfig.cern.ch:9135/Configuration/Server",
-          "ILC-Certification": "dips://voilcdiraconfig.cern.ch:9135/Configuration/Server",
+          "ILC-Production": "dips://voilcdiracconfig.cern.ch:9135/Configuration/Server",
+          "ILC-Certification": "dips://voilcdiracconfig.cern.ch:9135/Configuration/Server",
           },
       "default_setup": "ILC-Production",
       }
```

### Comparing `iLCDirac-34.0.0a3/src/iLCDirac.egg-info/PKG-INFO` & `iLCDirac-34.0.0a4/src/iLCDirac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iLCDirac
-Version: 34.0.0a3
+Version: 34.0.0a4
 Summary: iLCDirac is the iLC/CLIC/FCC extension of DIRAC
 Home-page: https://gitlab.cern.ch/clicdp/ilcdirac/ilcdirac.git
 Maintainer: Andre Sailer
 Maintainer-email: ilcdirac-support@cern.ch
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://its.cern.ch/jira/browse/ILCDIRAC
 Project-URL: Documentation, https://ilcdirac-doc.web.cern.ch/
```

### Comparing `iLCDirac-34.0.0a3/src/iLCDirac.egg-info/SOURCES.txt` & `iLCDirac-34.0.0a4/src/iLCDirac.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,15 @@
 src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py
 src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py
 src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py
+src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py
@@ -265,15 +266,17 @@
 src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py
+src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py
+src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py
 src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py
@@ -322,14 +325,15 @@
 src/ILCDIRAC/Workflow/Modules/AnalyseWN.py
 src/ILCDIRAC/Workflow/Modules/ApplicationScript.py
 src/ILCDIRAC/Workflow/Modules/Calibration.py
 src/ILCDIRAC/Workflow/Modules/CheckCollections.py
 src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py
 src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py
 src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py
+src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py
 src/ILCDIRAC/Workflow/Modules/DummyModule.py
 src/ILCDIRAC/Workflow/Modules/FailoverRequest.py
 src/ILCDIRAC/Workflow/Modules/FccAnalysis.py
 src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py
 src/ILCDIRAC/Workflow/Modules/GetSRMFile.py
 src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py
 src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py
@@ -361,15 +365,17 @@
 src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py
 src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py
 src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py
 src/ILCDIRAC/Workflow/Modules/__init__.py
 src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py
+src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py
+src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py
 src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py
```

### Comparing `iLCDirac-34.0.0a3/src/iLCDirac.egg-info/entry_points.txt` & `iLCDirac-34.0.0a4/src/iLCDirac.egg-info/entry_points.txt`

 * *Files identical despite different names*

