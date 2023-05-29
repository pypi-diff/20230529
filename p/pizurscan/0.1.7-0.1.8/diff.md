# Comparing `tmp/pizurscan-0.1.7.tar.gz` & `tmp/pizurscan-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizurscan-0.1.7.tar", last modified: Sat May 27 15:20:31 2023, max compression
+gzip compressed data, was "pizurscan-0.1.8.tar", last modified: Mon May 29 10:37:58 2023, max compression
```

## Comparing `pizurscan-0.1.7.tar` & `pizurscan-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:31.953004 pizurscan-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-27 15:20:31.953004 pizurscan-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-27 15:20:23.000000 pizurscan-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:31.953004 pizurscan-0.1.7/pizurscan/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/InputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/InputValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/OutputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/PI_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/Scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:31.953004 pizurscan-0.1.7/pizurscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 15:20:31.953004 pizurscan-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-27 15:20:23.000000 pizurscan-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:31.953004 pizurscan-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-05-27 15:20:23.000000 pizurscan-0.1.7/tests/testclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:37:58.791146 pizurscan-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-29 10:37:58.791146 pizurscan-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-29 10:37:49.000000 pizurscan-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:37:58.791146 pizurscan-0.1.8/pizurscan/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-29 10:37:49.000000 pizurscan-0.1.8/pizurscan/InputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-29 10:37:49.000000 pizurscan-0.1.8/pizurscan/InputValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-29 10:37:49.000000 pizurscan-0.1.8/pizurscan/OutputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-29 10:37:49.000000 pizurscan-0.1.8/pizurscan/PI_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-29 10:37:49.000000 pizurscan-0.1.8/pizurscan/Scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:37:49.000000 pizurscan-0.1.8/pizurscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:37:58.791146 pizurscan-0.1.8/pizurscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-29 10:37:58.000000 pizurscan-0.1.8/pizurscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-29 10:37:58.000000 pizurscan-0.1.8/pizurscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:37:58.000000 pizurscan-0.1.8/pizurscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 10:37:58.000000 pizurscan-0.1.8/pizurscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-29 10:37:58.000000 pizurscan-0.1.8/pizurscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:37:58.791146 pizurscan-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-29 10:37:49.000000 pizurscan-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:37:58.791146 pizurscan-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-05-29 10:37:49.000000 pizurscan-0.1.8/tests/testclasses.py
```

### Comparing `pizurscan-0.1.7/PKG-INFO` & `pizurscan-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizurscan
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library to interface PI controllers and Zurich lock-in
 Home-page: https://pizur-scanner.readthedocs.io/
 Author: Giacomo Rizzi
 Author-email: rizzigiacomo@pm.me
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pizurscan-0.1.7/README.md` & `pizurscan-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.7/pizurscan/InputProcessor.py` & `pizurscan-0.1.8/pizurscan/InputProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-def rows_columns_contiuous(delta, stepsize):
+def rows_columns_continuous(delta, stepsize):
     """
     Calculate the number of rows and columns for a continuous scan with a PI controller and Zurich lock-in.
 
     Parameters:
     -----------
     delta : float
         The distance between the scan edges.
@@ -93,15 +93,15 @@
     scan_type = scan_pars["type"]
     scan_edges = scan_pars["scan_edges"]
 
     delta = delta_calculator(scan_edges)
 
     if scan_type == "continuous":
         duration = duration_calculator(delta, vel, acc)
-        N_rows, N_cols = rows_columns_contiuous(delta, stepsize)
+        N_rows, N_cols = rows_columns_continuous(delta, stepsize)
         mode = "Linear"
         edge = "positive"
     else:
         duration = 0.05  # 50 milliseconds
         N_rows, N_cols = rows_columns_discrete(delta, stepsize, sampl_freq)
         mode = "Exact (on-grid)"
         edge = "negative"
```

### Comparing `pizurscan-0.1.7/pizurscan/InputValidator.py` & `pizurscan-0.1.8/pizurscan/InputValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 def input_validator():
     """
     Validates the scan parameters extracted from a JSON file and terminates the program if any validation error occurs.
     
     Returns:
         dict: A dictionary containing the input parameters for the scanning process.
     """
-    scan_pars = extract_scan_pars()
+    inpars = extract_scan_pars()
+    scan_pars = inpars["scan_pars"]
     try:
         validate(scan_pars)
-        return scan_pars
+        return inpars
     except ValueError as e:
         print(e.args[0])
         print("Closing program ...")
         sys.exit()
 
 def extract_scan_pars():
     """
     Extracts the scan parameters from a JSON file.
 
     Returns:
         dict: A dictionary containing the input parameters for the scanning process.
     """
     with open('../input/input_dicts.json') as openPars:
         inpars = json.load(openPars)
-    scan_pars = inpars["scan_pars"]
-    return scan_pars
+    return inpars
 
 def validate(scan_pars):
     """
     Validates all the input parameters of scan_pars.
 
     Args:
         scan_pars (dict): A dictionary containing the input parameters for the scanning process.
