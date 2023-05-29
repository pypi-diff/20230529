# Comparing `tmp/awsiot_credentialhelper-0.2.1.tar.gz` & `tmp/awsiot_credentialhelper-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsiot_credentialhelper-0.2.1.tar", max compression
+gzip compressed data, was "awsiot_credentialhelper-0.5.0.tar", max compression
```

## Comparing `awsiot_credentialhelper-0.2.1.tar` & `awsiot_credentialhelper-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     9764 2023-02-27 17:28:58.043339 awsiot_credentialhelper-0.2.1/LICENSE
--rw-r--r--   0        0        0     5207 2023-02-27 17:28:58.043339 awsiot_credentialhelper-0.2.1/README.md
--rw-r--r--   0        0        0     2670 2023-02-27 17:29:21.841114 awsiot_credentialhelper-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      433 2023-02-27 17:28:58.043339 awsiot_credentialhelper-0.2.1/src/awsiot_credentialhelper/__init__.py
--rw-r--r--   0        0        0    22191 2023-02-27 17:28:58.043339 awsiot_credentialhelper-0.2.1/src/awsiot_credentialhelper/boto3_session.py
--rw-r--r--   0        0        0        0 2023-02-27 17:28:58.043339 awsiot_credentialhelper-0.2.1/src/awsiot_credentialhelper/py.typed
--rw-r--r--   0        0        0     6234 1970-01-01 00:00:00.000000 awsiot_credentialhelper-0.2.1/setup.py
--rw-r--r--   0        0        0     6398 1970-01-01 00:00:00.000000 awsiot_credentialhelper-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     9764 2023-05-29 16:57:37.628360 awsiot_credentialhelper-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5207 2023-05-29 16:57:37.628360 awsiot_credentialhelper-0.5.0/README.md
+-rw-r--r--   0        0        0     2711 2023-05-29 16:57:50.884332 awsiot_credentialhelper-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      433 2023-05-29 16:57:37.632360 awsiot_credentialhelper-0.5.0/src/awsiot_credentialhelper/__init__.py
+-rw-r--r--   0        0        0    22140 2023-05-29 16:57:37.632360 awsiot_credentialhelper-0.5.0/src/awsiot_credentialhelper/boto3_session.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:57:37.632360 awsiot_credentialhelper-0.5.0/src/awsiot_credentialhelper/py.typed
+-rw-r--r--   0        0        0     6234 1970-01-01 00:00:00.000000 awsiot_credentialhelper-0.5.0/setup.py
+-rw-r--r--   0        0        0     6398 1970-01-01 00:00:00.000000 awsiot_credentialhelper-0.5.0/PKG-INFO
```

### Comparing `awsiot_credentialhelper-0.2.1/LICENSE` & `awsiot_credentialhelper-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awsiot_credentialhelper-0.2.1/README.md` & `awsiot_credentialhelper-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `awsiot_credentialhelper-0.2.1/pyproject.toml` & `awsiot_credentialhelper-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 [tool.poetry]
 name = "awsiot-credentialhelper"
-version = "0.2.1"
+version = "0.5.0"
 description = "AWS IoT Core Credential Provider Session Helper"
 authors = ["Gavin Adams <gavinaws@amazon.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/awslabs/aws-iot-core-credential-provider-session-helper"
 repository = "https://github.com/awslabs/aws-iot-core-credential-provider-session-helper"
 documentation = "https://aws-iot-core-credential-provider-session-helper.readthedocs.io"
@@ -53,20 +53,21 @@
 [tool.poetry.group.dev.dependencies]
 pytest-httpserver = "^1.0.6"
 trustme = "^0.9.0"
 coverage-conditional-plugin = "^0.8.0"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
-tests = ["tests", "*/tests"]
+# tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
 plugins = ["coverage_conditional_plugin"]
-source = ["awsiot_credentialhelper", "tests"]
+# source = ["awsiot_credentialhelper", "tests"]
+source = ["awsiot_credentialhelper"]
 
 [tool.coverage.coverage_conditional_plugin.rules]
 # Here we specify our pragma rules:
 py-gte-38 = "sys_version_info >= (3, 8)"
 os-not-linux = "not platform_system == 'linux'"
 
 [tool.coverage.report]
```

