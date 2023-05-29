# Comparing `tmp/install-pybci-0.2.2b0.tar.gz` & `tmp/install-pybci-0.2.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.2.2b0.tar", last modified: Sun May 28 22:40:20 2023, max compression
+gzip compressed data, was "install-pybci-0.2.2b1.tar", last modified: Mon May 29 00:08:06 2023, max compression
```

## Comparing `install-pybci-0.2.2b0.tar` & `install-pybci-0.2.2b1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.020716 install-pybci-0.2.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-28 22:40:20.016715 install-pybci-0.2.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.012715 install-pybci-0.2.2b0/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-28 22:40:19.000000 install-pybci-0.2.2b0/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-28 22:40:20.000000 install-pybci-0.2.2b0/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 22:40:19.000000 install-pybci-0.2.2b0/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-28 22:40:19.000000 install-pybci-0.2.2b0/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 22:40:20.000000 install-pybci-0.2.2b0/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.012715 install-pybci-0.2.2b0/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.016715 install-pybci-0.2.2b0/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.016715 install-pybci-0.2.2b0/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:40:20.016715 install-pybci-0.2.2b0/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 22:40:20.020716 install-pybci-0.2.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-28 22:39:38.000000 install-pybci-0.2.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.765080 install-pybci-0.2.2b1/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/setup.py
```

### Comparing `install-pybci-0.2.2b0/LICENSE` & `install-pybci-0.2.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/PKG-INFO` & `install-pybci-0.2.2b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.2b0
+Version: 0.2.2b1
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
@@ -66,22 +66,22 @@
         print("Current marker estimation: " + str(guess), end="\r")
         time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
-Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
+Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
 - run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo]
 - Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
-- Levels of print debug (info, error, none)
-- Retrieve feature data  
+- ~~Levels of print debug (info, error, none)~~
+- ~~Retrieve feature data~~
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.2b0/README.md` & `install-pybci-0.2.2b1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
@@ -42,22 +42,22 @@
         print("Current marker estimation: " + str(guess), end="\r")
         time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
-Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
+Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
 - run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo]
 - Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
-- Levels of print debug (info, error, none)
-- Retrieve feature data  
+- ~~Levels of print debug (info, error, none)~~
+- ~~Retrieve feature data~~
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.2b0/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.2.2b1/install_pybci.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.2b0
+Version: 0.2.2b1
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
@@ -66,22 +66,22 @@
         print("Current marker estimation: " + str(guess), end="\r")
         time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
-Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
+Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
 - run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo]
 - Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
