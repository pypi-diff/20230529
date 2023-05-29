# Comparing `tmp/neclib-0.8.0.tar.gz` & `tmp/neclib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neclib-0.8.0.tar", max compression
+gzip compressed data, was "neclib-0.9.0.tar", max compression
```

## Comparing `neclib-0.8.0.tar` & `neclib-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1114 2022-07-15 10:09:45.018982 neclib-0.8.0/LICENSE
--rw-r--r--   0        0        0      869 2022-07-15 10:09:45.018982 neclib-0.8.0/README.md
--rw-r--r--   0        0        0      495 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/__init__.py
--rw-r--r--   0        0        0      218 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/controllers/__init__.py
--rw-r--r--   0        0        0    11067 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/controllers/antenna_pid.py
--rw-r--r--   0        0        0      310 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/exceptions.py
--rw-r--r--   0        0        0       79 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/interfaces/__init__.py
--rw-r--r--   0        0        0     4134 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/interfaces/console_logger.py
--rw-r--r--   0        0        0      151 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/parameters/__init__.py
--rw-r--r--   0        0        0     8635 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/parameters/obsparam.py
--rw-r--r--   0        0        0      122 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/parameters/parser/__init__.py
--rw-r--r--   0        0        0     2137 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/parameters/parser/obsparam_data.py
--rw-r--r--   0        0        0     5757 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/parameters/parser/pointing_error_data.py
--rw-r--r--   0        0        0     4573 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/parameters/pointing_error.py
--rw-r--r--   0        0        0      435 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/simulators/__init__.py
--rw-r--r--   0        0        0     6819 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/simulators/antenna.py
--rw-r--r--   0        0        0      575 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/typing.py
--rw-r--r--   0        0        0     1289 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/units.py
--rw-r--r--   0        0        0      152 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/utils/__init__.py
--rw-r--r--   0        0        0     3630 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/utils/data_utils.py
--rw-r--r--   0        0        0     4037 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/utils/math_utils.py
--rw-r--r--   0        0        0     8234 2022-07-15 10:09:45.018982 neclib-0.8.0/neclib/utils/quantity_utils.py
--rw-r--r--   0        0        0     1093 2022-07-15 10:09:45.022980 neclib-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2084 2022-07-15 10:09:55.284712 neclib-0.8.0/setup.py
--rw-r--r--   0        0        0     2014 2022-07-15 10:09:55.285082 neclib-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1114 2022-08-03 06:24:59.136406 neclib-0.9.0/LICENSE
+-rw-r--r--   0        0        0      869 2022-08-03 06:24:59.136406 neclib-0.9.0/README.md
+-rw-r--r--   0        0        0      695 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/__init__.py
+-rw-r--r--   0        0        0      218 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/controllers/__init__.py
+-rw-r--r--   0        0        0    11063 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/controllers/antenna_pid.py
+-rw-r--r--   0        0        0      310 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/exceptions.py
+-rw-r--r--   0        0        0       79 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/interfaces/__init__.py
+-rw-r--r--   0        0        0     4134 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/interfaces/console_logger.py
+-rw-r--r--   0        0        0      151 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/parameters/__init__.py
+-rw-r--r--   0        0        0     8635 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/parameters/obsparam.py
+-rw-r--r--   0        0        0      122 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/parameters/parser/__init__.py
+-rw-r--r--   0        0        0     2137 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/parameters/parser/obsparam_data.py
+-rw-r--r--   0        0        0     5757 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/parameters/parser/pointing_error_data.py
+-rw-r--r--   0        0        0     4573 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/parameters/pointing_error.py
+-rw-r--r--   0        0        0      435 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/simulators/__init__.py
+-rw-r--r--   0        0        0     6815 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/simulators/antenna.py
+-rw-r--r--   0        0        0      369 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/typing.py
+-rw-r--r--   0        0        0     1289 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/units.py
+-rw-r--r--   0        0        0      152 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/utils/__init__.py
+-rw-r--r--   0        0        0     3630 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/utils/data_utils.py
+-rw-r--r--   0        0        0     4016 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/utils/math_utils.py
+-rw-r--r--   0        0        0     8234 2022-08-03 06:24:59.140406 neclib-0.9.0/neclib/utils/quantity_utils.py
+-rw-r--r--   0        0        0      786 2022-08-03 06:24:59.140406 neclib-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1881 2022-08-03 06:25:09.542570 neclib-0.9.0/setup.py
+-rw-r--r--   0        0        0     1700 2022-08-03 06:25:09.542926 neclib-0.9.0/PKG-INFO
```

### Comparing `neclib-0.8.0/LICENSE` & `neclib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/README.md` & `neclib-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/neclib/controllers/antenna_pid.py` & `neclib-0.9.0/neclib/controllers/antenna_pid.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,40 +21,40 @@
     implement.
 
 """
 
 __all__ = ["PIDController"]
 
 import time
-from typing import ClassVar, Dict, Tuple, Union
+from typing import ClassVar, Dict, Literal, Tuple, Union
 
 import astropy.units as u
 import numpy as np
 
 from .. import utils
-from ..typing import AngleUnit, Literal
+from ..typing import AngleUnit
 from ..utils import ParameterList
 
 
 # Indices for parameter lists.
 Last = -2
 Now = -1
 
 
 # Default values for PIDController.
 DefaultK_p = 1.0
 DefaultK_i = 0.5
 DefaultK_d = 0.3
 DefaultMaxSpeed = 2 << u.deg / u.s
-DefaultMaxAcceleration = 2 << u.deg / u.s ** 2
+DefaultMaxAcceleration = 2 << u.deg / u.s**2
 DefaultErrorIntegCount = 50
 DefaultThreshold = {
     "cmd_coord_change": 100 << u.arcsec,
     "accel_limit_off": 20 << u.arcsec,
-    "target_accel_ignore": 2 << u.deg / u.s ** 2,
+    "target_accel_ignore": 2 << u.deg / u.s**2,
 }
 ThresholdKeys = Literal["cmd_coord_change", "accel_limit_off", "target_accel_ignore"]
 
 
 class PIDController:
     """PID controller for telescope antenna.
