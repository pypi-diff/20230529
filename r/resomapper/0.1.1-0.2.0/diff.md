# Comparing `tmp/resomapper-0.1.1.tar.gz` & `tmp/resomapper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resomapper-0.1.1.tar", max compression
+gzip compressed data, was "resomapper-0.2.0.tar", max compression
```

## Comparing `resomapper-0.1.1.tar` & `resomapper-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1094 2023-05-05 11:04:09.977115 resomapper-0.1.1/LICENSE
--rw-r--r--   0        0        0      857 2023-05-16 13:35:39.204986 resomapper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2519 2023-05-16 10:30:49.425506 resomapper-0.1.1/README.md
--rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.1.1/resomapper/__init__.py
--rw-r--r--   0        0        0     5397 2023-05-08 14:25:05.768941 resomapper-0.1.1/resomapper/cli.py
--rw-r--r--   0        0        0    19985 2023-05-08 14:58:43.872095 resomapper-0.1.1/resomapper/file_system_functions.py
--rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.1.1/resomapper/myrelax/__init__.py
--rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.1.1/resomapper/myrelax/getT1TR.py
--rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.1.1/resomapper/myrelax/getT2T2star.py
--rw-r--r--   0        0        0     8162 2023-05-08 14:53:50.954940 resomapper-0.1.1/resomapper/preprocessing.py
--rw-r--r--   0        0        0    59244 2023-05-16 12:48:57.064898 resomapper-0.1.1/resomapper/processing.py
--rw-r--r--   0        0        0     8977 2023-05-08 14:19:25.250029 resomapper-0.1.1/resomapper/utils.py
--rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 resomapper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2817 2023-05-19 14:13:54.847958 resomapper-0.2.0/LICENSE
+-rw-r--r--   0        0        0      857 2023-05-29 13:48:33.041389 resomapper-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2931 2023-05-24 10:04:14.557416 resomapper-0.2.0/README.md
+-rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.2.0/resomapper/__init__.py
+-rw-r--r--   0        0        0     5581 2023-05-29 13:46:36.947032 resomapper-0.2.0/resomapper/cli.py
+-rw-r--r--   0        0        0    19722 2023-05-29 13:46:36.947032 resomapper-0.2.0/resomapper/file_system_functions.py
+-rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.2.0/resomapper/myrelax/__init__.py
+-rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.2.0/resomapper/myrelax/getT1TR.py
+-rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.2.0/resomapper/myrelax/getT2T2star.py
+-rw-r--r--   0        0        0     8166 2023-05-22 13:05:31.541382 resomapper-0.2.0/resomapper/preprocessing.py
+-rw-r--r--   0        0        0    69042 2023-05-29 13:46:36.947032 resomapper-0.2.0/resomapper/processing.py
+-rw-r--r--   0        0        0    19243 2023-05-29 13:46:36.962655 resomapper-0.2.0/resomapper/utils.py
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 resomapper-0.2.0/PKG-INFO
```

### Comparing `resomapper-0.1.1/pyproject.toml` & `resomapper-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resomapper"
-version = "0.1.1"
+version = "0.2.0"
 description = "Pipeline for processing MR images and generating parametric maps."
 authors = ["Biomedical-MR"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "resomapper" }
