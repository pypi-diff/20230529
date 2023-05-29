# Comparing `tmp/dLuxToliman-0.1.1.tar.gz` & `tmp/dLuxToliman-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dLuxToliman-0.1.1.tar", last modified: Mon May 29 06:22:15 2023, max compression
+gzip compressed data, was "dLuxToliman-0.1.2.tar", last modified: Mon May 29 09:10:40 2023, max compression
```

## Comparing `dLuxToliman-0.1.1.tar` & `dLuxToliman-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-05-29 06:22:15.039843 dLuxToliman-0.1.1/
--rw-r--r--   0 mcha5804   (501) staff       (20)       93 2023-05-29 04:35:46.000000 dLuxToliman-0.1.1/.gitignore
--rw-r--r--   0 mcha5804   (501) staff       (20)     1498 2023-05-29 03:55:35.000000 dLuxToliman-0.1.1/LICENSE
--rw-r--r--   0 mcha5804   (501) staff       (20)     3047 2023-05-29 06:22:15.039706 dLuxToliman-0.1.1/PKG-INFO
--rw-r--r--   0 mcha5804   (501) staff       (20)     2557 2023-05-29 06:18:10.000000 dLuxToliman-0.1.1/README.md
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-05-29 06:22:15.038882 dLuxToliman-0.1.1/dLuxToliman/
--rw-r--r--   0 mcha5804   (501) staff       (20)      516 2023-05-29 06:19:41.000000 dLuxToliman-0.1.1/dLuxToliman/__init__.py
--rw-r--r--   0 mcha5804   (501) staff       (20) 16777344 2023-05-29 04:35:46.000000 dLuxToliman-0.1.1/dLuxToliman/diffractive_pupil.npy
--rw-r--r--   0 mcha5804   (501) staff       (20)     2636 2023-05-29 04:35:46.000000 dLuxToliman-0.1.1/dLuxToliman/gradient_energy.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     1134 2023-05-29 04:35:46.000000 dLuxToliman-0.1.1/dLuxToliman/instruments.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     6731 2023-05-29 04:35:46.000000 dLuxToliman-0.1.1/dLuxToliman/optical_layers.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     8094 2023-05-29 06:12:39.000000 dLuxToliman-0.1.1/dLuxToliman/optics.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     8140 2023-05-29 04:35:46.000000 dLuxToliman-0.1.1/dLuxToliman/sources.py
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-05-29 06:22:15.039513 dLuxToliman-0.1.1/dLuxToliman.egg-info/
--rw-r--r--   0 mcha5804   (501) staff       (20)     3047 2023-05-29 06:22:14.000000 dLuxToliman-0.1.1/dLuxToliman.egg-info/PKG-INFO
--rw-r--r--   0 mcha5804   (501) staff       (20)      434 2023-05-29 06:22:15.000000 dLuxToliman-0.1.1/dLuxToliman.egg-info/SOURCES.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)        1 2023-05-29 06:22:14.000000 dLuxToliman-0.1.1/dLuxToliman.egg-info/dependency_links.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)       11 2023-05-29 06:22:14.000000 dLuxToliman-0.1.1/dLuxToliman.egg-info/requires.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)       12 2023-05-29 06:22:14.000000 dLuxToliman-0.1.1/dLuxToliman.egg-info/top_level.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)      361 2023-05-29 06:21:39.000000 dLuxToliman-0.1.1/pyproject.toml
--rw-r--r--   0 mcha5804   (501) staff       (20)       11 2023-05-29 04:35:46.000000 dLuxToliman-0.1.1/requirements.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)       38 2023-05-29 06:22:15.039905 dLuxToliman-0.1.1/setup.cfg
--rw-r--r--   0 mcha5804   (501) staff       (20)     1472 2023-05-29 04:35:46.000000 dLuxToliman-0.1.1/setup.py
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-05-29 09:10:40.348376 dLuxToliman-0.1.2/
+-rw-r--r--   0 mcha5804   (501) staff       (20)       93 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/.gitignore
+-rw-r--r--   0 mcha5804   (501) staff       (20)     1498 2023-05-29 03:55:35.000000 dLuxToliman-0.1.2/LICENSE
+-rw-r--r--   0 mcha5804   (501) staff       (20)     3110 2023-05-29 09:10:40.348238 dLuxToliman-0.1.2/PKG-INFO
+-rw-r--r--   0 mcha5804   (501) staff       (20)     2620 2023-05-29 08:56:27.000000 dLuxToliman-0.1.2/README.md
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-05-29 09:10:40.347185 dLuxToliman-0.1.2/dLuxToliman/
+-rw-r--r--   0 mcha5804   (501) staff       (20)      516 2023-05-29 09:03:03.000000 dLuxToliman-0.1.2/dLuxToliman/__init__.py
+-rw-r--r--   0 mcha5804   (501) staff       (20) 16777344 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/diffractive_pupil.npy
+-rw-r--r--   0 mcha5804   (501) staff       (20)     2636 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/gradient_energy.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     1134 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/instruments.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     6731 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/optical_layers.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     8094 2023-05-29 06:12:39.000000 dLuxToliman-0.1.2/dLuxToliman/optics.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     8140 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/sources.py
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-05-29 09:10:40.348066 dLuxToliman-0.1.2/dLuxToliman.egg-info/
+-rw-r--r--   0 mcha5804   (501) staff       (20)     3110 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/PKG-INFO
+-rw-r--r--   0 mcha5804   (501) staff       (20)      434 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/SOURCES.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)        1 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/dependency_links.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)       11 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/requires.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)       12 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/top_level.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)      361 2023-05-29 09:03:03.000000 dLuxToliman-0.1.2/pyproject.toml
+-rw-r--r--   0 mcha5804   (501) staff       (20)       11 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/requirements.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)       38 2023-05-29 09:10:40.348438 dLuxToliman-0.1.2/setup.cfg
+-rw-r--r--   0 mcha5804   (501) staff       (20)     1472 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/setup.py
```

### Comparing `dLuxToliman-0.1.1/LICENSE` & `dLuxToliman-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.1/PKG-INFO` & `dLuxToliman-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 Metadata-Version: 2.1
 Name: dLuxToliman