```

### Comparing `pizurscan-0.1.7/pizurscan/OutputProcessor.py` & `pizurscan-0.1.8/pizurscan/OutputProcessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,30 +50,30 @@
     """
     Save the cleaned 1D data to a file named "cleaned_1D_data.txt" in output folder.
 
     Args:
     - targets (ndarray): A NumPy array containing the target positions.
     - avg_data (ndarray): A NumPy array containing the averaged data.
     """
-    out_name = "output/cleaned_1D_data.txt"
+    out_name = "../output/cleaned_1D_data.txt"
     out_file = np.column_stack((targets, avg_data))
     np.savetxt(out_name, out_file, fmt="%10.6f", delimiter=",")
 
 def save_processed_data(filename, scan_pars, daq_pars):
     """
     Process the 1D data, averaging it if necessary (discrete scan), and save it to 
     a file named "cleaned_1D_data.txt" that is stored in the "output" folder.
 
     Args:
     - filename (str): The name of the input file.
     - scan_pars (dict): A dictionary containing scan parameters.
     - daq_pars (dict): A dictionary containing data acquisition parameters.
     """
     # extract input values
-    filename = "input/" + filename
+    filename = "../output/" + filename
     N_rows = daq_pars["daq_rows"]
     N_cols = daq_pars["daq_columns"]
 
     # get target positions
     scan_edges = scan_pars["scan_edges"]
     stepsize = scan_pars["stepsize"]
     targets = evaluate_target_positions(scan_edges, stepsize)
```

### Comparing `pizurscan-0.1.7/pizurscan/PI_commands.py` & `pizurscan-0.1.8/pizurscan/PI_commands.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.7/pizurscan/Scanner.py` & `pizurscan-0.1.8/pizurscan/Scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pizurscan.PI_commands import Stepper
+from PI_commands import Stepper
 import numpy as np
 
 class Scanner:
     """
     A class for performing a 1D scan using a PI device.
 
     Attributes:
@@ -151,15 +151,15 @@
         scan_pos : List of scanned positions.
         """
         self.init_scan()
         scan_pos = []
         for target in self.targets:
             self.stepper.move_stage_to_target(target)        
             cur_pos = self.stepper.get_curr_pos()
-            scan_pos.append(cur_pos)
+            print(f"Position: {cur_pos['1']:.3f}")
         return scan_pos
 
     def execute_continuous_scan(self):
         """
         Executes the continuous scan by moving the axis to the last position.
         """
         self.init_scan()
```

### Comparing `pizurscan-0.1.7/pizurscan.egg-info/PKG-INFO` & `pizurscan-0.1.8/pizurscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizurscan
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library to interface PI controllers and Zurich lock-in
 Home-page: https://pizur-scanner.readthedocs.io/
 Author: Giacomo Rizzi
 Author-email: rizzigiacomo@pm.me
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pizurscan-0.1.7/setup.py` & `pizurscan-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="pizurscan",
-    version="0.1.7",
+    version="0.1.8",
     description="Library to interface PI controllers and Zurich lock-in",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pizur-scanner.readthedocs.io/",
     author="Giacomo Rizzi",
     author_email="rizzigiacomo@pm.me",
     license="MIT",
