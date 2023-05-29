# Comparing `tmp/aiospamc-0.8.1.tar.gz` & `tmp/aiospamc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiospamc-0.8.1.tar", max compression
+gzip compressed data, was "aiospamc-0.9.0.tar", max compression
```

## Comparing `aiospamc-0.8.1.tar` & `aiospamc-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1074 2022-01-31 14:44:22.994625 aiospamc-0.8.1/LICENSE
--rw-r--r--   0        0        0     2502 2022-01-31 14:44:22.994625 aiospamc-0.8.1/README.rst
--rw-r--r--   0        0        0      558 2022-01-31 14:44:22.994625 aiospamc-0.8.1/aiospamc/__init__.py
--rw-r--r--   0        0        0     4682 2022-01-31 14:44:22.994625 aiospamc-0.8.1/aiospamc/client.py
--rw-r--r--   0        0        0     8356 2022-01-31 14:44:22.994625 aiospamc-0.8.1/aiospamc/connections.py
--rw-r--r--   0        0        0     5838 2022-01-31 14:44:22.994625 aiospamc-0.8.1/aiospamc/exceptions.py
--rw-r--r--   0        0        0    26209 2022-01-31 14:44:22.998625 aiospamc-0.8.1/aiospamc/frontend.py
--rw-r--r--   0        0        0     3315 2022-01-31 14:44:22.998625 aiospamc-0.8.1/aiospamc/header_values.py
--rw-r--r--   0        0        0    18879 2022-01-31 14:44:22.998625 aiospamc-0.8.1/aiospamc/incremental_parser.py
--rw-r--r--   0        0        0      583 2022-01-31 14:44:22.998625 aiospamc-0.8.1/aiospamc/options.py
--rw-r--r--   0        0        0     2622 2022-01-31 14:44:22.998625 aiospamc-0.8.1/aiospamc/requests.py
--rw-r--r--   0        0        0     6088 2022-01-31 14:44:22.998625 aiospamc-0.8.1/aiospamc/responses.py
--rw-r--r--   0        0        0     1245 2022-01-31 14:44:22.998625 aiospamc-0.8.1/aiospamc/user_warnings.py
--rw-r--r--   0        0        0     1959 2022-01-31 14:44:22.998625 aiospamc-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3295 2022-01-31 14:45:37.681239 aiospamc-0.8.1/setup.py
--rw-r--r--   0        0        0     3539 2022-01-31 14:45:37.681628 aiospamc-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-10-28 02:02:19.747279 aiospamc-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2502 2022-10-28 02:02:19.747279 aiospamc-0.9.0/README.rst
+-rw-r--r--   0        0        0      564 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/__init__.py
+-rw-r--r--   0        0        0     4682 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/client.py
+-rw-r--r--   0        0        0     8356 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/connections.py
+-rw-r--r--   0        0        0     5838 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/exceptions.py
+-rw-r--r--   0        0        0    26189 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/frontend.py
+-rw-r--r--   0        0        0     3720 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/header_values.py
+-rw-r--r--   0        0        0    18867 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/incremental_parser.py
+-rw-r--r--   0        0        0     2622 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/requests.py
+-rw-r--r--   0        0        0     6088 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/responses.py
+-rw-r--r--   0        0        0     1245 2022-10-28 02:02:19.747279 aiospamc-0.9.0/aiospamc/user_warnings.py
+-rw-r--r--   0        0        0     2001 2022-10-28 02:02:19.751278 aiospamc-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3299 1970-01-01 00:00:00.000000 aiospamc-0.9.0/setup.py
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 aiospamc-0.9.0/PKG-INFO
```

### Comparing `aiospamc-0.8.1/LICENSE` & `aiospamc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiospamc-0.8.1/README.rst` & `aiospamc-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiospamc-0.8.1/aiospamc/__init__.py` & `aiospamc-0.9.0/aiospamc/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     ping,
     process,
     report,
     report_if_spam,
     symbols,
     tell,
 )
-from .options import ActionOption, MessageClassOption
+from .header_values import ActionOption, MessageClassOption
 
 
 __author__ = "Michael Caley"
 __copyright__ = "Copyright 2016-2022 Michael Caley"
 __license__ = "MIT"
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 __email__ = "mjcaley@darkarctic.com"
 
 logger.disable(__package__)
```

### Comparing `aiospamc-0.8.1/aiospamc/client.py` & `aiospamc-0.9.0/aiospamc/client.py`

 * *Files identical despite different names*

### Comparing `aiospamc-0.8.1/aiospamc/connections.py` & `aiospamc-0.9.0/aiospamc/connections.py`

 * *Files identical despite different names*

### Comparing `aiospamc-0.8.1/aiospamc/exceptions.py` & `aiospamc-0.9.0/aiospamc/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiospamc-0.8.1/aiospamc/frontend.py` & `aiospamc-0.9.0/aiospamc/frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     Union,
 )
 
 from loguru import logger
 
 from .client import Client
 from .connections import Timeout