```

### Comparing `resomapper-0.1.1/README.md` & `resomapper-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-# resomapper
+![resomapper](docs/_static/logo_fixed_white.svg)
+
+[![PyPI version](https://img.shields.io/pypi/v/resomapper?color=blue)](https://pypi.python.org/pypi/resomapper)
+[![Documentation Status](https://readthedocs.org/projects/resomapper/badge/?version=latest)](https://resomapper.readthedocs.io/en/latest/?badge=latest)
+[![License: MIT](https://img.shields.io/badge/license-MIT-orange)](https://opensource.org/licenses/MIT)
 
 Welcome to `resomapper`, a pipeline for processing MR images and generating parametric maps. 
 
 This tool is designed and developed by the *Biomedical Magnetic Resonance Lab* at the *Instituto de Investigaciones Biomédicas "Alberto Sols"* (CSIC-UAM). This project aims to collect a series of MR image processing tools written in Python under a friendly user interface for the lab needs. It is designed to streamline the processing of images, starting from raw adquisition files (we use Bruker study folders) to end up with parametric maps such as T1, T2 or T2* maps, as well as diffusion metric maps derived from DTI analysis.
 
 Note that `resomapper` is a tool under active development, with new features and improvements still on the way. It is used in-house for preclinical MRI data, mainly for mouse brain imaging, but can be used for different types of MRI data. Any suggestions are welcome!
 
+For more info, visit the [whole documentation](https://resomapper.readthedocs.io/en/latest).
+
 ## Installation
 
-Soon, resomapper will be available for installation via pip. Please stay tuned.
+To install **resomapper**, follow these steps:
+
+1. Make sure that you have Python installed on your system. Versions supported are **3.8** and above. 
+
+    * *Optional: create a virtual environment with conda or venv.*
+
+2. Install **resommaper** and all its dependencies running the following command from your terminal:
 
-```bash
-pip install resomapper
-```
+    ```
+    pip install resomapper
+    ```
 
-It is recommended to use this tool from a virtual environment, that can be created with conda or venv.
+3. If you have already been using **resomapper** and there is any new version available, you can use the following command to update it:
+
+    ```
+    pip install resomapper --upgrade
+    ```
 
 ## Usage
 
-The main feature of `resomapper` is its Command Line Interface, that can be started directly from the terminal with a single command:
+Then, to start using **resomapper**, you'll need to follow these steps:
+
+1. Prepare a working directory (an empty folder located wherever you want) and store inside the studies you want to process as folders in *Bruker* raw format.
+
+2. Enter the command shown below to run the program's Command Line Interface. 
+
+    ```
+    resomapper_cli
+    ```
 
-```bash
-resomapper_cli
-```
-
-After running this command, you'll only need to follow the instructions that will be shown in the terminal. Initially, you will need to provide a folder containing the studies to be processed in Bruker format. This is also where the result files will be stored. The structure of this root folder is the following:
-
-```
-└── root_folder
-    ├── study_folder_1
-    │   ├── 1
-    │   ├── 2
-    │   ...
-    │   └── ...
-    ├── study_folder_2
-    │   ├── 1
-    │   ├── 2
-    │   ...
-    │   └── ...
-    ...
-    ├── * convertidos 
-    ├── * procesados
-    └── * supplfiles 
+3. Follow the instructions shown in the terminal.
 
-* Automatically created after processing, storing the results. 
-```
+4. Finally, retrieve all the resulting maps and files obtained after processing from the same working folder you selected at the start of the program.
 
-For more info, visit the [resomapper docs](https://resomapper.readthedocs.io/en/latest).
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
```

### Comparing `resomapper-0.1.1/resomapper/cli.py` & `resomapper-0.2.0/resomapper/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # import click
 import multiprocessing
 import os
 import traceback
 import warnings
-from pathlib import Path
 
 from colorama import just_fix_windows_console
 
 import resomapper.file_system_functions as fs
 from resomapper.preprocessing import Preprocessing
 from resomapper.processing import (
     DTIProcessor,
@@ -17,19 +16,14 @@
 )
 from resomapper.utils import Headermsg as hmg
 from resomapper.utils import Mask, ask_user
 
 warnings.filterwarnings("ignore")
 
 
-# @click.command()
-def test():
-    print("Testing if this works! aaa")
-
-
 def cli():
     """Comand Line Interface of resomapper:
 
     1. Select root directory where studies are stored.
     2. Convert Bruker studies to nifti.
     3. Select of modalities to be processed.
     4. Process selected studies and save results.
@@ -92,50 +86,55 @@
             print(
                 f'\n\n\n\n{hmg.new_patient1}{"_".join(patient_name)} {hmg.new_patient2}'
             )
         prev_patient_name = patient_name[:]
         current_modal = study_name.split("_")[0]
         print(f"\n\n{hmg.new_modal}Procesamiento del mapa de {current_modal}")
 
-        mask_path = Path("/".join(study.parts[:-1])) / "mask.nii"
-        if mask_path.exists():
-            reuse_mask = ask_user(
-                "¿Deseas reutilizar la máscara creada para este sujeto?"
-            )
-
-        if (not mask_path.exists()) or (not reuse_mask):
-            mask = Mask(study)
-            correct_selection = False
-            while not correct_selection:
-                mask.create_mask()
-                correct_selection = ask_user(
-                    "¿Es la previsualización de la selección lo que deseas?"
-                )
-            print(f"\n{hmg.info}Máscara creada correctamente.")
-
-        want_preprocess = ask_user("¿Deseas realizar un preprocesado de este estudio?")
+        # Mask specification and creation
+        masker = Mask(study)
+        mode = masker.select_mask_mode()
+        mask_path = masker.create_mask(mode)
 
         if study_name.startswith("DT"):
             dti_map_pro = DTIProcessor(root_path, study)
-            if want_preprocess:
+            ok_mask = dti_map_pro.check_DTI_data()
+            while not ok_mask:
+                mode = masker.select_mask_mode()
+                mask_path = masker.create_mask(mode)
+                ok_mask = dti_map_pro.check_DTI_data()
+
+            if ask_user("¿Deseas realizar un preprocesado de este estudio?"):
                 Preprocessing([study]).preprocess()
             dti_map_pro.process_DTI()
 
         elif study_name.startswith("MT"):
             mt_map_pro = MTProcessor(study, mask_path)
-            if want_preprocess:
+            ok_mask = mt_map_pro.check_MT_data()
+            while not ok_mask:
+                mode = masker.select_mask_mode()
+                mask_path = masker.create_mask(mode)
+                ok_mask = mt_map_pro.check_MT_data()
+
+            if ask_user("¿Deseas realizar un preprocesado de este estudio?"):
                 Preprocessing([study]).preprocess()
             mt_map_pro.process_MT()
 
         else:
             n_cpu = multiprocessing.cpu_count() - 1
             t_map_pro = TMapProcessor(
                 study, mask_path, n_cpu=n_cpu, fitting_mode="nonlinear"
             )
-            if want_preprocess:
+            ok_mask = t_map_pro.check_T_data()
+            while not ok_mask:
+                mode = masker.select_mask_mode()
+                mask_path = masker.create_mask(mode)
+                ok_mask = t_map_pro.check_T_data()
+
+            if ask_user("¿Deseas realizar un preprocesado de este estudio?"):
                 Preprocessing([study]).preprocess()
             t_map_pro.process_T_map(f_time_paths)
 
     fs_builder.empty_supplfiles()
     print(f"\n{hmg.success}Procesamiento terminado.")
```

### Comparing `resomapper-0.1.1/resomapper/file_system_functions.py` & `resomapper-0.2.0/resomapper/file_system_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,34 +30,33 @@
 def select_file():
     """Allows selection of a file."""
 
     root = tk.Tk()
     root.withdraw()
     file_path = filedialog.askopenfilename()
     root.destroy()
-    root.mainloop()
+    # root.mainloop()
 
     return Path(file_path)
 
 
 def check_cwd(cwd: bool, return_cwd=True):
     """Checks if current work directory contains the studies.
     Otherwise, changes path.
 
-    Parameters
-    ----------
-        cwd : boolean
-            If True we are in the correct path, if False we are not
-            and a change of path is needed
-        return_cwd : bool
-            Return or not current work directory
-    Returns
-    --------
-        Path-like, optional
-            Current work directory can be returned
+    Args:
+        cwd (bool): If True, it indicates that we are in the correct path. If False, it
+            indicates that we are not in the correct path and a change of path
+            is needed.
+        return_cwd (bool, optional): Indicates whether to return the current working
+            directory or not. Defaults to True.
+
+    Returns:
+        path-like or None: The current working directory if return_cwd is True,
+        otherwise None (nothing is returned).
     """
     if not cwd:
         while True:
             data_path = input("¿Cuál es el directorio actual de los datos?\n")
             try:
                 os.chdir(data_path)  # change cwd to a given path
                 if return_cwd:
@@ -160,63 +159,55 @@
         ]
 
     def get_converted_files(self, known_modals=False):
         """Get those files we want to transfer to 'procesados' folder.
         Returns  a list including *method.txt, *.nii, *DwEffBval.txt and
         *DwGradVec.txt files."""
 
+        # add an uderscore to distingish T2 from T2E and change DTI per DT
+        modals = []
+        method_files = []
+        nii_files = []
+        dti_files = []
         # ask user for which modalities are desired to be processed
         if known_modals is False:
             self.modals_to_process = self.ask_preprocessing()
 
-            # add an uderscore to distingish T2 from T2E and change DTI per DT
-            modals = []
             for modal in self.modals_to_process:
                 if modal == "DTI":
                     modals.append("DT_")
                 else:
                     modals.append(modal + "_")
 
-            method_files = []
-            nii_files = []
-            dti_files = []
             for modal in modals:
                 method_files += list(
                     self.path_converted.glob(f"*/{modal}*/*method.txt")
                 )
                 nii_files += list(self.path_converted.glob(f"*/{modal}*/*.nii*"))
                 dti_files += list(
                     self.path_converted.glob(f"*/{modal}*/*DwEffBval.txt")
                 ) + list(self.path_converted.glob(f"*/{modal}*/*DwGradVec.txt"))
 
-            return method_files + nii_files + dti_files
-
         else:
-            # known_modals only has one modality
-            # add an uderscore to distingish T2 from T2E and change DTI per DT
-            modals = []
             for modal in known_modals:
                 if modal == "DTI":
                     modals.append("DT_")
                 else:
                     modals.append(modal + "_")
 
-            method_files = []
-            nii_files = []
-            dti_files = []
             for modal in known_modals:
                 method_files += list(
                     self.path_converted.glob(f"*/{modal}*/*method.txt")
                 )
                 nii_files += list(self.path_converted.glob(f"*/{modal}*/*.nii*"))
                 dti_files += list(
                     self.path_converted.glob(f"*/{modal}*/*DwEffBval.txt")
                 ) + list(self.path_converted.glob(f"*/{modal}*/*DwGradVec.txt"))
 
-            return method_files + nii_files + dti_files
+        return method_files + nii_files + dti_files
 
     def transfer_files(self, src_paths=None, dst_paths=None):
         """Transfer files from 'convertidos' to 'procesados' folder.
         If folder alredy exists in destiny, it will not be overwritten.
 
         Parameters
         ----------
@@ -269,27 +260,27 @@
                 adq_lines = f.readlines()
         except FileNotFoundError:
             # patch to avoid 'variable referenced before assignment error'
             adq_lines = [""]
 
         # rename study subfolder
         if adq_lines[0] == "RAREVTR":  # T1
-            r_study_subfolder = Path("/".join(study_subfolder.parts[0:-1])) / (
+            r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
                 "T1_" + study_subfolder.parts[-1]
             )
             os.rename(study_subfolder, r_study_subfolder)
 
         elif adq_lines[0] == "MGE":  # T2STAR
-            r_study_subfolder = Path("/".join(study_subfolder.parts[0:-1])) / (
+            r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
                 "T2E_" + study_subfolder.parts[-1]
             )
             os.rename(study_subfolder, r_study_subfolder)
 
         elif adq_lines[0] == "DtiEpi":  # DIFFUSION
-            r_study_subfolder = Path("/".join(study_subfolder.parts[0:-1])) / (
+            r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
                 "DT_" + study_subfolder.parts[-1]
             )
             os.rename(study_subfolder, r_study_subfolder)
 
         elif adq_lines[0] == "MSME":  # T2, M0 or MT
             f_method = study_subfolder.parts[-1] + "_method.txt"
             path_met = study_subfolder / f_method  # path to *method.txt file
@@ -300,36 +291,33 @@
             except FileNotFoundError:
                 print(f"{hmg.error}Archivo no encontrado.")
 
             for line in met_lines:
                 if not line.startswith("EffectiveTE"):
                     continue
                 elif len(line) > 35:
-                    r_study_subfolder = Path("/".join(study_subfolder.parts[0:-1])) / (
+                    r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
                         "T2_" + study_subfolder.parts[-1]
                     )
                     os.rename(study_subfolder, r_study_subfolder)
                     return None
                 else:
                     if "MagTransOnOff = On \n" in met_lines:
                         r_study_subfolder = Path(
-                            "/".join(study_subfolder.parts[0:-1])
+                            "/".join(study_subfolder.parts[:-1])
                         ) / ("MT_" + study_subfolder.parts[-1])
                         os.rename(study_subfolder, r_study_subfolder)
-                        return None
                     elif ("MagTransOnOff = Off \n" in met_lines) and (
                         "DigFilter = Digital_Medium \n" in met_lines
                     ):
                         r_study_subfolder = Path(
-                            "/".join(study_subfolder.parts[0:-1])
+                            "/".join(study_subfolder.parts[:-1])
                         ) / ("M0_" + study_subfolder.parts[-1])
                         os.rename(study_subfolder, r_study_subfolder)
-                        return None
-                    else:
-                        return None
+                    return None
 
     def get_modality(self, study_subfolder_path: str):
         """Returns the modality of a subfolder path such as
         "C:// * //T2_convertidos*"
         """
         if study_subfolder_path.parts[-1][:3] == "T1_":
             return "T1"
@@ -374,26 +362,27 @@
                         or (
                             ("MT_map" in str([f for f in os.walk(subfolder)]))
                             and modal == "MT"
                         )
                     ):
                         patient = "_".join(subfolder.parts[-2].split("_")[1:])
                         msg = (
-                            f"La modalidad {processed_modal} del estudio {patient} ya ha "
-                            "sido procesada.\n¿Desea volver a procesarla?"
+                            f"La modalidad {processed_modal} del estudio {patient} ya "
+                            "ha sido procesada.\n¿Desea volver a procesarla?"
                         )
                         avoid_subfolder = ut.ask_user(msg)
                         if avoid_subfolder:  # if process again
                             ready = ""
                             while ready != "y":
                                 msg = (
-                                    f"\n{hmg.warn}El resultado del procesamiento anterior "
-                                    f"de {processed_modal} del estudio {patient} no se conservará.\n"
-                                    f'\n{hmg.ask}Si desea guardarlo debe hacerlo ahora. Pulse "y" para '
-                                    f"continuar.\n{hmg.pointer}"
+                                    f"\n{hmg.warn}El resultado del procesamiento "
+                                    f"anterior de {processed_modal} del estudio "
+                                    f"{patient} no se conservará.\n"
+                                    f"\n{hmg.ask}Si desea guardarlo debe hacerlo ahora."
+                                    f' Pulse "y" para continuar.\n{hmg.pointer}'
                                 )
                                 ready = input(msg)
                                 ready = ready.lower()
 
                     # remove folder and files contained in it
                     shutil.rmtree(str(subfolder))
                     # create folder again
```

### Comparing `resomapper-0.1.1/resomapper/myrelax/getT1TR.py` & `resomapper-0.2.0/resomapper/myrelax/getT1TR.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.1.1/resomapper/myrelax/getT2T2star.py` & `resomapper-0.2.0/resomapper/myrelax/getT2T2star.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.1.1/resomapper/preprocessing.py` & `resomapper-0.2.0/resomapper/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import warnings
 from math import trunc
 from tkinter.messagebox import askyesno
 
 import matplotlib.pyplot as plt
 import nibabel as nib
 import numpy as np
-from scipy.ndimage import rotate
+
+# from scipy.ndimage import rotate
 from skimage.restoration import denoise_nl_means
 from skimage.transform import rotate
 
 from resomapper.utils import Headermsg as hmg  # Added by Raquel
 from resomapper.utils import ask_user
 
 warnings.filterwarnings("ignore")
```

### Comparing `resomapper-0.1.1/resomapper/processing.py` & `resomapper-0.2.0/resomapper/processing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import glob
 import os
 import re
 import shutil
 import tkinter as tk
 import warnings
 from pathlib import Path
-from tkinter import *
 
 import dipy.reconst.dti as dti
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 from dipy.core.gradients import gradient_table
@@ -20,15 +19,15 @@
     _nlls_err_func,
     apparent_diffusion_coef,
     fractional_anisotropy,
 )
 
 from resomapper.myrelax import getT1TR, getT2T2star
 from resomapper.utils import Headermsg as hmg
-from resomapper.utils import ask_user
+from resomapper.utils import ask_user, check_shapes
 
 warnings.filterwarnings("ignore")
 
 
 ###############################################################################
 # MT PROCESSING
 ###############################################################################
@@ -39,14 +38,15 @@
         self.mt_study_path = mt_study_path
         self.mask_path = mask_path
         self.path_mt = path_mt
         self.path_m0 = path_m0
 
         self.rename_mt_on()
         self.get_associated_mt_off()
+        self.select_MT_acq()
 
     def rename_mt_on(self):
         for f in list(self.mt_study_path.glob("*.nii.gz")):
             new_filename = f.parts[-1].replace("procesado", "procesado_MT")
             shutil.move(os.path.join(f), os.path.join(self.mt_study_path, new_filename))
 
     def get_associated_mt_off(self):
@@ -66,152 +66,292 @@
         )
         study_path = list(study_path.glob("M0*"))[0]
         for f in list(study_path.glob("*.nii.gz")):
             new_filename = f.parts[-1].replace("convertido", "procesado_M0")
             shutil.copy(os.path.join(f), os.path.join(self.mt_study_path, new_filename))
         # return study_path
 
-    def compute_MT_map(self, mton_image: np.array, mtoff_image: np.array):
-        """Computes the formula required to get ratio MT map."""
-
-        mt_map = 100 * (1 - (mton_image / mtoff_image))
-        mt_map[mt_map < 0] = 0
-
-        return mt_map
-
-    def process_MT(self):
-        """Generates ratio MT maps. Saves map as a nifti file and
-        saves heatmaps as .png images."""
-
+    def select_MT_acq(self):
         n_mt = int(len(list(self.mt_study_path.glob("*.nii.gz"))) / 2)
 
         if n_mt == 1:
-            f_mton_path = list(self.mt_study_path.glob("procesado_MT_*.nii.gz"))[0]
-            f_mtoff_path = list(self.mt_study_path.glob("procesado_M0_*.nii.gz"))[0]
-
-            # from nifti to array
-            mt_on, affine1 = load_nifti(f_mton_path)
-            mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
-            mask, _ = load_nifti(self.mask_path)
-
-            # apply mask
-            mt_on = mt_on * mask
-            mt_off = mt_off * mask
-
-            # get maps
-            print(f"\n{hmg.info}Generando mapa de MT.")
-            mt_map = self.compute_MT_map(mt_on, mt_off)
-
-            # save as .nii file and save heatmaps
-            saving_path = str(self.mt_study_path / "MT_map.nii")
-            save_nifti(saving_path, mt_map.astype(np.float32), affine1)
-            Heatmap().save_heatmap(mt_map, "MT", out_path=str(self.mt_study_path))
+            mt_folders_list = [1]
         else:
             print(
-                f"\n{hmg.warn}Has adquirido imágenes de MT con diferentes slopes para este estudio ({n_mt})."
+                f"\n{hmg.warn}Has adquirido imágenes de MT con diferentes slopes para "
+                f"este estudio ({n_mt})."
             )
 
             input_ready = False
-            while input_ready == False:
+            while not input_ready:
                 mt_folders_input = input(
-                    f"\n{hmg.ask}Indica el número de la carpeta de adquisición que desas procesar (entre 1 y {n_mt}). "
-                    f'Si deseas procesar más de una carpeta, introduce los diferentes números separados por ",".\n{hmg.pointer}'
+                    f"\n{hmg.ask}Indica el número de la carpeta de adquisición que "
+                    f"desas procesar (entre 1 y {n_mt}). "
+                    "Si deseas procesar más de una carpeta, introduce los diferentes "
+                    f'números separados por ",".\n{hmg.pointer}'
                 )
                 mt_folders_input = mt_folders_input.split(",")
                 try:
                     mt_folders_list = [int(x.strip()) for x in mt_folders_input]
                     input_ready = True
                     for number in mt_folders_list:
                         if (number > n_mt) or (number < 1):
                             print(
-                                f"\n{hmg.error}Por favor, introduce números entre 1 y {n_mt}."
+                                f"\n{hmg.error}Por favor, introduce números entre "
+                                f"1 y {n_mt}."
                             )
                             input_ready = False
                             break
                 except Exception:
                     print(
-                        f'\n{hmg.error}Por favor, introduce sólo números separados por "," (si hay más de uno).'
+                        f"\n{hmg.error}Por favor, introduce sólo números separados por "
+                        '"," (si hay más de uno).'
                     )
 
-            mt_folders_list = [*set(mt_folders_list)]
+        self.n_mt_folders = n_mt
+        self.selected_mt_folders_list = mt_folders_list
 
-            if len(mt_folders_list) == 1:
-                subscan_index = mt_folders_list[0] - 1
+    def check_MT_data(self):
+        ok_masks_list = []
+        for i in self.selected_mt_folders_list:
+            if self.n_mt_folders == 1:
+                f_mton_path = list(self.mt_study_path.glob("procesado_MT_*.nii.gz"))[0]
+                f_mtoff_path = list(self.mt_study_path.glob("procesado_M0_*.nii.gz"))[0]
+                print(f"\n{hmg.info}Comprobando la máscara.")
+            else:
+                subscan_index = i - 1
                 f_mton_path = list(
                     self.mt_study_path.glob(
                         f"procesado_MT_*subscan_{subscan_index}.nii*"
                     )
                 )[0]
                 f_mtoff_path = list(
                     self.mt_study_path.glob(
                         f"procesado_M0_*subscan_{subscan_index}.nii*"
                     )
                 )[0]
+                print(f"\n{hmg.info}Comprobando la máscara (carpeta {i}).")
 
-                # from nifti to array
-                mt_on, affine1 = load_nifti(f_mton_path)
-                mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
-                mask, _ = load_nifti(self.mask_path)
-
-                # apply mask
-                mt_on = mt_on * mask
-                mt_off = mt_off * mask
+            ok_masks_list.extend(
+                (
+                    check_shapes(f_mton_path, self.mask_path),
+                    check_shapes(f_mtoff_path, self.mask_path),
+                )
+            )
+        return all(ok_masks_list)
+
+    def compute_MT_map(self, mton_image: np.array, mtoff_image: np.array):
+        """Computes the formula required to get ratio MT map."""
+
+        mt_map = 100 * (1 - (mton_image / mtoff_image))
+        mt_map[mt_map < 0] = 0
+
+        return mt_map
+
+    def process_MT(self):
+        """Generates ratio MT maps. Saves map as a nifti file and
+        saves heatmaps as .png images."""
+
+        for i in self.selected_mt_folders_list:
+            if self.n_mt_folders == 1:
+                f_mton_path = list(self.mt_study_path.glob("procesado_MT_*.nii.gz"))[0]
+                f_mtoff_path = list(self.mt_study_path.glob("procesado_M0_*.nii.gz"))[0]
+            else:
+                subscan_index = i - 1
+                f_mton_path = list(
+                    self.mt_study_path.glob(
+                        f"procesado_MT_*subscan_{subscan_index}.nii*"
+                    )
+                )[0]
+                f_mtoff_path = list(
+                    self.mt_study_path.glob(
+                        f"procesado_M0_*subscan_{subscan_index}.nii*"
+                    )
+                )[0]
+
+            # from nifti to array
+            mt_on, affine1 = load_nifti(f_mton_path)
+            mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
+            mask, _ = load_nifti(self.mask_path)
+
+            # check_shapes(mt_on, mask)
+            # check_shapes(mt_off, mask)
+
+            # apply mask
+            mt_on = mt_on * mask
+            mt_off = mt_off * mask
 
+            if len(self.selected_mt_folders_list) > 1:
+                # get maps
+                print(f"\n{hmg.info}Generando mapa de MT (carpeta {i}).")
+                mt_map = self.compute_MT_map(mt_on, mt_off)
+
+                os.mkdir(str(self.mt_study_path / str(i)))
+
+                # save as .nii file and save heatmaps
+                mt_map_filename = f"MT_map_{str(i)}.nii"
+                saving_path = os.path.join(
+                    str(self.mt_study_path), str(i), mt_map_filename
+                )
+                save_nifti(saving_path, mt_map.astype(np.float32), affine1)
+                Heatmap().save_heatmap(
+                    mt_map,
+                    "MT",
+                    out_path=os.path.join(str(self.mt_study_path), str(i)),
+                )
+            else:
                 # get maps
                 print(f"\n{hmg.info}Generando mapa de MT.")
                 mt_map = self.compute_MT_map(mt_on, mt_off)
 
                 # save as .nii file and save heatmaps
                 saving_path = str(self.mt_study_path / "MT_map.nii")
                 save_nifti(saving_path, mt_map.astype(np.float32), affine1)
                 Heatmap().save_heatmap(mt_map, "MT", out_path=str(self.mt_study_path))
 
-            else:
-                for i in mt_folders_list:
-                    subscan_index = i - 1
-                    f_mton_path = list(
-                        self.mt_study_path.glob(
-                            f"procesado_MT_*subscan_{subscan_index}.nii*"
-                        )
-                    )[0]
-                    f_mtoff_path = list(
-                        self.mt_study_path.glob(
-                            f"procesado_M0_*subscan_{subscan_index}.nii*"
-                        )
-                    )[0]
+        # n_mt = int(len(list(self.mt_study_path.glob("*.nii.gz"))) / 2)
 
-                    # from nifti to array
-                    mt_on, affine1 = load_nifti(f_mton_path)
-                    mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
-                    mask, _ = load_nifti(self.mask_path)
-
-                    # apply mask
-                    mt_on = mt_on * mask
-                    mt_off = mt_off * mask
-
-                    # get maps
-                    print(f"\n{hmg.info}Generando mapa de MT (carpeta {i}).")
-                    mt_map = self.compute_MT_map(mt_on, mt_off)
-
-                    try:
-                        os.mkdir(str(self.mt_study_path / str(i)))
-                    except Exception:
-                        pass
-
-                    # save as .nii file and save heatmaps
-                    mt_map_filename = "MT_map_" + str(i) + ".nii"
-                    saving_path = os.path.join(
-                        str(self.mt_study_path), str(i), mt_map_filename
-                    )
-                    save_nifti(saving_path, mt_map.astype(np.float32), affine1)
-                    Heatmap().save_heatmap(
-                        mt_map,
-                        "MT",
-                        out_path=os.path.join(str(self.mt_study_path), str(i)),
-                    )
+        # if n_mt == 1:
+        #     f_mton_path = list(self.mt_study_path.glob("procesado_MT_*.nii.gz"))[0]
+        #     f_mtoff_path = list(self.mt_study_path.glob("procesado_M0_*.nii.gz"))[0]
+
+        #     # from nifti to array
+        #     mt_on, affine1 = load_nifti(f_mton_path)
+        #     mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
+        #     mask, _ = load_nifti(self.mask_path)
+
+        #     check_shapes(mt_on, mask)
+        #     check_shapes(mt_off, mask)
+
+        #     # apply mask
+        #     mt_on = mt_on * mask
+        #     mt_off = mt_off * mask
+
+        #     # get maps
+        #     print(f"\n{hmg.info}Generando mapa de MT.")
+        #     mt_map = self.compute_MT_map(mt_on, mt_off)
+
+        #     # save as .nii file and save heatmaps
+        #     saving_path = str(self.mt_study_path / "MT_map.nii")
+        #     save_nifti(saving_path, mt_map.astype(np.float32), affine1)
+        #     Heatmap().save_heatmap(mt_map, "MT", out_path=str(self.mt_study_path))
+        # else:
+        #     print(
+        #         f"\n{hmg.warn}Has adquirido imágenes de MT con diferentes slopes "
+        #         f"para este estudio ({n_mt})."
+        #     )
+
+        #     input_ready = False
+        #     while not input_ready:
+        #         mt_folders_input = input(
+        #             f"\n{hmg.ask}Indica el número de la carpeta de adquisición que "
+        #             f"desas procesar (entre 1 y {n_mt}). "
+        #             "Si deseas procesar más de una carpeta, introduce los diferentes "
+        #             f'números separados por ",".\n{hmg.pointer}'
+        #         )
+        #         mt_folders_input = mt_folders_input.split(",")
+        #         try:
+        #             mt_folders_list = [int(x.strip()) for x in mt_folders_input]
+        #             input_ready = True
+        #             for number in mt_folders_list:
+        #                 if (number > n_mt) or (number < 1):
+        #                     print(
+        #                         f"\n{hmg.error}Por favor, introduce números entre 1 y"
+        #                         f" {n_mt}."
+        #                     )
+        #                     input_ready = False
+        #                     break
+        #         except Exception:
+        #             print(
+        #                 f'\n{hmg.error}Por favor, introduce sólo números separados'
+        #                 f' por "," (si hay más de uno).'
+        #             )
+
+        #     mt_folders_list = [*set(mt_folders_list)]
+
+        #     if len(mt_folders_list) == 1:
+        #         subscan_index = mt_folders_list[0] - 1
+        #         f_mton_path = list(
+        #             self.mt_study_path.glob(
+        #                 f"procesado_MT_*subscan_{subscan_index}.nii*"
+        #             )
+        #         )[0]
+        #         f_mtoff_path = list(
+        #             self.mt_study_path.glob(
+        #                 f"procesado_M0_*subscan_{subscan_index}.nii*"
+        #             )
+        #         )[0]
+
+        #         # from nifti to array
+        #         mt_on, affine1 = load_nifti(f_mton_path)
+        #         mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
+        #         mask, _ = load_nifti(self.mask_path)
+
+        #         check_shapes(mt_on, mask)
+        #         check_shapes(mt_off, mask)
+
+        #         # apply mask
+        #         mt_on = mt_on * mask
+        #         mt_off = mt_off * mask
+
+        #         # get maps
+        #         print(f"\n{hmg.info}Generando mapa de MT.")
+        #         mt_map = self.compute_MT_map(mt_on, mt_off)
+
+        #         # save as .nii file and save heatmaps
+        #         saving_path = str(self.mt_study_path / "MT_map.nii")
+        #         save_nifti(saving_path, mt_map.astype(np.float32), affine1)
+        #         Heatmap().save_heatmap(mt_map, "MT", out_path=str(self.mt_study_path))
+
+        #     else:
+        #         for i in mt_folders_list:
+        #             subscan_index = i - 1
+        #             f_mton_path = list(
+        #                 self.mt_study_path.glob(
+        #                     f"procesado_MT_*subscan_{subscan_index}.nii*"
+        #                 )
+        #             )[0]
+        #             f_mtoff_path = list(
+        #                 self.mt_study_path.glob(
+        #                     f"procesado_M0_*subscan_{subscan_index}.nii*"
+        #                 )
+        #             )[0]
+
+        #             # from nifti to array
+        #             mt_on, affine1 = load_nifti(f_mton_path)
+        #             mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
+        #             mask, _ = load_nifti(self.mask_path)
+
+        #             check_shapes(mt_on, mask)
+        #             check_shapes(mt_off, mask)
+
+        #             # apply mask
+        #             mt_on = mt_on * mask
+        #             mt_off = mt_off * mask
+
+        #             # get maps
+        #             print(f"\n{hmg.info}Generando mapa de MT (carpeta {i}).")
+        #             mt_map = self.compute_MT_map(mt_on, mt_off)
+
+        #             try:
+        #                 os.mkdir(str(self.mt_study_path / str(i)))
+        #             except Exception:
+        #                 pass
+
+        #             # save as .nii file and save heatmaps
+        #             mt_map_filename = f"MT_map_{str(i)}.nii"
+        #             saving_path = os.path.join(
+        #                 str(self.mt_study_path), str(i), mt_map_filename
+        #             )
+        #             save_nifti(saving_path, mt_map.astype(np.float32), affine1)
+        #             Heatmap().save_heatmap(
+        #                 mt_map,
+        #                 "MT",
+        #                 out_path=os.path.join(str(self.mt_study_path), str(i)),
+        #             )
 
 
 ###############################################################################
 # DTI PROCESSING
 ###############################################################################
 class DTIProcessor:
     def __init__(self, root_path: str, study_path: str) -> None:
@@ -222,15 +362,16 @@
         """
         Ask the user to enter b values, number of basal images and number of directions.
         """
         while True:
             try:
                 n_b_val = int(
                     input(
-                        f"\n{hmg.ask}¿Número de b valores para cada dirección?\n{hmg.pointer}"
+                        f"\n{hmg.ask}¿Número de b valores para cada dirección?"
+                        f"\n{hmg.pointer}"
                     )
                 )
                 break
             except ValueError:
                 print(f"{hmg.error}Debes introducir un número.")
         while True:
             try:
@@ -266,46 +407,52 @@
                 elif line.startswith("DwNDiffExpEach"):
                     n_b_val_real = int(re.search("\d+", line).group(0))
                 elif line.startswith("DwAoImages"):
                     n_basal_real = int(re.search("\d+", line).group(0))
 
         if n_b_val != n_b_val_real:
             print(
-                f"\n{hmg.warn}Has introducido un número de b valores diferente al adquirido."
+                f"\n{hmg.warn}Has introducido un número de b valores diferente "
+                "al adquirido."
             )
             print(
-                f"Has especificado {n_b_val}, cuando se adquirieron {n_b_val_real}. Se va a continuar con el valor real."
+                f"Has especificado {n_b_val}, cuando se adquirieron {n_b_val_real}. "
+                "Se va a continuar con el valor real."
             )
             n_b_val = n_b_val_real
         else:
             print(f"\n{hmg.info}Número de b valores correcto.")
 
         if n_basal != n_basal_real:
             print(
-                f"\n{hmg.warn}Has introducido un valor de imágenes basales diferente al adquirido."
+                f"\n{hmg.warn}Has introducido un valor de imágenes basales diferente "
+                "al adquirido."
             )
             print(
-                f"Has especificado {n_basal}, cuando se adquirieron {n_basal_real}. Se va a continuar con el valor real."
+                f"Has especificado {n_basal}, cuando se adquirieron {n_basal_real}. "
+                "Se va a continuar con el valor real."
             )
             n_basal = n_basal_real
         else:
             print(f"\n{hmg.info}Número de imágenes basales correcto.")
 
         if n_dirs != n_dirs_real:
             print(
-                f"\n{hmg.warn}Has introducido un valor de direcciones diferente al adquirido."
+                f"\n{hmg.warn}Has introducido un valor de direcciones diferente "
+                "al adquirido."
             )
             print(f"Has especificado {n_dirs}, cuando se adquirieron {n_dirs_real}.")
             valid_n_dirs = False
-            while valid_n_dirs == False:
+            while not valid_n_dirs:
                 if n_dirs > n_dirs_real:
                     while True:
                         try:
                             print(
-                                f"\nPrueba otra vez. Debes intruducir un valor menor o igual a {n_dirs_real}."
+                                "\nPrueba otra vez. Debes intruducir un valor "
+                                f"menor o igual a {n_dirs_real}."
                             )
                             n_dirs = int(
                                 input(
                                     f"{hmg.ask}¿Número de direcciones?\n{hmg.pointer}"
                                 )
                             )
                             break
@@ -313,51 +460,56 @@
                             print(f"{hmg.error}Debes introducir un número.")
                 else:
                     valid_n_dirs = True
 
         if n_dirs == n_dirs_real:
             print(f"\n{hmg.info}Número de direcciones correcto.")
             new_dirs = ask_user(
-                f"¿Deseas eliminar direcciones antes de continuar? En caso contrario, se continuará con el número original ({n_dirs_real})."
+                "¿Deseas eliminar direcciones antes de continuar? En caso contrario,"
+                f" se continuará con el número original ({n_dirs_real})."
             )
             if new_dirs:
                 while True:
                     try:
                         n_dirs_to_rm = int(
                             input(
-                                f"\n{hmg.ask}¿Cuántas direcciones deseas eliminar?\n{hmg.pointer}"
+                                f"\n{hmg.ask}¿Cuántas direcciones deseas eliminar?"
+                                f"\n{hmg.pointer}"
                             )
                         )
                         if 0 <= n_dirs_to_rm < n_dirs_real:
                             n_dirs = n_dirs_real - n_dirs_to_rm
                             break
                         else:
                             print(
-                                f"{hmg.error}Debes introducir un número entre 0 y {n_dirs_real}."
+                                f"{hmg.error}Debes introducir un número entre "
+                                f"0 y {n_dirs_real}."
                             )
                     except ValueError:
                         print(f"{hmg.error}Debes introducir un número.")
         else:
             new_dirs = True
             n_dirs_to_rm = n_dirs_real - n_dirs
             ok_n_dirs_to_rm = ask_user(f"¿Deseas eliminar {n_dirs_to_rm} direcciones?")
             if not ok_n_dirs_to_rm:
                 while True:
                     try:
                         n_dirs_to_rm = int(
                             input(
-                                f"\n{hmg.ask}¿Cuántas direcciones deseas eliminar?\n{hmg.pointer}"
+                                f"\n{hmg.ask}¿Cuántas direcciones deseas eliminar?"
+                                f"\n{hmg.pointer}"
                             )
                         )
                         if 0 <= n_dirs_to_rm < n_dirs_real:
                             n_dirs = n_dirs_real - n_dirs_to_rm
                             break
                         else:
                             print(
-                                f"{hmg.error}Debes introducir un número entre 0 y {n_dirs_real}."
+                                f"{hmg.error}Debes introducir un número entre "
+                                f"0 y {n_dirs_real}."
                             )
                     except ValueError:
                         print(f"{hmg.error}Debes introducir un número.")
             else:
                 n_dirs = n_dirs_real - n_dirs_to_rm
 
         indexes_to_rm = []
@@ -374,15 +526,16 @@
                         if (1 <= temp <= n_dirs_real) and (temp not in dirs_to_rm):
                             dirs_to_rm.append(temp)
                             break
                         elif temp in dirs_to_rm:
                             print(f"{hmg.error}Esa dirección ya la has especificado.")
                         else:
                             print(
-                                f"{hmg.error}Debes introducir un número entre 1 y {n_dirs_real}."
+                                f"{hmg.error}Debes introducir un número "
+                                f"entre 1 y {n_dirs_real}."
                             )
                     except ValueError:
                         print(f"{hmg.error}Debes introducir un número.")
 
             # Ir eliminando de abajo hacia arriba
             dirs_to_rm.sort(reverse=True)
 
@@ -405,15 +558,16 @@
             print(b_vals, "\n")
 
             print(f"{hmg.info}Mostrado listado de direcciones modificadas.\n")
             print(dirs, "\n")
         else:
             b_vals = np.loadtxt(src_bvals)
             print(
-                f"\n{hmg.info}Mostrado lista de valores b adquirida del archivo métodos.\n"
+                f"\n{hmg.info}Mostrado lista de valores b adquirida del archivo "
+                "métodos.\n"
             )
             print(b_vals, "\n")
 
             dirs = np.loadtxt(src_dirs)
             print(f"{hmg.info}Mostrado direcciones del archivo métodos.\n")
             print(dirs, "\n")
 
@@ -466,27 +620,53 @@
             pmap[pmap > 0.95] = float("nan")
 
         if self.f_R2_maps_slc is not None:
             pmap = pmap * self.f_R2_maps_slc
 
         return pmap
 
+    def check_DTI_data(self):
+        """Check the adquisited images for DTI maps match with the specified
+        mask by calling the 'check_shapes' function to compare their shapes.
+
+        Returns:
+            bool: True if the shapes of the image and mask match, False otherwise.
+        """
+        # read nii file with diffusion images and nii file with masks/rois
+        try:
+            nii_fname = (
+                self.study_path / f"{self.study_path.parts[-1][3:]}_subscan_0.nii.gz"
+            )
+            data, affine = load_nifti(nii_fname)
+        except FileNotFoundError:
+            nii_fname = self.study_path / f"{self.study_path.parts[-1][3:]}.nii.gz"
+            data, affine = load_nifti(nii_fname)
+
+        try:
+            mask, affine = load_nifti(self.study_path / "mask.nii")
+        except FileNotFoundError:
+            mask, affine = load_nifti(
+                Path("/".join(self.study_path.parts[:-1])) / "mask.nii"
+            )
+
+        return check_shapes(data, mask)
+
     def process_DTI(self):
         """Solves diffusion tensor using Non-Linear Least Squares (NLLS) and
         computes ADC, FA, MD, AD, RD and R^2 maps."""
 
         n_b_val, n_basal, n_dirs = self.ask_dti_info()
 
         # create B values and B dirs files
         f_bvals = self.root_path / "supplfiles" / "Bvalues.bval"
         f_dirs = self.root_path / "supplfiles" / "Bdirs.bvec"
 
         b_vals, dirs, n_b_val, n_basal, n_dirs, indexes_to_rm = self.get_bvals_n_dirs(
             n_b_val, n_basal, n_dirs
-        )  # Changed by Raquel: add args to function
+        )
 
         with open(f_bvals, "w") as f:
             for b_val in b_vals:
                 content = str(b_val) + " "
                 f.write(content)
 
         list_dirs = np.array(dirs).tolist()
@@ -512,14 +692,31 @@
         try:
             mask, affine = load_nifti(self.study_path / "mask.nii")
         except FileNotFoundError:
             mask, affine = load_nifti(
                 Path("/".join(self.study_path.parts[:-1])) / "mask.nii"
             )
 
+        # check_shapes(
+        #     data, mask, callback_func=self.process_DTI, study_path=self.study_path
+        # )
+        # ok_mask = check_shapes(data, mask)
+        # while not ok_mask:
+        #     mode = self.masker.select_mask_mode()
+        #     self.masker.create_mask(mode)
+        #     # while True:
+        #     #     try:
+        #     #         masker.create_mask(mode)
+        #     #         break
+        #     #     except PermissionError:
+        #     #         print("retrying")
+        #     #         time.sleep(5)
+        #     mask, affine = load_nifti(self.study_path / "mask.nii")
+        #     ok_mask = check_shapes(data, mask)
+
         # apply mask
         for i in range(data.shape[3]):  # para cada imagen de cada slice
             data[:, :, :, i] = data[:, :, :, i] * mask
 
         # read b values (bvals) and gradient directions (bvecs)
         bval_path = str(self.root_path / "supplfiles" / "bvalues.bval")
         bvec_path = str(self.root_path / "supplfiles" / "Bdirs.bvec")
@@ -615,15 +812,15 @@
 
         # get residuals: difference between real data and predicted data
         residuals = norm_data - predicted_signal
 
         R2_maps = []
         print(f"\n{hmg.info}Generando mapas de R\u00b2.")
         if n_b_val > 1:
-            for d in range(0, n_dirs):
+            for d in range(n_dirs):
                 # residuals
                 # dir_res = residuals[
                 #     :, :, :, (leap[d] + 1) : ((leap[d]) + (1 + n_b_val))
                 # ]
                 # full_res = np.concatenate((basal_residuals, dir_res), axis=-1)
 
                 # # data
@@ -844,15 +1041,15 @@
                     )
                 )
                 break
             except ValueError:
                 print("No has introducido un número correcto.")
 
         print("Deberás introducir los TR de mayor a menor.\n")
-        for i in range(0, n_tr):
+        for i in range(n_tr):
             tr = input(f"Introduce el tiempo de repetición {i+1}.\n")
             trs.append(tr)
 
         return trs
 
     def get_TE(self):
         init_te = int(input("¿Primer tiempo de eco en T2? "))
@@ -942,39 +1139,62 @@
         self, study_path: str, mask_path: str, n_cpu: int, fitting_mode="nonlinear"
     ) -> None:
         self.study_path = study_path
         self.mask_path = mask_path
         self.fitting_mode = fitting_mode
         self.n_cpu = n_cpu
 
+    def check_T_data(self):
+        """Check the adquisited images for T1, T2 or T2E maps match with the specified
+        mask by calling the 'check_shapes' function to compare their shapes.
+
+        Returns:
+            bool: True if the shapes of the image and mask match, False otherwise.
+        """
+        index = 4 if "T2E_" in str(self.study_path) else 3
+        try:
+            f_name = f"{self.study_path.parts[-1][index:]}_subscan_0.nii.gz"
+            f_path = str(self.study_path / f_name)
+            return check_shapes(f_path, self.mask_path)
+        except (NameError, FileNotFoundError):
+            f_name = f"{self.study_path.parts[-1][index:]}.nii.gz"
+            f_path = str(self.study_path / f_name)
+            return check_shapes(f_path, self.mask_path)
+
     def process_T_map(self, time_paths):
         """Processing of T1, T2, T2* maps using functions located in "myrelax".
         R^2 map is also computed. All maps are saved.
         """
 
         if "T2_" in str(self.study_path):
             method = "T2"
             print(f"\n{hmg.info}Generando mapa de T2.\n")
             try:
                 f_name = self.study_path.parts[-1][3:] + "_subscan_0.nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
+
+                # check_shapes(f_path, self.mask_path)
+
                 getT2T2star.TxyFitME(
                     f_path,
                     time_paths[1],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
                 )
 
-            except NameError:
+            except (NameError, FileNotFoundError):
                 f_name = self.study_path.parts[-1][3:] + ".nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
+
+                # check_shapes(f_path, self.mask_path)
+
                 getT2T2star.TxyFitME(
                     f_path,
                     time_paths[1],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
@@ -983,26 +1203,32 @@
         elif "T2E" in str(self.study_path):
             method = "T2E"
             print(f"\n{hmg.info}Generando mapa de T2E.\n")
             try:
                 f_name = self.study_path.parts[-1][4:] + "_subscan_0.nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
+
+                # check_shapes(f_path, self.mask_path)
+
                 getT2T2star.TxyFitME(
                     f_path,
                     time_paths[2],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
                 )
-            except NameError:
+            except (NameError, FileNotFoundError):
                 f_name = self.study_path.parts[-1][4:] + ".nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
+
+                # check_shapes(f_path, self.mask_path)
+
                 getT2T2star.TxyFitME(
                     f_path,
                     time_paths[2],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
@@ -1011,26 +1237,32 @@
         elif "T1" in str(self.study_path):
             method = "T1"
             print(f"\n{hmg.info}Generando mapa de T1.\n")
             try:
                 f_name = self.study_path.parts[-1][3:] + "_subscan_0.nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii.gz
+
+                # check_shapes(f_path, self.mask_path)
+
                 getT1TR.TxyFitME(
                     f_path,
                     time_paths[0],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
                 )
-            except NameError:
+            except (NameError, FileNotFoundError):
                 f_name = self.study_path.parts[-1][3:] + ".nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
+
+                # check_shapes(f_path, self.mask_path)
+
                 getT1TR.TxyFitME(
                     f_path,
                     time_paths[0],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
@@ -1108,16 +1340,16 @@
 
         return R2_map
 
     def select_threshold(self):
         while True:
             try:
                 th = input(
-                    f"\n{hmg.ask}Introduce el valor que quieres usar como tolerancia (R\u00b2)."
-                    f" Ha de ser un valor entre 0 y 1.\n{hmg.pointer}"
+                    f"\n{hmg.ask}Introduce el valor que quieres usar como tolerancia "
+                    f"(R\u00b2). Ha de ser un valor entre 0 y 1.\n{hmg.pointer}"
                 )
                 th = float(th)
                 if th > 0.99:
                     raise ValueError
                 return th
             except ValueError:
                 print(
@@ -1162,22 +1394,22 @@
                 )
 
     def change_vmin_vmax(self):
         while True:
             try:
                 vmin = float(input("Introduce el valor mínimo.\n"))
                 break
-            except:
+            except Exception:
                 print("No has introducido un número.")
 
         while True:
             try:
                 vmax = float(input("Introduce el valor máximo.\n"))
                 break
-            except:
+            except Exception:
                 print("No has introducido un número.")
 
         return vmin, vmax
 
     def compute_heatmaps(
         self,
         maps: np.array,
@@ -1192,53 +1424,54 @@
         n_slices = np.shape(maps)[0]
         if n_slices % 2 == 0:
             cols = int(np.divide(n_slices, 2))
         else:
             cols = int(np.divide(n_slices, 2) + 0.5)
         fig, ax = plt.subplots(2, cols, figsize=(10, 7))
         ax = ax.flatten()
+        plt.axis("off")
         cbar_ax = fig.add_axes([0.91, 0.3, 0.03, 0.4])
 
         for slc_idx, new_map in enumerate(maps):
             r_map = self.rotate(new_map)
             sns.heatmap(
                 r_map,
                 cmap=cmap,
                 xticklabels=False,
                 yticklabels=False,
                 vmin=vmin,
                 vmax=vmax,
                 cbar_ax=cbar_ax,
                 ax=ax[slc_idx],
             ).invert_xaxis()
-            ax[slc_idx].set_title(f"{map_type} slice {str(slc_idx)}")
+            ax[slc_idx].set_title(f"{map_type} slice {str(slc_idx + 1)}")
 
-            if ind == True:
+            if ind is True:
                 ind_fig = plt.figure(frameon=False, num=slc_idx + fig.number + 1)
                 sns.heatmap(
                     r_map,
                     cmap=cmap,
                     xticklabels=False,
                     yticklabels=False,
                     vmin=vmin,
                     vmax=vmax,
                 ).invert_xaxis()
                 if save == save:
                     ind_fig.savefig(
                         os.path.join(
-                            out_path, map_type + "_slice_" + str(slc_idx + 1) + ".png"
+                            out_path, f"{map_type}_slice_{str(slc_idx + 1)}.png"
                         )
                     )
                     plt.close(ind_fig)
 
         plt.suptitle(f"{map_type} slices")
         fig.tight_layout(rect=[0, 0, 0.9, 1])
 
-        if save == True:
-            fig.savefig(os.path.join(out_path, map_type + "_all_slices.png"))
+        if save is True:
+            fig.savefig(os.path.join(out_path, f"{map_type}_all_slices.png"))
             plt.close()
         else:
             fig.show()
 
     def save_ADC_heatmap(self, f_ADC_maps: np.array, study_path: str):
         """Save ADC heatmap. Opens a window to show the heatmaps per slice
         and allows to change color range and color map.
@@ -1248,67 +1481,72 @@
             Includes filtered ADC directions.
         study_path : Path
             Path to study folder.
         """
         f_ADC_maps[f_ADC_maps == 0.0] = np.nan
 
         cmap = plt.cm.turbo  # select default cmap
-        cmap.set_bad("black", 1)  # paints NaN values in black
+        # cmap.set_bad("black", 1)  # paints NaN values in black
         vmin = 0.1 * np.nanmax(f_ADC_maps) + np.nanmin(f_ADC_maps)
         vmax = 0.9 * np.nanmax(f_ADC_maps)
 
+        self.chosen_cmap = cmap
+        self.chosen_vmin = vmin
+        self.chosen_vmax = vmax
+
         for num_dir, ADC_map_dir in enumerate(f_ADC_maps):
             ADC_map_dir = np.rollaxis(ADC_map_dir, axis=2)
             # offer the possibility to change vmin, vmax and cmap in the adc map
             # of the first direction
             if num_dir == 0:
-                out_path = os.path.join(study_path, "Dir_" + str(num_dir + 1))
+                out_path = os.path.join(study_path, f"Dir_{str(num_dir + 1)}")
 
                 self.compute_heatmaps(
                     ADC_map_dir,
                     "ADC",
                     cmap,
                     vmin,
                     vmax,
                     out_path,
                     ind=False,
                     save=False,
                 )
 
                 print(
-                    f"\n{hmg.ask}Indica cómo quieres guardar los mapas en la ventana emergente."
+                    f"\n{hmg.ask}Indica cómo quieres guardar los mapas en la "
+                    "ventana emergente."
                 )
 
                 # create a frame
                 root = tk.Tk()
                 root.title("MyX")
 
                 # declaring string variable for storing values
-                color_min = IntVar()
-                color_max = IntVar()
-                colormap = StringVar()
+                color_min = tk.IntVar()
+                color_max = tk.IntVar()
+                colormap = tk.StringVar()
 
-                Label(root, text="Mínimo", font=("calibre", 10, "bold")).grid(
+                tk.Label(root, text="Mínimo", font=("calibre", 10, "bold")).grid(
                     row=0, column=0
                 )
-                Label(root, text="Máximo", font=("calibre", 10, "bold")).grid(
+                tk.Label(root, text="Máximo", font=("calibre", 10, "bold")).grid(
                     row=2, column=0
                 )
-                Label(root, text="Color", font=("calibre", 10, "bold")).grid(
+                tk.Label(root, text="Color", font=("calibre", 10, "bold")).grid(
                     row=4, column=0
                 )
 
                 # creating entries for inputs
-                color_min_entry = Entry(
+                color_min_entry = tk.Entry(
                     root, textvariable=color_min, font=("calibre", 10, "normal")
                 )
-                color_max_entry = Entry(
+                color_max_entry = tk.Entry(
                     root, textvariable=color_max, font=("calibre", 10, "normal")
                 )
-                colormap_entry = Entry(
+                colormap_entry = tk.Entry(
                     root, textvariable=colormap, font=("calibre", 10, "normal")
                 )
 
                 color_min_entry.grid(row=1, column=1)
                 color_max_entry.grid(row=3, column=1)
                 colormap_entry.grid(row=5, column=1)
 
@@ -1349,36 +1587,49 @@
                         color_min_val,
                         color_max_val,
                         out_path,
                         ind=True,
                         save=True,
                     )
 
+                    self.chosen_cmap = colormap_val
+                    self.chosen_vmin = color_min_val
+                    self.chosen_vmax = color_max_val
+
                     print(
-                        f"\n{hmg.info}Guardadas las direcciones: {num_dir+1} ", end=""
+                        f"\n{hmg.info}Guardadas las direcciones: {num_dir+1} ",
+                        end="",
+                        flush=True,
                     )
 
                     root.destroy()
                     root.quit()
 
-                Button(root, text="Actualizar", command=get_selection).grid(
+                tk.Button(root, text="Actualizar", command=get_selection).grid(
                     row=6, column=0
                 )
-                Button(root, text="Aceptar", command=close).grid(row=6, column=1)
+                tk.Button(root, text="Aceptar", command=close).grid(row=6, column=1)
 
                 root.mainloop()
 
             else:
-                out_path = study_path / ("Dir_" + str(num_dir + 1))
+                out_path = study_path / f"Dir_{str(num_dir + 1)}"
+
                 self.compute_heatmaps(
-                    ADC_map_dir, "ADC", cmap, vmin, vmax, out_path, ind=True, save=True
+                    ADC_map_dir,
+                    "ADC",
+                    self.chosen_cmap,
+                    self.chosen_vmin,
+                    self.chosen_vmax,
+                    out_path,
+                    ind=True,
+                    save=True,
                 )
-                print(f"{num_dir+1} ", end="")
-                plt.close("all")
-                plt.clf()
+
+                print(num_dir + 1, end=" ", flush=True)
         print()
         return vmin, vmax, cmap
 
     def save_heatmap(
         self,
         maps: np.array,
         map_type: str,
@@ -1422,17 +1673,17 @@
         )
 
         # create a frame
         root = tk.Tk()
         root.title("MyX")
 
         # declaring string variable for storing values
-        color_min = IntVar()
-        color_max = IntVar()
-        colormap = StringVar()
+        color_min = tk.IntVar()
+        color_max = tk.IntVar()
+        colormap = tk.StringVar()
 
         tk.Label(root, text="Mínimo", font=("calibre", 10, "bold")).grid(
             row=0, column=0
         )
         tk.Label(root, text="Máximo", font=("calibre", 10, "bold")).grid(
             row=2, column=0
         )
@@ -1492,11 +1743,11 @@
                 ind=True,
                 save=True,
             )
 
             root.destroy()
             root.quit()
 
-        Button(root, text="Actualizar", command=get_selection).grid(row=6, column=0)
-        Button(root, text="Aceptar", command=close).grid(row=6, column=1)
+        tk.Button(root, text="Actualizar", command=get_selection).grid(row=6, column=0)
+        tk.Button(root, text="Aceptar", command=close).grid(row=6, column=1)
 
         root.mainloop()
```