```

### Comparing `neclib-0.8.0/neclib/interfaces/console_logger.py` & `neclib-0.9.0/neclib/interfaces/console_logger.py`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/neclib/parameters/obsparam.py` & `neclib-0.9.0/neclib/parameters/obsparam.py`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/neclib/parameters/parser/obsparam_data.py` & `neclib-0.9.0/neclib/parameters/parser/obsparam_data.py`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/neclib/parameters/parser/pointing_error_data.py` & `neclib-0.9.0/neclib/parameters/parser/pointing_error_data.py`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/neclib/parameters/pointing_error.py` & `neclib-0.9.0/neclib/parameters/pointing_error.py`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/neclib/simulators/antenna.py` & `neclib-0.9.0/neclib/simulators/antenna.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Emulator for telescope antenna motion and corresponding encoder reading."""
 
 __all__ = ["AntennaEncoderEmulator"]
 
 import time
-from typing import Callable, ClassVar, List, Tuple, Union
+from typing import Callable, ClassVar, List, Literal, Tuple, Union
 
 import astropy.units as u
 import numpy as np
 
 from .. import utils
-from ..typing import AngleUnit, Literal
+from ..typing import AngleUnit
 from ..utils import AzElData, ParameterList
 
 # Indices for parameter lists.
 Last = -2
 Now = -1
 
 DefaultMomentOfInertia = [
@@ -153,19 +153,19 @@
             max(0, abs(_speed.az) - abs(self.cmd_speed.az)),
             max(0, abs(_speed.el) - abs(self.cmd_speed.el)),
         )  # How much over-sped when constant acceleration is assumed.
         accel0_duration = AzElData(
             sped_over.az / abs_accel.az, sped_over.el / abs_accel.el
         )  # How long the acceleration should be set to 0 to sustain command speed.
         next_position = AzElData(
-            accel.az * self.dt ** 2 / 2
+            accel.az * self.dt**2 / 2
             + self.speed.az * self.dt
             + self.position.az
             - sped_over.az * accel0_duration.az / 2,
-            accel.el * self.dt ** 2 / 2
+            accel.el * self.dt**2 / 2
             + self.speed.el * self.dt
             + self.position.el
             - sped_over.el * accel0_duration.el / 2,
         )
 
         self.speed.az = utils.clip(_speed.az, absmax=self.cmd_speed.az)
         self.speed.el = utils.clip(_speed.el, absmax=self.cmd_speed.el)
```

### Comparing `neclib-0.8.0/neclib/units.py` & `neclib-0.9.0/neclib/units.py`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/neclib/utils/data_utils.py` & `neclib-0.9.0/neclib/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/neclib/utils/math_utils.py` & `neclib-0.9.0/neclib/utils/math_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Utility functions for arithmetic operations."""
 
 __all__ = ["clip", "frange", "discretize", "counter"]
 
 import itertools
 import math