-from .header_values import MessageClassValue
-from .options import ActionOption, MessageClassOption
+from .header_values import ActionOption, MessageClassOption, MessageClassValue
 from .incremental_parser import parse_set_remove_value
 from .responses import Response
 from .requests import Request
 
 
 async def check(
     message: Union[bytes, SupportsBytes],
```

### Comparing `aiospamc-0.8.1/aiospamc/header_values.py` & `aiospamc-0.9.0/aiospamc/header_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/env python3
 
 """Collection of request and response header value objects."""
 
+from enum import Enum
 import getpass
 from dataclasses import dataclass, asdict
-from typing import Any, Dict
-
-from .options import ActionOption, MessageClassOption
+from typing import Any, Dict, Optional
 
 
 class HeaderValue:
     """Base class for header values."""
 
     def __bytes__(self) -> bytes:
         raise NotImplementedError
@@ -66,14 +65,21 @@
     def __int__(self) -> int:
         return self.length
 
     def __bytes__(self) -> bytes:
         return str(self.length).encode("ascii")
 
 
+class MessageClassOption(Enum):
+    """Option to be used for the MessageClass header."""
+
+    spam = "spam"
+    ham = "ham"
+
+
 @dataclass
 class MessageClassValue(HeaderValue):
     """MessageClass header.  Used to specify whether a message is 'spam' or
     'ham.'
     """
 
     value: MessageClassOption = MessageClassOption.ham
@@ -84,18 +90,30 @@
     def to_dict(self) -> Dict[str, Any]:
         """Converts the value to a dictionary."""
 
         return {"value": self.value.value}
 
 
 @dataclass
+class ActionOption:
+    """Option to be used in the DidRemove, DidSet, Set, and Remove headers.
+
+    :param local: An action will be performed on the SPAMD service's local database.
+    :param remote: An action will be performed on the SPAMD service's remote database.
+    """
+
+    local: Optional[bool]
+    remote: Optional[bool]
+
+
+@dataclass
 class SetOrRemoveValue(HeaderValue):
     """Base class for headers that implement "local" and "remote" rules."""
 
-    action: ActionOption = ActionOption(local=False, remote=False)
+    action: ActionOption
 
     def __bytes__(self) -> bytes:
         if not self.action.local and not self.action.remote:
             # if nothing is set, then return a blank string so the request
             # doesn't get tainted
             return b""
```

### Comparing `aiospamc-0.8.1/aiospamc/incremental_parser.py` & `aiospamc-0.9.0/aiospamc/incremental_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 from typing import Any, Callable, Mapping, Tuple, Union, Dict
 
 import loguru
 from loguru import logger
 
 from .exceptions import ParseError, NotEnoughDataError, TooMuchDataError
 from .header_values import (
+    ActionOption,
     BytesHeaderValue,
     CompressValue,
     ContentLengthValue,
     GenericHeaderValue,
     HeaderValue,
+    MessageClassOption,
     MessageClassValue,
     SetOrRemoveValue,
     SpamValue,
     UserValue,
 )
-from .options import ActionOption, MessageClassOption
 
 
 class States(Enum):
     """States for the parser state machine."""
 
     Status = auto()
     Header = auto()
```

### Comparing `aiospamc-0.8.1/aiospamc/requests.py` & `aiospamc-0.9.0/aiospamc/requests.py`

 * *Files identical despite different names*

### Comparing `aiospamc-0.8.1/aiospamc/responses.py` & `aiospamc-0.9.0/aiospamc/responses.py`

 * *Files identical despite different names*

### Comparing `aiospamc-0.8.1/aiospamc/user_warnings.py` & `aiospamc-0.9.0/aiospamc/user_warnings.py`

 * *Files identical despite different names*

### Comparing `aiospamc-0.8.1/pyproject.toml` & `aiospamc-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiospamc"
-version = "0.8.1"
+version = "0.9.0"
 description = "An asyncio-based library to communicate with SpamAssassin's SPAMD service."
 authors = ["Michael Caley <mjcaley@darkarctic.com>"]
 license = "MIT"
 readme = "README.rst"
 
 repository = "https://github.com/mjcaley/aiospamc"
 homepage = "https://github.com/mjcaley/aiospamc"
@@ -12,14 +12,15 @@
 
 classifiers = [
     'Development Status :: 4 - Beta',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Intended Audience :: Developers',
     'Intended Audience :: System Administrators',
     'License :: OSI Approved :: MIT License',
     'Topic :: Communications :: Email :: Filters'
 ]
 
 keywords = ["spam", "spamc", "spamassassin"]
@@ -61,23 +62,23 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 certifi = "*"
 loguru = "^0.6.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2"
-pytest-cov = "^3.0"
-pytest-asyncio = "^0.17.0"
-sphinx = "^4.2"
-pytest-mock = "^3.6"
+pytest = "^7.1"
+pytest-cov = "^4.0"
+pytest-asyncio = "^0.20"
+sphinx = "^5.3"
+pytest-mock = "^3.10"
 mock = "^4.0"
-coverage = {extras = ["toml"], version = "^6.0"}
-mypy = "^0.910"
-black = "21.9b0"
+coverage = {extras = ["toml"], version = "^6.5"}
+mypy = "^0.982"
+black = "^22"
 interrogate = "^1.5"
 trustme = "^0.9.0"
 reno = "^3.5.0"
 types-certifi = "^2021.10.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `aiospamc-0.8.1/setup.py` & `aiospamc-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['certifi', 'loguru>=0.6.0,<0.7.0']
 
 setup_kwargs = {
     'name': 'aiospamc',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': "An asyncio-based library to communicate with SpamAssassin's SPAMD service.",
     'long_description': "========\naiospamc\n========\n\n|pypi| |docs| |license| |unit| |integration| |python|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/aiospamc\n    :target: https://pypi.org/project/aiospamc/\n\n.. |unit| image:: https://github.com/mjcaley/aiospamc/actions/workflows/unit-tests.yml/badge.svg\n    :target: https://github.com/mjcaley/aiospamc/actions/workflows/unit-tests.yml\n\n.. |integration| image:: https://github.com/mjcaley/aiospamc/actions/workflows/integration-tests.yml/badge.svg\n    :target: https://github.com/mjcaley/aiospamc/actions/workflows/integration-tests.yml\n\n.. |docs| image:: https://readthedocs.org/projects/aiospamc/badge/?version=latest\n    :target: https://aiospamc.readthedocs.io/en/latest/\n\n.. |license| image:: https://img.shields.io/github/license/mjcaley/aiospamc\n    :target: ./LICENSE\n\n.. |python| image:: https://img.shields.io/pypi/pyversions/aiospamc\n    :target: https://python.org\n\n-----------\nDescription\n-----------\n\nPython asyncio-based library that implements the SPAMC/SPAMD client protocol used by SpamAssassin.\n\n-------------\nDocumentation\n-------------\n\nDocumentation can be found at: https://aiospamc.readthedocs.io/\n\n------------\nRequirements\n------------\n\n* Python 3.7 or higher\n\n-------\nExample\n-------\n\n.. code:: python\n    \n    import asyncio\n    import aiospamc\n\n\n    GTUBE = '''Subject: Test spam mail (GTUBE)\n    Message-ID: <GTUBE1.1010101@example.net>\n    Date: Wed, 23 Jul 2003 23:30:00 +0200\n    From: Sender <sender@example.net>\n    To: Recipient <recipient@example.net>\n    Precedence: junk\n    MIME-Version: 1.0\n    Content-Type: text/plain; charset=us-ascii\n    Content-Transfer-Encoding: 7bit\n\n    This is the GTUBE, the\n        Generic\n        Test for\n        Unsolicited\n        Bulk\n        Email\n\n    If your spam filter supports it, the GTUBE provides a test by which you\n    can verify that the filter is installed correctly and is detecting incoming\n    spam. You can send yourself a test mail containing the following string of\n    characters (in upper case and with no white spaces and line breaks):\n\n    XJS*C4JDBQADN1.NSBN3*2IDNEN*GTUBE-STANDARD-ANTI-UBE-TEST-EMAIL*C.34X\n\n    You should send this test mail from an account outside of your network.\n    '''.encode('ascii')\n\n    loop = asyncio.get_event_loop()\n    responses = loop.run_until_complete(asyncio.gather(\n\n        aiospamc.ping(host='localhost'),\n        aiospamc.check(GTUBE, host='localhost'),\n        aiospamc.headers(GTUBE, host='localhost')\n\n    ))\n    print(responses)\n",
     'author': 'Michael Caley',
     'author_email': 'mjcaley@darkarctic.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/mjcaley/aiospamc',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `aiospamc-0.8.1/PKG-INFO` & `aiospamc-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: aiospamc
-Version: 0.8.1
+Version: 0.9.0
 Summary: An asyncio-based library to communicate with SpamAssassin's SPAMD service.
 Home-page: https://github.com/mjcaley/aiospamc
 License: MIT
 Keywords: spam,spamc,spamassassin
 Author: Michael Caley
 Author-email: mjcaley@darkarctic.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Dist: certifi
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Project-URL: Documentation, https://aiospamc.readthedocs.io
```