-- Levels of print debug (info, error, none)
-- Retrieve feature data  
+- ~~Levels of print debug (info, error, none)~~
+- ~~Retrieve feature data~~
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.2b0/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.2.2b1/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/Configuration/EpochSettings.py` & `install-pybci-0.2.2b1/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.2.2b1/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.2.2b1/pybci/ThreadClasses/ClassifierThread.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,65 +5,62 @@
 class ClassifierThread(threading.Thread):
     features = []
     targets = []
     mode = "train"
     guess = None
     epochCounts = {} 
     def __init__(self, closeEvent,trainTestEvent, featureQueueTest,featureQueueTrain, classifierInfoQueue, classifierInfoRetrieveEvent, 
-                 classifierGuessMarkerQueue, classifierGuessMarkerEvent, logger = Logger(Logger.INFO), numStreamDevices = 1,
+                 classifierGuessMarkerQueue, classifierGuessMarkerEvent, queryFeaturesQueue, queryFeaturesEvent,
+                 logger = Logger(Logger.INFO), numStreamDevices = 1,
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
+        self.queryFeaturesQueue = queryFeaturesQueue
+        self.queryFeaturesEvent = queryFeaturesEvent
         self.numStreamDevices = numStreamDevices
         self.logger = logger
 
     def run(self):
         if self.numStreamDevices > 1:
             tempdatatrain = {}
             tempdatatest = {}
         while not self.closeEvent.is_set():
             if self.trainTestEvent.is_set(): # We're training!
                 try:
                     featuresSingle, devCount, target, self.epochCounts = self.featureQueueTrain.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
-                    if self.numStreamDevices > 1:
+                    if self.numStreamDevices > 1: # Collects multiple data strems feature sets and synchronise here
                         tempdatatrain[devCount] = featuresSingle
                         if len(tempdatatrain) == self.numStreamDevices:
-                            #print(tempdatatrain)
-                            #flattened_list = []
-                            #for value in tempdatatrain.values():
-                                #flattened_list.extend(value)
                             flattened_list = [item for sublist in tempdatatrain.values() for item in sublist]
                             tempdatatrain = {}
-                            #print(flattened_list)
                             self.targets.append(target)
                             self.features.append(flattened_list)
-
                         # need to check if all device data is captured, then flatten and append
                             if len(self.epochCounts) > 1: # check if there is more then one test condition
                                 minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
                                 if minNumKeyEpochs < self.minRequiredEpochs:
                                     pass
                                 else: 
                                     start = time.time()
                                     self.classifier.TrainModel(self.features, self.targets)
                                     if (self.logger.level == Logger.INFO):
                                         end = time.time()
                                         self.logger.log(Logger.INFO, f" classifier training time {end - start}")
                             if self.classifierGuessMarkerEvent.is_set():
                                 self.classifierGuessMarkerQueue.put(None)
-                    else:
+                    else: # Only one device to collect from
                         self.targets.append(target)
                         self.features.append(featuresSingle)
                         if len(self.epochCounts) > 1: # check if there is more then one test condition
                             minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
                             if minNumKeyEpochs < self.minRequiredEpochs:
                                 pass
                             else: 
@@ -101,10 +98,17 @@
                         self.classifierGuessMarkerQueue.put(self.guess)
                 except queue.Empty:
                     pass
             if self.classifierInfoRetrieveEvent.is_set():
                 classdata = {
                     "clf":self.classifier.clf,
                     "model":self.classifier.model,
+                    "torchModel":self.classifier.torchModel,
                     "accuracy":self.classifier.accuracy
                     }
-                self.classifierInfoQueue.put(classdata) 
+                self.classifierInfoQueue.put(classdata) 
+            if self.queryFeaturesEvent.is_set():
+                featureData = {
+                    "features":self.features,
+                    "targets":self.targets
+                }
+                self.queryFeaturesQueue.put(featureData)
```

### Comparing `install-pybci-0.2.2b0/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.2.2b1/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.2.2b1/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.2.2b1/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/Utils/Classifier.py` & `install-pybci-0.2.2b1/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.2.2b1/pybci/Utils/FeatureExtractor.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/Utils/LSLScanner.py` & `install-pybci-0.2.2b1/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/Utils/Logger.py` & `install-pybci-0.2.2b1/pybci/Utils/Logger.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b0/pybci/pybci.py` & `install-pybci-0.2.2b1/pybci/pybci.py`

 * *Files 12% similar despite different names*

```diff
@@ -86,48 +86,94 @@
             return True # uses return statements so user can check if connected with bool returned
         else:
             self.connected = False
             return False
 
     # set test and train boolean for changing  thread operation 
     def TrainMode(self):
+        """
+         Starts BCI training If PyBCI is connected to valid LSL data and marker streams, if not tries to scan and connect.
+        """
         if self.connected:
             self.logger.log(Logger.INFO,"Started training...")
             self.trainTestEvent.set()
         else:
             self.Connect()
 
     def TestMode(self):
+        """
+         Starts BCI testing If PyBCI is connected to valid LSL data and marker streams, if not tries to scan and connect.
+         (Need to check if invalid number of epochs are obtained and this is set)
+        """
         if self.connected:
             self.logger.log(Logger.INFO,"Started testing...")
             self.trainTestEvent.clear()
         else:
             self.Connect()
 
     # Get data from threads
     def CurrentClassifierInfo(self):
+        """
+        
+        """
         if self.connected:
             self.classifierInfoRetrieveEvent.set()
             classInfo = self.classifierInfoQueue.get()
             self.classifierInfoRetrieveEvent.clear()
             return classInfo
         else:
             self.Connect()
+            return {"Not Connected": None}
 
     def CurrentClassifierMarkerGuess(self):
+        """
+        Gets classifier current marker guess and targets.
+        Returns
+        -------
+        int
+            Returned int correlates to value of key from dict from ReceivedMarkerCount() when in testmode. 
+            If in trainmode returns None.
+        """
         if self.connected:
             # probably needs check that we're in test mode, maybe debu print if not?
             self.classifierGuessMarkerEvent.set()
             classGuess = self.classifierGuessMarkerQueue.get()
             self.classifierGuessMarkerEvent.clear()
             return classGuess
         else:
             self.Connect()
+            return {"Not Connected": None}
+
+    def CurrentFeaturesTargets(self):
+        """
+        Gets classifier current features and targets.
+        Returns
+        -------
+        dict
+            dict of "features" and "targets" where features is 2d list of feature data and targets is a 1d list of epoch targets as ints.
+            If not connected returns {"Not Connected": None}
+        """
+        if self.connected:
+            self.queryFeaturesEvent.set()
+            featureTargets = self.queryFeaturesQueue.get()
+            self.queryFeaturesEvent.clear() # still needs coding
+            return featureTargets
+        else:
+            self.Connect()
+            return {"Not Connected": None}
 
     def ReceivedMarkerCount(self):
+        """
+        Gets number of received training marker, their strings and their respective values to correlate with CurrentClassifierMarkerGuess().
+        Returns
+        -------
+        dict
+            Every key is a string received on the selected LSL marker stream, the value is a list where the first item is the marker id value, 
+            use with CurrentClassifierMarkerGuess() the second value is a received count for that marker type.
+        """
         if self.connected:
             self.markerCountRetrieveEvent.set()
             markers = self.markerCountQueue.get()
             self.markerCountRetrieveEvent.clear()
             return markers
         else:
             self.Connect()
@@ -139,15 +185,17 @@
         self.markerCountQueue = queue.Queue()
         self.classifierGuessMarkerQueue = queue.Queue()
         self.classifierGuessMarkerEvent = threading.Event()
         self.closeEvent = threading.Event() # used for closing threads
         self.trainTestEvent = threading.Event()
         self.markerCountRetrieveEvent = threading.Event()
         self.classifierInfoRetrieveEvent = threading.Event()
-        self.featureRetrieveEvent = threading.Event() # still needs coding
+
+        self.queryFeaturesQueue = queue.Queue()
+        self.queryFeaturesEvent  = threading.Event() # still needs coding
 
         self.trainTestEvent.set() # if set we're in train mode, if not we're in test mode, always start in train...
         self.logger.log(Logger.INFO," Starting threads initialisation...")
         # setup data thread
         self.dataThreads = []
         self.featureThreads = []
         for stream in self.dataStreams:
@@ -185,19 +233,23 @@
             self.ft.start()
             self.featureThreads.append(dt)
         # marker thread requires data and feature threads to push new markers too
         self.markerThread = MarkerThread(self.closeEvent,self.trainTestEvent, self.markerStream,self.dataThreads, self.featureThreads)
         self.markerThread.start()
         self.classifierThread = ClassifierThread(self.closeEvent,self.trainTestEvent, self.featureQueueTest,self.featureQueueTrain,
                                                  self.classifierInfoQueue, self.classifierInfoRetrieveEvent,
-                                                 self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent, self.logger,len(self.dataThreads),
+                                                 self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent, self.queryFeaturesQueue, self.queryFeaturesEvent,
+                                                 self.logger,len(self.dataThreads),
                                                 self.minimumEpochsRequired, clf = self.clf, model = self.model, torchModel = self.torchModel)
         self.classifierThread.start()
 
     def StopThreads(self):
+        """
+        Stops all PyBCI threads.
+        """
         self.closeEvent.set()
         self.markerThread.join()
         # wait for all threads to finish processing, probably worth pulling out finalised classifier information stored for later use.
         for dt in self.dataThreads:
             dt.join()
         for ft in self.featureThreads:
             ft.join()
@@ -209,25 +261,25 @@
         from sklearn.base import ClassifierMixin
         self.minimumEpochsRequired = minimumEpochsRequired
 
         if isinstance(clf, ClassifierMixin):
             self.clf = clf
         else:
             self.clf = None
-            self.logger.log(Logger.WARNING," Invalid or no sklearn classifier passed to clf, setting to SVM if no tensorflow or pytorch model passed.")
+            self.logger.log(Logger.INFO," Invalid or no sklearn classifier passed to clf. Checking tensorflow model... ")
             if isinstance(model, tf.keras.Model):
                 self.model = model
             else:
                 self.model = None
-                self.logger.log(Logger.WARNING," Invalid or no tensorflow model passed to model.")
+                self.logger.log(Logger.INFO," Invalid or no tensorflow model passed to model.  Checking pytorch torchModel...")
                 if callable(torchModel): # isinstance(torchModel, torch.nn.Module):
                     self.torchModel = model
                 else:
                     self.torchModel = None
-                    self.logger.log(Logger.WARNING," Invalid or no PyTorch model passed to model.")
+                    self.logger.log(Logger.INFO," Invalid or no PyTorch model passed to model. Defaulting to SVM by SkLearn")
     
 
     # Could move all configures to a configuration class, might make options into more descriptive classes?
     def ConfigureEpochWindowSettings(self, globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}):
         """allows globalWindowSettings to be modified, customWindowSettings is a dict with value names for marker strings which will appear on avalable markerStreams """
         valid = False
         for key in customEpochSettings.keys():
```

### Comparing `install-pybci-0.2.2b0/setup.py` & `install-pybci-0.2.2b1/setup.py`

 * *Files identical despite different names*