-Version: 0.1.1
+Version: 0.1.2
 Summary: A repo to hold the canonical dLux Toliman models.
 Home-page: https://github.com/maxecharles/dLuxToliman
 Author: Max Charles
 Author-email: max.charles@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/maxecharles/dLuxToliman/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dLuxToliman
 
+[![PyPI version](https://badge.fury.io/py/dLuxToliman.svg)](https://badge.fury.io/py/dLuxToliman)
 [![License](https://img.shields.io/badge/license-BSD%203--Clause-blue.svg)](LICENSE)
 
 ## Description
 
 [∂Lux](https://louisdesdoigts.github.io/dLux/) is an open-source differentiable optical modelling framework harnessing the structural isomorphism between optical systems and neural networks, giving forwards models of optical system as a _parametric neural network_.
+∂Lux is built in [Zodiax](https://github.com/LouisDesdoigts/zodiax) which is an open-source object-oriented [Jax](https://github.com/google/jax) framework built as an extension of [Equinox](https://github.com/patrick-kidger/equinox) for scientific programming.
 
-∂Lux is built in [Zodiax](https://github.com/LouisDesdoigts/zodiax) which is an open-source object-oriented [Jax](https://github.com/google/jax) framework built as an extension of [Equinox](https://github.com/patrick-kidger/equinox) for scientific programming. This framework allows for the creation of complex optical systems involving many planes, phase and amplitude screens in each, and propagate between them in the Fraunhofer or Fresnel regimes. This enables [fast phase retrieval](https://louisdesdoigts.github.io/dLux/notebooks/phase_retrieval_demo/), image deconvolution, and [hardware design in high dimensions](https://louisdesdoigts.github.io/dLux/notebooks/designing_a_mask/). Because ∂Lux models are fully differentiable, you can [optimize them by gradient descent over millions of parameters](https://louisdesdoigts.github.io/dLux/notebooks/flatfield_calibration/); or use [Hamiltonian Monte Carlo to accelerate MCMC sampling](https://louisdesdoigts.github.io/dLux/notebooks/HMC/). Our code is fully open-source under an MIT license, and we encourage you to use it and build on it to solve problems in astronomy and beyond.
+The primary goal of the Toliman mission is to discover Earth-sized exoplanets orbiting in Alpha Centauri, the closest star system to our own.
+To achieve this, the mission will employ a novel telescope design that will be able to detect subtle changes in the positions of the Alpha Centauri binary pair.
+These changes are caused by the gravitational reflex motion induced by an Earth-sized companion, and this cutting-edge technology will enable scientists to identify exoplanets too small to be detected by conventional telescopes.
+Toliman utilises a binary phase diffraction pupil to grasp the expected microarcsecond-scale astrometric signal.
 
-
-## Features
-
-This package contains pre-built optical simulation models for the Toliman instrument.
+**This repository/package contains pre-built ∂Lux models of the Toliman optical system**, and pre-built parametrised ∂Lux source objects for Alpha Centauri.
 
 ## Installation
 
 `dLuxToliman` is pip-installable. To install the latest release, simply run:
 
 ```bash
 pip install dLuxToliman
 ```
 
-## Usage  # TODO: Update this section for dLux 13.0
-
-Explain how users can import and use your package in their projects. Provide code examples or snippets if possible.
-
-## Contributing
+## Usage
 
-Let users know how they can contribute to your package, report issues, or submit pull requests.
+A very basic example of how to use this package is as follows:
 
-## Limitations
+```python
+# imports
+import dLuxToliman as dlT
+from matplotlib import pyplot as plt
+
+osys = dlT.TolimanOptics(psf_npixels=128, psf_oversample=1)  # creating Toliman optical system
+source = dlT.AlphaCen(nwavels=3, separation=8, position_angle=30)  # creating Alpha Centauri source
+psf = osys.model(source)  # running optical simulation
+
+# plotting
+plt.imshow(psf**.5, cmap = 'inferno')
+plt.title('Toliman $\sqrt{PSF}$')
+plt.show()
+```
 
-Outline any known limitations or caveats that users should be aware of when using your package.
+The above code generates the PSF for the Toliman optical system, with the Alpha Centauri source, and plots the PSF on a square root stretch.
 
 ## License
 
 This package is released under the BSD 3-Clause License. See the [LICENSE](LICENSE) file for more information.
 
-## Documentation  # TODO add
-
-If you have additional documentation or resources, provide links or instructions for accessing them.
-
 ## Support
 
-If you encounter any problems or have any questions related to Toliman models, please contact me at `max.charles@sydney.edu.au`.
+If you encounter any problems or have any questions related to Toliman models, please raise an issue or contact me at `max.charles@sydney.edu.au`.
```

### Comparing `dLuxToliman-0.1.1/dLuxToliman/__init__.py` & `dLuxToliman-0.1.2/dLuxToliman/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name = "dLuxToliman"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 
 # Import as modules
 from . import optics
 from . import optical_layers
 from . import gradient_energy
 from . import instruments
```

### Comparing `dLuxToliman-0.1.1/dLuxToliman/diffractive_pupil.npy` & `dLuxToliman-0.1.2/dLuxToliman/diffractive_pupil.npy`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.1/dLuxToliman/gradient_energy.py` & `dLuxToliman-0.1.2/dLuxToliman/gradient_energy.py`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.1/dLuxToliman/instruments.py` & `dLuxToliman-0.1.2/dLuxToliman/instruments.py`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.1/dLuxToliman/optical_layers.py` & `dLuxToliman-0.1.2/dLuxToliman/optical_layers.py`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.1/dLuxToliman/optics.py` & `dLuxToliman-0.1.2/dLuxToliman/optics.py`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.1/dLuxToliman/sources.py` & `dLuxToliman-0.1.2/dLuxToliman/sources.py`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.1/dLuxToliman.egg-info/PKG-INFO` & `dLuxToliman-0.1.2/dLuxToliman.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 Metadata-Version: 2.1
 Name: dLuxToliman
-Version: 0.1.1
+Version: 0.1.2
 Summary: A repo to hold the canonical dLux Toliman models.
 Home-page: https://github.com/maxecharles/dLuxToliman
 Author: Max Charles
 Author-email: max.charles@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/maxecharles/dLuxToliman/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dLuxToliman
 
+[![PyPI version](https://badge.fury.io/py/dLuxToliman.svg)](https://badge.fury.io/py/dLuxToliman)
 [![License](https://img.shields.io/badge/license-BSD%203--Clause-blue.svg)](LICENSE)
 
 ## Description
 
 [∂Lux](https://louisdesdoigts.github.io/dLux/) is an open-source differentiable optical modelling framework harnessing the structural isomorphism between optical systems and neural networks, giving forwards models of optical system as a _parametric neural network_.
+∂Lux is built in [Zodiax](https://github.com/LouisDesdoigts/zodiax) which is an open-source object-oriented [Jax](https://github.com/google/jax) framework built as an extension of [Equinox](https://github.com/patrick-kidger/equinox) for scientific programming.
 
-∂Lux is built in [Zodiax](https://github.com/LouisDesdoigts/zodiax) which is an open-source object-oriented [Jax](https://github.com/google/jax) framework built as an extension of [Equinox](https://github.com/patrick-kidger/equinox) for scientific programming. This framework allows for the creation of complex optical systems involving many planes, phase and amplitude screens in each, and propagate between them in the Fraunhofer or Fresnel regimes. This enables [fast phase retrieval](https://louisdesdoigts.github.io/dLux/notebooks/phase_retrieval_demo/), image deconvolution, and [hardware design in high dimensions](https://louisdesdoigts.github.io/dLux/notebooks/designing_a_mask/). Because ∂Lux models are fully differentiable, you can [optimize them by gradient descent over millions of parameters](https://louisdesdoigts.github.io/dLux/notebooks/flatfield_calibration/); or use [Hamiltonian Monte Carlo to accelerate MCMC sampling](https://louisdesdoigts.github.io/dLux/notebooks/HMC/). Our code is fully open-source under an MIT license, and we encourage you to use it and build on it to solve problems in astronomy and beyond.
+The primary goal of the Toliman mission is to discover Earth-sized exoplanets orbiting in Alpha Centauri, the closest star system to our own.
+To achieve this, the mission will employ a novel telescope design that will be able to detect subtle changes in the positions of the Alpha Centauri binary pair.
+These changes are caused by the gravitational reflex motion induced by an Earth-sized companion, and this cutting-edge technology will enable scientists to identify exoplanets too small to be detected by conventional telescopes.
+Toliman utilises a binary phase diffraction pupil to grasp the expected microarcsecond-scale astrometric signal.
 
-
-## Features
-
-This package contains pre-built optical simulation models for the Toliman instrument.
+**This repository/package contains pre-built ∂Lux models of the Toliman optical system**, and pre-built parametrised ∂Lux source objects for Alpha Centauri.
 
 ## Installation
 
 `dLuxToliman` is pip-installable. To install the latest release, simply run:
 
 ```bash
 pip install dLuxToliman
 ```
 
-## Usage  # TODO: Update this section for dLux 13.0
-
-Explain how users can import and use your package in their projects. Provide code examples or snippets if possible.
-
-## Contributing
+## Usage
 
-Let users know how they can contribute to your package, report issues, or submit pull requests.
+A very basic example of how to use this package is as follows:
 
-## Limitations
+```python
+# imports
+import dLuxToliman as dlT
+from matplotlib import pyplot as plt
+
+osys = dlT.TolimanOptics(psf_npixels=128, psf_oversample=1)  # creating Toliman optical system
+source = dlT.AlphaCen(nwavels=3, separation=8, position_angle=30)  # creating Alpha Centauri source
+psf = osys.model(source)  # running optical simulation
+
+# plotting
+plt.imshow(psf**.5, cmap = 'inferno')
+plt.title('Toliman $\sqrt{PSF}$')
+plt.show()
+```
 
-Outline any known limitations or caveats that users should be aware of when using your package.
+The above code generates the PSF for the Toliman optical system, with the Alpha Centauri source, and plots the PSF on a square root stretch.
 
 ## License
 
 This package is released under the BSD 3-Clause License. See the [LICENSE](LICENSE) file for more information.
 
-## Documentation  # TODO add
-
-If you have additional documentation or resources, provide links or instructions for accessing them.
-
 ## Support
 
-If you encounter any problems or have any questions related to Toliman models, please contact me at `max.charles@sydney.edu.au`.
+If you encounter any problems or have any questions related to Toliman models, please raise an issue or contact me at `max.charles@sydney.edu.au`.
```

### Comparing `dLuxToliman-0.1.1/setup.py` & `dLuxToliman-0.1.2/setup.py`

 * *Files identical despite different names*