### Comparing `awsiot_credentialhelper-0.2.1/src/awsiot_credentialhelper/boto3_session.py` & `awsiot_credentialhelper-0.5.0/src/awsiot_credentialhelper/boto3_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,16 +158,14 @@
 
         Raises:
             ValueError: Only ``private_key`` __or__ ``pkcs11`` argument are provided.
         """
         # Set logging level for awscrt if provided, otherwise default of no logging, just assertions
         if awscrt_log_level is not None:
             init_logging(log_level=awscrt_log_level, file_name="stdout")
-        else:
-            pass
 
         self._endpoint: str = endpoint
         self._role_alias: str = role_alias
         self._thing_name: str = thing_name
         self._certificate: bytes = self.__load_certificate(certificate)
         self._client_connection_type: str = "mtls"
         self._pkcs11: Pkcs11Config = Pkcs11Config(
@@ -366,16 +364,16 @@
                 expiry_time=credentials["expiration"],
             )
         else:
             raise ValueError(
                 f"Error {stream_completion_result} getting credentials: {json.loads(response.body.decode())}"
             )
 
-    @staticmethod
     def _mtls_client_connection(
+        self,
         url: ParseResult,
         certificate: bytes,
         private_key: bytes,
         port: int,
         verify_peer: bool = True,
         ca: bytes | None = None,
     ) -> HttpClientConnection:
@@ -420,16 +418,16 @@
                 bootstrap=bootstrap,
                 tls_connection_options=tls_conn_opt,
             )
             return connection_future.result(10)
         except AwsCrtError as e:
             raise ValueError(f"Error completing mTLS connection: {e}") from e
 
-    @staticmethod
     def _mtls_pkcs11_client_connection(
+        self,
         url: ParseResult,
         port: int,
         certificate: bytes,
         pkcs11: Pkcs11Config,
         verify_peer: bool = True,
         ca: bytes | None = None,
     ) -> HttpClientConnection:
@@ -484,16 +482,15 @@
                 tls_connection_options=tls_conn_opt,
             )
             return connection_future.result(10)
         except AwsCrtError as e:  # pragma: os-not-linux
             raise ValueError(f"Error completing mTLS connection: {e}") from e
         # ###### End coverage exclusion
 
-    @staticmethod
-    def __load_certificate(certificate: str | bytes) -> bytes:
+    def __load_certificate(self, certificate: str | bytes) -> bytes:
         """Load the certificate.
 
         Args:
             certificate: Representation of the certificate in PEM format.
 
         Returns:
             bytes: Return certificate in bytes.
