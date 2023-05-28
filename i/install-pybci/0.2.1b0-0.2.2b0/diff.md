# Comparing `tmp/install-pybci-0.2.1b0.tar.gz` & `tmp/install-pybci-0.2.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.2.1b0.tar", last modified: Sat May 27 02:47:17 2023, max compression
+gzip compressed data, was "install-pybci-0.2.2b0.tar", last modified: Sun May 28 22:40:20 2023, max compression
```

## Comparing `install-pybci-0.2.1b0.tar` & `install-pybci-0.2.2b0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.972166 install-pybci-0.2.1b0/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.972166 install-pybci-0.2.1b0/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.972166 install-pybci-0.2.1b0/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.020716 install-pybci-0.2.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-28 22:40:20.016715 install-pybci-0.2.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.012715 install-pybci-0.2.2b0/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-28 22:40:19.000000 install-pybci-0.2.2b0/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-28 22:40:20.000000 install-pybci-0.2.2b0/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 22:40:19.000000 install-pybci-0.2.2b0/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-28 22:40:19.000000 install-pybci-0.2.2b0/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 22:40:20.000000 install-pybci-0.2.2b0/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.012715 install-pybci-0.2.2b0/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.016715 install-pybci-0.2.2b0/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.016715 install-pybci-0.2.2b0/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.016715 install-pybci-0.2.2b0/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 22:40:20.020716 install-pybci-0.2.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/setup.py
```

### Comparing `install-pybci-0.2.1b0/LICENSE` & `install-pybci-0.2.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.1b0/PKG-INFO` & `install-pybci-0.2.2b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.1b0
+Version: 0.2.2b0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -18,19 +18,19 @@
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
@@ -74,11 +74,14 @@
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - ~~Combine multiple data streams for multi modal bci!~~
-- Add pytorch compatibility! 
+- ~~Add pytorch compatibility!~~ 
+- run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo]
 - Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
+- Levels of print debug (info, error, none)
+- Retrieve feature data  
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.1b0/README.md` & `install-pybci-0.2.2b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
@@ -50,11 +50,14 @@
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - ~~Combine multiple data streams for multi modal bci!~~
-- Add pytorch compatibility! 
+- ~~Add pytorch compatibility!~~ 
+- run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo]
 - Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
+- Levels of print debug (info, error, none)
+- Retrieve feature data  
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.1b0/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.2.2b0/install_pybci.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.1b0
+Version: 0.2.2b0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -18,19 +18,19 @@
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
@@ -74,11 +74,14 @@
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - ~~Combine multiple data streams for multi modal bci!~~
-- Add pytorch compatibility! 
+- ~~Add pytorch compatibility!~~ 
+- run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo]
 - Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
+- Levels of print debug (info, error, none)
+- Retrieve feature data  
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.1b0/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.2.2b0/install_pybci.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 pybci/ThreadClasses/DataReceiverThread.py
 pybci/ThreadClasses/FeatureProcessorThread.py
 pybci/ThreadClasses/MarkerThread.py
 pybci/ThreadClasses/__init__.py
 pybci/Utils/Classifier.py
 pybci/Utils/FeatureExtractor.py
 pybci/Utils/LSLScanner.py
+pybci/Utils/Logger.py
 pybci/Utils/__init__.py
```

### Comparing `install-pybci-0.2.1b0/pybci/Configuration/EpochSettings.py` & `install-pybci-0.2.2b0/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.1b0/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.2.2b0/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,14 @@
                     del sample[index] # remove the desired channels from the sample
                 for i,fifo in enumerate(dataFIFOs):
                     fifo.append((timestamp, sample[i]))
                 if self.trainTestEvent.is_set(): # We're training!
                     if self.startCounting: # we received a marker
                         posCount += 1
                         if posCount >= self.desiredCount:  # enough samples are in FIFO, chop up and put in dataqueue
