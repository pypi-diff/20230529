# Comparing `tmp/pyathena-3.0.2.tar.gz` & `tmp/pyathena-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyathena-3.0.2.tar", max compression
+gzip compressed data, was "pyathena-3.0.3.tar", max compression
```

## Comparing `pyathena-3.0.2.tar` & `pyathena-3.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1055 2023-05-17 14:43:32.683209 pyathena-3.0.2/LICENSE
--rw-r--r--   0        0        0    70055 2023-05-17 14:43:32.683209 pyathena-3.0.2/README.rst
--rw-r--r--   0        0        0     1923 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/__init__.py
--rw-r--r--   0        0        0       24 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     5157 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2554 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     7250 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9755 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2421 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/util.py
--rw-r--r--   0        0        0     5373 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/async_cursor.py
--rw-r--r--   0        0        0    21170 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/common.py
--rw-r--r--   0        0        0    10416 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/connection.py
--rw-r--r--   0        0        0     4209 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/converter.py
--rw-r--r--   0        0        0     5835 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/cursor.py
--rw-r--r--   0        0        0      660 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/error.py
--rw-r--r--   0        0        0       24 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2439 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    20474 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0     1216 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0     6571 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/formatter.py
--rw-r--r--   0        0        0    17085 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/model.py
--rw-r--r--   0        0        0      220 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5829 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1830 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     8327 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13589 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0     9822 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/util.py
--rw-r--r--   0        0        0        0 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/py.typed
--rw-r--r--   0        0        0    25104 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/result_set.py
--rw-r--r--   0        0        0       24 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      661 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    36892 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      884 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2638 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1210 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0     1948 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/util.py
--rw-r--r--   0        0        0     3482 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyproject.toml
--rw-r--r--   0        0        0    71494 1970-01-01 00:00:00.000000 pyathena-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-05-29 14:36:52.101374 pyathena-3.0.3/LICENSE
+-rw-r--r--   0        0        0    70055 2023-05-29 14:36:52.101374 pyathena-3.0.3/README.rst
+-rw-r--r--   0        0        0     1959 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     5193 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2590 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     7250 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9791 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2457 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/util.py
+-rw-r--r--   0        0        0     5409 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    21206 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/common.py
+-rw-r--r--   0        0        0    10452 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/connection.py
+-rw-r--r--   0        0        0     4245 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/converter.py
+-rw-r--r--   0        0        0     5835 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/cursor.py
+-rw-r--r--   0        0        0      660 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/error.py
+-rw-r--r--   0        0        0       24 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2475 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    20510 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0     1252 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0     6571 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/formatter.py
+-rw-r--r--   0        0        0    17121 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/model.py
+-rw-r--r--   0        0        0      220 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5865 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1866 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     8327 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13625 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0     9858 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/util.py
+-rw-r--r--   0        0        0        0 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/py.typed
+-rw-r--r--   0        0        0    25140 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/result_set.py
+-rw-r--r--   0        0        0       24 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      661 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    36928 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      884 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2638 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1246 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0     1984 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/util.py
+-rw-r--r--   0        0        0     3482 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0    71294 1970-01-01 00:00:00.000000 pyathena-3.0.3/PKG-INFO
```

### Comparing `pyathena-3.0.2/LICENSE` & `pyathena-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/README.rst` & `pyathena-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/pyathena/__init__.py` & `pyathena-3.0.3/pyathena/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import datetime
 from typing import TYPE_CHECKING, FrozenSet, Type
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection
 
