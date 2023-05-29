# Comparing `tmp/tcflow-0.0.8.tar.gz` & `tmp/tcflow-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcflow-0.0.8.tar", last modified: Tue Mar 28 16:05:56 2023, max compression
+gzip compressed data, was "tcflow-0.0.9.tar", last modified: Tue Apr 11 18:54:50 2023, max compression
```

## Comparing `tcflow-0.0.8.tar` & `tcflow-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 16:05:56.926226 tcflow-0.0.8/
--rw-rw-rw-   0        0        0    11558 2023-03-23 11:08:01.000000 tcflow-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     7499 2023-03-28 16:05:56.926226 tcflow-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6959 2023-03-23 11:08:01.000000 tcflow-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-03-28 16:05:56.926226 tcflow-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      950 2023-03-28 16:03:15.000000 tcflow-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-28 16:05:56.926226 tcflow-0.0.8/tcflow/
--rw-rw-rw-   0        0        0     2715 2023-03-27 14:19:06.000000 tcflow-0.0.8/tcflow/EMD_MD_OPs.py
--rw-rw-rw-   0        0        0     3891 2023-03-27 07:06:32.000000 tcflow-0.0.8/tcflow/EMD_reprocess_OPs.py
--rw-rw-rw-   0        0        0     5163 2023-03-28 15:57:53.000000 tcflow-0.0.8/tcflow/EMD_run.py
--rw-rw-rw-   0        0        0        0 2023-03-26 09:14:09.000000 tcflow-0.0.8/tcflow/__init__.py
--rw-rw-rw-   0        0        0     9180 2023-03-28 15:21:17.000000 tcflow-0.0.8/tcflow/input_gen.py
--rw-rw-rw-   0        0        0     8812 2023-03-23 11:08:01.000000 tcflow-0.0.8/tcflow/run_emd.py
--rw-rw-rw-   0        0        0     9501 2023-03-23 11:08:01.000000 tcflow-0.0.8/tcflow/run_nemd.py
-drwxrwxrwx   0        0        0        0 2023-03-28 16:05:56.926226 tcflow-0.0.8/tcflow.egg-info/
--rw-rw-rw-   0        0        0     7499 2023-03-28 16:05:56.000000 tcflow-0.0.8/tcflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-03-28 16:05:56.000000 tcflow-0.0.8/tcflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 16:05:56.000000 tcflow-0.0.8/tcflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-03-28 16:05:56.000000 tcflow-0.0.8/tcflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-28 16:05:56.000000 tcflow-0.0.8/tcflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 18:54:50.708644 tcflow-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-04-04 09:02:41.000000 tcflow-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     7499 2023-04-11 18:54:50.707642 tcflow-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6959 2023-04-04 09:02:41.000000 tcflow-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 18:54:50.708644 tcflow-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-04-11 09:21:24.000000 tcflow-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:54:50.702644 tcflow-0.0.9/tcflow/
+-rw-rw-rw-   0        0        0     2743 2023-04-11 09:17:35.000000 tcflow-0.0.9/tcflow/EMD_MD_OPs.py
+-rw-rw-rw-   0        0        0     3891 2023-04-11 10:12:49.000000 tcflow-0.0.9/tcflow/EMD_reprocess_OPs.py
+-rw-rw-rw-   0        0        0     5142 2023-04-11 10:01:59.000000 tcflow-0.0.9/tcflow/EMD_run.py
+-rw-rw-rw-   0        0        0     1984 2023-04-11 10:08:36.000000 tcflow-0.0.9/tcflow/NEMD_MD_OPs.py
+-rw-rw-rw-   0        0        0     6180 2023-04-11 18:34:20.000000 tcflow-0.0.9/tcflow/NEMD_reprocess_OPs.py
+-rw-rw-rw-   0        0        0     3736 2023-04-11 17:48:41.000000 tcflow-0.0.9/tcflow/NEMD_run.py
+-rw-rw-rw-   0        0        0        0 2023-04-04 09:02:41.000000 tcflow-0.0.9/tcflow/__init__.py
+-rw-rw-rw-   0        0        0     9180 2023-04-04 09:02:41.000000 tcflow-0.0.9/tcflow/input_gen.py
+-rw-rw-rw-   0        0        0     8812 2023-04-04 09:02:41.000000 tcflow-0.0.9/tcflow/run_emd.py
+-rw-rw-rw-   0        0        0     9501 2023-04-04 09:02:41.000000 tcflow-0.0.9/tcflow/run_nemd.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:54:50.707642 tcflow-0.0.9/tcflow.egg-info/
+-rw-rw-rw-   0        0        0     7499 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 18:54:50.000000 tcflow-0.0.9/tcflow.egg-info/top_level.txt
```

### Comparing `tcflow-0.0.8/LICENSE` & `tcflow-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tcflow-0.0.8/PKG-INFO` & `tcflow-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcflow
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework for thermal conductivity calculation based on EMD&NEMD methods
 Home-page: https://github.com/gdbhcxhmjk-z/ThermalConductivity-Workflow.git
 Author: Wenjie Zhang
 Author-email: gdbhcxhmjk@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tcflow-0.0.8/README.md` & `tcflow-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tcflow-0.0.8/setup.py` & `tcflow-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tcflow",