-                            start = time.time()
-
                             if len(self.customEpochSettings.keys())>0: #  custom marker received
                                 if self.customEpochSettings[self.currentMarker].splitCheck: # slice epochs into overlapping time windows
                                     window_length = self.customEpochSettings[self.currentMarker].windowLength
                                     window_overlap = self.customEpochSettings[self.currentMarker].windowOverlap
                                     window_start_time = self.markerTimestamp + self.customEpochSettings[self.currentMarker].tmin
                                     window_end_time = window_start_time + window_length
                                     while window_end_time <= self.markerTimestamp + self.customEpochSettings[self.currentMarker].tmax:
@@ -89,16 +87,14 @@
                                     self.startCounting = False
                                 else: # don't slice just take tmin to tmax time
                                     start_time = self.markerTimestamp + self.globalEpochSettings.tmin
                                     end_time = self.markerTimestamp + self.globalEpochSettings.tmax
                                     sliceDataFIFOs = [slice_fifo_by_time(fifo, start_time, end_time) for fifo in dataFIFOs]
                                     self.dataQueueTrain.put([sliceDataFIFOs, self.currentMarker, self.sr, self.devCount])
                             # reset flags and counters
-                            end = time.time()
-                            print(f"Data slicing process time {end - start}")
                             posCount = 0
                             self.startCounting = False
                 else: # in Test mode
                     if self.globalEpochSettings.splitCheck:
                         window_length = self.globalEpochSettings.windowLength
                         window_overlap = self.globalEpochSettings.windowOverlap
                     else:
@@ -111,24 +107,20 @@
                         #sliceDataFIFOs = [list(itertools.islice(d, fifoLength-window_samples, fifoLength)) for d in dataFIFOs]
                         if self.globalEpochSettings.splitCheck:
                             window_end_time += window_length * (1 - window_overlap)
                         else:
                             window_end_time = timestamp + window_length
             else:
                 pass
-                # add levels of debug 
-                # print("PyBCI: LSL pull_sample timed out, no data on stream...")
-
+                # add levels of debug?
 
     def ReceiveMarker(self, marker, timestamp): # timestamp will be used for non sample rate specific devices (pupil-labs gazedata)
-        #print(marker)
         if self.startCounting == False: # only one marker at a time allow, other in windowed timeframe ignored
             self.currentMarker = marker
             self.markerTimestamp = timestamp
             if len(self.customEpochSettings.keys())>0: #  custom marker received
                 if marker in self.customEpochSettings.keys():
                     self.desiredCount = int(self.customEpochSettings[marker].tmax * self.sr) # find number of samples after tmax to finish counting
                     self.startCounting = True
             else: # no custom markers set, use global settings
                 self.desiredCount = int(self.globalEpochSettings.tmax * self.sr) # find number of samples after tmax to finish counting
                 self.startCounting = True
-            #print(self.desiredCount)
```

### Comparing `install-pybci-0.2.1b0/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.2.2b0/pybci/ThreadClasses/ClassifierThread.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from ..Utils.Classifier import Classifier 
+from ..Utils.Logger import Logger
 import queue,threading, time
 
 class ClassifierThread(threading.Thread):
     features = []
     targets = []
     mode = "train"
     guess = None
     epochCounts = {} 
     def __init__(self, closeEvent,trainTestEvent, featureQueueTest,featureQueueTrain, classifierInfoQueue, classifierInfoRetrieveEvent, 
-                 classifierGuessMarkerQueue, classifierGuessMarkerEvent, printDebug = True, numStreamDevices = 1,
+                 classifierGuessMarkerQueue, classifierGuessMarkerEvent, logger = Logger(Logger.INFO), numStreamDevices = 1,
                  minRequiredEpochs = 10, clf = None, model = None, torchModel = None):
         super().__init__()
         self.trainTestEvent = trainTestEvent # responsible for tolling between train and test mode
         self.closeEvent = closeEvent # responsible for cosing threads
         self.featureQueueTest = featureQueueTest # gets feature data from feature processing thread
         self.featureQueueTrain = featureQueueTrain # gets feature data from feature processing thread
         self.classifier = Classifier(clf = clf, model = model, torchModel = torchModel) # sets classifier class, if clf and model passed, defaults to clf and sklearn
         self.minRequiredEpochs = minRequiredEpochs # the minimum number of epochs required for classifier attempt
         self.classifierInfoRetrieveEvent = classifierInfoRetrieveEvent
         self.classifierInfoQueue = classifierInfoQueue
         self.classifierGuessMarkerQueue = classifierGuessMarkerQueue
         self.classifierGuessMarkerEvent = classifierGuessMarkerEvent
         self.numStreamDevices = numStreamDevices