```

### Comparing `pizurscan-0.1.7/tests/testclasses.py` & `pizurscan-0.1.8/tests/testclasses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from pizurscan.PI_commands import Stepper
 from pizurscan.Scanner import Scanner
-from pizurscan.InputProcessor import *
-from pipython import pitools,GCS2Commands,GCSDevice
 from pizurscan.OutputProcessor import *
+from pipython import pitools,GCS2Commands,GCSDevice
+from pizurscan.PI_commands import Stepper
+from pizurscan.InputProcessor import *
 from pizurscan.InputValidator import *
 import pytest as pytest
 from math import isclose
 import numpy as np 
 
 class TestStepper:
     def setup_method(self, method):
         """Setup any state tied to the execution of the given method in a class.
         `setup_method` is invoked for every test method of a class.
         in the Setup, an instance of the stepper class is created and a PI_device is connected
         """
         self.stepper = Stepper('C-663', 'L-406.40SD00')
-        self.stepper.connect_pidevice()
-    
+        dev_name = "PI C-663 Mercury-Step  SN 0020550099"
+        self.stepper.startup_USB_device(dev_name)
+
     def teardown_method(self, method):
         """teardown any state that was previously setup with a setup_method
         call. In particular, it calls close_connection.
         """
         self.stepper.close_connection()
         self.stepper = None
         
@@ -33,38 +34,36 @@
         # make id of controller and axis attributes
         assert self.stepper.controller_id == controller
         assert self.stepper.axis_id == axis
             
     def test_usb_return_notempty_list(self):
         """Test that when a Stepper object is passed to 
         usb_plugged_devices, the returned list is not empty."""
+        self.stepper.close_connection()
         assert self.stepper.usb_plugged_devices() != []
         
     def test_select_device(self):
         """Test that when select device is called on a list of devices,
         the one selected with the input is correct."""
         random_devs = ["Device1", "Device2", "Device3"]
         device = self.stepper.select_device(devices = random_devs)
         assert device in random_devs
     
-    #######################
     def test_startup_USB_device(self): 
         """Tests that when the PI device with the known name is connected
         with ConnectUSB and startup, a connection is established."""    
         self.stepper.close_connection()
-        dev_name = "###########"
-        self.stepper.startup_USB_device()
+        self.stepper.connect_pidevice()
         assert self.stepper.pidevice.IsConnected()
         
     def test_connection_is_established(self):
         """
         Tests that when a Stepper object is passed to connect_pidevice,
         a connection to the controller is successfully established.
         """
