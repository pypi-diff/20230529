# Comparing `tmp/onyx_client-6.0.0.tar.gz` & `tmp/onyx_client-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onyx_client-6.0.0.tar", max compression
+gzip compressed data, was "onyx_client-6.1.0.tar", max compression
```

## Comparing `onyx_client-6.0.0.tar` & `onyx_client-6.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1090 2023-03-24 06:59:04.123449 onyx_client-6.0.0/LICENSE
--rw-r--r--   0        0        0     5829 2023-03-24 06:59:04.123449 onyx_client-6.0.0/README.md
--rw-r--r--   0        0        0       47 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/__init__.py
--rw-r--r--   0        0        0     1289 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/authorizer/__init__.py
--rw-r--r--   0        0        0     9359 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/client.py
--rw-r--r--   0        0        0       33 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/configuration/__init__.py
--rw-r--r--   0        0        0      290 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/configuration/configuration.py
--rw-r--r--   0        0        0       32 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/data/__init__.py
--rw-r--r--   0        0        0     1119 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/data/animation_keyframe.py
--rw-r--r--   0        0        0     1072 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/data/animation_value.py
--rw-r--r--   0        0        0      768 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/data/boolean_value.py
--rw-r--r--   0        0        0      383 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/data/date_information.py
--rw-r--r--   0        0        0     1297 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/data/device_command.py
--rw-r--r--   0        0        0      312 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/data/device_mode.py
--rw-r--r--   0        0        0     2030 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/data/numeric_value.py
--rw-r--r--   0        0        0      384 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/data/supported_versions.py
--rw-r--r--   0        0        0       24 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/device/__init__.py
--rw-r--r--   0        0        0      833 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/device/click.py
--rw-r--r--   0        0        0     1365 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/device/device.py
--rw-r--r--   0        0        0     1572 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/device/light.py
--rw-r--r--   0        0        0     2010 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/device/shutter.py
--rw-r--r--   0        0        0      663 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/device/switch.py
--rw-r--r--   0        0        0     2270 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/device/weather.py
--rw-r--r--   0        0        0       29 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/enum/__init__.py
--rw-r--r--   0        0        0      635 2023-03-24 06:59:04.123449 onyx_client-6.0.0/onyx_client/enum/action.py
--rw-r--r--   0        0        0      989 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/enum/device_type.py
--rw-r--r--   0        0        0       27 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/exception/__init__.py
--rw-r--r--   0        0        0      136 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/exception/invalid_command.py
--rw-r--r--   0        0        0      122 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/exception/update_exception.py
--rw-r--r--   0        0        0       23 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/group/__init__.py
--rw-r--r--   0        0        0      457 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/group/group.py
--rw-r--r--   0        0        0       27 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/helpers/__init__.py
--rw-r--r--   0        0        0     2751 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/helpers/url.py
--rw-r--r--   0        0        0       25 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/utils/__init__.py
--rw-r--r--   0        0        0      150 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/utils/const.py
--rw-r--r--   0        0        0     1823 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/utils/device_type.py
--rw-r--r--   0        0        0      125 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/utils/filter.py
--rw-r--r--   0        0        0     3373 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/utils/mapper.py
--rw-r--r--   0        0        0      536 2023-03-24 06:59:04.127449 onyx_client-6.0.0/onyx_client/utils/response.py
--rw-r--r--   0        0        0     2948 2023-03-24 06:59:41.799453 onyx_client-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     6734 1970-01-01 00:00:00.000000 onyx_client-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-29 18:58:42.717566 onyx_client-6.1.0/LICENSE
+-rw-r--r--   0        0        0     5830 2023-05-29 18:58:42.717566 onyx_client-6.1.0/README.md
+-rw-r--r--   0        0        0       47 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/__init__.py
+-rw-r--r--   0        0        0     1289 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/authorizer/__init__.py
+-rw-r--r--   0        0        0     9359 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/client.py
+-rw-r--r--   0        0        0       33 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/configuration/__init__.py
+-rw-r--r--   0        0        0      290 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/configuration/configuration.py
+-rw-r--r--   0        0        0       32 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/data/__init__.py
+-rw-r--r--   0        0        0     1119 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/data/animation_keyframe.py
+-rw-r--r--   0        0        0     1072 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/data/animation_value.py
+-rw-r--r--   0        0        0      768 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/data/boolean_value.py
+-rw-r--r--   0        0        0      383 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/data/date_information.py
+-rw-r--r--   0        0        0     1297 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/data/device_command.py
+-rw-r--r--   0        0        0      312 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/data/device_mode.py
+-rw-r--r--   0        0        0     2030 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/data/numeric_value.py
+-rw-r--r--   0        0        0      384 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/data/supported_versions.py
+-rw-r--r--   0        0        0       24 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/device/__init__.py
+-rw-r--r--   0        0        0      833 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/device/click.py
+-rw-r--r--   0        0        0     1365 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/device/device.py
+-rw-r--r--   0        0        0     1572 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/device/light.py
+-rw-r--r--   0        0        0     2010 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/device/shutter.py
+-rw-r--r--   0        0        0      663 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/device/switch.py
+-rw-r--r--   0        0        0     2270 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/device/weather.py
+-rw-r--r--   0        0        0       29 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/enum/__init__.py
+-rw-r--r--   0        0        0      635 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/enum/action.py
+-rw-r--r--   0        0        0      989 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/enum/device_type.py
+-rw-r--r--   0        0        0       27 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/exception/__init__.py
+-rw-r--r--   0        0        0      136 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/exception/invalid_command.py
+-rw-r--r--   0        0        0      122 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/exception/update_exception.py
+-rw-r--r--   0        0        0       23 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/group/__init__.py
+-rw-r--r--   0        0        0      457 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/group/group.py
+-rw-r--r--   0        0        0       27 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/helpers/__init__.py
+-rw-r--r--   0        0        0     2751 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/helpers/url.py
+-rw-r--r--   0        0        0       25 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/utils/__init__.py
+-rw-r--r--   0        0        0      150 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/utils/const.py
+-rw-r--r--   0        0        0     1823 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/utils/device_type.py
+-rw-r--r--   0        0        0      125 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/utils/filter.py
+-rw-r--r--   0        0        0     3373 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/utils/mapper.py
+-rw-r--r--   0        0        0      536 2023-05-29 18:58:42.717566 onyx_client-6.1.0/onyx_client/utils/response.py
+-rw-r--r--   0        0        0     2948 2023-05-29 18:59:08.385920 onyx_client-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6687 1970-01-01 00:00:00.000000 onyx_client-6.1.0/PKG-INFO
```

### Comparing `onyx_client-6.0.0/LICENSE` & `onyx_client-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/README.md` & `onyx_client-6.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Onyx Client
 
 [![](https://img.shields.io/github/license/muhlba91/onyx-client?style=for-the-badge)](LICENSE)
-[![](https://img.shields.io/github/workflow/status/muhlba91/onyx-client/Python%20package?style=for-the-badge)](https://github.com/muhlba91/onyx-client/actions)
+[![](https://img.shields.io/github/actions/workflow/status/muhlba91/onyx-client/release.yml?style=for-the-badge)](https://github.com/muhlba91/onyx-client/actions/workflows/release.yml)
 [![](https://img.shields.io/coveralls/github/muhlba91/onyx-client?style=for-the-badge)](https://github.com/muhlba91/onyx-client/)
 [![](https://img.shields.io/pypi/pyversions/onyx-client?style=for-the-badge)](https://pypi.org/project/onyx-client/)
 [![](https://img.shields.io/pypi/v/onyx-client?style=for-the-badge)](https://pypi.org/project/onyx-client/)
 [![](https://img.shields.io/github/release-date/muhlba91/onyx-client?style=for-the-badge)](https://github.com/muhlba91/onyx-client/releases)
 [![](https://img.shields.io/pypi/dm/onyx-client?style=for-the-badge)](https://pypi.org/project/onyx-client/)
 [![Known Vulnerabilities](https://snyk.io/test/github/muhlba91/onyx-client/badge.svg)](https://snyk.io/test/github/muhlba91/onyx-client/)
 <a href="https://www.buymeacoffee.com/muhlba91" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="28" width="150"></a>
@@ -18,16 +18,16 @@
 ## API Versions
 
 It is encouraged to always update Hella devices to the latest software. This will, mostly, also enforce using the newest
 API. In below table you can find an indication of what Hella API version is supported.
 
 | Hella API Version | Client Version    |
 |-------------------|-------------------|
-| v3                | > = 3.1.0 < 6.0.0 |
-| v2                | > = 2.5.0 < 3.0.0 |
+| v3                | >= 3.1.0          |
+| v2                | >= 2.5.0 < 3.0.0  |
 
 ## Installation
 
 The package is published in **(Test)PyPi** and can be installed via:
 
 ```bash
 pip install onyx-client
@@ -79,63 +79,63 @@
 ---
 
 ## Development
 
 The project uses [poetry](https://poetry.eustace.io/) and to install all dependencies and the build environment, run:
 
 ```bash
-$ pip install poetry
-$ poetry install
+pip install poetry
+poetry install
 ```
 
 ### Testing
 
 1) Install all dependencies as shown above.
 2) Run `pytest` by:
 
 ```bash
-$ poetry run pytest
+poetry run pytest
 # or
-$ pytest
+pytest
 ```
 
 ### Linting and Code Style
 
 The project uses [flakehell](https://github.com/life4/flakehell) as a wrapper for flake8,
 and [black](https://github.com/psf/black) for automated code style fixing, also
 using [pre-commit](https://pre-commit.com/).
 
 1) Install all dependencies as shown above.
 2) (Optional) Install pre-commit hooks:
 
 ```bash
-$ poetry run pre-commit install
+poetry run pre-commit install
 ```
 
 3) Run black:
 
 ```bash
-$ poetry run black .
+poetry run black .
 ```
 
 4) Run flakehell:
 
 ```bash
-$ poetry run flakehell lint
+poetry run flakehell lint
 ```
 
 ### Building
 
 This package uses [poetry-dynamic-versioning](https://github.com/mtkennerly/poetry-dynamic-versioning) which infers the
 version number based on the Git tags. Hence, to have a proper versioning for the distribution, use Python's build system
 like:
 
 ```bash
-$ pip install build
-$ python -m build
+pip install build
+python -m build
 ```
 
 Your distribution will be in the `dist` directory.
 
 ### Commit Message
 
 This project follows [Conventional Commits](https://www.conventionalcommits.org/), and your commit message must also
@@ -144,23 +144,23 @@
 ---
 
 ## Release
 
 To draft a release, use [standard-version](https://github.com/conventional-changelog/standard-version):
 
 ```bash
-$ standard-version
+standard-version
 # alternatively
-$ npx standard-version
+npx standard-version
 ```
 
 Finally, push with tags:
 
 ```bash
-$ git push --follow-tags
+git push --follow-tags
 ```
 
 ---
 
 ## Contributions
 
 Please feel free to contribute, be it with Issues or Pull Requests! Please read
```

#### html2text {}

```diff
@@ -1,69 +1,70 @@
 # Onyx Client [![](https://img.shields.io/github/license/muhlba91/onyx-
 client?style=for-the-badge)](LICENSE) [![](https://img.shields.io/github/
-workflow/status/muhlba91/onyx-client/Python%20package?style=for-the-badge)]
-(https://github.com/muhlba91/onyx-client/actions) [![](https://img.shields.io/
-coveralls/github/muhlba91/onyx-client?style=for-the-badge)](https://github.com/
-muhlba91/onyx-client/) [![](https://img.shields.io/pypi/pyversions/onyx-
-client?style=for-the-badge)](https://pypi.org/project/onyx-client/) [![](https:
-//img.shields.io/pypi/v/onyx-client?style=for-the-badge)](https://pypi.org/
-project/onyx-client/) [![](https://img.shields.io/github/release-date/muhlba91/
-onyx-client?style=for-the-badge)](https://github.com/muhlba91/onyx-client/
-releases) [![](https://img.shields.io/pypi/dm/onyx-client?style=for-the-badge)]
-(https://pypi.org/project/onyx-client/) [![Known Vulnerabilities](https://
-snyk.io/test/github/muhlba91/onyx-client/badge.svg)](https://snyk.io/test/
-github/muhlba91/onyx-client/) [Buy_Me_A_Coffee] This repository contains a
-**Python HTTP client** for [Hella](https://www.hella.info)' s [ONYX.CENTER API]
-(https://github.com/hella-info/onyx_api). --- ## API Versions It is encouraged
-to always update Hella devices to the latest software. This will, mostly, also
-enforce using the newest API. In below table you can find an indication of what
-Hella API version is supported. | Hella API Version | Client Version | |-------
-------------|-------------------| | v3 | > = 3.1.0 < 6.0.0 | | v2 | > = 2.5.0 <
-3.0.0 | ## Installation The package is published in **(Test)PyPi** and can be
-installed via: ```bash pip install onyx-client ``` ## Configuration The
-configuration defines **connection properties** as a `dict` for the application
-running. **Attention**: make sure to **read** the [Onyx API Access Control]
-(https://github.com/hella-info/onyx_api#access-control) description to
-**retrieve the fingerprint and access token**! | Option | Description | |------
-----------|--------------------------------------------------------------------
--------------| | fingerprint | The fingerprint of the ONYX.CENTER. | |
-access_token | The permanent access token. | | client_session | The initialized
-`aiohttp.ClientSession`. (Default: `None`, create new session.) | ### Access
-Control Helper The method `onyx_client.authorizer.exchange_code` takes the
-**API code** and performs the exchange to a **fingerprint and access token**.
-Please follow the **aforementioned documentation** to retrieve the code. ##
-Usage You can **instantiate** the client using the `onyx_client.client.create`
-method like: ```python import aiohttp from onyx_client.client import create
-from onyx_client.authorizer import exchange_code # by providing the fingerprint
-and access token only client = create(fingerprint="fingerprint",
+actions/workflow/status/muhlba91/onyx-client/release.yml?style=for-the-badge)]
+(https://github.com/muhlba91/onyx-client/actions/workflows/release.yml) [![]
+(https://img.shields.io/coveralls/github/muhlba91/onyx-client?style=for-the-
+badge)](https://github.com/muhlba91/onyx-client/) [![](https://img.shields.io/
+pypi/pyversions/onyx-client?style=for-the-badge)](https://pypi.org/project/
+onyx-client/) [![](https://img.shields.io/pypi/v/onyx-client?style=for-the-
+badge)](https://pypi.org/project/onyx-client/) [![](https://img.shields.io/
+github/release-date/muhlba91/onyx-client?style=for-the-badge)](https://
+github.com/muhlba91/onyx-client/releases) [![](https://img.shields.io/pypi/dm/
+onyx-client?style=for-the-badge)](https://pypi.org/project/onyx-client/) [!
+[Known Vulnerabilities](https://snyk.io/test/github/muhlba91/onyx-client/
+badge.svg)](https://snyk.io/test/github/muhlba91/onyx-client/) [Buy_Me_A
+Coffee] This repository contains a **Python HTTP client** for [Hella](https://
+www.hella.info)' s [ONYX.CENTER API](https://github.com/hella-info/onyx_api). -
+-- ## API Versions It is encouraged to always update Hella devices to the
+latest software. This will, mostly, also enforce using the newest API. In below
+table you can find an indication of what Hella API version is supported. |
+Hella API Version | Client Version | |-------------------|-------------------
+| | v3 | >= 3.1.0 | | v2 | >= 2.5.0 < 3.0.0 | ## Installation The package is
+published in **(Test)PyPi** and can be installed via: ```bash pip install onyx-
+client ``` ## Configuration The configuration defines **connection properties**
+as a `dict` for the application running. **Attention**: make sure to **read**
+the [Onyx API Access Control](https://github.com/hella-info/onyx_api#access-
+control) description to **retrieve the fingerprint and access token**! | Option
+| Description | |----------------|---------------------------------------------
+------------------------------------| | fingerprint | The fingerprint of the
+ONYX.CENTER. | | access_token | The permanent access token. | | client_session
+| The initialized `aiohttp.ClientSession`. (Default: `None`, create new
+session.) | ### Access Control Helper The method
+`onyx_client.authorizer.exchange_code` takes the **API code** and performs the
+exchange to a **fingerprint and access token**. Please follow the
+**aforementioned documentation** to retrieve the code. ## Usage You can
+**instantiate** the client using the `onyx_client.client.create` method like:
+```python import aiohttp from onyx_client.client import create from
+onyx_client.authorizer import exchange_code # by providing the fingerprint and
+access token only client = create(fingerprint="fingerprint",
 access_token="access_token") # by providing the fingerprint, access token and
 aiohttp client session client = create(fingerprint="fingerprint",
 access_token="access_token", client_session=aiohttp.ClientSession()) # by
 providing the configuration object client_session = aiohttp.ClientSession() #
 e.g. by exchanging the code first config = exchange_code("code",
 client_session) client = create(config=config, client_session=client_session)
 if client_session is not None else None ``` An **example** is shown in the
 **`examples` directory**. --- ## Development The project uses [poetry](https://
 poetry.eustace.io/) and to install all dependencies and the build environment,
-run: ```bash $ pip install poetry $ poetry install ``` ### Testing 1) Install
-all dependencies as shown above. 2) Run `pytest` by: ```bash $ poetry run
-pytest # or $ pytest ``` ### Linting and Code Style The project uses
-[flakehell](https://github.com/life4/flakehell) as a wrapper for flake8, and
-[black](https://github.com/psf/black) for automated code style fixing, also
-using [pre-commit](https://pre-commit.com/). 1) Install all dependencies as
-shown above. 2) (Optional) Install pre-commit hooks: ```bash $ poetry run pre-
-commit install ``` 3) Run black: ```bash $ poetry run black . ``` 4) Run
-flakehell: ```bash $ poetry run flakehell lint ``` ### Building This package
-uses [poetry-dynamic-versioning](https://github.com/mtkennerly/poetry-dynamic-
-versioning) which infers the version number based on the Git tags. Hence, to
-have a proper versioning for the distribution, use Python's build system like:
-```bash $ pip install build $ python -m build ``` Your distribution will be in
-the `dist` directory. ### Commit Message This project follows [Conventional
-Commits](https://www.conventionalcommits.org/), and your commit message must
-also adhere to the additional rules outlined in `.conform.yaml`. --- ## Release
-To draft a release, use [standard-version](https://github.com/conventional-
-changelog/standard-version): ```bash $ standard-version # alternatively $ npx
-standard-version ``` Finally, push with tags: ```bash $ git push --follow-tags
+run: ```bash pip install poetry poetry install ``` ### Testing 1) Install all
+dependencies as shown above. 2) Run `pytest` by: ```bash poetry run pytest # or
+pytest ``` ### Linting and Code Style The project uses [flakehell](https://
+github.com/life4/flakehell) as a wrapper for flake8, and [black](https://
+github.com/psf/black) for automated code style fixing, also using [pre-commit]
+(https://pre-commit.com/). 1) Install all dependencies as shown above. 2)
+(Optional) Install pre-commit hooks: ```bash poetry run pre-commit install ```
+3) Run black: ```bash poetry run black . ``` 4) Run flakehell: ```bash poetry
+run flakehell lint ``` ### Building This package uses [poetry-dynamic-
+versioning](https://github.com/mtkennerly/poetry-dynamic-versioning) which
+infers the version number based on the Git tags. Hence, to have a proper
+versioning for the distribution, use Python's build system like: ```bash pip
+install build python -m build ``` Your distribution will be in the `dist`
+directory. ### Commit Message This project follows [Conventional Commits]
+(https://www.conventionalcommits.org/), and your commit message must also
+adhere to the additional rules outlined in `.conform.yaml`. --- ## Release To
+draft a release, use [standard-version](https://github.com/conventional-
+changelog/standard-version): ```bash standard-version # alternatively npx
+standard-version ``` Finally, push with tags: ```bash git push --follow-tags
 ``` --- ## Contributions Please feel free to contribute, be it with Issues or
 Pull Requests! Please read the [Contribution guidelines](CONTRIBUTING.md) ##
 Supporting If you enjoy the application and want to support my efforts, please
 feel free to buy me a coffe. :) [Buy_Me_A_Coffee]
```

### Comparing `onyx_client-6.0.0/onyx_client/authorizer/__init__.py` & `onyx_client-6.1.0/onyx_client/authorizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/client.py` & `onyx_client-6.1.0/onyx_client/client.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/data/animation_keyframe.py` & `onyx_client-6.1.0/onyx_client/data/animation_keyframe.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/data/animation_value.py` & `onyx_client-6.1.0/onyx_client/data/animation_value.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/data/boolean_value.py` & `onyx_client-6.1.0/onyx_client/data/boolean_value.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/data/device_command.py` & `onyx_client-6.1.0/onyx_client/data/device_command.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/data/numeric_value.py` & `onyx_client-6.1.0/onyx_client/data/numeric_value.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/device/click.py` & `onyx_client-6.1.0/onyx_client/device/click.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/device/device.py` & `onyx_client-6.1.0/onyx_client/device/device.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/device/light.py` & `onyx_client-6.1.0/onyx_client/device/light.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/device/shutter.py` & `onyx_client-6.1.0/onyx_client/device/shutter.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/device/switch.py` & `onyx_client-6.1.0/onyx_client/device/switch.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/device/weather.py` & `onyx_client-6.1.0/onyx_client/device/weather.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/enum/action.py` & `onyx_client-6.1.0/onyx_client/enum/action.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/enum/device_type.py` & `onyx_client-6.1.0/onyx_client/enum/device_type.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/helpers/url.py` & `onyx_client-6.1.0/onyx_client/helpers/url.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/utils/device_type.py` & `onyx_client-6.1.0/onyx_client/utils/device_type.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/utils/mapper.py` & `onyx_client-6.1.0/onyx_client/utils/mapper.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/onyx_client/utils/response.py` & `onyx_client-6.1.0/onyx_client/utils/response.py`

 * *Files identical despite different names*

### Comparing `onyx_client-6.0.0/pyproject.toml` & `onyx_client-6.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "poetry>=1.4.0",
     "poetry-dynamic-versioning>=0.21.4"
 ]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "onyx-client"
-version = "6.0.0"
+version = "6.1.0"
 description = "HTTP Client for Hella's ONYX.CENTER API."
 license = "MIT"
 authors = [
     "Daniel Muehlbachler-Pietrzykowski <daniel.muehlbachler@niftyside.io>"
 ]
 readme = "README.md"
 repository = "https://github.com/muhlba91/onyx-client"
@@ -36,15 +36,15 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 pytest-cov = { extras = ["toml"], version = "^4.0.0" }
 flakeheaven = "^3.2.1"
 coverage = { extras = ["toml"], version = "^6.5.0" }
 black = "^23.1.0"
 pre-commit = "^3.1.1"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = "^0.21.0"
 aioresponses = "^0.7.4"
 coveralls = "^3.3.1"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
```

### Comparing `onyx_client-6.0.0/PKG-INFO` & `onyx_client-6.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: onyx-client
-Version: 6.0.0
+Version: 6.1.0
 Summary: HTTP Client for Hella's ONYX.CENTER API.
 Home-page: https://github.com/muhlba91/onyx-client
 License: MIT
 Keywords: hella-info,onyx,onyx-center
 Author: Daniel Muehlbachler-Pietrzykowski
 Author-email: daniel.muehlbachler@niftyside.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Project-URL: Repository, https://github.com/muhlba91/onyx-client
 Description-Content-Type: text/markdown
 
 # Onyx Client
 
 [![](https://img.shields.io/github/license/muhlba91/onyx-client?style=for-the-badge)](LICENSE)
-[![](https://img.shields.io/github/workflow/status/muhlba91/onyx-client/Python%20package?style=for-the-badge)](https://github.com/muhlba91/onyx-client/actions)
+[![](https://img.shields.io/github/actions/workflow/status/muhlba91/onyx-client/release.yml?style=for-the-badge)](https://github.com/muhlba91/onyx-client/actions/workflows/release.yml)
 [![](https://img.shields.io/coveralls/github/muhlba91/onyx-client?style=for-the-badge)](https://github.com/muhlba91/onyx-client/)
 [![](https://img.shields.io/pypi/pyversions/onyx-client?style=for-the-badge)](https://pypi.org/project/onyx-client/)
 [![](https://img.shields.io/pypi/v/onyx-client?style=for-the-badge)](https://pypi.org/project/onyx-client/)
 [![](https://img.shields.io/github/release-date/muhlba91/onyx-client?style=for-the-badge)](https://github.com/muhlba91/onyx-client/releases)
 [![](https://img.shields.io/pypi/dm/onyx-client?style=for-the-badge)](https://pypi.org/project/onyx-client/)
 [![Known Vulnerabilities](https://snyk.io/test/github/muhlba91/onyx-client/badge.svg)](https://snyk.io/test/github/muhlba91/onyx-client/)
 <a href="https://www.buymeacoffee.com/muhlba91" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="28" width="150"></a>
@@ -41,16 +40,16 @@
 ## API Versions
 
 It is encouraged to always update Hella devices to the latest software. This will, mostly, also enforce using the newest
 API. In below table you can find an indication of what Hella API version is supported.
 
 | Hella API Version | Client Version    |
 |-------------------|-------------------|
-| v3                | > = 3.1.0 < 6.0.0 |
-| v2                | > = 2.5.0 < 3.0.0 |
+| v3                | >= 3.1.0          |
+| v2                | >= 2.5.0 < 3.0.0  |
 
 ## Installation
 
 The package is published in **(Test)PyPi** and can be installed via:
 
 ```bash
 pip install onyx-client
@@ -102,63 +101,63 @@
 ---
 
 ## Development
 
 The project uses [poetry](https://poetry.eustace.io/) and to install all dependencies and the build environment, run:
 
 ```bash
-$ pip install poetry
-$ poetry install
+pip install poetry
+poetry install
 ```
 
 ### Testing
 
 1) Install all dependencies as shown above.
 2) Run `pytest` by:
 
 ```bash
-$ poetry run pytest
+poetry run pytest
 # or
-$ pytest
+pytest
 ```
 
 ### Linting and Code Style
 
 The project uses [flakehell](https://github.com/life4/flakehell) as a wrapper for flake8,
 and [black](https://github.com/psf/black) for automated code style fixing, also
 using [pre-commit](https://pre-commit.com/).
 
 1) Install all dependencies as shown above.
 2) (Optional) Install pre-commit hooks:
 
 ```bash
-$ poetry run pre-commit install
+poetry run pre-commit install
 ```
 
 3) Run black:
 
 ```bash
-$ poetry run black .
+poetry run black .
 ```
 
 4) Run flakehell:
 
 ```bash
-$ poetry run flakehell lint
+poetry run flakehell lint
 ```
 
 ### Building
 
 This package uses [poetry-dynamic-versioning](https://github.com/mtkennerly/poetry-dynamic-versioning) which infers the
 version number based on the Git tags. Hence, to have a proper versioning for the distribution, use Python's build system
 like:
 
 ```bash
-$ pip install build
-$ python -m build
+pip install build
+python -m build
 ```
 
 Your distribution will be in the `dist` directory.
 
 ### Commit Message
 
 This project follows [Conventional Commits](https://www.conventionalcommits.org/), and your commit message must also
@@ -167,23 +166,23 @@
 ---
 
 ## Release
 
 To draft a release, use [standard-version](https://github.com/conventional-changelog/standard-version):
 
 ```bash
-$ standard-version
+standard-version
 # alternatively
-$ npx standard-version
+npx standard-version
 ```
 
 Finally, push with tags:
 
 ```bash
-$ git push --follow-tags
+git push --follow-tags
 ```
 
 ---
 
 ## Contributions
 
 Please feel free to contribute, be it with Issues or Pull Requests! Please read
```

#### html2text {}

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 2.1 Name: onyx-client Version: 6.0.0 Summary: HTTP Client for
+Metadata-Version: 2.1 Name: onyx-client Version: 6.1.0 Summary: HTTP Client for
 Hella's ONYX.CENTER API. Home-page: https://github.com/muhlba91/onyx-client
 License: MIT Keywords: hella-info,onyx,onyx-center Author: Daniel Muehlbachler-
 Pietrzykowski Author-email: daniel.muehlbachler@niftyside.io Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3 Classifier: Topic :: Home Automation Requires-Dist:
-aiohttp (>=3.8.4,<4.0.0) Project-URL: Repository, https://github.com/muhlba91/
-onyx-client Description-Content-Type: text/markdown # Onyx Client [![](https://
-img.shields.io/github/license/muhlba91/onyx-client?style=for-the-badge)]
-(LICENSE) [![](https://img.shields.io/github/workflow/status/muhlba91/onyx-
-client/Python%20package?style=for-the-badge)](https://github.com/muhlba91/onyx-
-client/actions) [![](https://img.shields.io/coveralls/github/muhlba91/onyx-
-client?style=for-the-badge)](https://github.com/muhlba91/onyx-client/) [![]
-(https://img.shields.io/pypi/pyversions/onyx-client?style=for-the-badge)]
-(https://pypi.org/project/onyx-client/) [![](https://img.shields.io/pypi/v/
-onyx-client?style=for-the-badge)](https://pypi.org/project/onyx-client/) [![]
-(https://img.shields.io/github/release-date/muhlba91/onyx-client?style=for-the-
-badge)](https://github.com/muhlba91/onyx-client/releases) [![](https://
-img.shields.io/pypi/dm/onyx-client?style=for-the-badge)](https://pypi.org/
-project/onyx-client/) [![Known Vulnerabilities](https://snyk.io/test/github/
-muhlba91/onyx-client/badge.svg)](https://snyk.io/test/github/muhlba91/onyx-
-client/) [Buy_Me_A_Coffee] This repository contains a **Python HTTP client**
-for [Hella](https://www.hella.info)' s [ONYX.CENTER API](https://github.com/
-hella-info/onyx_api). --- ## API Versions It is encouraged to always update
-Hella devices to the latest software. This will, mostly, also enforce using the
-newest API. In below table you can find an indication of what Hella API version
-is supported. | Hella API Version | Client Version | |-------------------|-----
---------------| | v3 | > = 3.1.0 < 6.0.0 | | v2 | > = 2.5.0 < 3.0.0 | ##
-Installation The package is published in **(Test)PyPi** and can be installed
-via: ```bash pip install onyx-client ``` ## Configuration The configuration
-defines **connection properties** as a `dict` for the application running.
-**Attention**: make sure to **read** the [Onyx API Access Control](https://
-github.com/hella-info/onyx_api#access-control) description to **retrieve the
-fingerprint and access token**! | Option | Description | |----------------|----
------------------------------------------------------------------------------
-| | fingerprint | The fingerprint of the ONYX.CENTER. | | access_token | The
-permanent access token. | | client_session | The initialized
-`aiohttp.ClientSession`. (Default: `None`, create new session.) | ### Access
-Control Helper The method `onyx_client.authorizer.exchange_code` takes the
-**API code** and performs the exchange to a **fingerprint and access token**.
-Please follow the **aforementioned documentation** to retrieve the code. ##
-Usage You can **instantiate** the client using the `onyx_client.client.create`
-method like: ```python import aiohttp from onyx_client.client import create
-from onyx_client.authorizer import exchange_code # by providing the fingerprint
-and access token only client = create(fingerprint="fingerprint",
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic :: Home
+Automation Requires-Dist: aiohttp (>=3.8.4,<4.0.0) Project-URL: Repository,
+https://github.com/muhlba91/onyx-client Description-Content-Type: text/markdown
+# Onyx Client [![](https://img.shields.io/github/license/muhlba91/onyx-
+client?style=for-the-badge)](LICENSE) [![](https://img.shields.io/github/
+actions/workflow/status/muhlba91/onyx-client/release.yml?style=for-the-badge)]
+(https://github.com/muhlba91/onyx-client/actions/workflows/release.yml) [![]
+(https://img.shields.io/coveralls/github/muhlba91/onyx-client?style=for-the-
+badge)](https://github.com/muhlba91/onyx-client/) [![](https://img.shields.io/
+pypi/pyversions/onyx-client?style=for-the-badge)](https://pypi.org/project/
+onyx-client/) [![](https://img.shields.io/pypi/v/onyx-client?style=for-the-
+badge)](https://pypi.org/project/onyx-client/) [![](https://img.shields.io/
+github/release-date/muhlba91/onyx-client?style=for-the-badge)](https://
+github.com/muhlba91/onyx-client/releases) [![](https://img.shields.io/pypi/dm/
+onyx-client?style=for-the-badge)](https://pypi.org/project/onyx-client/) [!
+[Known Vulnerabilities](https://snyk.io/test/github/muhlba91/onyx-client/
+badge.svg)](https://snyk.io/test/github/muhlba91/onyx-client/) [Buy_Me_A
+Coffee] This repository contains a **Python HTTP client** for [Hella](https://
+www.hella.info)' s [ONYX.CENTER API](https://github.com/hella-info/onyx_api). -
+-- ## API Versions It is encouraged to always update Hella devices to the
+latest software. This will, mostly, also enforce using the newest API. In below
+table you can find an indication of what Hella API version is supported. |
+Hella API Version | Client Version | |-------------------|-------------------
+| | v3 | >= 3.1.0 | | v2 | >= 2.5.0 < 3.0.0 | ## Installation The package is
+published in **(Test)PyPi** and can be installed via: ```bash pip install onyx-
+client ``` ## Configuration The configuration defines **connection properties**
+as a `dict` for the application running. **Attention**: make sure to **read**
+the [Onyx API Access Control](https://github.com/hella-info/onyx_api#access-
+control) description to **retrieve the fingerprint and access token**! | Option
+| Description | |----------------|---------------------------------------------
+------------------------------------| | fingerprint | The fingerprint of the
+ONYX.CENTER. | | access_token | The permanent access token. | | client_session
+| The initialized `aiohttp.ClientSession`. (Default: `None`, create new
+session.) | ### Access Control Helper The method
+`onyx_client.authorizer.exchange_code` takes the **API code** and performs the
+exchange to a **fingerprint and access token**. Please follow the
+**aforementioned documentation** to retrieve the code. ## Usage You can
+**instantiate** the client using the `onyx_client.client.create` method like:
+```python import aiohttp from onyx_client.client import create from
+onyx_client.authorizer import exchange_code # by providing the fingerprint and
+access token only client = create(fingerprint="fingerprint",
 access_token="access_token") # by providing the fingerprint, access token and
 aiohttp client session client = create(fingerprint="fingerprint",
 access_token="access_token", client_session=aiohttp.ClientSession()) # by
 providing the configuration object client_session = aiohttp.ClientSession() #
 e.g. by exchanging the code first config = exchange_code("code",
 client_session) client = create(config=config, client_session=client_session)
 if client_session is not None else None ``` An **example** is shown in the
 **`examples` directory**. --- ## Development The project uses [poetry](https://
 poetry.eustace.io/) and to install all dependencies and the build environment,
-run: ```bash $ pip install poetry $ poetry install ``` ### Testing 1) Install
-all dependencies as shown above. 2) Run `pytest` by: ```bash $ poetry run
-pytest # or $ pytest ``` ### Linting and Code Style The project uses
-[flakehell](https://github.com/life4/flakehell) as a wrapper for flake8, and
-[black](https://github.com/psf/black) for automated code style fixing, also
-using [pre-commit](https://pre-commit.com/). 1) Install all dependencies as
-shown above. 2) (Optional) Install pre-commit hooks: ```bash $ poetry run pre-
-commit install ``` 3) Run black: ```bash $ poetry run black . ``` 4) Run
-flakehell: ```bash $ poetry run flakehell lint ``` ### Building This package
-uses [poetry-dynamic-versioning](https://github.com/mtkennerly/poetry-dynamic-
-versioning) which infers the version number based on the Git tags. Hence, to
-have a proper versioning for the distribution, use Python's build system like:
-```bash $ pip install build $ python -m build ``` Your distribution will be in
-the `dist` directory. ### Commit Message This project follows [Conventional
-Commits](https://www.conventionalcommits.org/), and your commit message must
-also adhere to the additional rules outlined in `.conform.yaml`. --- ## Release
-To draft a release, use [standard-version](https://github.com/conventional-
-changelog/standard-version): ```bash $ standard-version # alternatively $ npx
-standard-version ``` Finally, push with tags: ```bash $ git push --follow-tags
+run: ```bash pip install poetry poetry install ``` ### Testing 1) Install all
+dependencies as shown above. 2) Run `pytest` by: ```bash poetry run pytest # or
+pytest ``` ### Linting and Code Style The project uses [flakehell](https://
+github.com/life4/flakehell) as a wrapper for flake8, and [black](https://
+github.com/psf/black) for automated code style fixing, also using [pre-commit]
+(https://pre-commit.com/). 1) Install all dependencies as shown above. 2)
+(Optional) Install pre-commit hooks: ```bash poetry run pre-commit install ```
+3) Run black: ```bash poetry run black . ``` 4) Run flakehell: ```bash poetry
+run flakehell lint ``` ### Building This package uses [poetry-dynamic-
+versioning](https://github.com/mtkennerly/poetry-dynamic-versioning) which
+infers the version number based on the Git tags. Hence, to have a proper
+versioning for the distribution, use Python's build system like: ```bash pip
+install build python -m build ``` Your distribution will be in the `dist`
+directory. ### Commit Message This project follows [Conventional Commits]
+(https://www.conventionalcommits.org/), and your commit message must also
+adhere to the additional rules outlined in `.conform.yaml`. --- ## Release To
+draft a release, use [standard-version](https://github.com/conventional-
+changelog/standard-version): ```bash standard-version # alternatively npx
+standard-version ``` Finally, push with tags: ```bash git push --follow-tags
 ``` --- ## Contributions Please feel free to contribute, be it with Issues or
 Pull Requests! Please read the [Contribution guidelines](CONTRIBUTING.md) ##
 Supporting If you enjoy the application and want to support my efforts, please
 feel free to buy me a coffe. :) [Buy_Me_A_Coffee]
```

