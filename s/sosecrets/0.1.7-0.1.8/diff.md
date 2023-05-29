# Comparing `tmp/sosecrets-0.1.7.tar.gz` & `tmp/sosecrets-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosecrets-0.1.7.tar", max compression
+gzip compressed data, was "sosecrets-0.1.8.tar", max compression
```

## Comparing `sosecrets-0.1.7.tar` & `sosecrets-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1110 2023-05-28 15:14:56.204604 sosecrets-0.1.7/LICENSE
--rw-r--r--   0        0        0     1060 2023-05-29 18:56:29.458639 sosecrets-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5308 2023-05-29 18:56:29.469637 sosecrets-0.1.7/README.md
--rw-r--r--   0        0        0      142 2023-05-29 18:56:29.467637 sosecrets-0.1.7/src/sosecrets/__init__.py
--rw-r--r--   0        0        0        6 2023-05-29 18:50:19.809293 sosecrets-0.1.7/src/sosecrets/py.typed
--rw-r--r--   0        0        0     7770 2023-05-29 18:50:19.811293 sosecrets-0.1.7/src/sosecrets/secretdicts.py
--rw-r--r--   0        0        0     3075 2023-05-29 18:50:19.812292 sosecrets-0.1.7/src/sosecrets/secrets.pyi
--rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 sosecrets-0.1.7/setup.py
--rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 sosecrets-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-05-28 15:14:56.204604 sosecrets-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1060 2023-05-29 19:03:59.269758 sosecrets-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5308 2023-05-29 19:01:44.726100 sosecrets-0.1.8/README.md
+-rw-r--r--   0        0        0      133 2023-05-29 19:01:44.712100 sosecrets-0.1.8/src/sosecrets/__init__.py
+-rw-r--r--   0        0        0        6 2023-05-29 18:50:19.809293 sosecrets-0.1.8/src/sosecrets/py.typed
+-rw-r--r--   0        0        0     7770 2023-05-29 18:50:19.811293 sosecrets-0.1.8/src/sosecrets/secretdicts.py
+-rw-r--r--   0        0        0     3075 2023-05-29 18:50:19.812292 sosecrets-0.1.8/src/sosecrets/secrets.pyi
+-rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 sosecrets-0.1.8/setup.py
+-rw-r--r--   0        0        0     5821 1970-01-01 00:00:00.000000 sosecrets-0.1.8/PKG-INFO
```

### Comparing `sosecrets-0.1.7/LICENSE` & `sosecrets-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sosecrets-0.1.7/pyproject.toml` & `sosecrets-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "sosecrets"
-version = "0.1.7"
+version = "0.1.8"
 description = "Simple wrapper to secure your secrets."
 authors = ["Jim Chng <jimchng@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["secrets", "security"]
 include = ["src/sosecrets/py.typed", "src/sosecrets/secrets.pyi"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.7"
 sosecrets-core = "^1.0.4"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 
@@ -23,15 +23,15 @@
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.1.7"
+current_version = "0.1.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `sosecrets-0.1.7/README.md` & `sosecrets-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # sosecrets
 
 `sosecrets` is a Python module that provides a secure way to handle sensitive data by encapsulating it and only exposing it through a controlled interface.
 
-Version: 0.1.7
+Version: 0.1.8
 
 [Documentation](https://sosecrets.readthedocs.io/en/latest/)
 
 ## Installation
 
 To install `sosecrets`, you can use pip:
```

### Comparing `sosecrets-0.1.7/src/sosecrets/secretdicts.py` & `sosecrets-0.1.8/src/sosecrets/secretdicts.py`

 * *Files identical despite different names*

### Comparing `sosecrets-0.1.7/src/sosecrets/secrets.pyi` & `sosecrets-0.1.8/src/sosecrets/secrets.pyi`

 * *Files identical despite different names*

### Comparing `sosecrets-0.1.7/setup.py` & `sosecrets-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 {'': ['*']}
 
 install_requires = \
 ['sosecrets-core>=1.0.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'sosecrets',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Simple wrapper to secure your secrets.',
-    'long_description': '# sosecrets\n\n`sosecrets` is a Python module that provides a secure way to handle sensitive data by encapsulating it and only exposing it through a controlled interface.\n\nVersion: 0.1.7\n\n[Documentation](https://sosecrets.readthedocs.io/en/latest/)\n\n## Installation\n\nTo install `sosecrets`, you can use pip:\n\n```bash\npip install sosecrets\n```\n\n## Usage\n\nHere\'s are the examples of how to use `sosecrets`:\n\n### Secret\n\nHere\'s an example of how to use `Secret`:\n\n```python\nfrom sosecrets import Secret\n\n# Create a secret value\nsecret_value = Secret("my secret value")\n\n# Use the secret value while keeping it encapsulated\nresult = secret_value.apply(len)\nprint(result)  # Output: 14\n\n# Get the value of the secret\nvalue = secret_value.expose_secret()\nprint(value)  # Output: "my secret value"\n```\n\nIn this example, we create a `Secret` object with the value "my secret value". We then use the `apply` method to apply the `len` function to the secret value while keeping it encapsulated. Finally, we use the `expose_secret` method to retrieve the value of the secret.\n\n### ImmutableSecretMapping\n\nHere\'s an example of how to use `ImmutableSecretMapping`:\n\n```python\nfrom pathlib import Path\nfrom sosecrets import ImmutableSecretMapping\nfrom dotenv import dotenv_values\n\n# Define the path to the `.env` file\nTHIS_SCRIPT_FILE_PATH = Path(__file__)\nEXAMPLES = THIS_SCRIPT_FILE_PATH.parent / \'.env\'\n\n# Load the environment variables and store them securely\nsecret_env_dict = ImmutableSecretMapping.from_func(dotenv_values, dotenv_path=EXAMPLES)\n\n# Get a dictionary of the exposed values of the secret variables\nexposed_dict = secret_env_dict.expose_dict()\nprint("exposed_dict: ", exposed_dict)\n\n# Print the `ImmutableSecretMapping` object itself\nprint("secret_env_dict: ", secret_env_dict)\n\n# Get the value associated with a key using the `get()` method\nvalue0 = secret_env_dict.get(\'value0\')\nprint("value0: ", value0)\n\n# Get the exposed value of a key using the `get_exposed()` method\nvalue1 = secret_env_dict.get_exposed(\'value1\')\nprint("value1: ", value1)\n```\n\nThe example code does the following:\n\n1. Imports the necessary packages: `Path` from `pathlib`, `src` from the `sosecrets` module, `ImmutableSecretMapping` from `secretdicts` in the `sosecrets` module, and `dotenv_values` from the `dotenv` package.\n2. Defines the path to a `.env` file that contains environment variables to be loaded.\n3. Uses `ImmutableSecretMapping.from_func(dotenv_values, dotenv_path=EXAMPLES)` to load the environment variables from the `.env` file and store them in an instance of `ImmutableSecretMapping`.\n4. Prints the exposed dictionary of the `ImmutableSecretMapping` object using the `expose_dict()` method.\n5. Prints the `ImmutableSecretMapping` object itself.\n6. Gets a value from the `ImmutableSecretMapping` object using the `get()` method and prints it.\n7. Gets the exposed value of a key using the `get_exposed()` method## The Output\n\n### MutableSecretMapping\n\nSimilar to `ImmutableSecretMapping`.\n\n## Use Cases\nsosecrets can be used in a variety of scenarios where sensitive data needs to be securely handled. Here are some common use cases:\n\nStoring API keys, passwords, and other credentials: sosecrets can be used to securely store sensitive information such as API keys, passwords, and other credentials that are required for authentication or authorization in an application.\n\nHandling personal identifiable information (PII): sosecrets can be used to protect personal identifiable information (PII) such as names, addresses, social security numbers, and other sensitive data that needs to be kept confidential.\n\n## API Reference\n\n### `Secret`\n\nThe `Secret` class encapsulates a secret value and only exposes it through a controlled interface.\n\n```\nSecret(value: Optional[T] = None, func: Optional[Callable[[Any], T]] = None, func_args: Tuple[Any] = tuple(), func_kwargs: Dict[str, Any] = dict()) -> SecretType\n```\n\n- `value`: The secret value to encapsulate.\n- `func`: A function to generate the secret value.\n- `func_args`: The positional arguments to pass to the `func` function.\n- `func_kwargs`: The keyword arguments to pass to the `func` function.\n\n#### `apply`\n\nThe `apply` method applies a function to the secret value while keeping it encapsulated.\n\n```python\napply(self, func: Callable[[Any], Any], *args: Tuple[Any], **kwargs: Dict[str, Any]) -> SecretType:\n```\n\n- `func`: The function to apply to the secret value.\n- `args`: The positional arguments to pass to the `func` function.\n- `kwargs`: The keyword arguments to pass to the `func` function.\n\n#### `expose_secret`\n\nThe `expose_secret` method returns the value of the secret.\n\n```python\ndef expose_secret(self) -> T:\n```\n\n### Exceptions\n\n`sosecrets` defines the following exceptions:\n\n#### `CannotInstantiateExposeSecret`\n\nRaised when attempting to instantiate the `__expose_secret__` class.\n\n#### `CannotInheritFromSecret`\n\nRaised when attempting to subclass the `Secret` class.\n\n#### `FuncAndValueCannotBeBothPassed`\n\nRaised when both `value` and `func` arguments are passed to the `Secret` constructor.\n\n## Contributing\n\nContributions are welcome! Let me know if you need help with anything else.',
+    'long_description': '# sosecrets\n\n`sosecrets` is a Python module that provides a secure way to handle sensitive data by encapsulating it and only exposing it through a controlled interface.\n\nVersion: 0.1.8\n\n[Documentation](https://sosecrets.readthedocs.io/en/latest/)\n\n## Installation\n\nTo install `sosecrets`, you can use pip:\n\n```bash\npip install sosecrets\n```\n\n## Usage\n\nHere\'s are the examples of how to use `sosecrets`:\n\n### Secret\n\nHere\'s an example of how to use `Secret`:\n\n```python\nfrom sosecrets import Secret\n\n# Create a secret value\nsecret_value = Secret("my secret value")\n\n# Use the secret value while keeping it encapsulated\nresult = secret_value.apply(len)\nprint(result)  # Output: 14\n\n# Get the value of the secret\nvalue = secret_value.expose_secret()\nprint(value)  # Output: "my secret value"\n```\n\nIn this example, we create a `Secret` object with the value "my secret value". We then use the `apply` method to apply the `len` function to the secret value while keeping it encapsulated. Finally, we use the `expose_secret` method to retrieve the value of the secret.\n\n### ImmutableSecretMapping\n\nHere\'s an example of how to use `ImmutableSecretMapping`:\n\n```python\nfrom pathlib import Path\nfrom sosecrets import ImmutableSecretMapping\nfrom dotenv import dotenv_values\n\n# Define the path to the `.env` file\nTHIS_SCRIPT_FILE_PATH = Path(__file__)\nEXAMPLES = THIS_SCRIPT_FILE_PATH.parent / \'.env\'\n\n# Load the environment variables and store them securely\nsecret_env_dict = ImmutableSecretMapping.from_func(dotenv_values, dotenv_path=EXAMPLES)\n\n# Get a dictionary of the exposed values of the secret variables\nexposed_dict = secret_env_dict.expose_dict()\nprint("exposed_dict: ", exposed_dict)\n\n# Print the `ImmutableSecretMapping` object itself\nprint("secret_env_dict: ", secret_env_dict)\n\n# Get the value associated with a key using the `get()` method\nvalue0 = secret_env_dict.get(\'value0\')\nprint("value0: ", value0)\n\n# Get the exposed value of a key using the `get_exposed()` method\nvalue1 = secret_env_dict.get_exposed(\'value1\')\nprint("value1: ", value1)\n```\n\nThe example code does the following:\n\n1. Imports the necessary packages: `Path` from `pathlib`, `src` from the `sosecrets` module, `ImmutableSecretMapping` from `secretdicts` in the `sosecrets` module, and `dotenv_values` from the `dotenv` package.\n2. Defines the path to a `.env` file that contains environment variables to be loaded.\n3. Uses `ImmutableSecretMapping.from_func(dotenv_values, dotenv_path=EXAMPLES)` to load the environment variables from the `.env` file and store them in an instance of `ImmutableSecretMapping`.\n4. Prints the exposed dictionary of the `ImmutableSecretMapping` object using the `expose_dict()` method.\n5. Prints the `ImmutableSecretMapping` object itself.\n6. Gets a value from the `ImmutableSecretMapping` object using the `get()` method and prints it.\n7. Gets the exposed value of a key using the `get_exposed()` method## The Output\n\n### MutableSecretMapping\n\nSimilar to `ImmutableSecretMapping`.\n\n## Use Cases\nsosecrets can be used in a variety of scenarios where sensitive data needs to be securely handled. Here are some common use cases:\n\nStoring API keys, passwords, and other credentials: sosecrets can be used to securely store sensitive information such as API keys, passwords, and other credentials that are required for authentication or authorization in an application.\n\nHandling personal identifiable information (PII): sosecrets can be used to protect personal identifiable information (PII) such as names, addresses, social security numbers, and other sensitive data that needs to be kept confidential.\n\n## API Reference\n\n### `Secret`\n\nThe `Secret` class encapsulates a secret value and only exposes it through a controlled interface.\n\n```\nSecret(value: Optional[T] = None, func: Optional[Callable[[Any], T]] = None, func_args: Tuple[Any] = tuple(), func_kwargs: Dict[str, Any] = dict()) -> SecretType\n```\n\n- `value`: The secret value to encapsulate.\n- `func`: A function to generate the secret value.\n- `func_args`: The positional arguments to pass to the `func` function.\n- `func_kwargs`: The keyword arguments to pass to the `func` function.\n\n#### `apply`\n\nThe `apply` method applies a function to the secret value while keeping it encapsulated.\n\n```python\napply(self, func: Callable[[Any], Any], *args: Tuple[Any], **kwargs: Dict[str, Any]) -> SecretType:\n```\n\n- `func`: The function to apply to the secret value.\n- `args`: The positional arguments to pass to the `func` function.\n- `kwargs`: The keyword arguments to pass to the `func` function.\n\n#### `expose_secret`\n\nThe `expose_secret` method returns the value of the secret.\n\n```python\ndef expose_secret(self) -> T:\n```\n\n### Exceptions\n\n`sosecrets` defines the following exceptions:\n\n#### `CannotInstantiateExposeSecret`\n\nRaised when attempting to instantiate the `__expose_secret__` class.\n\n#### `CannotInheritFromSecret`\n\nRaised when attempting to subclass the `Secret` class.\n\n#### `FuncAndValueCannotBeBothPassed`\n\nRaised when both `value` and `func` arguments are passed to the `Secret` constructor.\n\n## Contributing\n\nContributions are welcome! Let me know if you need help with anything else.',
     'author': 'Jim Chng',
     'author_email': 'jimchng@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `sosecrets-0.1.7/PKG-INFO` & `sosecrets-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: sosecrets
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple wrapper to secure your secrets.
 License: MIT
 Keywords: secrets,security
 Author: Jim Chng
 Author-email: jimchng@outlook.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sosecrets-core (>=1.0.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # sosecrets
 
 `sosecrets` is a Python module that provides a secure way to handle sensitive data by encapsulating it and only exposing it through a controlled interface.
 
-Version: 0.1.7
+Version: 0.1.8
 
 [Documentation](https://sosecrets.readthedocs.io/en/latest/)
 
 ## Installation
 
 To install `sosecrets`, you can use pip:
```