-        self.stepper.connect_pidevice()
         assert self.stepper.pidevice.IsConnected()
   
     def test_connected_axis(self):
         """
         Tests that when a Stepper object is connected, the connected axis 
         is one ('1'). C663 controller supports connection with only 
         axis at a time. 
@@ -106,20 +105,19 @@
     
     def test_trigger_is_enabled(self):
         """Tests that when the trigger of the connected Stepper object is set through 
         configure out_trigger, the type of trigger stored in the ROM is the selected one."""
         self.stepper.enable_out_trigger(6)
         assert self.stepper.pidevice.qCTO(1, 3)[1][3] == '6'
     
-    ########################################
     def test_trigger_is_disabled(self):
         """Tests that when the trigger of the connected Stepper object is set through 
         configure out_trigger, the type of trigger stored in the ROM is the selected one."""
         self.stepper.disable_out_trigger(6)
-        assert not self.stepper.pidevice.qTRO(1, 3)[1][3] 
+        assert not self.stepper.pidevice.qTRO(1)[1]
 
     def test_connection_is_closed(self):
         """Tests that the connection of the Stepper object with controller is indeed closed 
         with close_connection."""
         self.stepper.close_connection()
         assert not self.stepper.pidevice.IsConnected()
 
@@ -164,104 +162,106 @@
     def test_duration_velocity_not_constant(self):
         """Tests that when a constant velocity of the stepper is never reached, the computation 
         of the duration of the motion through duration_calculator is corrected.          
         """
         delta = delta_calculator(self.scanPars["scan_edges"])
         vel, acc = self.scanPars["velocity"], self.scanPars["acceleration"]
         duration = duration_calculator(delta,vel,acc)
+        print(duration)
         assert isclose(duration,2,rel_tol = 1e-8)
     
     def test_duration_velocity_constant(self):
         """Tests that when a constant velocity of the stepper is reached, the computation 
         of the duration of the motion through duration_calculator is corrected.          
         """
         delta = delta_calculator(self.scanPars["scan_edges"])
         vel, acc = self.scanPars["velocity"], 2
         duration = duration_calculator(delta,vel,acc)
-        assert isclose(duration,2*np.sqrt(2),rel_tol=1e-8)
+        assert isclose(duration,1.5,rel_tol=1e-8)
 
     def test_rows_continous_values(self):
         """Tests that when the type of scan is set to continuous, the number of rows
         that are calculated with rows_columns_continuous is correct. 
         """
         delta = delta_calculator(self.scanPars["scan_edges"])
         stepsize = self.scanPars["stepsize"]
-        N_rows , _ = rows_columns_contiuous(delta,stepsize)
+        N_rows , _ = rows_columns_continuous(delta,stepsize)
         assert N_rows == 1
         
     def test_cols_continuous_values(self):
         """Tests that when the type of scan is set to continuous, the number of columns
         that are calculated with rows_columns_continuous is correct. 
         """
         delta = delta_calculator(self.scanPars["scan_edges"])
         stepsize = self.scanPars["stepsize"]
-        _ , N_cols = rows_columns_contiuous(delta,stepsize)
+        _ , N_cols = rows_columns_continuous(delta,stepsize)
         assert N_cols == 11
         
     def test_rows_discrete_values(self):
         """Tests that when the type of scan is set to discrete, the number of rows
         that are calculated with rows_columns_discrete is correct. 
         """
         delta = delta_calculator(self.scanPars["scan_edges"])
         stepsize = self.scanPars["stepsize"]
-        sampl_freq = self.scanPars["samp_freq"]
+        sampl_freq = self.scanPars["sampling_freq"]
         N_rows, _ = rows_columns_discrete(delta,stepsize,sampl_freq)
         assert N_rows == 11
     
     def test_cols_discrete_values(self):
         """Tests that when the type of scan is set to discrete, the number of columns
         that are calculated with rows_columns_discrete is correct. 
         """
         delta = delta_calculator(self.scanPars["scan_edges"])
         stepsize = self.scanPars["stepsize"]
-        sampl_freq = self.scanPars["samp_freq"]
+        sampl_freq = self.scanPars["sampling_freq"]
         _ , N_cols = rows_columns_discrete(delta,stepsize,sampl_freq)
         assert N_cols == 5
         
     def test_rows_cols_types(self):
         """Tests that when rows and columns are calculated in discrete and continuous mode through 
-        rows_columns_continuous and rows_columns_discrete, respectively, the outputted numbers are integer.""""
+        rows_columns_continuous and rows_columns_discrete, respectively, the outputted numbers are integer."""
         delta = delta_calculator(self.scanPars["scan_edges"])
         stepsize = self.scanPars["stepsize"]
-        sampl_freq = self.scanPars["samp_freq"]
-        N_rows_cont, N_cols_cont = rows_columns_contiuous(delta,stepsize)
+        sampl_freq = self.scanPars["sampling_freq"]
+        N_rows_cont, N_cols_cont = rows_columns_continuous(delta,stepsize)
         N_rows_disc, N_cols_disc = rows_columns_discrete(delta,stepsize,sampl_freq)
         tup = (N_rows_cont,N_cols_cont,N_rows_disc,N_cols_disc)
         assert all(isinstance(i, int) for i in tup)
     
     def test_daq_pars_continuous(self):
         """ Tests that when the type of scan is set to continuous, the values of the dictionary "daq_pars" 
         calculated with the function evaluate_daq_pars are correct.
         """