-        self.printDebug = printDebug
+        self.logger = logger
 
     def run(self):
         if self.numStreamDevices > 1:
             tempdatatrain = {}
             tempdatatest = {}
         while not self.closeEvent.is_set():
             if self.trainTestEvent.is_set(): # We're training!
@@ -44,65 +45,62 @@
                             #print(flattened_list)
                             self.targets.append(target)
                             self.features.append(flattened_list)
 
                         # need to check if all device data is captured, then flatten and append
                             if len(self.epochCounts) > 1: # check if there is more then one test condition
                                 minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
-                                #print("minNumKeyEpochs"+str(minNumKeyEpochs))
                                 if minNumKeyEpochs < self.minRequiredEpochs:
                                     pass
                                 else: 
                                     start = time.time()
                                     self.classifier.TrainModel(self.features, self.targets)
-                                    if (self.printDebug):
+                                    if (self.logger.level == Logger.INFO):
                                         end = time.time()
-                                        print(f"PyBCI: Info - classifier training time {end - start}")
+                                        self.logger.log(Logger.INFO, f" classifier training time {end - start}")
                             if self.classifierGuessMarkerEvent.is_set():
                                 self.classifierGuessMarkerQueue.put(None)
                     else:
                         self.targets.append(target)
                         self.features.append(featuresSingle)
                         if len(self.epochCounts) > 1: # check if there is more then one test condition
                             minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
-                            #print("minNumKeyEpochs"+str(minNumKeyEpochs))
                             if minNumKeyEpochs < self.minRequiredEpochs:
                                 pass
                             else: 
                                 start = time.time()
                                 self.classifier.TrainModel(self.features, self.targets)
-                                if (self.printDebug):
+                                if (self.logger.level == Logger.INFO):
                                     end = time.time()
-                                    print(f"PyBCI: Info - classifier training time {end - start}")
+                                    self.logger.log(Logger.INFO, f" classifier training time {end - start}")
                         if self.classifierGuessMarkerEvent.is_set():
                             self.classifierGuessMarkerQueue.put(None)
                 except queue.Empty:
                     pass
             else: # We're testing!
                 try:
                     featuresSingle, devCount = self.featureQueueTest.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
                     if self.numStreamDevices > 1:
                         tempdatatest[devCount] = featuresSingle
                         if len(tempdatatest) == self.numStreamDevices:
                             flattened_list = []
                             for value in tempdatatest.values():
                                 flattened_list.extend(value)
                             tempdatatest = {}
-                            #self.features.append(flattened_list)
                             start = time.time()
                             self.guess = self.classifier.TestModel(flattened_list)
-                            if (self.printDebug):
+                            if (self.logger.level == Logger.INFO):
                                 end = time.time()
-                                print(f"PyBCI: Info - classifier testing time {end - start}")
+                                self.logger.log(Logger.INFO, f" classifier testing time {end - start}")
                     else:
                         start = time.time()
                         self.guess = self.classifier.TestModel(featuresSingle)
-                        if (self.printDebug):
+                        if (self.logger.level == Logger.INFO):
                             end = time.time()