-from typing import Generator
-
-from ..typing import Literal
+from typing import Generator, Literal
 
 
 def clip(
     value: float, minimum: float = None, maximum: float = None, *, absmax: float = None
 ) -> float:
     """Limit the ``value`` to the range [``minimum``, ``maximum``].
```

### Comparing `neclib-0.8.0/neclib/utils/quantity_utils.py` & `neclib-0.9.0/neclib/utils/quantity_utils.py`

 * *Files identical despite different names*

### Comparing `neclib-0.8.0/setup.py` & `neclib-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,35 +10,34 @@
  'neclib.simulators',
  'neclib.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['n-const>=1.1.0,<2.0.0', 'numpy>=1.19,<2.0']
+['astropy>=5.0.4,<6.0.0',
+ 'n-const>=1.1.0,<2.0.0',
+ 'numpy>=1.22,<2.0',
+ 'ogameasure>=0.5,<0.6']
 
 extras_require = \
-{':python_version < "3.8"': ['astropy>=3.0,<4.0',
-                             'importlib-metadata>=4.4,<5.0',
-                             'typing-extensions>=3.0,<5.0'],
- ':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.8,<0.9'],
- ':python_version >= "3.8"': ['astropy>=5.0.4,<6.0.0']}
+{':sys_platform == "linux"': ['pyinterface>=1.6,<2.0']}
 
 setup_kwargs = {
     'name': 'neclib',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Pure Python tools for NECST.',
     'long_description': '# neclib\n\n[![PyPI](https://img.shields.io/pypi/v/neclib.svg?label=PyPI&style=flat-square)](https://pypi.org/pypi/neclib/)\n[![Python](https://img.shields.io/pypi/pyversions/neclib.svg?label=Python&color=yellow&style=flat-square)](https://pypi.org/pypi/neclib/)\n[![Test](https://img.shields.io/github/workflow/status/necst-telescope/neclib/Test?logo=github&label=Test&style=flat-square)](https://github.com/necst-telescope/neclib/actions)\n[![License](https://img.shields.io/badge/license-MIT-blue.svg?label=License&style=flat-square)](LICENSE)\n\nPure Python tools for NECST.\n\n## Features\n\nThis library provides:\n\n- Miscellaneous tools for NECST system.\n\n## Installation\n\n```shell\npip install neclib\n```\n\n## Usage\n\nSee the [API reference](https://necst-telescope.github.io/neclib/_source/neclib.html).\n\n---\n\nThis library is using [Semantic Versioning](https://semver.org).\n',
     'author': 'KaoruNishikawa',
     'author_email': 'k.nishikawa@a.phys.nagoya-u.ac.jp',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://necst-telescope.github.io/neclib/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `neclib-0.8.0/PKG-INFO` & `neclib-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: neclib
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pure Python tools for NECST.
 Home-page: https://necst-telescope.github.io/neclib/
 License: MIT
 Author: KaoruNishikawa
 Author-email: k.nishikawa@a.phys.nagoya-u.ac.jp
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: astropy (>=3.0,<4.0); python_version < "3.8"
-Requires-Dist: astropy (>=5.0.4,<6.0.0); python_version >= "3.8"
-Requires-Dist: dataclasses (>=0.8,<0.9); python_version >= "3.6" and python_version < "3.7"
-Requires-Dist: importlib-metadata (>=4.4,<5.0); python_version < "3.8"
+Requires-Dist: astropy (>=5.0.4,<6.0.0)
 Requires-Dist: n-const (>=1.1.0,<2.0.0)
-Requires-Dist: numpy (>=1.19,<2.0)
-Requires-Dist: typing-extensions (>=3.0,<5.0); python_version < "3.8"
+Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: ogameasure (>=0.5,<0.6)
+Requires-Dist: pyinterface (>=1.6,<2.0); sys_platform == "linux"
 Project-URL: Repository, https://github.com/necst-telescope/neclib
 Description-Content-Type: text/markdown
 
 # neclib
 
 [![PyPI](https://img.shields.io/pypi/v/neclib.svg?label=PyPI&style=flat-square)](https://pypi.org/pypi/neclib/)
 [![Python](https://img.shields.io/pypi/pyversions/neclib.svg?label=Python&color=yellow&style=flat-square)](https://pypi.org/pypi/neclib/)
```