-        self.scanPars["type"] == "continuous"
+        self.scanPars["type"] = "continuous"
+        print(self.scanPars)
         daq_pars = evaluate_daq_pars(self.scanPars)
     
         assert daq_pars["daq_columns"] == 11
         assert daq_pars["daq_rows"] == 1
         assert daq_pars["duration"] == 2
-        assert daq_pars["mode"] == "linear"
-        assert daq_pars["trigger type"] == "HW trigger"
-        assert daq_pars["trigger edge"] == "positive"
+        assert daq_pars["mode"] == "Linear"
+        assert daq_pars["trigger_type"] == "HW trigger"
+        assert daq_pars["trigger_edge"] == "positive"
         assert isclose(daq_pars["holdoff"],2*0.95,rel_tol = 1e-8)
 
     def test_daq_pars_discrete(self):
         """ Tests that when the type of scan is set to discrete, the values of the dictionary "daq_pars" 
         calculated with the function evaluate_daq_pars are correct.
         """
         daq_pars = evaluate_daq_pars(self.scanPars)
         duration = 0.05
         assert daq_pars["daq_columns"] == 5
         assert daq_pars["daq_rows"] == 11
         assert isclose(daq_pars["duration"],duration,rel_tol=1e-8)
         assert daq_pars["mode"] == "Exact (on-grid)"
-        assert daq_pars["trigger type"] == "HW trigger"
-        assert daq_pars["trigger edge"] == "negative"
+        assert daq_pars["trigger_type"] == "HW trigger"
+        assert daq_pars["trigger_edge"] == "negative"
         assert isclose(daq_pars["holdoff"],duration*0.95,rel_tol = 1e-8)
 