-                            print(f"PyBCI: Info - classifier testing time {end - start}")
+                            self.logger.log(Logger.INFO, f" classifier testing time {end - start}")
                     if self.classifierGuessMarkerEvent.is_set():
                         self.classifierGuessMarkerQueue.put(self.guess)
                 except queue.Empty:
                     pass
             if self.classifierInfoRetrieveEvent.is_set():
                 classdata = {
                     "clf":self.classifier.clf,
```

### Comparing `install-pybci-0.2.1b0/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.2.2b0/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import threading
-import time
 from collections import deque
 import itertools
 
 class DataReceiverThread(threading.Thread):
     """Responsible for receiving data from accepted LSL outlet, slices samples based on tmin+tmax basis, 
     starts counter for received samples after marker is received in ReceiveMarker.
     """
@@ -17,39 +16,36 @@
         self.dataQueueTrain = dataQueueTrain
         self.dataQueueTest = dataQueueTest
         self.dataStreamInlet = dataStreamInlet
         self.customEpochSettings = customEpochSettings
         self.globalEpochSettings = globalEpochSettings
         self.streamChsDropDict = streamChsDropDict
         self.sr = dataStreamInlet.info().nominal_srate()
-        #self.dataType = dataStreamInlet.info().type()
         self.devCount = devCount # used for tracking which device is sending data to feature extractor
         
     def run(self):
         posCount = 0
         chCount = self.dataStreamInlet.info().channel_count()
         maxTime = (self.globalEpochSettings.tmin + self.globalEpochSettings.tmax)
         if len(self.customEpochSettings.keys())>0:
             if  max([self.customEpochSettings[x].tmin + self.customEpochSettings[x].tmax for x in self.customEpochSettings]) > maxTime:
                 maxTime = max([self.customEpochSettings[x].tmin + self.customEpochSettings[x].tmax for x in self.customEpochSettings])
         fifoLength = int(self.dataStreamInlet.info().nominal_srate()*maxTime)
-        #print(fifoLength)
         dataFIFOs = [deque(maxlen=fifoLength) for ch in range(chCount - len(self.streamChsDropDict))]
         while not self.closeEvent.is_set():
             sample, timestamp = self.dataStreamInlet.pull_sample(timeout = 1)
             if sample != None:
                 for index in sorted(self.streamChsDropDict, reverse=True):
                     del sample[index] # remove the desired channels from the sample
                 for i,fifo in enumerate(dataFIFOs):
                     fifo.append(sample[i])
                 if self.trainTestEvent.is_set(): # We're training!
                     if self.startCounting: # we received a marker
                         posCount+=1
                         if posCount >= self.desiredCount:  # enough samples are in FIFO, chop up and put in dataqueue
-                            #start = time.time()
                             if len(self.customEpochSettings.keys())>0: #  custom marker received
                                 if self.customEpochSettings[self.currentMarker].splitCheck: # slice epochs in to overlapping time windows
                                     window_samples =int(self.customEpochSettings[self.currentMarker].windowLength * self.sr) #number of samples in each window
                                     increment = int((1-self.customEpochSettings[self.currentMarker].windowOverlap)*window_samples) # if windows overlap each other by how many samples
                                     while posCount - window_samples > 0:
                                         sliceDataFIFOs = [list(itertools.islice(d, posCount - window_samples, posCount)) for d in dataFIFOs]
                                         self.dataQueueTrain.put([sliceDataFIFOs, self.currentMarker, self.sr,  self.devCount])
@@ -86,21 +82,18 @@
                             posCount = int((1-self.globalEpochSettings.windowOverlap)*window_samples) # offset poscoutn based on window overlap 
                         else:
                             posCount = 0
                         self.dataQueueTest.put([sliceDataFIFOs, self.sr, self.devCount])
             else:
                 pass
                 # add levels of debug 
-                # print("PyBCI: LSL pull_sample timed out, no data on stream...")
 
     def ReceiveMarker(self, marker, timestamp): # timestamp will be used for non sample rate specific devices (pupil-labs gazedata)
-        #print(marker)
         if self.startCounting == False: # only one marker at a time allow, other in windowed timeframe ignored
             self.currentMarker = marker
             if len(self.customEpochSettings.keys())>0: #  custom marker received
                 if marker in self.customEpochSettings.keys():
                     self.desiredCount = int(self.customEpochSettings[marker].tmax * self.sr) # find number of samples after tmax to finish counting
                     self.startCounting = True
             else: # no custom markers set, use global settings
                 self.desiredCount = int(self.globalEpochSettings.tmax * self.sr) # find number of samples after tmax to finish counting
                 self.startCounting = True
-            #print(self.desiredCount)
```

### Comparing `install-pybci-0.2.1b0/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.2.2b0/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import threading, queue
 from ..Utils.FeatureExtractor import GenericFeatureExtractor
 from ..Configuration.EpochSettings import GlobalEpochSettings
-import time
-
 class FeatureProcessorThread(threading.Thread):
-
     tempDeviceEpochLogger = []
     def __init__(self, closeEvent, trainTestEvent, dataQueueTrain,dataQueueTest,
                 featureQueueTest,featureQueueTrain,  totalDevices,markerCountRetrieveEvent,markerCountQueue, customEpochSettings = {}, 
                 globalEpochSettings = GlobalEpochSettings(),
                 featureExtractor = GenericFeatureExtractor()):
         super().__init__()
         self.markerCountQueue = markerCountQueue
@@ -21,15 +18,14 @@
         self.featureExtractor = featureExtractor
         self.totalDevices = totalDevices
         self.markerCountRetrieveEvent = markerCountRetrieveEvent
         self.epochCounts = {}
         self.customEpochSettings = customEpochSettings
         self.globalWindowSettings = globalEpochSettings
         self.tempDeviceEpochLogger = [0 for x in range(self.totalDevices)]
-        
     def run(self):
         while not self.closeEvent.is_set():
             if self.markerCountRetrieveEvent.is_set():
                 self.markerCountQueue.put(self.epochCounts)
             if self.trainTestEvent.is_set(): # We're training!
                 try:
                     dataFIFOs, currentMarker, sr, devCount = self.dataQueueTrain.get_nowait() #[sliceDataFIFOs, self.currentMarker, self.sr, self.devCount
```

### Comparing `install-pybci-0.2.1b0/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.2.2b0/pybci/ThreadClasses/MarkerThread.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import threading
 
 class MarkerThread(threading.Thread):
     """Receives Marker on chosen lsl Marker outlet. Pushes marker to data threads for framing epochs, 
     also sends markers to featureprocessing thread for epoch counting and multiple device synchronisation.
-    
     """
     def __init__(self,closeEvent, trainTestEvent, markerStreamInlet, dataThreads, featureThreads):#, lock):
         super().__init__()
         self.trainTestEvent = trainTestEvent
         self.closeEvent = closeEvent
         self.markerStreamInlet = markerStreamInlet
         self.dataThreads = dataThreads
@@ -19,12 +18,11 @@
             if self.trainTestEvent.is_set(): # We're training!
                 if marker != None:
                     marker = marker[0]
                     for thread in self.dataThreads:
                         thread.ReceiveMarker(marker, timestamp)
                     for thread in self.featureThreads:
                         thread.ReceiveMarker(marker, timestamp)
-                    #self.featureThread.ReceiveMarker(marker, timestamp)
                 else:
                     pass
                     # add levels of debug 
                     # print("PyBCI: LSL pull_sample timed out, no marker on stream...")
```

### Comparing `install-pybci-0.2.1b0/pybci/Utils/Classifier.py` & `install-pybci-0.2.2b0/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.1b0/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.2.2b0/pybci/Utils/FeatureExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 class GenericFeatureExtractor():
 
     def __init__(self, freqbands = [[1.0, 4.0], [4.0, 8.0], [8.0, 12.0], [12.0, 20.0]], featureChoices = GeneralFeatureChoices()):
         super().__init__()
         self.freqbands = freqbands
         self.featureChoices = featureChoices
-        for key, value in self.featureChoices.__dict__.items():
-            print(f"{key} = {value}")
+        #for key, value in self.featureChoices.__dict__.items():
+        #    print(f"{key} = {value}")
         selFeats = sum([self.featureChoices.appr_entropy,
             self.featureChoices.perm_entropy,
             self.featureChoices.spec_entropy,
             self.featureChoices.svd_entropy,
             self.featureChoices.samp_entropy,
             self.featureChoices.rms,
             self.featureChoices.meanPSD,
@@ -42,15 +42,15 @@
         desired frequency bands average power.
         Inputs:
             epoch = 2D list or 2D numpy array [chs, samples]
             target = string of received marker type
             sr = samplerate of current device
         Returns:
             features = 2D numpy array of size (chs, (len(freqbands) + sum(True in self.featureChoices)))
-            target = same as input target
+            target = same as input target, can be useful for using a baseline number differently
         NOTE: Any channels with a constant value will generate warnings in any frequency based features (constant level == no frequency components).
         """
         #print(np.array(epoch).shape)
         numchs = len(epoch)
         features = np.zeros(numchs * self.numFeatures)
         for k, ch in enumerate(epoch):
             #ch = np.isnan(ch)
```

### Comparing `install-pybci-0.2.1b0/pybci/pybci.py` & `install-pybci-0.2.2b0/pybci/pybci.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,83 @@
 from .Utils.LSLScanner import LSLScanner
+from .Utils.Logger import Logger
 from .ThreadClasses.FeatureProcessorThread import FeatureProcessorThread
 from .ThreadClasses.DataReceiverThread import DataReceiverThread
 from .ThreadClasses.AsyncDataReceiverThread import AsyncDataReceiverThread
 from .ThreadClasses.MarkerThread import MarkerThread
 from .ThreadClasses.ClassifierThread import ClassifierThread
 from .Configuration.EpochSettings import GlobalEpochSettings, IndividualEpochSetting
 from .Configuration.FeatureSettings import GeneralFeatureChoices
 import queue, threading, copy
 import tensorflow as tf
-import torch
+#import torch
 import torch.nn as nn
-tf.get_logger().setLevel('ERROR')
+
+#tf.get_logger().setLevel('ERROR')
 
 class PyBCI:
-    printDebug = True   # boolean, used to toggle print statements from LSLScanner class
     globalEpochSettings = GlobalEpochSettings()
     customEpochSettings = {}
     minimumEpochsRequired = 10
     markerThread = []
     dataThreads = []
     streamChsDropDict= {}
     dataStreams = []
     markerStream = None
     connected = False
     epochCounts = {} # holds markers received, their target ids and number received of each
     classifierInformation = []
 
-    def __init__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, printDebug = True,
+    def __init__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, loggingLevel = Logger.INFO,
                  globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}, streamChsDropDict = {},
                  streamCustomFeatureExtract = {},
                  minimumEpochsRequired = 10, clf= None, model = None, torchModel = None):
         """
         The PyBCI object stores data from available lsl time series data streams (EEG, pupilometry, EMG, etc.)
         and holds a configurable number of samples based on lsl marker strings.
         If no marker strings are available on the LSL the class will close and return an error.
         Parameters:
         dataStreams (List of strings): Allows user to set custom acceptable EEG stream definitions, if None defaults to streamTypes scan
         markerStream (List of strings): Allows user to set custom acceptable Marker stream definitions, if None defaults to markerTypes scan
         streamTypes (List of strings): Allows user to set custom acceptable EEG type definitions, ignored if dataStreams not None
         markerTypes (List of strings): Allows user to set custom acceptable Marker type definitions, ignored if markerStream not None
-        printDebug (bool): If true prints LSLScanner debug information
+        loggingLevel (string): Sets PyBCI print level, ('info' prints all statements, 'warning' is only warning messages, and 'none' is no prints from PyBCI)
         globalEpochSettings (GlobalEpochSettings): Sets global timing settings for epochs.
         customEpochSettings (dict {marker name string:IndividualEpochSettings()}): Sets individual timing settings for epochs.
         streamChsDropDict (dict {datastream name string: list(ints)}): Keys for dict should be respective datastreams with corresponding list of which channels to drop.
         streamCustomFeatureExtract (dict {datastream type string: customClass()}): allows dict to be passed of datastream type with custom feature extractor class for analysing data.
         minimumEpochsRequired (Int): minimm number of required epochs before model fitting begins, must be of each type of received markers and mroe then 1 type of marker to classify.
         clf (ClassifierMixin): Allows custom Sklearn model to be passed.
         model (model):Allows custom tensorflow model to be passed.
+        torchmodel ([torchModel(), torch.nn.Module] ): Currently a list where first item is torchmodel analysis function, second is torch model, check pytorch example - likely to change
         """
         self.streamCustomFeatureExtract = streamCustomFeatureExtract
         self.globalEpochSettings = globalEpochSettings
         self.customEpochSettings = customEpochSettings
         self.streamChsDropDict = streamChsDropDict
         self.lslScanner = LSLScanner(self, dataStreams, markerStream,streamTypes, markerTypes)
-        self.printDebug = printDebug
-        #if self.printDebug == False:
+        self.loggingLevel = loggingLevel
+        self.logger = Logger(self.loggingLevel)
         self.ConfigureMachineLearning(minimumEpochsRequired,  clf, model, torchModel) # configure first, connect second
         self.Connect()
        
-    def __enter__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, printDebug = True,
+    def __enter__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, loggingLevel = Logger.INFO,
                  globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}, streamChsDropDict = {},
-                 freqbands = [[1.0, 4.0], [4.0, 8.0], [8.0, 12.0], [12.0, 20.0]], featureChoices = GeneralFeatureChoices()): # with bci
-        self.freqbands = freqbands
-        self.featureChoices = featureChoices
+                 streamCustomFeatureExtract = {},
+                 minimumEpochsRequired = 10, clf= None, model = None, torchModel = None): # with bci
+        """
+        Please look at PyBCI.__init__ (same setup and description)
+        """
+        self.streamCustomFeatureExtract = streamCustomFeatureExtract
         self.globalEpochSettings = globalEpochSettings
         self.customEpochSettings = customEpochSettings
         self.streamChsDropDict = streamChsDropDict
         self.lslScanner = LSLScanner(self, dataStreams, markerStream,streamTypes, markerTypes)
-        self.printDebug = printDebug
+        self.loggingLevel = loggingLevel
+        self.ConfigureMachineLearning(minimumEpochsRequired,  clf, model, torchModel) # configure first, connect second
         self.Connect()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.StopThreads()
 
     def Connect(self): # Checks valid data and markers streams are present, controls dependant functions by setting self.connected
         if self.lslScanner.CheckAvailableLSL():
@@ -81,24 +87,22 @@
         else:
             self.connected = False
             return False
 
     # set test and train boolean for changing  thread operation 
     def TrainMode(self):
         if self.connected:
-            if self.printDebug:
-                print("PyBCI: Started training...")
+            self.logger.log(Logger.INFO,"Started training...")
             self.trainTestEvent.set()
         else:
             self.Connect()
 
     def TestMode(self):
         if self.connected:
-            if self.printDebug:
-                print("PyBCI: Started testing...")
+            self.logger.log(Logger.INFO,"Started testing...")
             self.trainTestEvent.clear()
         else:
             self.Connect()
 
     # Get data from threads
     def CurrentClassifierInfo(self):
         if self.connected:
@@ -138,16 +142,15 @@
         self.closeEvent = threading.Event() # used for closing threads
         self.trainTestEvent = threading.Event()
         self.markerCountRetrieveEvent = threading.Event()
         self.classifierInfoRetrieveEvent = threading.Event()
         self.featureRetrieveEvent = threading.Event() # still needs coding
 
         self.trainTestEvent.set() # if set we're in train mode, if not we're in test mode, always start in train...
-        if self.printDebug:
-            print("PyBCI: Starting threads initialisation...")
+        self.logger.log(Logger.INFO," Starting threads initialisation...")
         # setup data thread
         self.dataThreads = []
         self.featureThreads = []
         for stream in self.dataStreams:
             self.dataQueueTrain = queue.Queue()
             self.dataQueueTest = queue.Queue()
 
@@ -182,81 +185,75 @@
             self.ft.start()
             self.featureThreads.append(dt)
         # marker thread requires data and feature threads to push new markers too
         self.markerThread = MarkerThread(self.closeEvent,self.trainTestEvent, self.markerStream,self.dataThreads, self.featureThreads)
         self.markerThread.start()
         self.classifierThread = ClassifierThread(self.closeEvent,self.trainTestEvent, self.featureQueueTest,self.featureQueueTrain,
                                                  self.classifierInfoQueue, self.classifierInfoRetrieveEvent,
-                                                 self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent, self.printDebug,len(self.dataThreads),
+                                                 self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent, self.logger,len(self.dataThreads),
                                                 self.minimumEpochsRequired, clf = self.clf, model = self.model, torchModel = self.torchModel)
         self.classifierThread.start()
 
     def StopThreads(self):
         self.closeEvent.set()
         self.markerThread.join()
         # wait for all threads to finish processing, probably worth pulling out finalised classifier information stored for later use.
         for dt in self.dataThreads:
             dt.join()
         for ft in self.featureThreads:
             ft.join()
         self.classifierThread.join()
         self.connected = False
-        if self.printDebug:
-            print("PyBCI: Threads stopped.")
+        self.logger.log(Logger.INFO," Threads stopped.")
 
     def ConfigureMachineLearning(self, minimumEpochsRequired = 10, clf = None, model = None, torchModel = None):
         from sklearn.base import ClassifierMixin
         self.minimumEpochsRequired = minimumEpochsRequired
+
         if isinstance(clf, ClassifierMixin):
             self.clf = clf
         else:
             self.clf = None
-            if self.printDebug:
-                print("PyBCI: Error - Invalid sklearn classifier passed to clf, setting to SVM if no tensorflow model passed either.")
-        if isinstance(model, tf.keras.Model):
-            self.model = model
-        else:
-            self.model = None
-            if self.printDebug:
-                print("PyBCI: Error - Invalid tensorflow model passed to model, setting to None.")
-        if callable(torchModel): # isinstance(torchModel, torch.nn.Module):
-            self.torchModel = model
-        else:
-            self.torchModel = None
-            if self.printDebug:
-                print("PyBCI: Error - Invalid PyTorch model passed to model, setting to None.")
+            self.logger.log(Logger.WARNING," Invalid or no sklearn classifier passed to clf, setting to SVM if no tensorflow or pytorch model passed.")
+            if isinstance(model, tf.keras.Model):
+                self.model = model
+            else:
+                self.model = None
+                self.logger.log(Logger.WARNING," Invalid or no tensorflow model passed to model.")
+                if callable(torchModel): # isinstance(torchModel, torch.nn.Module):
+                    self.torchModel = model
+                else:
+                    self.torchModel = None
+                    self.logger.log(Logger.WARNING," Invalid or no PyTorch model passed to model.")
     
 
     # Could move all configures to a configuration class, might make options into more descriptive classes?
     def ConfigureEpochWindowSettings(self, globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}):
         """allows globalWindowSettings to be modified, customWindowSettings is a dict with value names for marker strings which will appear on avalable markerStreams """
         valid = False
         for key in customEpochSettings.keys():
             if isinstance(customEpochSettings[key], IndividualEpochSetting):
                 valid = True
             else:
                 valid = False
-                if self.printDebug:
-                    print("PyBCI: Error - Invalid datatype passed for customWindowSettings, create dict of wanted markers \
-                          using class bci.IndividualEpochSetting() as value to configure individual epoch window settings.")
-                    break
+                self.logger.log(Logger.WARNING," Invalid datatype passed for customWindowSettings, create dict of wanted markers \
+                        using class bci.IndividualEpochSetting() as value to configure individual epoch window settings.")
+                break
         #if isinstance(customWindowSettings[key], GlobalEpochSettings()):
         if valid:   
             self.customEpochSettings = customEpochSettings
             if globalEpochSettings.windowLength > globalEpochSettings.tmax + globalEpochSettings.tmin:
-                if self.printDebug:
-                    print("PyBCI: Error - windowLength < (tmin+tmax), pass vaid settings to ConfigureEpochWindowSettings")
+                self.logger.log(Logger.WARNING," windowLength < (tmin+tmax), pass vaid settings to ConfigureEpochWindowSettings")
             else:
                 self.globalWindowglobalEpochSettingsSettings = globalEpochSettings
                 self.ResetThreadsAfterConfigs()
 
     def ConfigureDataStreamChannels(self,streamChsDropDict = {}):
         # potentially should move configuration to generic class which can be used for both test and train
         self.streamChsDropDict = streamChsDropDict 
         self.ResetThreadsAfterConfigs()
 
     def ResetThreadsAfterConfigs(self):
         if self.connected:
-            if self.printDebug:
-                print("PyBCI: Resetting threads after BCI reconfiguration...")
+            self.logger.log(Logger.INFO,"Resetting threads after BCI reconfiguration...")
             self.StopThreads()
             self.Connect()
```

### Comparing `install-pybci-0.2.1b0/setup.py` & `install-pybci-0.2.2b0/setup.py`

 * *Files identical despite different names*