-__version__: str = "3.0.2"
+__version__: str = "3.0.3"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.0.2/pyathena/arrow/async_cursor.py` & `pyathena-3.0.3/pyathena/arrow/async_cursor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 from concurrent.futures import Future
 from multiprocessing import cpu_count
 from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Union
 
 from pyathena import ProgrammingError
 from pyathena.arrow.converter import (
```

### Comparing `pyathena-3.0.2/pyathena/arrow/converter.py` & `pyathena-3.0.3/pyathena/arrow/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 from builtins import isinstance
 from copy import deepcopy
 from datetime import date, datetime
 from typing import Any, Callable, Dict, Optional, Type, Union
 
 from pyathena.converter import (
```

### Comparing `pyathena-3.0.2/pyathena/arrow/cursor.py` & `pyathena-3.0.3/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/pyathena/arrow/result_set.py` & `pyathena-3.0.3/pyathena/arrow/result_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
```

### Comparing `pyathena-3.0.2/pyathena/arrow/util.py` & `pyathena-3.0.3/pyathena/arrow/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 from typing import TYPE_CHECKING, Any, Dict, Tuple, cast
 
 if TYPE_CHECKING:
     from pyarrow import Schema
     from pyarrow.lib import DataType
```

### Comparing `pyathena-3.0.2/pyathena/async_cursor.py` & `pyathena-3.0.3/pyathena/async_cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 from concurrent.futures import Future
 from concurrent.futures.thread import ThreadPoolExecutor
 from multiprocessing import cpu_count
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 from pyathena.common import CursorIterator
```

### Comparing `pyathena-3.0.2/pyathena/common.py` & `pyathena-3.0.3/pyathena/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 import sys
 import time
 from abc import ABCMeta, abstractmethod
 from datetime import datetime, timedelta, timezone
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
```

### Comparing `pyathena-3.0.2/pyathena/connection.py` & `pyathena-3.0.3/pyathena/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 import os
 import time
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type
 
 from boto3.session import Session
 from botocore.config import Config
```

### Comparing `pyathena-3.0.2/pyathena/converter.py` & `pyathena-3.0.3/pyathena/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import binascii
 import json
 import logging
 from abc import ABCMeta, abstractmethod
 from copy import deepcopy
 from datetime import date, datetime, time
 from decimal import Decimal
```

### Comparing `pyathena-3.0.2/pyathena/cursor.py` & `pyathena-3.0.3/pyathena/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/pyathena/error.py` & `pyathena-3.0.3/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/pyathena/fastparquet/util.py` & `pyathena-3.0.3/pyathena/fastparquet/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 from typing import TYPE_CHECKING, Any, Dict, Tuple
 
 if TYPE_CHECKING:
     from fastparquet.parquet_thrift import SchemaElement
     from fastparquet.schema import SchemaHelper
```

### Comparing `pyathena-3.0.2/pyathena/filesystem/s3.py` & `pyathena-3.0.3/pyathena/filesystem/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import itertools
 import logging
 import re
 from concurrent.futures.thread import ThreadPoolExecutor
 from copy import deepcopy
 from multiprocessing import cpu_count
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Pattern, Tuple, cast
```

### Comparing `pyathena-3.0.2/pyathena/filesystem/s3_object.py` & `pyathena-3.0.3/pyathena/filesystem/s3_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
 _logger = logging.getLogger(__name__)  # type: ignore
```

### Comparing `pyathena-3.0.2/pyathena/formatter.py` & `pyathena-3.0.3/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/pyathena/model.py` & `pyathena-3.0.3/pyathena/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Pattern
 
 from pyathena.error import DataError
```

### Comparing `pyathena-3.0.2/pyathena/pandas/async_cursor.py` & `pyathena-3.0.3/pyathena/pandas/async_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 from concurrent.futures import Future
 from multiprocessing import cpu_count
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Tuple, Union
 
 from pyathena import ProgrammingError
 from pyathena.async_cursor import AsyncCursor
```

### Comparing `pyathena-3.0.2/pyathena/pandas/converter.py` & `pyathena-3.0.3/pyathena/pandas/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 from copy import deepcopy
 from typing import Any, Callable, Dict, Optional, Type
 
 from pyathena.converter import (
     Converter,
     _to_binary,
```

### Comparing `pyathena-3.0.2/pyathena/pandas/cursor.py` & `pyathena-3.0.3/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/pyathena/pandas/result_set.py` & `pyathena-3.0.3/pyathena/pandas/result_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 from collections import abc
 from multiprocessing import cpu_count
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
```

### Comparing `pyathena-3.0.2/pyathena/pandas/util.py` & `pyathena-3.0.3/pyathena/pandas/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import concurrent
 import logging
 import textwrap
 import uuid
 from collections import OrderedDict
 from concurrent.futures.process import ProcessPoolExecutor
 from concurrent.futures.thread import ThreadPoolExecutor
```

### Comparing `pyathena-3.0.2/pyathena/result_set.py` & `pyathena-3.0.3/pyathena/result_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import collections
 import logging
 from abc import abstractmethod
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
```

### Comparing `pyathena-3.0.2/pyathena/sqlalchemy/arrow.py` & `pyathena-3.0.3/pyathena/sqlalchemy/arrow.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/pyathena/sqlalchemy/base.py` & `pyathena-3.0.3/pyathena/sqlalchemy/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import re
 from distutils.util import strtobool
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
```

### Comparing `pyathena-3.0.2/pyathena/sqlalchemy/pandas.py` & `pyathena-3.0.3/pyathena/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/pyathena/sqlalchemy/requirements.py` & `pyathena-3.0.3/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.2/pyathena/sqlalchemy/types.py` & `pyathena-3.0.3/pyathena/sqlalchemy/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 from datetime import date, datetime
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 from sqlalchemy.sql.type_api import TypeEngine
 
 if TYPE_CHECKING:
     from sqlalchemy import Dialect
```

### Comparing `pyathena-3.0.2/pyathena/util.py` & `pyathena-3.0.3/pyathena/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 import re
 from typing import Any, Callable, Iterable, Optional, Pattern, Tuple
 
 import tenacity
 from tenacity import after_log, retry_if_exception, stop_after_attempt, wait_exponential
```

### Comparing `pyathena-3.0.2/pyproject.toml` & `pyathena-3.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyAthena"
-version = "3.0.2"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
+version = "3.0.3"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
 description = "Python DB API 2.0 (PEP 249) client for Amazon Athena"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyathena-3.0.2/PKG-INFO` & `pyathena-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: pyathena
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Home-page: https://github.com/laughingman7743/PyAthena/
 License: MIT
 Author: laughingman7743
 Author-email: laughingman7743@gmail.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Front-Ends
 Provides-Extra: arrow
 Provides-Extra: fastparquet
 Provides-Extra: pandas
 Provides-Extra: sqlalchemy
 Requires-Dist: boto3 (>=1.26.4)
 Requires-Dist: botocore (>=1.29.4)
```