-    version="0.0.8",
+    version="0.0.9",
     author="Wenjie Zhang",
     author_email="gdbhcxhmjk@163.com",
     description="A framework for thermal conductivity calculation based on EMD&NEMD methods",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gdbhcxhmjk-z/ThermalConductivity-Workflow.git",
     packages=setuptools.find_packages(),
```

### Comparing `tcflow-0.0.8/tcflow/EMD_MD_OPs.py` & `tcflow-0.0.9/tcflow/EMD_MD_OPs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import List
 import os,json
 from dflow import SlurmRemoteExecutor, Step, Workflow, argo_range,upload_artifact,download_artifact
 from dflow.python import OP, OPIO, Artifact, OPIOSign, PythonOPTemplate, Slices
 from pathlib import Path
 import dpdata
-
+from . import input_gen
 
 class RunNVT(OP):
     def __init__(self):
         pass
 
     @classmethod
     def get_input_sign(cls):
         return OPIOSign({
             "data":Artifact(Path),
             "input": Artifact(Path),
-            "input_gen":Artifact(Path),
+            #"input_gen":Artifact(Path),
             "force_field":Artifact(List[Path]),
         })
 
     @classmethod
     def get_output_sign(cls):
         return OPIOSign({
             "dump":Artifact(Path),
@@ -56,15 +56,15 @@
 
     @classmethod
     def get_input_sign(cls):
         return OPIOSign({
             "name":str,
             "param":dict,
             "data":Artifact(Path),
-            "input_gen":Artifact(Path),
+            #"input_gen":Artifact(Path),
             "force_field":Artifact(List[Path]),
         })
 
     @classmethod
     def get_output_sign(cls):
         return OPIOSign({
             "dat": Artifact(Path),
@@ -75,18 +75,18 @@
     def execute(
             self,
             op_in: OPIO,
     ) -> OPIO:
         name = op_in["name"]
         param = op_in["param"]
         data = op_in["data"]
-        gen = op_in["input_gen"]
+        #gen = op_in["input_gen"]
         force_field = op_in["force_field"]
-        Path('input_gen.py').symlink_to(gen)
-        import input_gen
+        #Path('input_gen.py').symlink_to(gen)
+        #import input_gen
         name=Path(name)
         name.mkdir()
         cwd = os.getcwd()
         os.chdir(name)
         for field in force_field:
             Path(field.parts[-1]).symlink_to(field)
         Path('data.lammps').symlink_to(data)
```

### Comparing `tcflow-0.0.8/tcflow/EMD_reprocess_OPs.py` & `tcflow-0.0.9/tcflow/EMD_reprocess_OPs.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.0.8/tcflow/EMD_run.py` & `tcflow-0.0.9/tcflow/EMD_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from pathlib import Path
 import dpdata
 import numpy as np
 import time
 from monty.serialization import loadfn
 
 import tcflow,matplotlib,sportran
-from tcflow.EMD_MD_OPs import RunNVT,RunNVE
-from tcflow.EMD_reprocess_OPs import MakeConfigurations,analysis
-from tcflow.input_gen import NVT_input,NVE_input
+from .EMD_MD_OPs import RunNVT,RunNVE
+from .EMD_reprocess_OPs import MakeConfigurations,analysis
+from .input_gen import NVT_input,NVE_input
 
 from dflow.plugins import bohrium
 from dflow.plugins.bohrium import TiefblueClient
 from dflow import config, s3_config
 from dflow.plugins.dispatcher import DispatcherExecutor
 
 machine_param = loadfn("machine.json")
@@ -41,15 +41,15 @@
     # run ../scripts/start-slurm.sh first to start up a slurm cluster
     # from EMD_OPs import RunNVT,RunNVE,MakeConfigurations,analysis
     param = loadfn("parameters.json")
     NVT_input(param)
     NVT_input = upload_artifact("NVT.lammps")
     data_input = upload_artifact(param["structure"])
     force_field = upload_artifact(param["force_field"])
-    gen = upload_artifact("input_gen.py")
+    #gen = upload_artifact("input_gen.py")
     gpu_dispatcher_executor = DispatcherExecutor(
         machine_dict={
             "batch_type": "Bohrium",
             "context_type": "Bohrium",
             "remote_profile": {
                 "email": email,
                 "password": password,
@@ -78,34 +78,34 @@
             },
         },
     )
 
     wf = Workflow("emd-tc")
     NVT = Step("NVT",
                 PythonOPTemplate(RunNVT,image=lammps_image,python_packages=upload_python_packages,),
-                artifacts={"data":data_input,"input":NVT_input,"input_gen":gen,"force_field":force_field},
+                artifacts={"data":data_input,"input":NVT_input,"force_field":force_field},#"input_gen":gen,
                 executor=gpu_dispatcher_executor)
     wf.add(NVT)
     Configurations=Step("Config",
                 PythonOPTemplate(MakeConfigurations,image=tc_image),
                 parameters={"numb_lmp":param['num_configurations']},
                 artifacts={"dump": NVT.outputs.artifacts["dump"]},
                 executor=cpu_dispatcher_executor)
     wf.add(Configurations)
     NVE = Step("NVE",
                  PythonOPTemplate(RunNVE,image=lammps_image,python_packages=upload_python_packages,
                                   slices=Slices("{{item}}",
                                                 #sub_path=True,
                                                 input_parameter=["name"],
                                                 input_artifact=["data"],
-                                                output_artifact=["dat","log"],
+                                                output_artifact=["dat"],
                                                 )
                                   ),
                  parameters={"name":Configurations.outputs.parameters["name"],"param":param,},
-                 artifacts={"data":Configurations.outputs.artifacts["configurations"],"input_gen":gen,"force_field":force_field},
+                 artifacts={"data":Configurations.outputs.artifacts["configurations"],"force_field":force_field},#"input_gen":gen,
                  with_param=argo_range(param['num_configurations']),
                  key="nve-{{item}}",
                  executor=gpu_dispatcher_executor)
     wf.add(NVE)
     thermal_conductivity = Step("cepstral-analysis",
                 PythonOPTemplate(analysis,image=tc_image,),
                 parameters={"param":param},
```

### Comparing `tcflow-0.0.8/tcflow/input_gen.py` & `tcflow-0.0.9/tcflow/input_gen.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.0.8/tcflow/run_emd.py` & `tcflow-0.0.9/tcflow/run_emd.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.0.8/tcflow/run_nemd.py` & `tcflow-0.0.9/tcflow/run_nemd.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.0.8/tcflow.egg-info/PKG-INFO` & `tcflow-0.0.9/tcflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcflow
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework for thermal conductivity calculation based on EMD&NEMD methods
 Home-page: https://github.com/gdbhcxhmjk-z/ThermalConductivity-Workflow.git
 Author: Wenjie Zhang
 Author-email: gdbhcxhmjk@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