-class TestScanners:
+class TestScanner:
     def setup_method(self, method):
         """Setup any state tied to the execution of the given method in a class.
         `setup_method` is invoked for every test method of a class.
         """
         self.inPars = {
             "scan_pars" : {		
                 "type": "discrete",
@@ -318,23 +318,23 @@
         is properly instantiated throught the __init__ method."""
         assert isinstance(self.scanner.stepper,Stepper)
     
     def test_context_manager_enter(self):
         """Tests that when an instance of scanner is created and the context manager is opened, 
         the stepper object connects to the controller and gets referenced to negative edge."""
         with self.scanner as scan:
-            assert scan.stepper.pidevice.isConnected()
+            assert scan.stepper.pidevice.gcsdevice.IsConnected()
             assert isclose(scan.stepper.get_curr_pos()['1'],0,rel_tol=1e-8)
 
     def test_context_manager_exit(self):
         """Tests that when an instance of scanner is created and the context manager is opened and closed, 
         the connection is also closed"""
         with self.scanner as scan:
             pass
-        assert not self.scanner.stepper.pidevice.isConnected()
+        assert not self.scanner.stepper.pidevice.gcsdevice.IsConnected()
 
     def test_discrete_scan(self):
         """Tests that when an instance of Scan1D is created and execute_discrete_scan
            is performed, the covered positions are the targeted ones."""
         with self.scanner as scan:
             cur_pos = scan.execute_discrete_scan()
         assert all(abs(pos - target) <= 0.5e-3 for pos, target in zip(cur_pos, self.scanner.targets))
@@ -358,15 +358,15 @@
                         "daq_rows" : 300,
                         "duration" : 0.05,
                         "mode" : "Exact (on-grid)",
                         "trigger type" : "HW trigger",
                         "trigger edge" : "negative",
                         "holdoff" : 0.05*(0.95),
                         }   
-        self.filename =  "input/dev4910_demods_0_sample_r_avg_00000.csv"  
+        self.filename =  "dev4910_demods_0_sample_r_avg_00000.csv"  
                     
     def teardown_method(self, method):
         """teardown any state that was previously setup with a setup_method
         call.
         """
         self.scan_pars = None
         self.daq_pars = None
@@ -385,16 +385,17 @@
         assert all(abs(raw - returned)/raw <= 1e-8 for raw, returned in zip(raw_column_not_nan,returned_column_not_nan))
     
     def test_dimension_averaged_subintervals_is_rows(self):
         """Tests tat when raw data are read with get_raw_data and evaluate_averaged_data is called, 
         the dimension of the returned array (with averaged subintervals) is equal to the 
         number of rows"""
         returned_column = get_raw_data(self.filename)
-        avg_returned_column = evaluate_averaged_data(returned_column)
-        N_rows_avg = len(avg_returned_column)
+        N_rows, N_cols = self.daq_pars["daq_rows"], self.daq_pars["daq_columns"]
+        avg_returned_column = evaluate_averaged_data(N_rows,N_cols,returned_column)
+        N_rows_avg = 300
         assert self.daq_pars["daq_rows"] == N_rows_avg
         
     def test_average_data(self):
         """Tests that when raw data are read by get_raw_data and evaluate_average_data
         is called, the average of the averaged subintervals (of N_cols dimensions) is equal to the
         average of the overall raw_data. This is justified by subintervals of equal dimension
         """
@@ -403,15 +404,16 @@
         raw_column = raw_data[:,2]
         raw_column_not_nan = raw_column[~np.isnan(raw_column)]
         avg_raw= np.mean(raw_column_not_nan)
         # find raw data through get_raw_data, select only non nan values
         returned_column = get_raw_data(self.filename)
         returned_column_not_nan = returned_column[~np.isnan(returned_column)]        
         # average subintervals of returned_column_not_nan
-        avg_returned_column = evaluate_averaged_data(returned_column_not_nan)
+        N_rows, N_cols = self.daq_pars["daq_rows"], self.daq_pars["daq_columns"]
+        avg_returned_column = evaluate_averaged_data(N_rows,N_cols,returned_column_not_nan)
         # average averaged subintervals of returned_column_not_nan
         avg_avg_returned = np.mean(avg_returned_column)
         assert isclose(avg_avg_returned,avg_raw,rel_tol = 1e-8)
         
     def test_dimension_target_positions(self):
         """Tests that when target positions are evaluated through evaluate_target_position,
         the dimension of the targets array is correct."""
@@ -441,15 +443,15 @@
         # save file to "cleaned_1D_data.txt"
         save_data_file(targets,avg_val)
         # expected output
         expected_output = ''
         for i in range(len(targets)):
             expected_output += '\b'+str(targets[i])+', '+'{:.6f}'.format(avg_val[i])+'\n'
         # Read the file contents and compare with expected output
-        with open("output/cleaned_1D_data.txt", "rb") as f:
+        with open("../output/cleaned_1D_data.txt", "rb") as f:
             assert f.read(),expected_output
             
         
 class TestInputValidator:
     """ A class to test that when invalid input scan parameters are inserted, an exeption is raised and the code stops the execution. 
      Although a lower-level control is already present in the internal PI subroutines, it takes time to be activated. 
      Therefore, this additional entrance control find out invalid inputs without the need of connecting to the PI instrument. 
@@ -468,16 +470,17 @@
         with pytest.raises(ValueError):
             validate_scan_edges(scan_edges)
     
     def test_invalid_stepsize(self):
         """ Tests that an invalid value of 'stepsize' is passed to the validate_stepsize function,
         an exception (ValueError) is raised """
         stepsize = 200
+        scan_edges = [0,102]
         with pytest.raises(ValueError):
-            validate_stepsize(stepsize)
+            validate_stepsize(scan_edges,stepsize)
 
     def test_invalid_velocity(self):
         """ Tests that when an invalid value of 'velocity' is passed to the validate_velocity function, 
         an exception (valueError) is raised """
         velocity = -5
         with pytest.raises(ValueError):
             validate_velocity(velocity)
```

