# Comparing `tmp/mlqd-1.0.0.tar.gz` & `tmp/mlqd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlqd-1.0.0.tar", last modified: Mon Mar 27 10:56:53 2023, max compression
+gzip compressed data, was "mlqd-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mlqd-1.0.0.tar` & `mlqd-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0    33535 2023-03-27 10:48:36.756128 mlqd-1.0.0/README.md
--rwxr-xr-x   0        0        0        0 2023-03-27 09:23:43.026281 mlqd-1.0.0/mlqd/__init__.py
--rwxr-xr-x   0        0        0     6829 2023-03-27 09:36:42.901032 mlqd-1.0.0/mlqd/cnn.py
--rwxr-xr-x   0        0        0    11602 2023-03-27 07:44:58.340394 mlqd-1.0.0/mlqd/createQD.py
--rwxr-xr-x   0        0        0     1113 2023-03-27 07:44:58.341644 mlqd-1.0.0/mlqd/data.py
--rwxr-xr-x   0        0        0     2248 2023-03-27 07:44:58.342052 mlqd-1.0.0/mlqd/essential_param.py
--rwxr-xr-x   0        0        0    24925 2023-03-27 09:37:07.249636 mlqd-1.0.0/mlqd/evolution.py
--rwxr-xr-x   0        0        0     9642 2023-03-27 07:44:58.342676 mlqd-1.0.0/mlqd/hp.py
--rwxr-xr-x   0        0        0     4179 2023-03-27 09:35:21.594686 mlqd-1.0.0/mlqd/hyperopt_optim.py
--rwxr-xr-x   0        0        0     1967 2023-03-27 07:44:58.343157 mlqd-1.0.0/mlqd/lic.py
--rwxr-xr-x   0        0        0     6676 2023-03-27 07:44:58.343485 mlqd-1.0.0/mlqd/ml_dyn.py
--rwxr-xr-x   0        0        0     4215 2023-03-27 07:44:58.343711 mlqd-1.0.0/mlqd/plot.py
--rwxr-xr-x   0        0        0    12554 2023-03-27 07:44:58.343963 mlqd-1.0.0/mlqd/prep_input.py
--rwxr-xr-x   0        0        0     8718 2023-03-27 09:33:26.634449 mlqd-1.0.0/mlqd/train_ml.py
--rwxr-xr-x   0        0        0     4053 2023-03-27 07:44:58.344420 mlqd-1.0.0/mlqd/useQD.py
--rwxr-xr-x   0        0        0      592 2023-03-27 10:51:28.141079 mlqd-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    34039 1970-01-01 00:00:00.000000 mlqd-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    33512 2023-05-20 08:42:59.727409 mlqd-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/__init__.py
+-rw-r--r--   0        0        0     6829 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/cnn.py
+-rw-r--r--   0        0        0    11602 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/createQD.py
+-rw-r--r--   0        0        0     1113 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/data.py
+-rw-r--r--   0        0        0     2248 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/essential_param.py
+-rw-r--r--   0        0        0    24925 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/evolution.py
+-rw-r--r--   0        0        0     9642 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/hp.py
+-rw-r--r--   0        0        0     4179 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/hyperopt_optim.py
+-rw-r--r--   0        0        0     1889 2023-05-29 05:25:50.692535 mlqd-1.1.1/mlqd/lic.py
+-rw-r--r--   0        0        0     6676 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/ml_dyn.py
+-rw-r--r--   0        0        0     4215 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/plot.py
+-rw-r--r--   0        0        0    12554 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/prep_input.py
+-rw-r--r--   0        0        0     8718 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/train_ml.py
+-rw-r--r--   0        0        0     4053 2023-05-11 06:25:02.000000 mlqd-1.1.1/mlqd/useQD.py
+-rw-r--r--   0        0        0      731 2023-05-29 04:48:44.350837 mlqd-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    34176 1970-01-01 00:00:00.000000 mlqd-1.1.1/PKG-INFO
```

### Comparing `mlqd-1.0.0/README.md` & `mlqd-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,40 +5,38 @@
 
 * **Kernel Ridge Regression (KRR)-based recursive (iterative) Quantum Dissipative Dynamics method:** Here is the corresponding article $\boldsymbol{\rightarrow}$ [Speeding up quantum dissipative dynamics of open systems with kernel methods](https://iopscience.iop.org/article/10.1088/1367-2630/ac3261 "Named link title"). Recently, we have performed a comparative study where KKR method outperforms NN models, here is the article $\boldsymbol{\rightarrow}$ [A comparative study of different machine learning methods for dissipative quantum dynamics](https://dx.doi.org/10.1088/2632-2153/ac9a9d "Named link title")
 * **AIQD non-recursive  (non-iterative) approach:** Here is the corresponding article $\boldsymbol{\rightarrow}$ [Predicting the future of excitation energy transfer in light-harvesting complex with artificial intelligence-based quantum dynamics](https://doi.org/10.1038/s41467-022-29621-w "Named link title") 
 * **The blazingly fast OSTL non-recursive (non-iterative) approach:** Here is the corresponding article $\boldsymbol{\rightarrow}$ [One-Shot Trajectory Learning of Open Quantum Systems Dynamics]( https://doi.org/10.1021/acs.jpclett.2c01242 "Named link title")
 
 *We have also released a database with quantum dissipative dynamics datasets https://doi.org/10.48550/arXiv.2301.12096, you can use it to train your own model*
 
+For hands-on-paractice
 **MLQD provides**
 
 * Propagation of dynamics with the existing trained models [[Click here](#propagation)]
 * Training convolutional neural networks (CNN) and KRR models on the data [[Click here](#training)]
 * Transformation of data into input files X and Y [[Click here](#preparation)] and direct training with out transformation [[Click here](#nopreparation)]
 * Optimization of the hyperparameters in CNN and KRR models [[Click here](#preparation)]
 * Auto-plotting
 
 **You can also Run MLQD on the XACS cloud computing platform (https://xacs.xmu.edu.cn/) and the user manual is here (http://mlatom.com/manual/#mlqd)**
 
 ### Installation and dependencies
 
-Download the GitHub repository and go to Jupyter Notebooks folder to run the notebooks. 
-Do not change the name of the MLQD folder as the system will look for the MLQD folder. 
-
 *Some dependencies:* 
 
 Create a conda environment 
 
 ```conda create --name mlqd```
 
 Activate the environment
 
 ```conda activate mlqd```
 
-Install the following required dependencies
+While installing MLQD, it will also install the following required dependencies
 
 * tensorflow  ```conda install -c conda-forge tensorflow```
 
 * scikit-learn ```conda install -c anaconda scikit-learn```
 
 * hyperopt ```conda install -c conda-forge hyperopt```
 
@@ -50,14 +48,18 @@
 
 MLQD provides User-Manual and to get to that, we need to import ```quant_dyn``` class from ```evolution.py``` [in MLQD folder]
 
 ``` from mlqd.evolution import quant_dyn ```
 
 and then call ```quant_dyn``` with out passing any parameters, i.e.,  ``` quant_dyn()``` 
 
+
+For hands-on-paractice, we provide Jupyter Notebooks at https://github.com/Arif-PhyChem/MLQD
+
+
 ## Dynamics Propagation <a name="propagation"></a> [[Go to Top](#Top)]
 (***Go to Jupyter_Notebooks folder for ready made scripts***)
 We provide already trained QD models which can be found here [coming soon], you can download them and test the code. If you want to train your own model, then go to [Training on your own data](#training) section. First of all, we need to import ```quant_dyn``` class from ```evolution.py``` .
 
 ``` from evolution import quant_dyn ```
 
 * **KRR model:**
```

### Comparing `mlqd-1.0.0/mlqd/cnn.py` & `mlqd-1.1.1/mlqd/cnn.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/createQD.py` & `mlqd-1.1.1/mlqd/createQD.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/data.py` & `mlqd-1.1.1/mlqd/data.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/essential_param.py` & `mlqd-1.1.1/mlqd/essential_param.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/evolution.py` & `mlqd-1.1.1/mlqd/evolution.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/hp.py` & `mlqd-1.1.1/mlqd/hp.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/hyperopt_optim.py` & `mlqd-1.1.1/mlqd/hyperopt_optim.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/lic.py` & `mlqd-1.1.1/mlqd/lic.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 """%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
 
                 Statement
 
   %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 """
 
-__intro__= "MLQD is a python package developed for Machine Learning-based Quantum Dissipative Dynamics,\n \t\t\t\t  Version 1.0.0\n\t\t\t https://github.com/Arif-PhyChem/MLQD" 
-__author__ = "\n \t\t\t Copyright (c) 2022 Arif Ullah"
-__copyright__ = "\nAll rights reserved. This work is licensed under the Attribution-NonCommercial-NoDerivatives 4.0\n \t International http://creativecommons.org/licenses/by-nc-nd/4.0/) license.\n\t\t\t See LICENSE.CC-BY-NC-ND-4.0"
+__intro__= "MLQD is a python package developed for Machine Learning-based Quantum Dissipative Dynamics,\n \t\t\t\t  Version 1.1.1\n\t\t\t https://github.com/Arif-PhyChem/MLQD" 
+__author__ = "\n \t\t\t Copyright (c) 2023 Arif Ullah"
+__copyright__ = "\nAll rights reserved. This work is licensed under the Apache Software License 2.0"
 __mod__= "\n\nThe above copyright notice and this permission notice shall be included \nin all copies or substantial portions of the Software."
 __disclaimer__="\n\nThe software is provided \"as is\" without warranty of any kind, express or implied, \nincluding but not limited to the warranties ofmerchantability, fitness for a particular \npurpose and noninfringement. In no event shall the authors or copyright holders be \nliable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, \narising from, out of or in connection with the software or the use or other dealings in the software."
-__cite__="\n\n\t\t\t\t Cite as:\n\n1) Ullah A. and Dral P. O., New Journal of Physics, 2021, 23(11), 113019\n2) Ullah A. and Dral P. O., Nature Communications, 2022, 13(1), 1930\n3) Ullah A. and Dral P. O., Journal of Physical Chemistry Letters, 2022, 13(26), 6037\n4) Rodriguez L. E. H.; Ullah A.; Espinosa K. J. R.; Dral P. O. and A. A. Kananenka, Machine Learning: Science and Technology, 2022, 3(4), 045016"
+__cite__="\n\n\t\t\t\t Cite as:\n\n1) Ullah A. and Dral P. O., New Journal of Physics, 2021, 23(11), 113019\n2) Ullah A. and Dral P. O., Nature Communications, 2022, 13(1), 1930\n3) Ullah A. and Dral P. O., Journal of Physical Chemistry Letters, 2022, 13(26), 6037\n4) Rodriguez L. E. H.; Ullah A.; Espinosa K. J. R.; Dral P. O. and A. A. Kananenka, Machine Learning: Science and Technology, 2022, 3(4), 045016\n5), Ullah A. and Dral P. O., 2023, arXiv.2303.01264"
 __contributers__="\nContributers List:\n\n1) Arif Ullah (main) \n2) Pavlo O. Dral"
 def statement():
     print('=================================================================')
     print(__intro__)
     print(__author__)
     print(__copyright__)
     print(__mod__)
```

### Comparing `mlqd-1.0.0/mlqd/ml_dyn.py` & `mlqd-1.1.1/mlqd/ml_dyn.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/plot.py` & `mlqd-1.1.1/mlqd/plot.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/prep_input.py` & `mlqd-1.1.1/mlqd/prep_input.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/train_ml.py` & `mlqd-1.1.1/mlqd/train_ml.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/mlqd/useQD.py` & `mlqd-1.1.1/mlqd/useQD.py`

 * *Files identical despite different names*

### Comparing `mlqd-1.0.0/PKG-INFO` & `mlqd-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 Metadata-Version: 2.1
 Name: mlqd
-Version: 1.0.0
+Version: 1.1.1
 Summary: MLQD: A Python Package for Machine Learning-based Quantum Dissipative Dynamics
-Author-email: Arif Ullah <ua2024@xmu.edu.cn>
+Author-email: Arif Ullah <arif@ahu.edu.cn>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Requires-Dist: tensorflow>=2.12.0
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: hyperopt>=0.2.7
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: mlatom==2.3.3
 Project-URL: Documentation, https://github.com/Arif-PhyChem/MLQD
 Project-URL: Source, https://github.com/Arif-PhyChem/MLQD
 
 # MLQD- A Python package for Machine Learning-based Quantum Dissipative Dynamics <a name="Top"></a>
 In MLQD, we provide three Machine Learning (ML) methods for propagating Qauntum Dissipative Dynamics **[For Licence statement, please [[Click here](#licence)]]**
 
 **The corresponding preprint is on arXiv http://arxiv.org/abs/2303.01264**
 
 * **Kernel Ridge Regression (KRR)-based recursive (iterative) Quantum Dissipative Dynamics method:** Here is the corresponding article $\boldsymbol{\rightarrow}$ [Speeding up quantum dissipative dynamics of open systems with kernel methods](https://iopscience.iop.org/article/10.1088/1367-2630/ac3261 "Named link title"). Recently, we have performed a comparative study where KKR method outperforms NN models, here is the article $\boldsymbol{\rightarrow}$ [A comparative study of different machine learning methods for dissipative quantum dynamics](https://dx.doi.org/10.1088/2632-2153/ac9a9d "Named link title")
 * **AIQD non-recursive  (non-iterative) approach:** Here is the corresponding article $\boldsymbol{\rightarrow}$ [Predicting the future of excitation energy transfer in light-harvesting complex with artificial intelligence-based quantum dynamics](https://doi.org/10.1038/s41467-022-29621-w "Named link title") 
 * **The blazingly fast OSTL non-recursive (non-iterative) approach:** Here is the corresponding article $\boldsymbol{\rightarrow}$ [One-Shot Trajectory Learning of Open Quantum Systems Dynamics]( https://doi.org/10.1021/acs.jpclett.2c01242 "Named link title")
 
 *We have also released a database with quantum dissipative dynamics datasets https://doi.org/10.48550/arXiv.2301.12096, you can use it to train your own model*
 
+For hands-on-paractice
 **MLQD provides**
 
 * Propagation of dynamics with the existing trained models [[Click here](#propagation)]
 * Training convolutional neural networks (CNN) and KRR models on the data [[Click here](#training)]
 * Transformation of data into input files X and Y [[Click here](#preparation)] and direct training with out transformation [[Click here](#nopreparation)]
 * Optimization of the hyperparameters in CNN and KRR models [[Click here](#preparation)]
 * Auto-plotting
 
 **You can also Run MLQD on the XACS cloud computing platform (https://xacs.xmu.edu.cn/) and the user manual is here (http://mlatom.com/manual/#mlqd)**
 
 ### Installation and dependencies
 
-Download the GitHub repository and go to Jupyter Notebooks folder to run the notebooks. 
-Do not change the name of the MLQD folder as the system will look for the MLQD folder. 
-
 *Some dependencies:* 
 
 Create a conda environment 
 
 ```conda create --name mlqd```
 
 Activate the environment
 
 ```conda activate mlqd```
 
-Install the following required dependencies
+While installing MLQD, it will also install the following required dependencies
 
 * tensorflow  ```conda install -c conda-forge tensorflow```
 
 * scikit-learn ```conda install -c anaconda scikit-learn```
 
 * hyperopt ```conda install -c conda-forge hyperopt```
 
@@ -62,14 +65,18 @@
 
 MLQD provides User-Manual and to get to that, we need to import ```quant_dyn``` class from ```evolution.py``` [in MLQD folder]
 
 ``` from mlqd.evolution import quant_dyn ```
 
 and then call ```quant_dyn``` with out passing any parameters, i.e.,  ``` quant_dyn()``` 
 
+
+For hands-on-paractice, we provide Jupyter Notebooks at https://github.com/Arif-PhyChem/MLQD
+
+
 ## Dynamics Propagation <a name="propagation"></a> [[Go to Top](#Top)]
 (***Go to Jupyter_Notebooks folder for ready made scripts***)
 We provide already trained QD models which can be found here [coming soon], you can download them and test the code. If you want to train your own model, then go to [Training on your own data](#training) section. First of all, we need to import ```quant_dyn``` class from ```evolution.py``` .
 
 ``` from evolution import quant_dyn ```
 
 * **KRR model:**
```