```

### Comparing `awsiot_credentialhelper-0.2.1/setup.py` & `awsiot_credentialhelper-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['awscrt>=0.16.9,<0.17.0',
  'boto3>=1.20.27,<2.0.0',
  'botocore>=1.23.27,<2.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'awsiot-credentialhelper',
-    'version': '0.2.1',
+    'version': '0.5.0',
     'description': 'AWS IoT Core Credential Provider Session Helper',
     'long_description': '# AWS IoT Core Credential Provider Session Helper\n\n[![PyPI](https://img.shields.io/pypi/v/awsiot-credentialhelper.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/awsiot-credentialhelper.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/awsiot-credentialhelper)][pypi status]\n[![License](https://img.shields.io/pypi/l/awsiot-credentialhelper)][license]\n\n[![Tests](https://github.com/awslabs/aws-iot-core-credential-provider-session-helper/workflows/Tests/badge.svg)][tests]\n[![codecov](https://codecov.io/gh/awslabs/aws-iot-core-credential-provider-session-helper/branch/main/graph/badge.svg?token=8V1XZY37BQ)](https://codecov.io/gh/awslabs/aws-iot-core-credential-provider-session-helper)\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/awsiot-credentialhelper/\n[tests]: https://github.com/awslabs/aws-iot-core-credential-provider-session-helper/actions?workflow=Tests\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nThis package provides an easy way to create a **refreshable** Boto3 Session using the [AWS IoT Core credential provider](https://docs.aws.amazon.com/iot/latest/developerguide/authorizing-direct-aws.html).\n\n<p align="center">\n<a href="https://awslabs.github.io/aws-iot-core-credential-provider-session-helper/">Package documentation</a>\n</p>\n\n## Features\n\n- Automatic refresh of [Boto3 credentials](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) through requests to the AWS IoT Core credential provider. No need to manage or maintain refresh times.\n- Uses the underlying [AWS CRT Python](https://github.com/awslabs/aws-crt-python) bindings for querying the credential provider instead of the Python standard library. This provides support for both certificate and private keys as files _or_ as environment variables.\n- Extensible to using other TLS methods such as PKCS#11 hardware security modules (see Advanced section).\n- Only requires four function calls to create a session helper, Boto3 session, Boto3 client, and then client API calls.\n\n## Requirements\n\n- Python 3.8 - 3.11. Support not include for 3.7 as that version will be end of life in June, 2023. If 3.7 support _is_ important, please open an issue to discuss.\n\n## Installation\n\nYou can install _AWS IoT Core Credential Provider Session Helper_ via [pip] from [PyPI]:\n\n```console\npython3 -m pip install awsiot-credentialhelper\n```\n\n## Usage\n\nPrior to use, ensure all cloud-side resources for IAM and AWS IoT Core have been properly created and configured. Then, with the AWS IoT registered X.509 certificate and corresponding private key (e.g., `iot_thing.pem` and `iot_thing.pem.key`), you can create and use the helper as follows:\n\n```python\nfrom awsiot_credentialhelper.boto3_session import Boto3SessionProvider\n\n# Create boto3 session object\nboto3_session = Boto3SessionProvider(\n    endpoint="your_endpoint.credentials.iot.us-west-2.amazonaws.com",\n    role_alias="your_aws_iot_role_alias_name",\n    certificate="iot_thing.pem",\n    private_key="iot_thing.pem.key",\n    thing_name="iot_thing",\n).get_session()\n\n# Use in regular Boto3 chained operations, such as returning caller identity\nprint(boto3_session.client("sts").get_caller_identity())\n{\'UserId\': \'AROA...F3D:4686c...0a0d\', \'Account\': \'1234567890\', \'Arn\': \'arn:aws:sts::1234567890:assumed-role/iam_role_name/4686c...0a0d\', \'ResponseMetadata\': {\'RequestId\': \'cc04...10bc\', \'HTTPStatusCode\': 200, \'HTTPHeaders\': {\'x-amzn-requestid\': \'cc04...10bc\', \'content-type\': \'text/xml\', \'content-length\': \'554\', \'date\': \'Tue, 21 Feb 2023 21:18:23 GMT\'}, \'RetryAttempts\': 0}}\n\n# Or by creating a service client and making API calls\niot = boto3_session.client("iot")\nresult = iot.list_things()\n```\n\nPlease see the [package documentation](https://awslabs.github.io/aws-iot-core-credential-provider-session-helper/) for more details and advanced use.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [Apache 2.0 license][license].\nDetails on third party packages used by this package can be found [here](https://github.com/awslabs/aws-iot-core-credential-provider-session-helper/blob/main/THIRD-PARTY-LICENSES.txt).\n\n## Issues\n\nIf you encounter any problems, please [file an issue](https://github.com/awslabs/aws-iot-core-credential-provider-session-helper/issues/new) along with a detailed description.\n\n## Credits\n\nThis project template was generated from a fork of [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/awslabs/aws-iot-core-credential-provider-session-helper/blob/main/LICENSE\n[contributor guide]: https://github.com/awslabs/aws-iot-core-credential-provider-session-helper/blob/main/CONTRIBUTING.md\n',
     'author': 'Gavin Adams',
     'author_email': 'gavinaws@amazon.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/awslabs/aws-iot-core-credential-provider-session-helper',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['awsiot_credentialhelper'] package_data = \ {'': ['*']}
 install_requires = \ ['awscrt>=0.16.9,<0.17.0', 'boto3>=1.20.27,<2.0.0',
 'botocore>=1.23.27,<2.0.0', 'typing-extensions>=4.5.0,<5.0.0'] setup_kwargs =
-{ 'name': 'awsiot-credentialhelper', 'version': '0.2.1', 'description': 'AWS
+{ 'name': 'awsiot-credentialhelper', 'version': '0.5.0', 'description': 'AWS
 IoT Core Credential Provider Session Helper', 'long_description': '# AWS IoT
 Core Credential Provider Session Helper\n\n[![PyPI](https://img.shields.io/
 pypi/v/awsiot-credentialhelper.svg)][pypi status]\n[![Status](https://
 img.shields.io/pypi/status/awsiot-credentialhelper.svg)][pypi status]\n[!
 [Python Version](https://img.shields.io/pypi/pyversions/awsiot-
 credentialhelper)][pypi status]\n[![License](https://img.shields.io/pypi/l/
 awsiot-credentialhelper)][license]\n\n[![Tests](https://github.com/awslabs/aws-
```

### Comparing `awsiot_credentialhelper-0.2.1/PKG-INFO` & `awsiot_credentialhelper-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsiot-credentialhelper
-Version: 0.2.1
+Version: 0.5.0
 Summary: AWS IoT Core Credential Provider Session Helper
 Home-page: https://github.com/awslabs/aws-iot-core-credential-provider-session-helper
 License: Apache-2.0
 Author: Gavin Adams
 Author-email: gavinaws@amazon.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awsiot-credentialhelper Version: 0.2.1 Summary: AWS
+Metadata-Version: 2.1 Name: awsiot-credentialhelper Version: 0.5.0 Summary: AWS
 IoT Core Credential Provider Session Helper Home-page: https://github.com/
 awslabs/aws-iot-core-credential-provider-session-helper License: Apache-2.0
 Author: Gavin Adams Author-email: gavinaws@amazon.com Requires-Python:
 >=3.8,<4.0 Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

