# Comparing `tmp/tufup-0.4.9.tar.gz` & `tmp/tufup-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tufup-0.4.9.tar", last modified: Fri Feb 24 12:35:41 2023, max compression
+gzip compressed data, was "tufup-0.5.0.tar", last modified: Mon May 29 14:14:08 2023, max compression
```

## Comparing `tufup-0.4.9.tar` & `tufup-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 dvg       (1000) dvg       (1000)        0 2023-02-24 12:35:41.126883 tufup-0.4.9/
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     1063 2022-04-13 15:05:55.000000 tufup-0.4.9/LICENSE
--rw-rw-r--   0 dvg       (1000) dvg       (1000)    14481 2023-02-24 12:35:41.126883 tufup-0.4.9/PKG-INFO
--rw-rw-r--   0 dvg       (1000) dvg       (1000)    12636 2023-02-03 11:22:42.000000 tufup-0.4.9/README.md
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     1319 2023-02-03 09:51:18.000000 tufup-0.4.9/pyproject.toml
--rw-rw-r--   0 dvg       (1000) dvg       (1000)       38 2023-02-24 12:35:41.126883 tufup-0.4.9/setup.cfg
-drwxrwxr-x   0 dvg       (1000) dvg       (1000)        0 2023-02-24 12:35:41.122883 tufup-0.4.9/src/
-drwxrwxr-x   0 dvg       (1000) dvg       (1000)        0 2023-02-24 12:35:41.122883 tufup-0.4.9/src/tufup/
--rw-rw-r--   0 dvg       (1000) dvg       (1000)      857 2023-02-24 12:31:47.000000 tufup-0.4.9/src/tufup/__init__.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)      282 2022-07-08 07:14:47.000000 tufup-0.4.9/src/tufup/__main__.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)    15226 2022-11-04 20:34:30.000000 tufup-0.4.9/src/tufup/client.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     4759 2022-07-08 07:14:47.000000 tufup-0.4.9/src/tufup/common.py
-drwxrwxr-x   0 dvg       (1000) dvg       (1000)        0 2023-02-24 12:35:41.122883 tufup-0.4.9/src/tufup/repo/
--rw-rw-r--   0 dvg       (1000) dvg       (1000)    36637 2023-02-24 12:32:46.000000 tufup-0.4.9/src/tufup/repo/__init__.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)    11991 2023-02-24 12:32:46.000000 tufup-0.4.9/src/tufup/repo/cli.py
-drwxrwxr-x   0 dvg       (1000) dvg       (1000)        0 2023-02-24 12:35:41.122883 tufup-0.4.9/src/tufup/utils/
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     3623 2022-07-08 07:14:47.000000 tufup-0.4.9/src/tufup/utils/__init__.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     9479 2022-11-04 16:04:29.000000 tufup-0.4.9/src/tufup/utils/platform_specific.py
-drwxrwxr-x   0 dvg       (1000) dvg       (1000)        0 2023-02-24 12:35:41.122883 tufup-0.4.9/src/tufup.egg-info/
--rw-rw-r--   0 dvg       (1000) dvg       (1000)    14481 2023-02-24 12:35:41.000000 tufup-0.4.9/src/tufup.egg-info/PKG-INFO
--rw-rw-r--   0 dvg       (1000) dvg       (1000)      614 2023-02-24 12:35:41.000000 tufup-0.4.9/src/tufup.egg-info/SOURCES.txt
--rw-rw-r--   0 dvg       (1000) dvg       (1000)        1 2023-02-24 12:35:41.000000 tufup-0.4.9/src/tufup.egg-info/dependency_links.txt
--rw-rw-r--   0 dvg       (1000) dvg       (1000)       37 2023-02-24 12:35:41.000000 tufup-0.4.9/src/tufup.egg-info/entry_points.txt
--rw-rw-r--   0 dvg       (1000) dvg       (1000)      141 2023-02-24 12:35:41.000000 tufup-0.4.9/src/tufup.egg-info/requires.txt
--rw-rw-r--   0 dvg       (1000) dvg       (1000)        6 2023-02-24 12:35:41.000000 tufup-0.4.9/src/tufup.egg-info/top_level.txt
-drwxrwxr-x   0 dvg       (1000) dvg       (1000)        0 2023-02-24 12:35:41.122883 tufup-0.4.9/tests/
--rw-rw-r--   0 dvg       (1000) dvg       (1000)    13488 2022-07-22 12:51:12.000000 tufup-0.4.9/tests/test_client.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     7000 2022-07-08 07:14:47.000000 tufup-0.4.9/tests/test_common.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)      269 2022-11-04 16:04:29.000000 tufup-0.4.9/tests/test_package.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)    34409 2023-02-24 12:32:46.000000 tufup-0.4.9/tests/test_repo.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     9258 2023-02-24 12:32:46.000000 tufup-0.4.9/tests/test_repo_cli.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     1215 2022-07-08 07:14:47.000000 tufup-0.4.9/tests/test_tests.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     3827 2022-07-08 07:14:47.000000 tufup-0.4.9/tests/test_utils.py
--rw-rw-r--   0 dvg       (1000) dvg       (1000)     9168 2022-11-04 16:04:29.000000 tufup-0.4.9/tests/test_utils_platform_specific.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.812245 tufup-0.5.0/
+-rw-rw-rw-   0        0        0     1084 2022-03-25 16:00:29.000000 tufup-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0    14727 2023-05-29 14:14:08.812245 tufup-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12845 2023-05-29 09:58:53.000000 tufup-0.5.0/README.md
+-rw-rw-rw-   0        0        0     1366 2023-05-29 14:10:44.000000 tufup-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 14:14:08.812245 tufup-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.781003 tufup-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.796624 tufup-0.5.0/src/tufup/
+-rw-rw-rw-   0        0        0      893 2023-05-29 14:12:06.000000 tufup-0.5.0/src/tufup/__init__.py
+-rw-rw-rw-   0        0        0      292 2022-07-01 14:31:47.000000 tufup-0.5.0/src/tufup/__main__.py
+-rw-rw-rw-   0        0        0    15506 2023-05-29 14:10:44.000000 tufup-0.5.0/src/tufup/client.py
+-rw-rw-rw-   0        0        0     4907 2022-07-01 14:31:47.000000 tufup-0.5.0/src/tufup/common.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.796624 tufup-0.5.0/src/tufup/repo/
+-rw-rw-rw-   0        0        0    37645 2023-05-29 14:10:44.000000 tufup-0.5.0/src/tufup/repo/__init__.py
+-rw-rw-rw-   0        0        0    12311 2023-05-29 09:58:53.000000 tufup-0.5.0/src/tufup/repo/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.796624 tufup-0.5.0/src/tufup/utils/
+-rw-rw-rw-   0        0        0     3739 2022-11-28 08:44:28.000000 tufup-0.5.0/src/tufup/utils/__init__.py
+-rw-rw-rw-   0        0        0     9721 2022-11-18 17:21:40.000000 tufup-0.5.0/src/tufup/utils/platform_specific.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.796624 tufup-0.5.0/src/tufup.egg-info/
+-rw-rw-rw-   0        0        0    14727 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      141 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.812245 tufup-0.5.0/tests/
+-rw-rw-rw-   0        0        0    13902 2023-05-29 14:10:44.000000 tufup-0.5.0/tests/test_client.py
+-rw-rw-rw-   0        0        0     7162 2022-07-01 14:31:47.000000 tufup-0.5.0/tests/test_common.py
+-rw-rw-rw-   0        0        0      279 2022-09-26 20:49:28.000000 tufup-0.5.0/tests/test_package.py
+-rw-rw-rw-   0        0        0    35282 2023-05-29 09:58:53.000000 tufup-0.5.0/tests/test_repo.py
+-rw-rw-rw-   0        0        0     9484 2023-05-29 09:58:53.000000 tufup-0.5.0/tests/test_repo_cli.py
+-rw-rw-rw-   0        0        0     1249 2022-06-22 14:44:45.000000 tufup-0.5.0/tests/test_tests.py
+-rw-rw-rw-   0        0        0     3926 2022-11-28 08:44:28.000000 tufup-0.5.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0     9387 2022-09-29 11:58:03.000000 tufup-0.5.0/tests/test_utils_platform_specific.py
```

### Comparing `tufup-0.4.9/LICENSE` & `tufup-0.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Dennis
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Dennis
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tufup-0.4.9/PKG-INFO` & `tufup-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,246 +1,246 @@
-Metadata-Version: 2.1
-Name: tufup
-Version: 0.4.9
-Summary: Automated updates for stand-alone Python applications, built upon python-tuf.
-Author-email: dennisvang <djvg@protonmail.com>
-License: MIT License
-        
-        Copyright (c) 2022 Dennis
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: source, https://github.com/dennisvang/tufup
-Project-URL: documentation, https://tufup.readthedocs.io/en/latest/
-Project-URL: issues, https://github.com/dennisvang/tufup/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# tufup
-
-![Build](https://github.com/dennisvang/tufup/actions/workflows/python-package.yml/badge.svg)
-[![PyPI](https://img.shields.io/pypi/v/tufup)](https://pypi.org/project/tufup/)
-[![Documentation Status](https://readthedocs.org/projects/tufup/badge/?version=latest)](https://tufup.readthedocs.io/en/latest/?badge=latest)
-
-A simple software updater for stand-alone Python *applications*.
-
-## Application updates and TUF
-
-A basic update-cycle for a [self-updating application][15] could look like this: 
-
-1. the app's development team create a new release, and make it available on a server
-2. an older version of the app, out in the wild, contacts the server to check for updates
-3. the old app finds the new release, downloads it, and installs it
-4. goto 1.
-
-The principle is relatively simple, as long as you don't consider the security risks involved.
-
-Unfortunately, in the real world, [security cannot be neglected][16]: You don't want to install untrusted software on your system.
-
-So, how can we make sure our update-cycle is secure? This is where things get quite complicated.
-
-Luckily, [python-tuf][1], the reference implementation for [TUF][2] (The Update Framework) takes care of this complexity. If used properly, TUF ensures a high level of security for your update system.
-
-That's why the `tufup` package is built on top of `python-tuf`.
-
-It is highly advisable to read the [TUF documentation][11] before proceeding. 
-
-
-## Quickstart
-
-The easiest way to understand how `tufup` works is by example. A minimal example of an application that uses `tufup` can be found in the companion repository: 
-**[tufup-example][10]**
-
-The example repository shows how to integrate the `tufup` client into your app, and it shows you how to set up a `tufup` update-repository.
-
->NOTE: Although the tufup-example repository uses PyInstaller to bundle an application, `tufup` can be used with ***any*** type of application bundle, even plain python scripts.  
-
-## Questions and Issues
-
-If you have questions about `tufup`, or need help getting started, please post a question on [Stack Overflow][13], add a `tufup` tag, and we will help you there.
-
-If you encounter bugs or other problems that are likely to affect other users, please create a [new issue][14] here.
-
-## Some background
-
-The `tufup` package was inspired by [PyUpdater][3], and uses a general approach to updating that is directly based on PyUpdater's implementation.
-
-> NOTE: `tufup` is completely *independent* of PyUpdater. In fact, `tufup` was created as a replacement for PyUpdater, given the fact that [PyUpdater has been archived and is no longer maintained][17]. 
-
-However, whereas PyUpdater implements a *custom* security mechanism to ensure authenticity (and integrity) of downloaded update files, `tufup` is built on top of the security mechanisms implemented in the [python-tuf][1] package, a.k.a. `tuf`.
-By entrusting the design of security measures to the security professionals, `tufup` can focus on high-level tools.
-
-Although `tuf` supports highly complex security infrastructures, see e.g. [PEP458][5], it also offers sufficient flexibility to allow *application* developers to tailor the security level to their use case.
-For details and best practices, refer to the [tuf docs][2].
-
-Based on the intended use, the `tufup` package supports only the top-level roles offered by `tuf`. At this time we do not support delegations.
-
->NOTE: Whereas PyUpdater is tightly integrated with PyInstaller, `tufup` is completely *independent* of the type of packaging solution.
-> At its core, `tufup` simply moves bundles of files from A to B, securely, regardless of how these bundles were created. 
-> A bundle may consist of a simple python script, a PyInstaller bundle, a PEX package, or any other collection of files and folders. 
-
-## Overview
-
-Borrowing TUF terminology, we distinguish between a *repo*-side (repository) and a *client*-side (application).
-
-Below you'll find a list of the basic steps that occur in an application update cycle. 
-Steps covered by `tufup` are **highlighted**.
-
-On the *repo*-side, the app *developer*
-
-- modifies the application code
-- **creates a new application archive file and corresponding patch file**
-- **signs the resulting files cryptographically**
-- deploys these files to a server
-
-On the *client*-side, the *application*
-
-- **checks for updates**
-- **downloads update files**
-- **applies the update files (i.e. installation)**
-
-The `tuf` package is used under the hood to check for updates and download update files in a secure manner, so `tufup` can safely apply the update.
-See the [tuf docs][4] for more information.
-
-## Archives and patches
-
-*Internally*, `tufup` works with *archives* (gzipped bundles of files and folders) and *patches* (binary differences between subsequent archives).
-Each archive, except the first one, has a corresponding patch file.
-
-Archive filenames and patch filenames follow the pattern
-
-`<name>-<version><suffix>` 
-
-where `name` is a short string that may contain alphanumeric characters, underscores, and hyphens, `version` is a version string according to the [PEP440][6] specification, and `suffix` is either `'.tar.gz'` or `'.patch'`.
-
-Patches are typically smaller than archives, so the tufup *client* will always attempt to update using one or more patches.
-However, if the total amount of patch data is greater than the desired full archive file, a full update will be performed.
-
-If this sounds confusing, don't worry: it is all handled internally.
-
-## How updates are created (repo-side)
-
-When a new release of your application is ready, the following steps need to be taken to enable clients to update to that new release:
-
-1. Create an application archive for the new release.
-2. Create a patch from the current archive to the new archive.
-3. Add hashes for the newly created archive file and patch file to the `tuf` metadata.
-4. Sign the modified `tuf` metadata files.
-5. Upload the new target files, i.e. archive and patch, and the updated metadata files, to the update server.
-
-The `tufup.repo` module and the `tufup` CLI provide convenient ways to streamline steps 1 to 4, based on the `tuf` [basic repo example][7].
-Step 5 is not covered by `tufup`, as it depends on the implementation.
-
-The signed metadata and hashes ensure both authenticity and integrity of the update files (see [tuf docs][2]).
-In order to sign the metadata, we need access to the private key files for the applicable `tuf` roles.
-
-## How updates are applied (client-side)
-
-By default, updates are applied by copying all files and folders from the latest archive to the current app installation directory.
-
-Here's what happens during the update process:
-
-- The latest archive is either downloaded in full, as described above, or it is derived from the current archive by applying one or more downloaded patches.
-- Once the latest archive is available on disk, it is decompressed to a temporary directory.
-- A default install script is then started, which copies the new files and folders from the temporary directory to the current app installation directory. On Windows, this script is started in a new process, after which the currently running process will exit.
-- Alternatively, you can specify a custom install script to do whatever you want with the new files.
-
-The default install script accepts an optional `purge_dst_dir` argument, which will cause *ALL* files and folders to be deleted from the app installation directory, before moving the new files into place.
-This is a convenient way to remove any stale files and folders from the app installation directory.
-
->**WARNING**: The `purge_dst_dir` option should *only* be used if the app is properly installed in its *own separate* directory.
-If this is not the case, for example if the app is running from the Windows `Desktop` directory, any *unrelated* files or folders in this directory will also be deleted! 
-
-## App versions and release channels
-
-When adding an application bundle to your `tufup` repository, you need to specify an app version string.
-This version string is used in the archive filename, and must be [PEP440][18] compliant (internally we use [`packaging.version.Version`][20]).
-
-The `tufup` client inspects these version strings to determine if updates are available.
-
-By default, when the `tufup` client looks for updates, it only includes final releases.
-Pre-releases are filtered out, unless you explicitly specify a "pre-release" channel.
-Refer to the [`Client.check_for_updates()`][21] method for details:
-
-> If `pre` is specified, pre-releases are included, down to the specified level. 
-> Pre-release identifiers follow the PEP440 specification, i.e. `'a'`, `'b'`, or `'rc'`, for alpha, beta, and release candidate, respectively.
-
-For example, suppose your latest final-release is `1.3.0`, and your latest pre-release is `2.0.0a3`. 
-An app in the field still has old version `1.0.0`. 
-If this app checks either the default channel, the release-candidate (`'rc'`) channel, or the beta (`'b'`) channel, it finds version `1.3.0` available.
-If the app checks the alpha channel (`'a'`), it finds `2.0.0a3`.
-
-Just to be clear: `tufup` assumes a typical linear release history without branching, so
-
-```none
-0.0 < 0.1a < 0.1b < 0.1rc < 0.1rc0 < 0.1rc1 < 0.1 < ...
-```
-
-## Migrating from other update frameworks
-
-Here's one way to migrate from another update framework, such as `pyupdater`, to `tufup`:
-
-1. Add `tufup` to your main application environment as a core dependency, and move `pyupdater` from core dependencies to development dependencies.
-2. Replace all `pyupdater` client code (and configuration) in your application by the `tufup` client.
-3. Initialize the `tufup` repository, so the root metadata file `root.json` exists.
-4. Modify your PyInstaller `.spec` file (from PyUpdater) to ensure that the `root.json` file is included in your package.
-5. Build, package, and sign using `pyupdater`, and deploy to your server, as usual. 
-This ensures that your `pyupdater` clients currently in the field will be able to update to the new `tufup` client.
-6. From here on, new updates will be deployed using `tufup`.
-7. If you want to enable a patch update from the `pyupdater` version to the new `tufup` version, extract the latest PyUpdater archive and add the resulting bundle to the `tufup` repository. 
-8. To skip patch creation, just create a new app bundle and add that to the `tufup` repository. 
-9. BEWARE: Keep the `pyupdater` repository in place as long as necessary to allow all clients to update.
-10. From now on, build, package, sign and deploy using `tufup`, as described elsewhere in this document.
-
-## Platform support
-
-The `tufup.client` tools are aimed primarily at **Windows** and **macOS** applications, whereas the `tufup.repo` tools are platform independent, as `tufup.repo` is just a thin layer on top of `python-tuf`. 
-
-Although `tufup.client` could also be used for Linux applications, those are probably better off using native packaging solutions, or solutions such as Flatpak or Snapcraft. 
-Read the [Python packaging overview][8] for more information.
-
-Platform dependence for `tufup.client` is related to file handling and process handling during the installation procedure, as can be seen in [tufup.utils.platform_specific][12].
-A custom, platform *de*pendent, installation procedure can be specified via the optional `install` argument for the `Client.update()` method.
-
-
-
-[1]: https://github.com/theupdateframework/python-tuf
-[2]: https://theupdateframework.io/
-[3]: https://github.com/Digital-Sapphire/PyUpdater/
-[4]: https://theupdateframework.io/overview/#software-updates-101
-[5]: https://peps.python.org/pep-0458/
-[6]: https://peps.python.org/pep-0440/
-[7]: https://github.com/theupdateframework/python-tuf/blob/develop/examples/repo_example/basic_repo.py
-[8]: https://packaging.python.org/en/latest/overview/
-[9]: https://pythonhosted.org/not-so-tuf/
-[10]: https://github.com/dennisvang/tufup-example
-[11]: https://theupdateframework.io/metadata/
-[12]: https://github.com/dennisvang/tufup/blob/master/src/tufup/utils/platform_specific.py
-[13]: https://stackoverflow.com/questions/ask
-[14]: https://github.com/dennisvang/tufup/issues
-[15]: https://theupdateframework.io/overview/#software-updates-101
-[16]: https://theupdateframework.io/security/
-[17]: https://github.com/Digital-Sapphire/PyUpdater#this-is-the-end
-[18]: https://peps.python.org/pep-0440/
-[19]: https://peps.python.org/pep-0440/#public-version-identifiers
-[20]: https://packaging.pypa.io/en/stable/version.html#packaging.version.Version
-[21]: https://github.com/dennisvang/tufup/blob/master/src/tufup/client.py
+Metadata-Version: 2.1
+Name: tufup
+Version: 0.5.0
+Summary: Automated updates for stand-alone Python applications, built upon python-tuf.
+Author-email: dennisvang <djvg@protonmail.com>
+License: MIT License
+        
+        Copyright (c) 2022 Dennis
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: source, https://github.com/dennisvang/tufup
+Project-URL: documentation, https://tufup.readthedocs.io/en/latest/
+Project-URL: issues, https://github.com/dennisvang/tufup/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# tufup
+
+![Build](https://github.com/dennisvang/tufup/actions/workflows/python-package.yml/badge.svg)
+[![PyPI](https://img.shields.io/pypi/v/tufup)](https://pypi.org/project/tufup/)
+[![Documentation Status](https://readthedocs.org/projects/tufup/badge/?version=latest)](https://tufup.readthedocs.io/en/latest/?badge=latest)
+
+A simple software updater for stand-alone Python *applications*.
+
+## Application updates and TUF
+
+A basic update-cycle for a [self-updating application][15] could look like this: 
+
+1. the app's development team create a new release, and make it available on a server
+2. an older version of the app, out in the wild, contacts the server to check for updates
+3. the old app finds the new release, downloads it, and installs it
+4. goto 1.
+
+The principle is relatively simple, as long as you don't consider the security risks involved.
+
+Unfortunately, in the real world, [security cannot be neglected][16]: You don't want to install untrusted software on your system.
+
+So, how can we make sure our update-cycle is secure? This is where things get quite complicated.
+
+Luckily, [python-tuf][1], the reference implementation for [TUF][2] (The Update Framework) takes care of this complexity. If used properly, TUF ensures a high level of security for your update system.
+
+That's why the `tufup` package is built on top of `python-tuf`.
+
+It is highly advisable to read the [TUF documentation][11] before proceeding. 
+
+
+## Quickstart
+
+The easiest way to understand how `tufup` works is by example. A minimal example of an application that uses `tufup` can be found in the companion repository: 
+**[tufup-example][10]**
+
+The example repository shows how to integrate the `tufup` client into your app, and it shows you how to set up a `tufup` update-repository.
+
+>NOTE: Although the tufup-example repository uses PyInstaller to bundle an application, `tufup` can be used with ***any*** type of application bundle, even plain python scripts.  
+
+## Questions and Issues
+
+If you have questions about `tufup`, or need help getting started, please post a question on [Stack Overflow][13], add a `tufup` tag, and we will help you there.
+
+If you encounter bugs or other problems that are likely to affect other users, please create a [new issue][14] here.
+
+## Some background
+
+The `tufup` package was inspired by [PyUpdater][3], and uses a general approach to updating that is directly based on PyUpdater's implementation.
+
+> NOTE: `tufup` is completely *independent* of PyUpdater. In fact, `tufup` was created as a replacement for PyUpdater, given the fact that [PyUpdater has been archived and is no longer maintained][17]. 
+
+However, whereas PyUpdater implements a *custom* security mechanism to ensure authenticity (and integrity) of downloaded update files, `tufup` is built on top of the security mechanisms implemented in the [python-tuf][1] package, a.k.a. `tuf`.
+By entrusting the design of security measures to the security professionals, `tufup` can focus on high-level tools.
+
+Although `tuf` supports highly complex security infrastructures, see e.g. [PEP458][5], it also offers sufficient flexibility to allow *application* developers to tailor the security level to their use case.
+For details and best practices, refer to the [tuf docs][2].
+
+Based on the intended use, the `tufup` package supports only the top-level roles offered by `tuf`. At this time we do not support delegations.
+
+>NOTE: Whereas PyUpdater is tightly integrated with PyInstaller, `tufup` is completely *independent* of the type of packaging solution.
+> At its core, `tufup` simply moves bundles of files from A to B, securely, regardless of how these bundles were created. 
+> A bundle may consist of a simple python script, a PyInstaller bundle, a PEX package, or any other collection of files and folders. 
+
+## Overview
+
+Borrowing TUF terminology, we distinguish between a *repo*-side (repository) and a *client*-side (application).
+
+Below you'll find a list of the basic steps that occur in an application update cycle. 
+Steps covered by `tufup` are **highlighted**.
+
+On the *repo*-side, the app *developer*
+
+- modifies the application code
+- **creates a new application archive file and corresponding patch file**
+- **signs the resulting files cryptographically**
+- deploys these files to a server
+
+On the *client*-side, the *application*
+
+- **checks for updates**
+- **downloads update files**
+- **applies the update files (i.e. installation)**
+
+The `tuf` package is used under the hood to check for updates and download update files in a secure manner, so `tufup` can safely apply the update.
+See the [tuf docs][4] for more information.
+
+## Archives and patches
+
+*Internally*, `tufup` works with *archives* (gzipped bundles of files and folders) and *patches* (binary differences between subsequent archives).
+Each archive, except the first one, has a corresponding patch file.
+
+Archive filenames and patch filenames follow the pattern
+
+`<name>-<version><suffix>` 
+
+where `name` is a short string that may contain alphanumeric characters, underscores, and hyphens, `version` is a version string according to the [PEP440][6] specification, and `suffix` is either `'.tar.gz'` or `'.patch'`.
+
+Patches are typically smaller than archives, so the tufup *client* will always attempt to update using one or more patches.
+However, if the total amount of patch data is greater than the desired full archive file, a full update will be performed.
+
+If this sounds confusing, don't worry: it is all handled internally.
+
+## How updates are created (repo-side)
+
+When a new release of your application is ready, the following steps need to be taken to enable clients to update to that new release:
+
+1. Create an application archive for the new release.
+2. Create a patch from the current archive to the new archive.
+3. Add hashes for the newly created archive file and patch file to the `tuf` metadata.
+4. Sign the modified `tuf` metadata files.
+5. Upload the new target files, i.e. archive and patch, and the updated metadata files, to the update server.
+
+The `tufup.repo` module and the `tufup` CLI provide convenient ways to streamline steps 1 to 4, based on the `tuf` [basic repo example][7].
+Step 5 is not covered by `tufup`, as it depends on the implementation.
+
+The signed metadata and hashes ensure both authenticity and integrity of the update files (see [tuf docs][2]).
+In order to sign the metadata, we need access to the private key files for the applicable `tuf` roles.
+
+## How updates are applied (client-side)
+
+By default, updates are applied by copying all files and folders from the latest archive to the current app installation directory.
+
+Here's what happens during the update process:
+
+- The latest archive is either downloaded in full, as described above, or it is derived from the current archive by applying one or more downloaded patches.
+- Once the latest archive is available on disk, it is decompressed to a temporary directory.
+- A default install script is then started, which copies the new files and folders from the temporary directory to the current app installation directory. On Windows, this script is started in a new process, after which the currently running process will exit.
+- Alternatively, you can specify a custom install script to do whatever you want with the new files.
+
+The default install script accepts an optional `purge_dst_dir` argument, which will cause *ALL* files and folders to be deleted from the app installation directory, before moving the new files into place.
+This is a convenient way to remove any stale files and folders from the app installation directory.
+
+>**WARNING**: The `purge_dst_dir` option should *only* be used if the app is properly installed in its *own separate* directory.
+If this is not the case, for example if the app is running from the Windows `Desktop` directory, any *unrelated* files or folders in this directory will also be deleted! 
+
+## App versions and release channels
+
+When adding an application bundle to your `tufup` repository, you need to specify an app version string.
+This version string is used in the archive filename, and must be [PEP440][18] compliant (internally we use [`packaging.version.Version`][20]).
+
+The `tufup` client inspects these version strings to determine if updates are available.
+
+By default, when the `tufup` client looks for updates, it only includes final releases.
+Pre-releases are filtered out, unless you explicitly specify a "pre-release" channel.
+Refer to the [`Client.check_for_updates()`][21] method for details:
+
+> If `pre` is specified, pre-releases are included, down to the specified level. 
+> Pre-release identifiers follow the PEP440 specification, i.e. `'a'`, `'b'`, or `'rc'`, for alpha, beta, and release candidate, respectively.
+
+For example, suppose your latest final-release is `1.3.0`, and your latest pre-release is `2.0.0a3`. 
+An app in the field still has old version `1.0.0`. 
+If this app checks either the default channel, the release-candidate (`'rc'`) channel, or the beta (`'b'`) channel, it finds version `1.3.0` available.
+If the app checks the alpha channel (`'a'`), it finds `2.0.0a3`.
+
+Just to be clear: `tufup` assumes a typical linear release history without branching, so
+
+```none
+0.0 < 0.1a < 0.1b < 0.1rc < 0.1rc0 < 0.1rc1 < 0.1 < ...
+```
+
+## Migrating from other update frameworks
+
+Here's one way to migrate from another update framework, such as `pyupdater`, to `tufup`:
+
+1. Add `tufup` to your main application environment as a core dependency, and move `pyupdater` from core dependencies to development dependencies.
+2. Replace all `pyupdater` client code (and configuration) in your application by the `tufup` client.
+3. Initialize the `tufup` repository, so the root metadata file `root.json` exists.
+4. Modify your PyInstaller `.spec` file (from PyUpdater) to ensure that the `root.json` file is included in your package.
+5. Build, package, and sign using `pyupdater`, and deploy to your server, as usual. 
+This ensures that your `pyupdater` clients currently in the field will be able to update to the new `tufup` client.
+6. From here on, new updates will be deployed using `tufup`.
+7. If you want to enable a patch update from the `pyupdater` version to the new `tufup` version, extract the latest PyUpdater archive and add the resulting bundle to the `tufup` repository. 
+8. To skip patch creation, just create a new app bundle and add that to the `tufup` repository. 
+9. BEWARE: Keep the `pyupdater` repository in place as long as necessary to allow all clients to update.
+10. From now on, build, package, sign and deploy using `tufup`, as described elsewhere in this document.
+
+## Platform support
+
+The `tufup.client` tools are aimed primarily at **Windows** and **macOS** applications, whereas the `tufup.repo` tools are platform independent, as `tufup.repo` is just a thin layer on top of `python-tuf`. 
+
+Although `tufup.client` could also be used for Linux applications, those are probably better off using native packaging solutions, or solutions such as Flatpak or Snapcraft. 
+Read the [Python packaging overview][8] for more information.
+
+Platform dependence for `tufup.client` is related to file handling and process handling during the installation procedure, as can be seen in [tufup.utils.platform_specific][12].
+A custom, platform *de*pendent, installation procedure can be specified via the optional `install` argument for the `Client.update()` method.
+
+
+
+[1]: https://github.com/theupdateframework/python-tuf
+[2]: https://theupdateframework.io/
+[3]: https://github.com/Digital-Sapphire/PyUpdater/
+[4]: https://theupdateframework.io/overview/#software-updates-101
+[5]: https://peps.python.org/pep-0458/
+[6]: https://peps.python.org/pep-0440/
+[7]: https://github.com/theupdateframework/python-tuf/blob/develop/examples/repo_example/basic_repo.py
+[8]: https://packaging.python.org/en/latest/overview/
+[9]: https://pythonhosted.org/not-so-tuf/
+[10]: https://github.com/dennisvang/tufup-example
+[11]: https://theupdateframework.io/metadata/
+[12]: https://github.com/dennisvang/tufup/blob/master/src/tufup/utils/platform_specific.py
+[13]: https://stackoverflow.com/questions/ask
+[14]: https://github.com/dennisvang/tufup/issues
+[15]: https://theupdateframework.io/overview/#software-updates-101
+[16]: https://theupdateframework.io/security/
+[17]: https://github.com/Digital-Sapphire/PyUpdater#this-is-the-end
+[18]: https://peps.python.org/pep-0440/
+[19]: https://peps.python.org/pep-0440/#public-version-identifiers
+[20]: https://packaging.pypa.io/en/stable/version.html#packaging.version.Version
+[21]: https://github.com/dennisvang/tufup/blob/master/src/tufup/client.py
```

### Comparing `tufup-0.4.9/README.md` & `tufup-0.5.0/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,209 +1,209 @@
-# tufup
-
-![Build](https://github.com/dennisvang/tufup/actions/workflows/python-package.yml/badge.svg)
-[![PyPI](https://img.shields.io/pypi/v/tufup)](https://pypi.org/project/tufup/)
-[![Documentation Status](https://readthedocs.org/projects/tufup/badge/?version=latest)](https://tufup.readthedocs.io/en/latest/?badge=latest)
-
-A simple software updater for stand-alone Python *applications*.
-
-## Application updates and TUF
-
-A basic update-cycle for a [self-updating application][15] could look like this: 
-
-1. the app's development team create a new release, and make it available on a server
-2. an older version of the app, out in the wild, contacts the server to check for updates
-3. the old app finds the new release, downloads it, and installs it
-4. goto 1.
-
-The principle is relatively simple, as long as you don't consider the security risks involved.
-
-Unfortunately, in the real world, [security cannot be neglected][16]: You don't want to install untrusted software on your system.
-
-So, how can we make sure our update-cycle is secure? This is where things get quite complicated.
-
-Luckily, [python-tuf][1], the reference implementation for [TUF][2] (The Update Framework) takes care of this complexity. If used properly, TUF ensures a high level of security for your update system.
-
-That's why the `tufup` package is built on top of `python-tuf`.
-
-It is highly advisable to read the [TUF documentation][11] before proceeding. 
-
-
-## Quickstart
-
-The easiest way to understand how `tufup` works is by example. A minimal example of an application that uses `tufup` can be found in the companion repository: 
-**[tufup-example][10]**
-
-The example repository shows how to integrate the `tufup` client into your app, and it shows you how to set up a `tufup` update-repository.
-
->NOTE: Although the tufup-example repository uses PyInstaller to bundle an application, `tufup` can be used with ***any*** type of application bundle, even plain python scripts.  
-
-## Questions and Issues
-
-If you have questions about `tufup`, or need help getting started, please post a question on [Stack Overflow][13], add a `tufup` tag, and we will help you there.
-
-If you encounter bugs or other problems that are likely to affect other users, please create a [new issue][14] here.
-
-## Some background
-
-The `tufup` package was inspired by [PyUpdater][3], and uses a general approach to updating that is directly based on PyUpdater's implementation.
-
-> NOTE: `tufup` is completely *independent* of PyUpdater. In fact, `tufup` was created as a replacement for PyUpdater, given the fact that [PyUpdater has been archived and is no longer maintained][17]. 
-
-However, whereas PyUpdater implements a *custom* security mechanism to ensure authenticity (and integrity) of downloaded update files, `tufup` is built on top of the security mechanisms implemented in the [python-tuf][1] package, a.k.a. `tuf`.
-By entrusting the design of security measures to the security professionals, `tufup` can focus on high-level tools.
-
-Although `tuf` supports highly complex security infrastructures, see e.g. [PEP458][5], it also offers sufficient flexibility to allow *application* developers to tailor the security level to their use case.
-For details and best practices, refer to the [tuf docs][2].
-
-Based on the intended use, the `tufup` package supports only the top-level roles offered by `tuf`. At this time we do not support delegations.
-
->NOTE: Whereas PyUpdater is tightly integrated with PyInstaller, `tufup` is completely *independent* of the type of packaging solution.
-> At its core, `tufup` simply moves bundles of files from A to B, securely, regardless of how these bundles were created. 
-> A bundle may consist of a simple python script, a PyInstaller bundle, a PEX package, or any other collection of files and folders. 
-
-## Overview
-
-Borrowing TUF terminology, we distinguish between a *repo*-side (repository) and a *client*-side (application).
-
-Below you'll find a list of the basic steps that occur in an application update cycle. 
-Steps covered by `tufup` are **highlighted**.
-
-On the *repo*-side, the app *developer*
-
-- modifies the application code
-- **creates a new application archive file and corresponding patch file**
-- **signs the resulting files cryptographically**
-- deploys these files to a server
-
-On the *client*-side, the *application*
-
-- **checks for updates**
-- **downloads update files**
-- **applies the update files (i.e. installation)**
-
-The `tuf` package is used under the hood to check for updates and download update files in a secure manner, so `tufup` can safely apply the update.
-See the [tuf docs][4] for more information.
-
-## Archives and patches
-
-*Internally*, `tufup` works with *archives* (gzipped bundles of files and folders) and *patches* (binary differences between subsequent archives).
-Each archive, except the first one, has a corresponding patch file.
-
-Archive filenames and patch filenames follow the pattern
-
-`<name>-<version><suffix>` 
-
-where `name` is a short string that may contain alphanumeric characters, underscores, and hyphens, `version` is a version string according to the [PEP440][6] specification, and `suffix` is either `'.tar.gz'` or `'.patch'`.
-
-Patches are typically smaller than archives, so the tufup *client* will always attempt to update using one or more patches.
-However, if the total amount of patch data is greater than the desired full archive file, a full update will be performed.
-
-If this sounds confusing, don't worry: it is all handled internally.
-
-## How updates are created (repo-side)
-
-When a new release of your application is ready, the following steps need to be taken to enable clients to update to that new release:
-
-1. Create an application archive for the new release.
-2. Create a patch from the current archive to the new archive.
-3. Add hashes for the newly created archive file and patch file to the `tuf` metadata.
-4. Sign the modified `tuf` metadata files.
-5. Upload the new target files, i.e. archive and patch, and the updated metadata files, to the update server.
-
-The `tufup.repo` module and the `tufup` CLI provide convenient ways to streamline steps 1 to 4, based on the `tuf` [basic repo example][7].
-Step 5 is not covered by `tufup`, as it depends on the implementation.
-
-The signed metadata and hashes ensure both authenticity and integrity of the update files (see [tuf docs][2]).
-In order to sign the metadata, we need access to the private key files for the applicable `tuf` roles.
-
-## How updates are applied (client-side)
-
-By default, updates are applied by copying all files and folders from the latest archive to the current app installation directory.
-
-Here's what happens during the update process:
-
-- The latest archive is either downloaded in full, as described above, or it is derived from the current archive by applying one or more downloaded patches.
-- Once the latest archive is available on disk, it is decompressed to a temporary directory.
-- A default install script is then started, which copies the new files and folders from the temporary directory to the current app installation directory. On Windows, this script is started in a new process, after which the currently running process will exit.
-- Alternatively, you can specify a custom install script to do whatever you want with the new files.
-
-The default install script accepts an optional `purge_dst_dir` argument, which will cause *ALL* files and folders to be deleted from the app installation directory, before moving the new files into place.
-This is a convenient way to remove any stale files and folders from the app installation directory.
-
->**WARNING**: The `purge_dst_dir` option should *only* be used if the app is properly installed in its *own separate* directory.
-If this is not the case, for example if the app is running from the Windows `Desktop` directory, any *unrelated* files or folders in this directory will also be deleted! 
-
-## App versions and release channels
-
-When adding an application bundle to your `tufup` repository, you need to specify an app version string.
-This version string is used in the archive filename, and must be [PEP440][18] compliant (internally we use [`packaging.version.Version`][20]).
-
-The `tufup` client inspects these version strings to determine if updates are available.
-
-By default, when the `tufup` client looks for updates, it only includes final releases.
-Pre-releases are filtered out, unless you explicitly specify a "pre-release" channel.
-Refer to the [`Client.check_for_updates()`][21] method for details:
-
-> If `pre` is specified, pre-releases are included, down to the specified level. 
-> Pre-release identifiers follow the PEP440 specification, i.e. `'a'`, `'b'`, or `'rc'`, for alpha, beta, and release candidate, respectively.
-
-For example, suppose your latest final-release is `1.3.0`, and your latest pre-release is `2.0.0a3`. 
-An app in the field still has old version `1.0.0`. 
-If this app checks either the default channel, the release-candidate (`'rc'`) channel, or the beta (`'b'`) channel, it finds version `1.3.0` available.
-If the app checks the alpha channel (`'a'`), it finds `2.0.0a3`.
-
-Just to be clear: `tufup` assumes a typical linear release history without branching, so
-
-```none
-0.0 < 0.1a < 0.1b < 0.1rc < 0.1rc0 < 0.1rc1 < 0.1 < ...
-```
-
-## Migrating from other update frameworks
-
-Here's one way to migrate from another update framework, such as `pyupdater`, to `tufup`:
-
-1. Add `tufup` to your main application environment as a core dependency, and move `pyupdater` from core dependencies to development dependencies.
-2. Replace all `pyupdater` client code (and configuration) in your application by the `tufup` client.
-3. Initialize the `tufup` repository, so the root metadata file `root.json` exists.
-4. Modify your PyInstaller `.spec` file (from PyUpdater) to ensure that the `root.json` file is included in your package.
-5. Build, package, and sign using `pyupdater`, and deploy to your server, as usual. 
-This ensures that your `pyupdater` clients currently in the field will be able to update to the new `tufup` client.
-6. From here on, new updates will be deployed using `tufup`.
-7. If you want to enable a patch update from the `pyupdater` version to the new `tufup` version, extract the latest PyUpdater archive and add the resulting bundle to the `tufup` repository. 
-8. To skip patch creation, just create a new app bundle and add that to the `tufup` repository. 
-9. BEWARE: Keep the `pyupdater` repository in place as long as necessary to allow all clients to update.
-10. From now on, build, package, sign and deploy using `tufup`, as described elsewhere in this document.
-
-## Platform support
-
-The `tufup.client` tools are aimed primarily at **Windows** and **macOS** applications, whereas the `tufup.repo` tools are platform independent, as `tufup.repo` is just a thin layer on top of `python-tuf`. 
-
-Although `tufup.client` could also be used for Linux applications, those are probably better off using native packaging solutions, or solutions such as Flatpak or Snapcraft. 
-Read the [Python packaging overview][8] for more information.
-
-Platform dependence for `tufup.client` is related to file handling and process handling during the installation procedure, as can be seen in [tufup.utils.platform_specific][12].
-A custom, platform *de*pendent, installation procedure can be specified via the optional `install` argument for the `Client.update()` method.
-
-
-
-[1]: https://github.com/theupdateframework/python-tuf
-[2]: https://theupdateframework.io/
-[3]: https://github.com/Digital-Sapphire/PyUpdater/
-[4]: https://theupdateframework.io/overview/#software-updates-101
-[5]: https://peps.python.org/pep-0458/
-[6]: https://peps.python.org/pep-0440/
-[7]: https://github.com/theupdateframework/python-tuf/blob/develop/examples/repo_example/basic_repo.py
-[8]: https://packaging.python.org/en/latest/overview/
-[9]: https://pythonhosted.org/not-so-tuf/
-[10]: https://github.com/dennisvang/tufup-example
-[11]: https://theupdateframework.io/metadata/
-[12]: https://github.com/dennisvang/tufup/blob/master/src/tufup/utils/platform_specific.py
-[13]: https://stackoverflow.com/questions/ask
-[14]: https://github.com/dennisvang/tufup/issues
-[15]: https://theupdateframework.io/overview/#software-updates-101
-[16]: https://theupdateframework.io/security/
-[17]: https://github.com/Digital-Sapphire/PyUpdater#this-is-the-end
-[18]: https://peps.python.org/pep-0440/
-[19]: https://peps.python.org/pep-0440/#public-version-identifiers
-[20]: https://packaging.pypa.io/en/stable/version.html#packaging.version.Version
-[21]: https://github.com/dennisvang/tufup/blob/master/src/tufup/client.py
+# tufup
+
+![Build](https://github.com/dennisvang/tufup/actions/workflows/python-package.yml/badge.svg)
+[![PyPI](https://img.shields.io/pypi/v/tufup)](https://pypi.org/project/tufup/)
+[![Documentation Status](https://readthedocs.org/projects/tufup/badge/?version=latest)](https://tufup.readthedocs.io/en/latest/?badge=latest)
+
+A simple software updater for stand-alone Python *applications*.
+
+## Application updates and TUF
+
+A basic update-cycle for a [self-updating application][15] could look like this: 
+
+1. the app's development team create a new release, and make it available on a server
+2. an older version of the app, out in the wild, contacts the server to check for updates
+3. the old app finds the new release, downloads it, and installs it
+4. goto 1.
+
+The principle is relatively simple, as long as you don't consider the security risks involved.
+
+Unfortunately, in the real world, [security cannot be neglected][16]: You don't want to install untrusted software on your system.
+
+So, how can we make sure our update-cycle is secure? This is where things get quite complicated.
+
+Luckily, [python-tuf][1], the reference implementation for [TUF][2] (The Update Framework) takes care of this complexity. If used properly, TUF ensures a high level of security for your update system.
+
+That's why the `tufup` package is built on top of `python-tuf`.
+
+It is highly advisable to read the [TUF documentation][11] before proceeding. 
+
+
+## Quickstart
+
+The easiest way to understand how `tufup` works is by example. A minimal example of an application that uses `tufup` can be found in the companion repository: 
+**[tufup-example][10]**
+
+The example repository shows how to integrate the `tufup` client into your app, and it shows you how to set up a `tufup` update-repository.
+
+>NOTE: Although the tufup-example repository uses PyInstaller to bundle an application, `tufup` can be used with ***any*** type of application bundle, even plain python scripts.  
+
+## Questions and Issues
+
+If you have questions about `tufup`, or need help getting started, please post a question on [Stack Overflow][13], add a `tufup` tag, and we will help you there.
+
+If you encounter bugs or other problems that are likely to affect other users, please create a [new issue][14] here.
+
+## Some background
+
+The `tufup` package was inspired by [PyUpdater][3], and uses a general approach to updating that is directly based on PyUpdater's implementation.
+
+> NOTE: `tufup` is completely *independent* of PyUpdater. In fact, `tufup` was created as a replacement for PyUpdater, given the fact that [PyUpdater has been archived and is no longer maintained][17]. 
+
+However, whereas PyUpdater implements a *custom* security mechanism to ensure authenticity (and integrity) of downloaded update files, `tufup` is built on top of the security mechanisms implemented in the [python-tuf][1] package, a.k.a. `tuf`.
+By entrusting the design of security measures to the security professionals, `tufup` can focus on high-level tools.
+
+Although `tuf` supports highly complex security infrastructures, see e.g. [PEP458][5], it also offers sufficient flexibility to allow *application* developers to tailor the security level to their use case.
+For details and best practices, refer to the [tuf docs][2].
+
+Based on the intended use, the `tufup` package supports only the top-level roles offered by `tuf`. At this time we do not support delegations.
+
+>NOTE: Whereas PyUpdater is tightly integrated with PyInstaller, `tufup` is completely *independent* of the type of packaging solution.
+> At its core, `tufup` simply moves bundles of files from A to B, securely, regardless of how these bundles were created. 
+> A bundle may consist of a simple python script, a PyInstaller bundle, a PEX package, or any other collection of files and folders. 
+
+## Overview
+
+Borrowing TUF terminology, we distinguish between a *repo*-side (repository) and a *client*-side (application).
+
+Below you'll find a list of the basic steps that occur in an application update cycle. 
+Steps covered by `tufup` are **highlighted**.
+
+On the *repo*-side, the app *developer*
+
+- modifies the application code
+- **creates a new application archive file and corresponding patch file**
+- **signs the resulting files cryptographically**
+- deploys these files to a server
+
+On the *client*-side, the *application*
+
+- **checks for updates**
+- **downloads update files**
+- **applies the update files (i.e. installation)**
+
+The `tuf` package is used under the hood to check for updates and download update files in a secure manner, so `tufup` can safely apply the update.
+See the [tuf docs][4] for more information.
+
+## Archives and patches
+
+*Internally*, `tufup` works with *archives* (gzipped bundles of files and folders) and *patches* (binary differences between subsequent archives).
+Each archive, except the first one, has a corresponding patch file.
+
+Archive filenames and patch filenames follow the pattern
+
+`<name>-<version><suffix>` 
+
+where `name` is a short string that may contain alphanumeric characters, underscores, and hyphens, `version` is a version string according to the [PEP440][6] specification, and `suffix` is either `'.tar.gz'` or `'.patch'`.
+
+Patches are typically smaller than archives, so the tufup *client* will always attempt to update using one or more patches.
+However, if the total amount of patch data is greater than the desired full archive file, a full update will be performed.
+
+If this sounds confusing, don't worry: it is all handled internally.
+
+## How updates are created (repo-side)
+
+When a new release of your application is ready, the following steps need to be taken to enable clients to update to that new release:
+
+1. Create an application archive for the new release.
+2. Create a patch from the current archive to the new archive.
+3. Add hashes for the newly created archive file and patch file to the `tuf` metadata.
+4. Sign the modified `tuf` metadata files.
+5. Upload the new target files, i.e. archive and patch, and the updated metadata files, to the update server.
+
+The `tufup.repo` module and the `tufup` CLI provide convenient ways to streamline steps 1 to 4, based on the `tuf` [basic repo example][7].
+Step 5 is not covered by `tufup`, as it depends on the implementation.
+
+The signed metadata and hashes ensure both authenticity and integrity of the update files (see [tuf docs][2]).
+In order to sign the metadata, we need access to the private key files for the applicable `tuf` roles.
+
+## How updates are applied (client-side)
+
+By default, updates are applied by copying all files and folders from the latest archive to the current app installation directory.
+
+Here's what happens during the update process:
+
+- The latest archive is either downloaded in full, as described above, or it is derived from the current archive by applying one or more downloaded patches.
+- Once the latest archive is available on disk, it is decompressed to a temporary directory.
+- A default install script is then started, which copies the new files and folders from the temporary directory to the current app installation directory. On Windows, this script is started in a new process, after which the currently running process will exit.
+- Alternatively, you can specify a custom install script to do whatever you want with the new files.
+
+The default install script accepts an optional `purge_dst_dir` argument, which will cause *ALL* files and folders to be deleted from the app installation directory, before moving the new files into place.
+This is a convenient way to remove any stale files and folders from the app installation directory.
+
+>**WARNING**: The `purge_dst_dir` option should *only* be used if the app is properly installed in its *own separate* directory.
+If this is not the case, for example if the app is running from the Windows `Desktop` directory, any *unrelated* files or folders in this directory will also be deleted! 
+
+## App versions and release channels
+
+When adding an application bundle to your `tufup` repository, you need to specify an app version string.
+This version string is used in the archive filename, and must be [PEP440][18] compliant (internally we use [`packaging.version.Version`][20]).
+
+The `tufup` client inspects these version strings to determine if updates are available.
+
+By default, when the `tufup` client looks for updates, it only includes final releases.
+Pre-releases are filtered out, unless you explicitly specify a "pre-release" channel.
+Refer to the [`Client.check_for_updates()`][21] method for details:
+
+> If `pre` is specified, pre-releases are included, down to the specified level. 
+> Pre-release identifiers follow the PEP440 specification, i.e. `'a'`, `'b'`, or `'rc'`, for alpha, beta, and release candidate, respectively.
+
+For example, suppose your latest final-release is `1.3.0`, and your latest pre-release is `2.0.0a3`. 
+An app in the field still has old version `1.0.0`. 
+If this app checks either the default channel, the release-candidate (`'rc'`) channel, or the beta (`'b'`) channel, it finds version `1.3.0` available.
+If the app checks the alpha channel (`'a'`), it finds `2.0.0a3`.
+
+Just to be clear: `tufup` assumes a typical linear release history without branching, so
+
+```none
+0.0 < 0.1a < 0.1b < 0.1rc < 0.1rc0 < 0.1rc1 < 0.1 < ...
+```
+
+## Migrating from other update frameworks
+
+Here's one way to migrate from another update framework, such as `pyupdater`, to `tufup`:
+
+1. Add `tufup` to your main application environment as a core dependency, and move `pyupdater` from core dependencies to development dependencies.
+2. Replace all `pyupdater` client code (and configuration) in your application by the `tufup` client.
+3. Initialize the `tufup` repository, so the root metadata file `root.json` exists.
+4. Modify your PyInstaller `.spec` file (from PyUpdater) to ensure that the `root.json` file is included in your package.
+5. Build, package, and sign using `pyupdater`, and deploy to your server, as usual. 
+This ensures that your `pyupdater` clients currently in the field will be able to update to the new `tufup` client.
+6. From here on, new updates will be deployed using `tufup`.
+7. If you want to enable a patch update from the `pyupdater` version to the new `tufup` version, extract the latest PyUpdater archive and add the resulting bundle to the `tufup` repository. 
+8. To skip patch creation, just create a new app bundle and add that to the `tufup` repository. 
+9. BEWARE: Keep the `pyupdater` repository in place as long as necessary to allow all clients to update.
+10. From now on, build, package, sign and deploy using `tufup`, as described elsewhere in this document.
+
+## Platform support
+
+The `tufup.client` tools are aimed primarily at **Windows** and **macOS** applications, whereas the `tufup.repo` tools are platform independent, as `tufup.repo` is just a thin layer on top of `python-tuf`. 
+
+Although `tufup.client` could also be used for Linux applications, those are probably better off using native packaging solutions, or solutions such as Flatpak or Snapcraft. 
+Read the [Python packaging overview][8] for more information.
+
+Platform dependence for `tufup.client` is related to file handling and process handling during the installation procedure, as can be seen in [tufup.utils.platform_specific][12].
+A custom, platform *de*pendent, installation procedure can be specified via the optional `install` argument for the `Client.update()` method.
+
+
+
+[1]: https://github.com/theupdateframework/python-tuf
+[2]: https://theupdateframework.io/
+[3]: https://github.com/Digital-Sapphire/PyUpdater/
+[4]: https://theupdateframework.io/overview/#software-updates-101
+[5]: https://peps.python.org/pep-0458/
+[6]: https://peps.python.org/pep-0440/
+[7]: https://github.com/theupdateframework/python-tuf/blob/develop/examples/repo_example/basic_repo.py
+[8]: https://packaging.python.org/en/latest/overview/
+[9]: https://pythonhosted.org/not-so-tuf/
+[10]: https://github.com/dennisvang/tufup-example
+[11]: https://theupdateframework.io/metadata/
+[12]: https://github.com/dennisvang/tufup/blob/master/src/tufup/utils/platform_specific.py
+[13]: https://stackoverflow.com/questions/ask
+[14]: https://github.com/dennisvang/tufup/issues
+[15]: https://theupdateframework.io/overview/#software-updates-101
+[16]: https://theupdateframework.io/security/
+[17]: https://github.com/Digital-Sapphire/PyUpdater#this-is-the-end
+[18]: https://peps.python.org/pep-0440/
+[19]: https://peps.python.org/pep-0440/#public-version-identifiers
+[20]: https://packaging.pypa.io/en/stable/version.html#packaging.version.Version
+[21]: https://github.com/dennisvang/tufup/blob/master/src/tufup/client.py
```

### Comparing `tufup-0.4.9/src/tufup/__init__.py` & `tufup-0.5.0/src/tufup/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import logging
-import sys
-
-from tufup.repo import cli
-from tufup.utils import input_bool
-
-# https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
-# https://semver.org/
-__version__ = '0.4.9'
-
-logger = logging.getLogger(__name__)
-
-
-def main(args=None):
-    print(f'tufup version: {__version__}')
-    # default to --help
-    if args is None:
-        args = sys.argv[1:] or ['--help']
-
-    # parse command line arguments
-    options = cli.get_parser().parse_args(args=args)
-
-    # cli debugging
-    if options.debug:
-        logging.basicConfig(level=logging.DEBUG, stream=sys.stdout, force=True)
-
-    # process command
-    try:
-        options.func(options)
-    except Exception:  # noqa
-        logger.exception(f'Failed to process command: {args}')
-
-
-if __name__ == '__main__':
-    logging.basicConfig(level=logging.INFO)
-    main()
+import logging
+import sys
+
+from tufup.repo import cli
+from tufup.utils import input_bool
+
+# https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
+# https://semver.org/
+__version__ = '0.5.0'
+
+logger = logging.getLogger(__name__)
+
+
+def main(args=None):
+    print(f'tufup version: {__version__}')
+    # default to --help
+    if args is None:
+        args = sys.argv[1:] or ['--help']
+
+    # parse command line arguments
+    options = cli.get_parser().parse_args(args=args)
+
+    # cli debugging
+    if options.debug:
+        logging.basicConfig(level=logging.DEBUG, stream=sys.stdout, force=True)
+
+    # process command
+    try:
+        options.func(options)
+    except Exception:  # noqa
+        logger.exception(f'Failed to process command: {args}')
+
+
+if __name__ == '__main__':
+    logging.basicConfig(level=logging.INFO)
+    main()
```

### Comparing `tufup-0.4.9/src/tufup/client.py` & `tufup-0.5.0/src/tufup/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,360 +1,358 @@
-import bsdiff4
-import logging
-import pathlib
-import shutil
-import sys
-import tempfile
-from typing import Callable, Dict, Iterator, List, Optional, Tuple, Union
-from urllib import parse
-
-import requests
-from requests.auth import AuthBase
-from tuf.api.exceptions import DownloadError, UnsignedMetadataError
-from tuf.api.metadata import TargetFile
-import tuf.ngclient
-# RequestsFetcher is "private", but we'll just have to live with that, for now.
-from tuf.ngclient._internal.requests_fetcher import RequestsFetcher  # noqa
-
-from tufup.common import TargetMeta
-from tufup.utils.platform_specific import install_update
-
-logger = logging.getLogger(__name__)
-
-DEFAULT_EXTRACT_DIR = pathlib.Path(tempfile.gettempdir()) / 'tufup'
-
-
-class Client(tuf.ngclient.Updater):
-    def __init__(
-            self,
-            app_name: str,
-            app_install_dir: pathlib.Path,
-            current_version: str,
-            metadata_dir: pathlib.Path,
-            metadata_base_url: str,
-            target_dir: pathlib.Path,
-            target_base_url: str,
-            extract_dir: Optional[pathlib.Path] = None,
-            refresh_required: bool = False,
-            session_auth: Optional[Dict[str, Union[Tuple[str, str], AuthBase]]] = None,
-            **kwargs,
-    ):
-        # tuf.ngclient.Updater.__init__ loads local root metadata automatically
-        super().__init__(
-            metadata_dir=str(metadata_dir),
-            metadata_base_url=metadata_base_url,
-            target_dir=str(target_dir),
-            target_base_url=target_base_url,
-            fetcher=AuthRequestsFetcher(session_auth=session_auth),
-            **kwargs,
-        )
-        self.app_install_dir = app_install_dir
-        self.extract_dir = extract_dir
-        self.refresh_required = refresh_required
-        self.current_archive = TargetMeta(name=app_name, version=current_version)
-        self.current_archive_local_path = target_dir / self.current_archive.path
-        self.new_archive_local_path: Optional[pathlib.Path] = None
-        self.new_archive_info: Optional[TargetFile] = None
-        self.new_targets: Optional[dict] = None
-        self.downloaded_target_files = {}
-
-    @property
-    def trusted_target_metas(self) -> list:
-        """
-        Return a list of available trusted targets, as TargetMeta objects.
-
-        This is convenient because TargetMeta objects can be sorted by version.
-        """
-        # todo: _trusted_set is private, but ideally we would use a public
-        #  interface (if only tuf.ngclient exposed one...)
-        _trusted_target_metas = []
-        if self._trusted_set.targets:
-            _trusted_target_metas = [
-                TargetMeta(target_path=key)
-                for key in self._trusted_set.targets.signed.targets.keys()
-            ]
-            logger.debug(f'{len(_trusted_target_metas)} TargetMeta objects created')
-        else:
-            logger.warning('targets metadata not found')
-        return _trusted_target_metas
-
-    def get_targetinfo(self, target_path: Union[str, TargetMeta]) -> Optional[TargetFile]:
-        """Extend Updater.get_targetinfo to handle TargetMeta input args."""
-        if isinstance(target_path, TargetMeta):
-            target_path = target_path.target_path_str
-        return super().get_targetinfo(target_path=target_path)
-
-    @property
-    def updates_available(self):
-        if self.new_targets is None:
-            logger.warning('Please call check_for_updates first.')
-            return False
-        else:
-            return len(self.new_targets) > 0
-
-    def download_and_apply_update(
-            self,
-            skip_confirmation: bool = False,
-            install: Optional[Callable] = None,
-            progress_hook: Optional[Callable] = None,
-            **kwargs,
-    ):
-        """
-        Download and apply available updates.
-
-        Note that `check_for_updates` must be called first.
-
-        This downloads the files found by `check_for_updates`, applies any
-        patches, and extracts the resulting archive to the `extract_dir`. At
-        that point, the update is ready to be installed (i.e. moved into
-        place). This is done by calling `install` with the specified `**kwargs`.
-
-        The default `install` callable moves the content of `extract_dir` to
-        `app_install_dir`, and exits the application (not necessarily in that
-        order).
-
-        The **kwargs are passed on to the 'install' callable
-
-        The default `install` callable accepts two additional arguments:
-
-            `purge_dst_dir` (default False): if True, *ALL* content will be
-            deleted from the `app_install_dir`
-
-            `exclude_from_purge` (default None): list of paths to exclude
-            from purge
-
-            **DANGER**: Only set `purge_dst_dir=True` if your app is
-            installed in its own separate directory, otherwise this will
-            cause unrelated files and folders to be deleted.
-        """
-        if install is None:
-            install = install_update
-        if self.updates_available and self._download_updates(
-                progress_hook=progress_hook
-        ):
-            self._apply_updates(
-                install=install, skip_confirmation=skip_confirmation, **kwargs
-            )
-
-    def check_for_updates(
-            self, pre: Optional[str] = None, patch: bool = True
-    ) -> Optional[TargetMeta]:
-        """
-        Check if any updates are available, based on current app version.
-
-        Returns latest archive meta, if a new archive is found.
-
-        Final releases are always included. Pre-releases are excluded by
-        default. If `pre` is specified, pre-releases are included, down to
-        the specified level. Pre-release identifiers follow the PEP440
-        specification, i.e. 'a', 'b', or 'rc', for alpha, beta, and release
-        candidate, respectively.
-
-        If `patch` is `False`, a full update is enforced.
-        """
-        included = {None: '', '': '', 'a': 'abrc', 'b': 'brc', 'rc': 'rc'}
-        # refresh top-level metadata (root -> timestamp -> snapshot -> targets)
-        try:
-            self.refresh()
-        except (DownloadError, UnsignedMetadataError) as e:
-            logger.warning(f'Cannot refresh metadata: {e}')
-            if self.refresh_required:
-                logger.warning('Exiting: refresh is required')
-                sys.exit()
-            return None
-        # check for new target files (archives and patches)
-        logger.debug(f'current archive: {self.current_archive.filename}')
-        all_new_targets = dict(
-            (target_meta, self.get_targetinfo(target_meta))
-            for target_meta in self.trusted_target_metas
-            if target_meta.name == self.current_archive.name
-            and target_meta.version > self.current_archive.version
-        )
-        logger.debug(f'{len(all_new_targets)} new *targets* found')
-        # determine latest archive, filtered by the specified pre-release level
-        new_archives = dict(
-            item for item in all_new_targets.items()
-            if item[0].is_archive
-            and (not item[0].version.pre or item[0].version.pre[0] in included[pre])
-        )
-        new_archive_meta = None
-        if new_archives:
-            logger.debug(f'{len(new_archives)} new *archives* found')
-            new_archive_meta, self.new_archive_info = sorted(
-                new_archives.items()
-            )[-1]
-            self.new_archive_local_path = pathlib.Path(
-                self.target_dir, new_archive_meta.path.name
-            )
-            # patches must include all pre-releases and final releases up to,
-            # and including, the latest archive as determined above
-            new_patches = dict(
-                item for item in all_new_targets.items()
-                if item[0].is_patch
-                and item[0].version <= new_archive_meta.version
-            )
-            # determine size of patch update and archive update
-            total_patch_size = sum(
-                target_file.length for target_file in new_patches.values()
-            )
-            # use file size to decide if we want to do a patch update or a
-            # full update (if there are no patches, or if the current archive
-            # is not available, we must do a full update)
-            self.new_targets = new_patches
-            no_patches = total_patch_size == 0
-            patches_too_big = total_patch_size > self.new_archive_info.length
-            current_archive_not_found = not self.current_archive_local_path.exists()
-            if not patch or no_patches or patches_too_big or current_archive_not_found:
-                self.new_targets = {new_archive_meta: self.new_archive_info}
-                logger.debug('full update available')
-            else:
-                logger.debug('patch update(s) available')
-        else:
-            self.new_targets = {}
-            logger.debug('no new archives found')
-        return new_archive_meta
-
-    def _download_updates(self, progress_hook: Optional[Callable]) -> bool:
-        # download the new targets selected in check_for_updates
-        for target_meta, target_file in self.new_targets.items():
-            # check if the target file has already been downloaded
-            local_path_str = self.find_cached_target(targetinfo=target_file)
-            if not local_path_str:
-                # attach progress hook
-                if progress_hook:
-                    self._fetcher.attach_progress_hook(
-                        hook=progress_hook, bytes_expected=target_file.length
-                    )
-                # download the target file
-                local_path_str = self.download_target(targetinfo=target_file)
-            self.downloaded_target_files[target_meta] = pathlib.Path(local_path_str)
-        return len(self.downloaded_target_files) == len(self.new_targets)
-
-    def _apply_updates(
-            self,
-            install: Callable,
-            skip_confirmation: bool,
-            **kwargs,
-    ):
-        """
-        kwargs are passed on to the 'install' callable
-
-        Note this has a side-effect: if self.extract_dir is not specified,
-        an extract_dir is created in a platform-specific temporary location.
-        """
-        # patch current archive (if we have patches) or use new full archive
-        archive_bytes = None
-        for target, file_path in sorted(self.downloaded_target_files.items()):
-            if target.is_archive:
-                # just ensure the full archive file is available
-                assert len(self.downloaded_target_files) == 1
-                assert self.new_archive_local_path.exists()
-            elif target.is_patch:
-                # create new archive by patching current archive (patches
-                # must be sorted by increasing version)
-                if archive_bytes is None:
-                    archive_bytes = self.current_archive_local_path.read_bytes()
-                archive_bytes = bsdiff4.patch(archive_bytes, file_path.read_bytes())
-        if archive_bytes:
-            # verify the patched archive length and hash
-            self.new_archive_info.verify_length_and_hashes(data=archive_bytes)
-            # write the patched new archive
-            self.new_archive_local_path.write_bytes(archive_bytes)
-        # extract archive to temporary directory
-        if self.extract_dir is None:
-            self.extract_dir = DEFAULT_EXTRACT_DIR
-            self.extract_dir.mkdir(exist_ok=True)
-            logger.debug(f'default extract dir created: {self.extract_dir}')
-        # extract
-        shutil.unpack_archive(
-            filename=self.new_archive_local_path, extract_dir=self.extract_dir
-        )
-        logger.debug(f'files extracted to {self.extract_dir}')
-        # install
-        confirmation_message = f'Install update in {self.app_install_dir}? [y]/n'
-        if skip_confirmation or input(confirmation_message) in ['y', '']:
-            # start a script that moves the extracted files to the app install
-            # directory (overwrites existing files), then exit current process
-            install(
-                src_dir=self.extract_dir,
-                dst_dir=self.app_install_dir,
-                **kwargs,
-            )
-        else:
-            logger.warning('Installation aborted.')
-        # todo: clean up deprecated local archive
-
-
-class AuthRequestsFetcher(RequestsFetcher):
-    def __init__(
-            self,
-            session_auth: Optional[Dict[str, Union[Tuple[str, str], AuthBase]]] = None,
-    ) -> None:
-        """
-        This extends the default tuf RequestsFetcher, so we can specify
-        authentication tuples (or custom authentication objects) for each
-        session.
-
-        session_auth (optional):
-
-            dict of the form {<scheme and server>: (<username>, <password>), ...}
-            or {<scheme and server>: <requests.auth.AuthBase>, ...}
-            or some combination of those
-
-        where <scheme and server> can be e.g. https://example.com
-        or http://localhost:8000.
-
-        Naming follows [RFC 2396][1], which defines a generic uri as:
-
-            <scheme>://<authority><path>?<query>
-
-        where <authority> can be <server>.
-
-        Also see session authentication example in requests docs: [1][2][3]
-
-        [1]: https://datatracker.ietf.org/doc/html/rfc2396#section-3
-        [2]: https://docs.python-requests.org/en/master/user/advanced/#session-objects
-        [3]: https://docs.python-requests.org/en/latest/user/advanced/#custom-authentication
-        [4]: https://docs.python-requests.org/en/master/api/#sessionapi
-        """
-        super().__init__()
-        self.session_auth = session_auth or {}
-        # default progress hook does nothing
-        self._progress = lambda bytes_new: None
-
-    def attach_progress_hook(self, hook: Callable, bytes_expected: int):
-        """
-        Allow clients to attach a progress hook which gets called after every
-        downloaded chunk.
-
-        The hook must accept two kwargs: bytes_downloaded and bytes_expected
-        """
-        def progress(
-                bytes_new: int,
-                _cache: List[int] = [],  # noqa: mutable default intentional
-        ):
-            # mutable default is used to keep track of downloaded chunk sizes
-            _cache.append(bytes_new)
-            return hook(
-                bytes_downloaded=sum(_cache), bytes_expected=bytes_expected
-            )
-
-        self._progress = progress
-
-    def _get_session(self, url: str) -> requests.Session:
-        # set the Session.auth attribute for the specified server, if available
-        session = super()._get_session(url=url)
-        # determine session_auth key
-        parsed_url = parse.urlparse(url)
-        key = parse.urlunparse(
-            parse.ParseResult._make(
-                [parsed_url.scheme, parsed_url.netloc, '', '', '', '']
-            )
-        )
-        session.auth = self.session_auth.get(key)
-        return session
-
-    def _chunks(self, response: "requests.Response") -> Iterator[bytes]:
-        """Call progress hook for every chunk."""
-        for data in super()._chunks(response=response):
-            self._progress(bytes_new=len(data))
-            yield data
+import bsdiff4
+import logging
+import pathlib
+import shutil
+import sys
+import tempfile
+from typing import Callable, Dict, Iterator, List, Optional, Tuple, Union
+from urllib import parse
+
+import requests
+from requests.auth import AuthBase
+from tuf.api.exceptions import DownloadError, UnsignedMetadataError
+import tuf.ngclient
+
+from tufup.common import TargetMeta
+from tufup.utils.platform_specific import install_update
+
+logger = logging.getLogger(__name__)
+
+DEFAULT_EXTRACT_DIR = pathlib.Path(tempfile.gettempdir()) / 'tufup'
+
+
+class Client(tuf.ngclient.Updater):
+    def __init__(
+            self,
+            app_name: str,
+            app_install_dir: pathlib.Path,
+            current_version: str,
+            metadata_dir: pathlib.Path,
+            metadata_base_url: str,
+            target_dir: pathlib.Path,
+            target_base_url: str,
+            extract_dir: Optional[pathlib.Path] = None,
+            refresh_required: bool = False,
+            session_auth: Optional[Dict[str, Union[Tuple[str, str], AuthBase]]] = None,
+            **kwargs,
+    ):
+        # tuf.ngclient.Updater.__init__ loads local root metadata automatically
+        super().__init__(
+            metadata_dir=str(metadata_dir),
+            metadata_base_url=metadata_base_url,
+            target_dir=str(target_dir),
+            target_base_url=target_base_url,
+            fetcher=AuthRequestsFetcher(session_auth=session_auth),
+            **kwargs,
+        )
+        self.app_install_dir = app_install_dir
+        self.extract_dir = extract_dir
+        self.refresh_required = refresh_required
+        self.current_archive = TargetMeta(name=app_name, version=current_version)
+        self.current_archive_local_path = target_dir / self.current_archive.path
+        self.new_archive_local_path: Optional[pathlib.Path] = None
+        self.new_archive_info: Optional[tuf.ngclient.TargetFile] = None
+        self.new_targets: Optional[dict] = None
+        self.downloaded_target_files = {}
+
+    @property
+    def trusted_target_metas(self) -> list:
+        """
+        Return a list of available trusted targets, as TargetMeta objects.
+
+        This is convenient because TargetMeta objects can be sorted by version.
+        """
+        # todo: _trusted_set is private, but ideally we would use a public
+        #  interface (if only tuf.ngclient exposed one...)
+        _trusted_target_metas = []
+        if self._trusted_set.targets:
+            _trusted_target_metas = [
+                TargetMeta(target_path=key)
+                for key in self._trusted_set.targets.signed.targets.keys()
+            ]
+            logger.debug(f'{len(_trusted_target_metas)} TargetMeta objects created')
+        else:
+            logger.warning('targets metadata not found')
+        return _trusted_target_metas
+
+    def get_targetinfo(self, target_path: Union[str, TargetMeta]) -> Optional[tuf.ngclient.TargetFile]:
+        """Extend Updater.get_targetinfo to handle TargetMeta input args."""
+        if isinstance(target_path, TargetMeta):
+            target_path = target_path.target_path_str
+        return super().get_targetinfo(target_path=target_path)
+
+    @property
+    def updates_available(self):
+        if self.new_targets is None:
+            logger.warning('Please call check_for_updates first.')
+            return False
+        else:
+            return len(self.new_targets) > 0
+
+    def download_and_apply_update(
+            self,
+            skip_confirmation: bool = False,
+            install: Optional[Callable] = None,
+            progress_hook: Optional[Callable] = None,
+            **kwargs,
+    ):
+        """
+        Download and apply available updates.
+
+        Note that `check_for_updates` must be called first.
+
+        This downloads the files found by `check_for_updates`, applies any
+        patches, and extracts the resulting archive to the `extract_dir`. At
+        that point, the update is ready to be installed (i.e. moved into
+        place). This is done by calling `install` with the specified `**kwargs`.
+
+        The default `install` callable moves the content of `extract_dir` to
+        `app_install_dir`, and exits the application (not necessarily in that
+        order).
+
+        The **kwargs are passed on to the 'install' callable
+
+        The default `install` callable accepts two additional arguments:
+
+            `purge_dst_dir` (default False): if True, *ALL* content will be
+            deleted from the `app_install_dir`
+
+            `exclude_from_purge` (default None): list of paths to exclude
+            from purge
+
+            **DANGER**: Only set `purge_dst_dir=True` if your app is
+            installed in its own separate directory, otherwise this will
+            cause unrelated files and folders to be deleted.
+        """
+        if install is None:
+            install = install_update
+        if self.updates_available and self._download_updates(
+                progress_hook=progress_hook
+        ):
+            self._apply_updates(
+                install=install, skip_confirmation=skip_confirmation, **kwargs
+            )
+
+    def check_for_updates(
+            self, pre: Optional[str] = None, patch: bool = True
+    ) -> Optional[TargetMeta]:
+        """
+        Check if any updates are available, based on current app version.
+
+        Returns latest archive meta, if a new archive is found.
+
+        Final releases are always included. Pre-releases are excluded by
+        default. If `pre` is specified, pre-releases are included, down to
+        the specified level. Pre-release identifiers follow the PEP440
+        specification, i.e. 'a', 'b', or 'rc', for alpha, beta, and release
+        candidate, respectively.
+
+        If `patch` is `False`, a full update is enforced.
+        """
+        included = {None: '', '': '', 'a': 'abrc', 'b': 'brc', 'rc': 'rc'}
+        # refresh top-level metadata (root -> timestamp -> snapshot -> targets)
+        try:
+            self.refresh()
+        except (DownloadError, UnsignedMetadataError) as e:
+            logger.warning(f'Cannot refresh metadata: {e}')
+            if self.refresh_required:
+                logger.warning('Exiting: refresh is required')
+                sys.exit()
+            return None
+        # check for new target files (archives and patches)
+        logger.debug(f'current archive: {self.current_archive.filename}')
+        all_new_targets = dict(
+            (target_meta, self.get_targetinfo(target_meta))
+            for target_meta in self.trusted_target_metas
+            if target_meta.name == self.current_archive.name
+            and target_meta.version > self.current_archive.version
+        )
+        logger.debug(f'{len(all_new_targets)} new *targets* found')
+        # determine latest archive, filtered by the specified pre-release level
+        new_archives = dict(
+            item for item in all_new_targets.items()
+            if item[0].is_archive
+            and (not item[0].version.pre or item[0].version.pre[0] in included[pre])
+        )
+        new_archive_meta = None
+        if new_archives:
+            logger.debug(f'{len(new_archives)} new *archives* found')
+            new_archive_meta, self.new_archive_info = sorted(
+                new_archives.items()
+            )[-1]
+            self.new_archive_local_path = pathlib.Path(
+                self.target_dir, new_archive_meta.path.name
+            )
+            # patches must include all pre-releases and final releases up to,
+            # and including, the latest archive as determined above
+            new_patches = dict(
+                item for item in all_new_targets.items()
+                if item[0].is_patch
+                and item[0].version <= new_archive_meta.version
+            )
+            # determine size of patch update and archive update
+            total_patch_size = sum(
+                target_file.length for target_file in new_patches.values()
+            )
+            # use file size to decide if we want to do a patch update or a
+            # full update (if there are no patches, or if the current archive
+            # is not available, we must do a full update)
+            self.new_targets = new_patches
+            no_patches = total_patch_size == 0
+            patches_too_big = total_patch_size > self.new_archive_info.length
+            current_archive_not_found = not self.current_archive_local_path.exists()
+            if not patch or no_patches or patches_too_big or current_archive_not_found:
+                self.new_targets = {new_archive_meta: self.new_archive_info}
+                logger.debug('full update available')
+            else:
+                logger.debug('patch update(s) available')
+        else:
+            self.new_targets = {}
+            logger.debug('no new archives found')
+        return new_archive_meta
+
+    def _download_updates(self, progress_hook: Optional[Callable]) -> bool:
+        # download the new targets selected in check_for_updates
+        for target_meta, target_file in self.new_targets.items():
+            # check if the target file has already been downloaded
+            local_path_str = self.find_cached_target(targetinfo=target_file)
+            if not local_path_str:
+                # attach progress hook
+                if progress_hook:
+                    self._fetcher.attach_progress_hook(
+                        hook=progress_hook, bytes_expected=target_file.length
+                    )
+                # download the target file
+                local_path_str = self.download_target(targetinfo=target_file)
+            self.downloaded_target_files[target_meta] = pathlib.Path(local_path_str)
+        return len(self.downloaded_target_files) == len(self.new_targets)
+
+    def _apply_updates(
+            self,
+            install: Callable,
+            skip_confirmation: bool,
+            **kwargs,
+    ):
+        """
+        kwargs are passed on to the 'install' callable
+
+        Note this has a side-effect: if self.extract_dir is not specified,
+        an extract_dir is created in a platform-specific temporary location.
+        """
+        # patch current archive (if we have patches) or use new full archive
+        archive_bytes = None
+        for target, file_path in sorted(self.downloaded_target_files.items()):
+            if target.is_archive:
+                # just ensure the full archive file is available
+                assert len(self.downloaded_target_files) == 1
+                assert self.new_archive_local_path.exists()
+            elif target.is_patch:
+                # create new archive by patching current archive (patches
+                # must be sorted by increasing version)
+                if archive_bytes is None:
+                    archive_bytes = self.current_archive_local_path.read_bytes()
+                archive_bytes = bsdiff4.patch(archive_bytes, file_path.read_bytes())
+        if archive_bytes:
+            # verify the patched archive length and hash
+            self.new_archive_info.verify_length_and_hashes(data=archive_bytes)
+            # write the patched new archive
+            self.new_archive_local_path.write_bytes(archive_bytes)
+        # extract archive to temporary directory
+        if self.extract_dir is None:
+            self.extract_dir = DEFAULT_EXTRACT_DIR
+            self.extract_dir.mkdir(exist_ok=True)
+            logger.debug(f'default extract dir created: {self.extract_dir}')
+        # extract
+        shutil.unpack_archive(
+            filename=self.new_archive_local_path, extract_dir=self.extract_dir
+        )
+        logger.debug(f'files extracted to {self.extract_dir}')
+        # install
+        confirmation_message = f'Install update in {self.app_install_dir}? [y]/n'
+        if skip_confirmation or input(confirmation_message) in ['y', '']:
+            # start a script that moves the extracted files to the app install
+            # directory (overwrites existing files), then exit current process
+            install(
+                src_dir=self.extract_dir,
+                dst_dir=self.app_install_dir,
+                **kwargs,
+            )
+        else:
+            logger.warning('Installation aborted.')
+        # todo: clean up deprecated local archive
+
+
+class AuthRequestsFetcher(tuf.ngclient.RequestsFetcher):
+    # RequestsFetcher is public as of python-tuf v2.1.0 (see python-tuf #2277)
+    def __init__(
+            self,
+            session_auth: Optional[Dict[str, Union[Tuple[str, str], AuthBase]]] = None,
+    ) -> None:
+        """
+        This extends the default tuf RequestsFetcher, so we can specify
+        authentication tuples (or custom authentication objects) for each
+        session.
+
+        session_auth (optional):
+
+            dict of the form {<scheme and server>: (<username>, <password>), ...}
+            or {<scheme and server>: <requests.auth.AuthBase>, ...}
+            or some combination of those
+
+        where <scheme and server> can be e.g. https://example.com
+        or http://localhost:8000.
+
+        Naming follows [RFC 2396][1], which defines a generic uri as:
+
+            <scheme>://<authority><path>?<query>
+
+        where <authority> can be <server>.
+
+        Also see session authentication example in requests docs: [1][2][3]
+
+        [1]: https://datatracker.ietf.org/doc/html/rfc2396#section-3
+        [2]: https://docs.python-requests.org/en/master/user/advanced/#session-objects
+        [3]: https://docs.python-requests.org/en/latest/user/advanced/#custom-authentication
+        [4]: https://docs.python-requests.org/en/master/api/#sessionapi
+        """
+        super().__init__()
+        self.session_auth = session_auth or {}
+        # default progress hook does nothing
+        self._progress = lambda bytes_new: None
+
+    def attach_progress_hook(self, hook: Callable, bytes_expected: int):
+        """
+        Allow clients to attach a progress hook which gets called after every
+        downloaded chunk.
+
+        The hook must accept two kwargs: bytes_downloaded and bytes_expected
+        """
+        def progress(
+                bytes_new: int,
+                _cache: List[int] = [],  # noqa: mutable default intentional
+        ):
+            # mutable default is used to keep track of downloaded chunk sizes
+            _cache.append(bytes_new)
+            return hook(
+                bytes_downloaded=sum(_cache), bytes_expected=bytes_expected
+            )
+
+        self._progress = progress
+
+    def _get_session(self, url: str) -> requests.Session:
+        # set the Session.auth attribute for the specified server, if available
+        session = super()._get_session(url=url)
+        # determine session_auth key
+        parsed_url = parse.urlparse(url)
+        key = parse.urlunparse(
+            parse.ParseResult._make(
+                [parsed_url.scheme, parsed_url.netloc, '', '', '', '']
+            )
+        )
+        session.auth = self.session_auth.get(key)
+        return session
+
+    def _chunks(self, response: "requests.Response") -> Iterator[bytes]:
+        """Call progress hook for every chunk."""
+        for data in super()._chunks(response=response):
+            self._progress(bytes_new=len(data))
+            yield data
```

### Comparing `tufup-0.4.9/src/tufup/common.py` & `tufup-0.5.0/src/tufup/common.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-import logging
-import pathlib
-import re
-from typing import Optional, Union
-
-import bsdiff4
-from packaging.version import Version, InvalidVersion
-
-logger = logging.getLogger(__name__)
-
-SUFFIX_ARCHIVE = '.tar.gz'
-SUFFIX_PATCH = '.patch'
-
-
-class TargetMeta(object):
-    filename_pattern = '{name}-{version}{suffix}'
-    filename_regex = re.compile(
-        r'^(?P<name>[\w-]+)-(?P<version>.+)(?P<suffix>\.tar\.gz|\.patch)$'
-    )
-
-    def __init__(
-            self,
-            target_path: Union[None, str, pathlib.Path] = None,
-            name: Optional[str] = None,
-            version: Optional[str] = None,
-            is_archive: Optional[bool] = True,
-    ):
-        """
-
-        Initialize either with target_path, or with name, version, archive.
-        """
-        super().__init__()
-        if target_path is None:
-            target_path = TargetMeta.compose_filename(
-                name=name, version=version, is_archive=is_archive
-            )
-        self.target_path_str = str(target_path)  # keep the original for reference
-        self.path = pathlib.Path(target_path)
-
-    def __str__(self):
-        return str(self.target_path_str)
-
-    def __repr__(self):
-        return f'{self.__class__.__name__}(target_path="{self.target_path_str}")'
-
-    def __hash__(self):
-        """
-        This makes the object hashable, so it can be used as dict key or set
-        member.
-
-        https://docs.python.org/3/glossary.html#term-hashable
-
-        """
-        return hash(tuple(self.__dict__.items()))
-
-    def __eq__(self, other):
-        if type(other) != type(self):
-            return NotImplemented
-        return vars(self) == vars(other)
-
-    def __lt__(self, other):
-        """
-        This makes the object sortable, based on the *version* property,
-        without having to specify an explicit sorting key. Note this
-        disregards app name, platform, and suffixes.
-        """
-        if type(other) != type(self):
-            return NotImplemented
-        return self.version < other.version
-
-    @property
-    def filename(self):
-        return self.path.name
-
-    @property
-    def name(self) -> Optional[str]:
-        """The app name."""
-        match_dict = self.parse_filename(self.filename)
-        return match_dict.get('name')
-
-    @property
-    def version(self) -> Optional[Version]:
-        match_dict = self.parse_filename(self.filename)
-        try:
-            version = Version(match_dict.get('version', ''))
-        except InvalidVersion:
-            version = None
-            logger.debug(f'No valid version in filename: {self.filename}')
-        return version
-
-    @property
-    def suffix(self) -> Optional[str]:
-        """Returns the filename suffix, either '.tar.gz', '.patch', or None."""
-        match_dict = self.parse_filename(self.filename)
-        return match_dict.get('suffix')
-
-    @property
-    def is_archive(self) -> bool:
-        return self.suffix == SUFFIX_ARCHIVE
-
-    @property
-    def is_patch(self) -> bool:
-        return self.suffix == SUFFIX_PATCH
-
-    @property
-    def is_other(self) -> bool:
-        return self.suffix not in [SUFFIX_ARCHIVE, SUFFIX_PATCH]
-
-    @classmethod
-    def parse_filename(cls, filename: str) -> dict:
-        """
-        Parse a filename to extract app name, version, and suffix.
-
-        We do not impose any versioning requirements yet, such as defined in
-        packaging.version.VERSION_PATTERN.
-        """
-        match = cls.filename_regex.search(string=filename)
-        return match.groupdict() if match else {}
-
-    @classmethod
-    def compose_filename(cls, name: str, version: str, is_archive: bool):
-        suffix = SUFFIX_ARCHIVE if is_archive else SUFFIX_PATCH
-        return cls.filename_pattern.format(name=name, version=version, suffix=suffix)
-
-
-class Patcher(object):
-    @classmethod
-    def create_patch(cls, src_path: pathlib.Path, dst_path: pathlib.Path) -> pathlib.Path:
-        """
-        Create a binary patch file based on source and destination files.
-
-        Patch file path matches destination file path, except for suffix.
-        """
-        # replace suffix twice, in case we have a .tar.gz
-        patch_path = dst_path.with_suffix('').with_suffix(SUFFIX_PATCH)
-        bsdiff4.file_diff(src_path=src_path, dst_path=dst_path, patch_path=patch_path)
-        return patch_path
-
-    @classmethod
-    def apply_patch(cls, src_path: pathlib.Path, patch_path: pathlib.Path):
-        """
-        Apply binary patch file to source file to create destination file.
-
-        Destination file path matches patch file path, except for suffix.
-        """
-        dst_path = patch_path.with_suffix(SUFFIX_ARCHIVE)
-        bsdiff4.file_patch(src_path=src_path, dst_path=dst_path, patch_path=patch_path)
-        return dst_path
+import logging
+import pathlib
+import re
+from typing import Optional, Union
+
+import bsdiff4
+from packaging.version import Version, InvalidVersion
+
+logger = logging.getLogger(__name__)
+
+SUFFIX_ARCHIVE = '.tar.gz'
+SUFFIX_PATCH = '.patch'
+
+
+class TargetMeta(object):
+    filename_pattern = '{name}-{version}{suffix}'
+    filename_regex = re.compile(
+        r'^(?P<name>[\w-]+)-(?P<version>.+)(?P<suffix>\.tar\.gz|\.patch)$'
+    )
+
+    def __init__(
+            self,
+            target_path: Union[None, str, pathlib.Path] = None,
+            name: Optional[str] = None,
+            version: Optional[str] = None,
+            is_archive: Optional[bool] = True,
+    ):
+        """
+
+        Initialize either with target_path, or with name, version, archive.
+        """
+        super().__init__()
+        if target_path is None:
+            target_path = TargetMeta.compose_filename(
+                name=name, version=version, is_archive=is_archive
+            )
+        self.target_path_str = str(target_path)  # keep the original for reference
+        self.path = pathlib.Path(target_path)
+
+    def __str__(self):
+        return str(self.target_path_str)
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}(target_path="{self.target_path_str}")'
+
+    def __hash__(self):
+        """
+        This makes the object hashable, so it can be used as dict key or set
+        member.
+
+        https://docs.python.org/3/glossary.html#term-hashable
+
+        """
+        return hash(tuple(self.__dict__.items()))
+
+    def __eq__(self, other):
+        if type(other) != type(self):
+            return NotImplemented
+        return vars(self) == vars(other)
+
+    def __lt__(self, other):
+        """
+        This makes the object sortable, based on the *version* property,
+        without having to specify an explicit sorting key. Note this
+        disregards app name, platform, and suffixes.
+        """
+        if type(other) != type(self):
+            return NotImplemented
+        return self.version < other.version
+
+    @property
+    def filename(self):
+        return self.path.name
+
+    @property
+    def name(self) -> Optional[str]:
+        """The app name."""
+        match_dict = self.parse_filename(self.filename)
+        return match_dict.get('name')
+
+    @property
+    def version(self) -> Optional[Version]:
+        match_dict = self.parse_filename(self.filename)
+        try:
+            version = Version(match_dict.get('version', ''))
+        except InvalidVersion:
+            version = None
+            logger.debug(f'No valid version in filename: {self.filename}')
+        return version
+
+    @property
+    def suffix(self) -> Optional[str]:
+        """Returns the filename suffix, either '.tar.gz', '.patch', or None."""
+        match_dict = self.parse_filename(self.filename)
+        return match_dict.get('suffix')
+
+    @property
+    def is_archive(self) -> bool:
+        return self.suffix == SUFFIX_ARCHIVE
+
+    @property
+    def is_patch(self) -> bool:
+        return self.suffix == SUFFIX_PATCH
+
+    @property
+    def is_other(self) -> bool:
+        return self.suffix not in [SUFFIX_ARCHIVE, SUFFIX_PATCH]
+
+    @classmethod
+    def parse_filename(cls, filename: str) -> dict:
+        """
+        Parse a filename to extract app name, version, and suffix.
+
+        We do not impose any versioning requirements yet, such as defined in
+        packaging.version.VERSION_PATTERN.
+        """
+        match = cls.filename_regex.search(string=filename)
+        return match.groupdict() if match else {}
+
+    @classmethod
+    def compose_filename(cls, name: str, version: str, is_archive: bool):
+        suffix = SUFFIX_ARCHIVE if is_archive else SUFFIX_PATCH
+        return cls.filename_pattern.format(name=name, version=version, suffix=suffix)
+
+
+class Patcher(object):
+    @classmethod
+    def create_patch(cls, src_path: pathlib.Path, dst_path: pathlib.Path) -> pathlib.Path:
+        """
+        Create a binary patch file based on source and destination files.
+
+        Patch file path matches destination file path, except for suffix.
+        """
+        # replace suffix twice, in case we have a .tar.gz
+        patch_path = dst_path.with_suffix('').with_suffix(SUFFIX_PATCH)
+        bsdiff4.file_diff(src_path=src_path, dst_path=dst_path, patch_path=patch_path)
+        return patch_path
+
+    @classmethod
+    def apply_patch(cls, src_path: pathlib.Path, patch_path: pathlib.Path):
+        """
+        Apply binary patch file to source file to create destination file.
+
+        Destination file path matches patch file path, except for suffix.
+        """
+        dst_path = patch_path.with_suffix(SUFFIX_ARCHIVE)
+        bsdiff4.file_patch(src_path=src_path, dst_path=dst_path, patch_path=patch_path)
+        return dst_path
```

### Comparing `tufup-0.4.9/src/tufup/repo/__init__.py` & `tufup-0.5.0/src/tufup/repo/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,917 +1,917 @@
-from copy import deepcopy
-from datetime import datetime, timedelta
-import inspect
-import json
-import logging
-import pathlib
-try:
-    # workaround for PyInstaller issue 6911 (setuptools issue 3089)
-    import setuptools.config.expand  # noqa
-except AssertionError as e:
-    pass  # assuming we are on the client side...
-import shutil
-from typing import Any, Dict, Iterable, List, Optional, TypedDict, Union
-
-from securesystemslib.exceptions import CryptoError
-from securesystemslib.interface import (
-    generate_and_write_ed25519_keypair_with_prompt,
-    generate_and_write_unencrypted_ed25519_keypair,
-    import_ed25519_publickey_from_file,
-    import_ed25519_privatekey_from_file,
-)
-from securesystemslib.signer import SSlibSigner
-from tuf.api.metadata import (
-    SPECIFICATION_VERSION,
-    TOP_LEVEL_ROLE_NAMES,
-    Key,
-    Metadata,
-    MetaFile,
-    Role,
-    Root,
-    Snapshot,
-    TargetFile,
-    Targets,
-    Timestamp,
-)
-from tuf.api.serialization.json import JSONSerializer
-
-from tufup.common import Patcher, SUFFIX_ARCHIVE, SUFFIX_PATCH, TargetMeta
-
-logger = logging.getLogger(__name__)
-
-"""
-
-https://github.com/theupdateframework/python-tuf/blob/develop/examples/repo_example/basic_repo.py
-
-"""
-
-__all__ = [
-    'DEFAULT_KEY_MAP',
-    'DEFAULT_KEYS_DIR_NAME',
-    'DEFAULT_META_DIR_NAME',
-    'DEFAULT_REPO_DIR_NAME',
-    'DEFAULT_TARGETS_DIR_NAME',
-    'in_',
-    'Keys',
-    'make_gztar_archive',
-    'Repository',
-    'Roles',
-    'SUFFIX_JSON',
-    'SUFFIX_PUB',
-    'TOP_LEVEL_ROLE_NAMES',
-]
-
-# copied from python-tuf basic_repo.py
-SPEC_VERSION = ".".join(SPECIFICATION_VERSION)
-
-
-# copied from python-tuf basic_repo.py
-def in_(days: float) -> datetime:
-    """Returns a timestamp for the specified number of days from now."""
-    return datetime.utcnow().replace(microsecond=0) + timedelta(days=days)
-
-
-def make_gztar_archive(
-        src_dir: Union[pathlib.Path, str],
-        dst_dir: Union[pathlib.Path, str],
-        app_name: str,
-        version: str,
-        **kwargs,  # allowed kwargs are passed on to shutil.make_archive
-) -> Optional[TargetMeta]:
-    # remove disallowed kwargs
-    for key in ['base_name', 'root_dir', 'format']:
-        if kwargs.pop(key, None):
-            logger.warning(f'{key} ignored: using default')
-    # ensure paths
-    src_dir = pathlib.Path(src_dir)
-    dst_dir = pathlib.Path(dst_dir)
-    # compose archive path and check existence
-    archive_filename = TargetMeta.compose_filename(
-        name=app_name, version=version, is_archive=True
-    )
-    archive_path = dst_dir / archive_filename
-    if archive_path.exists():
-        if input(f'Found existing archive: {archive_path}.\nOverwrite? [n]/y') != 'y':
-            print('Using existing archive.')
-            return TargetMeta(archive_path)
-    # make archive
-    base_name = str(dst_dir / archive_filename.replace(SUFFIX_ARCHIVE, ''))
-    archive_path_str = shutil.make_archive(
-        base_name=base_name,  # archive file path, no suffix
-        root_dir=str(src_dir),  # paths in archive will be relative to root_dir
-        format='gztar',
-        **kwargs,
-    )
-    return TargetMeta(target_path=archive_path_str)
-
-
-class RolesDict(TypedDict):
-    root: Any
-    targets: Any
-    snapshot: Any
-    timestamp: Any
-
-
-DEFAULT_REPO_DIR_NAME = 'repository'
-DEFAULT_KEYS_DIR_NAME = 'keystore'
-DEFAULT_META_DIR_NAME = 'metadata'
-DEFAULT_TARGETS_DIR_NAME = 'targets'
-DEFAULT_KEY_MAP = RolesDict((key, [key]) for key in TOP_LEVEL_ROLE_NAMES)  # noqa
-DEFAULT_EXPIRATION_DAYS = RolesDict(root=365, targets=7, snapshot=7, timestamp=1)
-DEFAULT_THRESHOLDS = RolesDict(root=1, targets=1, snapshot=1, timestamp=1)
-SUFFIX_JSON = '.json'
-SUFFIX_PUB = '.pub'
-FILENAME_ROOT = Root.type + SUFFIX_JSON
-FILENAME_TARGETS = Targets.type + SUFFIX_JSON
-FILENAME_SNAPSHOT = Snapshot.type + SUFFIX_JSON
-FILENAME_TIMESTAMP = Timestamp.type + SUFFIX_JSON
-
-
-class Base(object):
-    def __init__(self, dir_path: Union[pathlib.Path, str, None]):
-        """
-        dir_path: directory where all key files are stored
-        encrypted: names of the keys that are (to be) encrypted
-        key_map: maps top-level role names to lists of key names
-        """
-        if dir_path is None:
-            dir_path = pathlib.Path.cwd()
-        # enforce pathlib.Path
-        self.dir_path = pathlib.Path(dir_path)
-        if not self.dir_path.exists():
-            if input(f'Create directory {self.dir_path}? [y]/n') in ['y', '']:
-                self.dir_path.mkdir(parents=True)
-                print(f'Directory created: {self.dir_path}')
-
-
-class Keys(Base):
-    filename_pattern = '{key_name}'
-
-    def __init__(
-            self,
-            dir_path: Union[pathlib.Path, str, None] = None,
-            encrypted: Optional[List[str]] = None,
-            key_map: Optional[RolesDict] = None,
-            thresholds: Optional[RolesDict] = None,
-    ):
-        if dir_path is None:
-            dir_path = pathlib.Path.cwd() / DEFAULT_KEYS_DIR_NAME
-        super().__init__(dir_path=dir_path)
-        if encrypted is None:
-            encrypted = []
-        if key_map is None:
-            key_map = deepcopy(DEFAULT_KEY_MAP)
-        if thresholds is None:
-            thresholds = DEFAULT_THRESHOLDS.copy()
-        self.encrypted = encrypted
-        self.key_map = key_map
-        self.thresholds = thresholds
-        # top-level roles
-        self.root: List[Dict[str, Any]] = []
-        self.targets: List[Dict[str, Any]] = []
-        self.snapshot: List[Dict[str, Any]] = []
-        self.timestamp: List[Dict[str, Any]] = []
-        # import public keys from dir_path, if it exists
-        self.import_all_public_keys()
-
-    def import_all_public_keys(self):
-        for role_name, key_list in self.key_map.items():
-            for key_name in key_list:
-                self.import_public_key(role_name=role_name, key_name=key_name)
-
-    def import_public_key(self, role_name: str, key_name: Optional[str] = None):
-        """Import public key for specified role."""
-        if key_name is None:
-            key_name = role_name
-        public_key_path = self.public_key_path(key_name=key_name)
-        if public_key_path.exists():
-            ssl_key = import_ed25519_publickey_from_file(
-                filepath=str(public_key_path)
-            )
-            getattr(self, role_name).append(ssl_key)
-            logger.debug(f'public key imported: {public_key_path}')
-        else:
-            logger.debug(f'file does not exist: {public_key_path}')
-
-    def create(self):
-        all_key_names = []
-        for key_list in self.key_map.values():
-            all_key_names.extend(key_list)
-        unique_key_names = set(all_key_names)
-        logger.debug(f'creating key-pairs: {unique_key_names}')
-        for key_name in unique_key_names:
-            default_private_key_path = self.private_key_path(key_name=key_name)
-            self.create_key_pair(
-                private_key_path=default_private_key_path,
-                encrypted=key_name in self.encrypted,
-            )
-        # import the newly created public keys
-        self.import_all_public_keys()
-
-    @staticmethod
-    def create_key_pair(
-            private_key_path: pathlib.Path, encrypted: bool
-    ) -> pathlib.Path:
-        if encrypted:
-            # encrypt private key
-            logger.debug(f'set encryption password for private key')
-            generate_keypair = generate_and_write_ed25519_keypair_with_prompt
-        else:
-            # do not encrypt private key (for automated signing)
-            generate_keypair = generate_and_write_unencrypted_ed25519_keypair
-        public_key_path = private_key_path.with_suffix(SUFFIX_PUB)
-        proceed = True
-        if public_key_path.exists():
-            logger.warning(f'Public key already exists: {public_key_path}')
-            proceed = input(f'Overwrite key pair? [n]/y') == 'y'
-        if proceed:
-            file_path_str = generate_keypair(filepath=str(private_key_path))
-            logger.info(f'key-pair created: {file_path_str}, {public_key_path}')
-        return public_key_path
-
-    def private_key_path(self, key_name: str) -> pathlib.Path:
-        return self.dir_path / self.filename_pattern.format(key_name=key_name)
-
-    def public_key_path(self, key_name: str) -> pathlib.Path:
-        return self.private_key_path(key_name=key_name).with_suffix(SUFFIX_PUB)
-
-    def public(self):
-        # return a dict that maps key ids to *public* key objects
-        return {
-            ssl_key['keyid']: Key.from_securesystemslib_key(key_dict=ssl_key)
-            for attr_name, ssl_keys in vars(self).items()
-            if attr_name in TOP_LEVEL_ROLE_NAMES
-            for ssl_key in ssl_keys
-        }
-
-    def roles(self):
-        # return a dict that maps role names to key ids and key thresholds
-        roles_map = dict()
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            ssl_keys = getattr(self, role_name)
-            role_keys = None
-            if ssl_keys:
-                unique_key_ids = list(set(ssl_key['keyid'] for ssl_key in ssl_keys))
-                role_keys = Role(
-                    keyids=unique_key_ids, threshold=self.thresholds[role_name]
-                )
-            roles_map[role_name] = role_keys
-        return roles_map
-
-    @classmethod
-    def find_private_key(cls, key_name: str, key_dirs: List[Union[pathlib.Path, str]]):
-        private_key_path = None
-        private_key_filename = cls.filename_pattern.format(key_name=key_name)
-        for key_dir in key_dirs:
-            key_dir = pathlib.Path(key_dir)  # ensure Path
-            for path in key_dir.iterdir():
-                if path.is_file() and path.name == private_key_filename:
-                    private_key_path = path
-                    break
-        return private_key_path
-
-
-class Roles(Base):
-    filename_pattern = '{version}{role_name}{suffix}'
-
-    def __init__(self, dir_path: Union[pathlib.Path, str, None] = None):
-        """
-        TUF roles
-
-        - root metadata tells us:
-            + all the known keys (key id and public key value)
-            + which keys belong to each role
-            + how many signatures are needed for each role
-        - targets metadata tells us:
-            + which target files are available (filename, size, hash)
-        - snapshots metatadata tells us:
-            + which version of the targets-metadata file to expect
-        - timestamp metadata tells us:
-            + which version of the snapshot-metadata file to expect
-
-        """
-        if dir_path is None:
-            dir_path = pathlib.Path.cwd() / DEFAULT_META_DIR_NAME
-        super().__init__(dir_path=dir_path)
-        # top-level roles
-        self.root: Optional[Metadata[Root]] = None
-        self.targets: Optional[Metadata[Targets]] = None
-        self.snapshot: Optional[Metadata[Snapshot]] = None
-        self.timestamp: Optional[Metadata[Timestamp]] = None
-        # import roles from dir_path, if it exists
-        self._import_roles(role_names=TOP_LEVEL_ROLE_NAMES)
-
-    def _import_roles(self, role_names: Iterable[str]):
-        """Import roles from metadata files."""
-        file_paths = []
-        if self.dir_path.exists():
-            file_paths = [p for p in self.dir_path.iterdir() if p.is_file()]
-        for role_name in role_names:
-            # exclude (root) filenames starting with a version
-            role_paths = [p for p in file_paths if p.name.startswith(role_name)]
-            if role_paths:
-                # there should be only one for each role
-                setattr(self, role_name, Metadata.from_file(str(role_paths[0])))
-
-    def initialize(
-            self, keys: Keys, expiration_days: Optional[RolesDict] = None
-    ):
-        if expiration_days is None:
-            expiration_days = DEFAULT_EXPIRATION_DAYS.copy()
-        # based on python-tuf basic_repo.py
-        common_kwargs = dict(version=1, spec_version=SPEC_VERSION)
-        # role-specific kwargs
-        initial_data = {
-            Root: dict(
-                expires=in_(expiration_days['root']),
-                keys=keys.public(),
-                roles=keys.roles(),
-                # repo is relatively static, no need for consistent snapshots
-                consistent_snapshot=False,
-            ),
-            Targets: dict(
-                expires=in_(expiration_days['targets']),
-                targets=dict(),
-            ),
-            Snapshot: dict(
-                expires=in_(expiration_days['snapshot']),
-                meta={FILENAME_TARGETS: MetaFile(version=1)},
-            ),
-            Timestamp: dict(
-                expires=in_(expiration_days['timestamp']),
-                snapshot_meta=MetaFile(version=1),
-            ),
-        }
-        for role_class, role_kwargs in initial_data.items():
-            attr_name = role_class.type
-            if getattr(self, attr_name) is None:
-                # intialize role only if there is no role yet
-                setattr(
-                    self,
-                    attr_name,
-                    Metadata(
-                        signed=role_class(**common_kwargs, **role_kwargs),
-                        signatures=dict(),
-                    ),
-                )
-
-    def add_or_update_target(
-            self,
-            local_path: Union[pathlib.Path, str],
-            url_path_segments: Optional[List[str]] = None,
-    ):
-        # based on python-tuf basic_repo.py
-        local_path = pathlib.Path(local_path)
-        # build url path
-        url_path_segments = url_path_segments or []
-        url_path_segments.append(local_path.name)
-        url_path = '/'.join(url_path_segments)
-        target_file_info = TargetFile.from_file(
-            target_file_path=url_path, local_path=str(local_path)
-        )
-        # note we assume self.targets has been initialized
-        self.targets.signed.targets[url_path] = target_file_info
-
-    def remove_target(self, local_path: Union[pathlib.Path, str]) -> bool:
-        removed = False
-        targets_dict = self.targets.signed.targets
-        for target_url in targets_dict:
-            # assume target filenames only occur once
-            if target_url.endswith(local_path.name):
-                removed = targets_dict.pop(target_url, None) is not None
-                break
-        if removed:
-            local_path.unlink()
-        return removed
-
-    def add_public_key(
-            self, role_name: str, public_key_path: Union[pathlib.Path, str]
-    ):
-        """Import a public key from file and add it to the specified role."""
-        # based on python-tuf basic_repo.py
-        ssl_key = import_ed25519_publickey_from_file(filepath=str(public_key_path))
-        self.root.signed.add_key(
-            role=role_name, key=Key.from_securesystemslib_key(ssl_key)
-        )
-
-    def set_signature_threshold(self, role_name: str, threshold: int):
-        self.root.signed.roles[role_name].threshold = threshold
-
-    def set_expiration_date(self, role_name: str, days: int):
-        role = getattr(self, role_name)
-        if hasattr(role, 'signed'):
-            role.signed.expires = in_(days)
-
-    def sign_role(
-            self, role_name: str, private_key_path: Union[pathlib.Path, str]
-    ):
-        """
-        Sign role using specified private key.
-
-        We sign off on the role.signed part, and the signature is added to
-        the role.signatures list.
-        """
-        # based on python-tuf basic_repo.py
-        try:
-            # assume unencrypted
-            ssl_key = import_ed25519_privatekey_from_file(
-                filepath=str(private_key_path), prompt=False
-            )
-        except CryptoError as e:
-            # possibly encrypted: try to import with password
-            logger.debug(f'private key import attempt without password failed: {e}')
-            ssl_key = import_ed25519_privatekey_from_file(
-                filepath=str(private_key_path), prompt=True
-            )
-        signer = SSlibSigner(ssl_key)
-        getattr(self, role_name).sign(signer, append=True)
-
-    def file_path(self, role_name: str, version: Optional[int] = None):
-        version_str = ''
-        if role_name == Root.type and version is not None:
-            # "... all released versions of root metadata files MUST always
-            # be provided so that outdated clients can update to the latest
-            # available root."
-            # https://theupdateframework.github.io/specification/latest/#writing-consistent-snapshots
-            version_str = f'{version}.'
-        return self.dir_path / self.filename_pattern.format(
-            version=version_str, role_name=role_name, suffix=SUFFIX_JSON
-        )
-
-    def file_exists(self, role_name: str):
-        """
-        Return True if any metadata file exists for the specified role,
-        ignoring any versions in the filename.
-        """
-        return any(
-            path.exists() for path in self.dir_path.iterdir()
-            if path.is_file() and role_name in path.name
-        )
-
-    def persist_role(self, role_name: str):
-        """
-        Save specified role to corresponding metadata file.
-
-        In case of root, make sure "root.json" always represents the latest
-        version (in addition to x.root.json).
-        """
-        # based on python-tuf basic_repo.py (but without consistent snapshots)
-        role = getattr(self, role_name)
-        file_path = self.file_path(
-            role_name=role_name, version=role.signed.version
-        )
-        role.to_file(
-            filename=str(file_path), serializer=JSONSerializer(compact=False)
-        )
-        if role_name == Root.type:
-            # Copy the latest root metadata to 'root.json' (without version),
-            # to use as trusted root metadata for distribution with the
-            # client. This is convenient, otherwise we would need to modify
-            # the version in the filename every time root is updated.
-            # Moreover, we can now easily access the latest root metadata,
-            # without having to check the version in the filename.
-            client_root_file_path = self.file_path(role_name=Root.type)
-            client_root_file_path.unlink(missing_ok=True)
-            shutil.copy(src=file_path, dst=client_root_file_path)
-
-    def get_latest_archive(self) -> Optional[TargetMeta]:
-        """
-        Returns TargetMeta for latest archive.
-
-        Note that all pre-release versions are always included: On the repo
-        side, there is no difference between final releases an pre-releases.
-        Pre-release specifiers are only used on the Client side, to filter
-        available updates).
-        """
-        # Note this is similar to the logic in Client._check_updates, but not
-        # exactly the same. Merging the implementations would overcomplicate
-        # things.
-        latest_archive = None
-        # sort by version
-        signed_targets = self.targets.signed.targets if self.targets else dict()
-        targets = sorted(
-            TargetMeta(key) for key in signed_targets.keys()
-        )
-        # extract only the archives
-        archives = [target for target in targets if target.is_archive]
-        if archives:
-            latest_archive = archives[-1]
-        return latest_archive
-
-
-class Repository(object):
-    """High-level tools for repository management."""
-    config_filename = '.tufup-repo-config'
-
-    def __init__(
-            self,
-            app_name: str,
-            app_version_attr: Optional[str] = None,
-            repo_dir: Union[pathlib.Path, str, None] = None,
-            keys_dir: Union[pathlib.Path, str, None] = None,
-            key_map: Optional[RolesDict] = None,
-            encrypted_keys: Optional[List[str]] = None,
-            expiration_days: Optional[RolesDict] = None,
-            thresholds: Optional[RolesDict] = None,
-    ):
-        if repo_dir is None:
-            repo_dir = pathlib.Path.cwd() / DEFAULT_REPO_DIR_NAME
-        if keys_dir is None:
-            keys_dir = pathlib.Path.cwd() / DEFAULT_KEYS_DIR_NAME
-        if key_map is None:
-            key_map = deepcopy(DEFAULT_KEY_MAP)
-        if encrypted_keys is None:
-            encrypted_keys = []
-        if expiration_days is None:
-            expiration_days = DEFAULT_EXPIRATION_DAYS.copy()
-        if thresholds is None:
-            thresholds = DEFAULT_THRESHOLDS.copy()
-        self.app_name = app_name
-        self.app_version_attr = app_version_attr
-        # force path object and resolve, in case of relative paths
-        self.repo_dir = pathlib.Path(repo_dir).resolve()
-        self.keys_dir = pathlib.Path(keys_dir).resolve()
-        self.key_map = key_map
-        self.encrypted_keys = encrypted_keys
-        self.expiration_days = expiration_days
-        self.thresholds = thresholds
-        # keys and roles
-        self.keys: Optional[Keys] = None
-        self.roles: Optional[Roles] = None
-        self.revoked_key_names = []
-
-    @property
-    def config_dict(self):
-        """dict to be saved to configuration file."""
-        # attributes matching __init__ arguments are stored as configuration
-        config_items = inspect.signature(self.__init__).parameters.keys()
-        return {item: getattr(self, item) for item in config_items}
-
-    @property
-    def metadata_dir(self) -> pathlib.Path:
-        return self.repo_dir / DEFAULT_META_DIR_NAME
-
-    @property
-    def targets_dir(self) -> pathlib.Path:
-        return self.repo_dir / DEFAULT_TARGETS_DIR_NAME
-
-    @property
-    def app_version(self) -> str:
-        # read version from specified module attribute without importing
-        version = ''
-        if self.app_version_attr:
-            version = str(
-                setuptools.config.expand.read_attr(self.app_version_attr)  # noqa
-            )
-        return version
-
-    @classmethod
-    def get_config_file_path(cls) -> pathlib.Path:
-        return pathlib.Path.cwd() / cls.config_filename
-
-    def save_config(self):
-        """Save current configuration."""
-        # todo: write directories relative to config file dir?
-        file_path = self.get_config_file_path()
-        file_path.write_text(
-            data=json.dumps(
-                self.config_dict, default=str, sort_keys=True, indent=4
-            ),
-            encoding='utf-8',
-        )
-
-    @classmethod
-    def load_config(cls) -> dict:
-        """Load configuration dict from file."""
-        file_path = cls.get_config_file_path()
-        config_dict = dict()
-        try:
-            config_dict = json.loads(file_path.read_text())
-        except FileNotFoundError:
-            logger.warning(f'config file not found: {file_path}')
-        except json.JSONDecodeError:
-            logger.warning(f'config file invalid: {file_path}')
-        return config_dict
-
-    @classmethod
-    def from_config(cls):
-        """Create Repository instance from configuration file."""
-        instance = cls(**cls.load_config())
-        instance._load_keys_and_roles(create_keys=False)
-        return instance
-
-    def initialize(self):
-        """
-        Initialize (or update) the local repository.
-
-        This includes:
-
-        - create directories if they do not exist
-        - import public keys from existing files, or create new key pairs
-        - import roles from existing metadata files
-        - create root metadata file if it does not exist
-
-        Safe to call for existing keys and roles.
-        """
-        # Ensure dirs exist
-        for path in [self.keys_dir, self.metadata_dir, self.targets_dir]:
-            path.mkdir(parents=True, exist_ok=True)
-
-        # Load keys and roles
-        self._load_keys_and_roles(create_keys=True)
-
-        # Publish root metadata (save 1.root.json and copy to root.json)
-        if not self.roles.file_path('root').exists():
-            self.publish_changes(private_key_dirs=[self.keys_dir])
-
-    def refresh_expiration_date(self, role_name: str, days: Optional[int] = None):
-        if days is None:
-            days = self.expiration_days.get(role_name)
-        self.roles.set_expiration_date(role_name=role_name, days=days)
-
-    def replace_key(
-            self,
-            old_key_name: str,
-            new_public_key_path: Union[pathlib.Path, str],
-            new_private_key_encrypted: bool,
-    ):
-        """
-        Replace an existing key by a new one, e.g. after a key compromise.
-
-        Note the changes are not published yet: call publish_changes() for that.
-        """
-        self.revoked_key_names = []
-        # Load old public key from file to obtain its key_id
-        public_key_path = self.keys.public_key_path(key_name=old_key_name)
-        old_key_id = import_ed25519_publickey_from_file(
-            filepath=str(public_key_path)
-        )['keyid']
-        # Get new key name from public key path
-        new_public_key_path = pathlib.Path(new_public_key_path)  # force path
-        # A key may be used for multiple roles, so we check the key id for
-        # all roles.
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            try:
-                # remove old key_id from roles dict, if found, and remove key
-                # from keys dict if it is no longer used by any roles
-                self.roles.root.signed.revoke_key(
-                    role=role_name, keyid=old_key_id
-                )
-                # move old key name from key_map to revoked_key_map
-                self.key_map[role_name].remove(old_key_name)
-                # to ensure continuity, changes to root must be signed both
-                # with the new key and the old key (in addition to unmodified
-                # keys), so we keep track of revoked keys until signed
-                self.revoked_key_names.append(old_key_name)
-                logger.debug(f'Key revoked for {role_name}: {old_key_name}')
-            except ValueError:
-                logger.debug(f'{role_name} does not have key {old_key_name}')
-            else:
-                # add new key_id
-                self.add_key(
-                    role_name=role_name,
-                    public_key_path=new_public_key_path,
-                    encrypted=new_private_key_encrypted,
-                )
-
-    def add_key(
-            self,
-            role_name: str,
-            public_key_path: Union[pathlib.Path, str],
-            encrypted: bool,
-    ):
-        """
-        Register a new public key for the specified role.
-
-        Note the changes are not published yet: call publish_changes() for that.
-        """
-        public_key_path = pathlib.Path(public_key_path)
-        # add new key to metadata
-        self.roles.add_public_key(
-            role_name=role_name, public_key_path=public_key_path
-        )
-        # add new key to key map
-        key_name = public_key_path.with_suffix('').name
-        if key_name not in self.key_map[role_name]:
-            self.key_map[role_name].append(key_name)
-        # add new key to encrypted keys if necessary
-        already_present = key_name in self.encrypted_keys
-        if encrypted and not already_present:
-            self.encrypted_keys.append(key_name)
-
-    def add_bundle(
-            self,
-            new_bundle_dir: Union[pathlib.Path, str],
-            new_version: Optional[str] = None,
-            skip_patch: bool = False,
-    ):
-        """
-        Adds a new application bundle to the local repository.
-
-        An archive file is created from the app bundle, and this file is
-        added to the tuf repository. If a previous archive version is found,
-        a patch file is also created and added to the repository, unless
-        `skip_patch` is True.
-
-        Note the changes are not published yet: call `publish_changes()` for
-        that.
-        """
-        # enforce path object
-        new_bundle_dir = pathlib.Path(new_bundle_dir)
-        # determine new version
-        if new_version is None:
-            # todo: should we check for a valid version string?
-            new_version = self.app_version
-        # create archive from latest app bundle
-        logger.info(f'Creating new archive from bundle: {new_bundle_dir}')
-        new_archive = make_gztar_archive(
-            src_dir=new_bundle_dir,
-            dst_dir=self.targets_dir,
-            app_name=self.app_name,
-            version=new_version,
-        )
-        logger.info(f'Archive ready: {new_archive}')
-        # check latest archive before registering the new one
-        latest_archive = self.roles.get_latest_archive()
-        if not latest_archive or latest_archive.version < new_archive.version:
-            # register new archive
-            self.roles.add_or_update_target(local_path=new_archive.path)
-            # create patch, if possible, and register that too
-            if latest_archive and not skip_patch:
-                patch_path = Patcher.create_patch(
-                    src_path=self.targets_dir / latest_archive.path,
-                    dst_path=self.targets_dir / new_archive.path,
-                )
-                self.roles.add_or_update_target(local_path=patch_path)
-
-    def remove_latest_bundle(self):
-        """
-        Removes the *latest* app bundle from the local repository.
-
-        This deletes the bundle's archive file and corresponding patch file
-        from the targets directory, and updates the tuf repository metadata
-        accordingly.
-
-        Note the changes are not published yet: call publish_changes() for that
-        """
-        # Get latest archive
-        latest_archive = self.roles.get_latest_archive()
-        if latest_archive:
-            # remove latest archive and corresponding patch
-            archive_path = self.targets_dir / latest_archive.target_path_str
-            patch_path = archive_path.with_suffix('').with_suffix(SUFFIX_PATCH)
-            for target_path in [archive_path, patch_path]:
-                removed = self.roles.remove_target(local_path=target_path)
-                logger.info(
-                    f'target {"removed" if removed else "not found"}: {target_path}'
-                )
-
-    def publish_changes(self, private_key_dirs: List[Union[pathlib.Path, str]]):
-        """
-        Publish all modified roles. That is, if a role has changed w.r.t. to
-        the version on disk:
-
-        - update expiration date (if not yet updated)
-        - bump version (if not yet bumped)
-        - sign
-        - save to disk
-
-        If a role has not been modified, it is skipped.
-        """
-        # todo: implement custom Metadata subclass with extra methods:
-        #  modified, set_expiration_date, sign, persist, etc. So we can do
-        #  e.g role.set_expiration_date(days=1) instead of passing the
-        #  role_name around
-        for role_name in ['root', 'targets', 'snapshot', 'timestamp']:
-            role = getattr(self.roles, role_name)
-            # filename without version is always the latest version
-            latest_file_path = self.roles.file_path(
-                role_name=role_name, version=None
-            )
-            # if the file does not exist yet, the role is considered modified,
-            # and we don't want to bump version and expiration date again
-            modified = True
-            expires_bumped = True
-            version_bumped = True
-            if latest_file_path.exists():
-                latest_role = Metadata.from_file(filename=str(latest_file_path))
-                modified = role.signed != latest_role.signed
-                expires_bumped = role.signed.expires != latest_role.signed.expires
-                version_bumped = role.signed.version > latest_role.signed.version
-            if modified:
-                # set new expiration date
-                if not expires_bumped:
-                    self.roles.set_expiration_date(
-                        role_name=role_name,
-                        days=self.expiration_days.get(role_name),
-                    )
-                # bump version
-                if not version_bumped:
-                    role.signed.version += 1
-                # sign metadata and persist changes
-                role.signatures.clear()
-                self.threshold_sign(
-                    role_name=role_name, private_key_dirs=private_key_dirs
-                )
-                # update version in dependent metadata
-                dependent = None
-                if role_name == 'root':
-                    # Not all changes to root require a re-sign of the other
-                    # metadata files (e.g. we could just add some additional
-                    # valid keys). However, to be on the safe side,
-                    # we'll force a re-sign cascade by bumping the targets
-                    # version. Note this may cause a double version bump for
-                    # targets, but that should not matter.
-                    if self.roles.file_path(
-                            role_name='targets', version=None
-                    ).exists():
-                        self.roles.targets.signed.version += 1
-                elif role_name == 'targets':
-                    dependent = self.roles.snapshot.signed.meta[FILENAME_TARGETS]
-                elif role_name == 'snapshot':
-                    dependent = self.roles.timestamp.signed.snapshot_meta
-                if dependent:
-                    dependent.version = role.signed.version
-                logger.info(f'Published changes for {role_name}.')
-            else:
-                logger.info(f'No changes detected for {role_name}.')
-                # Check if signature count meets threshold
-                threshold = self.roles.root.signed.roles[role_name].threshold
-                if len(role.signatures) < threshold:
-                    logger.info(
-                        f'{role_name} threshold not met. Trying to sign...'
-                    )
-                    signature_count = self.threshold_sign(
-                        role_name=role_name, private_key_dirs=private_key_dirs
-                    )
-                    logger.info(f'Added {signature_count} signatures.')
-        # update config if key_map has changed
-        if self.config_dict != self.load_config():
-            self.save_config()
-            logger.info('Config file updated.')
-
-    def threshold_sign(
-            self,
-            role_name: str,
-            private_key_dirs: List[Union[pathlib.Path, str]],
-    ) -> int:
-        """
-        Sign the metadata file for a specific role, and save changes to disk.
-
-        Use this to sign and save without making any changes to the actual
-        signed metadata.
-
-        In case of root key rotation, both the old private key and the new
-        private key are required.
-
-        Returns the number of signatures created.
-        """
-        signature_count = 0
-        # sign role with all required keys that can be found
-        key_names = set(self.key_map.get(role_name, []))
-        if role_name == 'root':
-            # set ensures uniqueness
-            key_names = key_names.union(self.revoked_key_names)
-        for key_name in key_names:
-            private_key_path = self.keys.find_private_key(
-                key_name=key_name, key_dirs=private_key_dirs
-            )
-            if private_key_path:
-                self.roles.sign_role(
-                    role_name=role_name,
-                    private_key_path=private_key_path,
-                )
-                signature_count += 1
-                if key_name in self.revoked_key_names:
-                    self.revoked_key_names.remove(key_name)
-                    if key_name in self.encrypted_keys:
-                        self.encrypted_keys.remove(key_name)
-            else:
-                logger.warning(f'Private key not found: {key_name}')
-        if not signature_count:
-            raise Exception(f'No private keys found for {role_name}.')
-        # save changes to disk
-        self.roles.persist_role(role_name=role_name)
-        return signature_count
-
-    def _load_keys_and_roles(self, create_keys: bool = False):
-        # todo: make public, rename load_keys_and_metadata
-        if self.keys is None:
-            logger.info('Importing public keys...')
-            self.keys = Keys(
-                dir_path=self.keys_dir,
-                encrypted=self.encrypted_keys,
-                key_map=self.key_map,
-                thresholds=self.thresholds,
-            )
-            if create_keys:
-                # safe to call if keys exist
-                self.keys.create()
-            logger.info('Public keys imported.')
-        if self.roles is None:
-            logger.info('Importing metadata...')
-            self.roles = Roles(dir_path=self.metadata_dir)
-            self.roles.initialize(
-                keys=self.keys, expiration_days=self.expiration_days
-            )
-            logger.info('Metadata imported.')
+from copy import deepcopy
+from datetime import datetime, timedelta
+import inspect
+import json
+import logging
+import pathlib
+try:
+    # workaround for PyInstaller issue 6911 (setuptools issue 3089)
+    import setuptools.config.expand  # noqa
+except AssertionError as e:
+    pass  # assuming we are on the client side...
+import shutil
+from typing import Any, Dict, Iterable, List, Optional, TypedDict, Union
+
+from securesystemslib.exceptions import CryptoError
+from securesystemslib.interface import (
+    generate_and_write_ed25519_keypair_with_prompt,
+    generate_and_write_unencrypted_ed25519_keypair,
+    import_ed25519_publickey_from_file,
+    import_ed25519_privatekey_from_file,
+)
+# SSlibKey see: https://github.com/secure-systems-lab/securesystemslib/pull/456
+from securesystemslib.signer import SSlibKey, SSlibSigner
+from tuf.api.metadata import (
+    SPECIFICATION_VERSION,
+    TOP_LEVEL_ROLE_NAMES,
+    Metadata,
+    MetaFile,
+    Role,
+    Root,
+    Snapshot,
+    TargetFile,
+    Targets,
+    Timestamp,
+)
+from tuf.api.serialization.json import JSONSerializer
+
+from tufup.common import Patcher, SUFFIX_ARCHIVE, SUFFIX_PATCH, TargetMeta
+
+logger = logging.getLogger(__name__)
+
+"""
+
+https://github.com/theupdateframework/python-tuf/blob/develop/examples/repo_example/basic_repo.py
+
+"""
+
+__all__ = [
+    'DEFAULT_KEY_MAP',
+    'DEFAULT_KEYS_DIR_NAME',
+    'DEFAULT_META_DIR_NAME',
+    'DEFAULT_REPO_DIR_NAME',
+    'DEFAULT_TARGETS_DIR_NAME',
+    'in_',
+    'Keys',
+    'make_gztar_archive',
+    'Repository',
+    'Roles',
+    'SUFFIX_JSON',
+    'SUFFIX_PUB',
+    'TOP_LEVEL_ROLE_NAMES',
+]
+
+# copied from python-tuf basic_repo.py
+SPEC_VERSION = ".".join(SPECIFICATION_VERSION)
+
+
+# copied from python-tuf basic_repo.py
+def in_(days: float) -> datetime:
+    """Returns a timestamp for the specified number of days from now."""
+    return datetime.utcnow().replace(microsecond=0) + timedelta(days=days)
+
+
+def make_gztar_archive(
+        src_dir: Union[pathlib.Path, str],
+        dst_dir: Union[pathlib.Path, str],
+        app_name: str,
+        version: str,
+        **kwargs,  # allowed kwargs are passed on to shutil.make_archive
+) -> Optional[TargetMeta]:
+    # remove disallowed kwargs
+    for key in ['base_name', 'root_dir', 'format']:
+        if kwargs.pop(key, None):
+            logger.warning(f'{key} ignored: using default')
+    # ensure paths
+    src_dir = pathlib.Path(src_dir)
+    dst_dir = pathlib.Path(dst_dir)
+    # compose archive path and check existence
+    archive_filename = TargetMeta.compose_filename(
+        name=app_name, version=version, is_archive=True
+    )
+    archive_path = dst_dir / archive_filename
+    if archive_path.exists():
+        if input(f'Found existing archive: {archive_path}.\nOverwrite? [n]/y') != 'y':
+            print('Using existing archive.')
+            return TargetMeta(archive_path)
+    # make archive
+    base_name = str(dst_dir / archive_filename.replace(SUFFIX_ARCHIVE, ''))
+    archive_path_str = shutil.make_archive(
+        base_name=base_name,  # archive file path, no suffix
+        root_dir=str(src_dir),  # paths in archive will be relative to root_dir
+        format='gztar',
+        **kwargs,
+    )
+    return TargetMeta(target_path=archive_path_str)
+
+
+class RolesDict(TypedDict):
+    root: Any
+    targets: Any
+    snapshot: Any
+    timestamp: Any
+
+
+DEFAULT_REPO_DIR_NAME = 'repository'
+DEFAULT_KEYS_DIR_NAME = 'keystore'
+DEFAULT_META_DIR_NAME = 'metadata'
+DEFAULT_TARGETS_DIR_NAME = 'targets'
+DEFAULT_KEY_MAP = RolesDict((key, [key]) for key in TOP_LEVEL_ROLE_NAMES)  # noqa
+DEFAULT_EXPIRATION_DAYS = RolesDict(root=365, targets=7, snapshot=7, timestamp=1)
+DEFAULT_THRESHOLDS = RolesDict(root=1, targets=1, snapshot=1, timestamp=1)
+SUFFIX_JSON = '.json'
+SUFFIX_PUB = '.pub'
+FILENAME_ROOT = Root.type + SUFFIX_JSON
+FILENAME_TARGETS = Targets.type + SUFFIX_JSON
+FILENAME_SNAPSHOT = Snapshot.type + SUFFIX_JSON
+FILENAME_TIMESTAMP = Timestamp.type + SUFFIX_JSON
+
+
+class Base(object):
+    def __init__(self, dir_path: Union[pathlib.Path, str, None]):
+        """
+        dir_path: directory where all key files are stored
+        encrypted: names of the keys that are (to be) encrypted
+        key_map: maps top-level role names to lists of key names
+        """
+        if dir_path is None:
+            dir_path = pathlib.Path.cwd()
+        # enforce pathlib.Path
+        self.dir_path = pathlib.Path(dir_path)
+        if not self.dir_path.exists():
+            if input(f'Create directory {self.dir_path}? [y]/n') in ['y', '']:
+                self.dir_path.mkdir(parents=True)
+                print(f'Directory created: {self.dir_path}')
+
+
+class Keys(Base):
+    filename_pattern = '{key_name}'
+
+    def __init__(
+            self,
+            dir_path: Union[pathlib.Path, str, None] = None,
+            encrypted: Optional[List[str]] = None,
+            key_map: Optional[RolesDict] = None,
+            thresholds: Optional[RolesDict] = None,
+    ):
+        if dir_path is None:
+            dir_path = pathlib.Path.cwd() / DEFAULT_KEYS_DIR_NAME
+        super().__init__(dir_path=dir_path)
+        if encrypted is None:
+            encrypted = []
+        if key_map is None:
+            key_map = deepcopy(DEFAULT_KEY_MAP)
+        if thresholds is None:
+            thresholds = DEFAULT_THRESHOLDS.copy()
+        self.encrypted = encrypted
+        self.key_map = key_map
+        self.thresholds = thresholds
+        # top-level roles
+        self.root: List[Dict[str, Any]] = []
+        self.targets: List[Dict[str, Any]] = []
+        self.snapshot: List[Dict[str, Any]] = []
+        self.timestamp: List[Dict[str, Any]] = []
+        # import public keys from dir_path, if it exists
+        self.import_all_public_keys()
+
+    def import_all_public_keys(self):
+        for role_name, key_list in self.key_map.items():
+            for key_name in key_list:
+                self.import_public_key(role_name=role_name, key_name=key_name)
+
+    def import_public_key(self, role_name: str, key_name: Optional[str] = None):
+        """Import public key for specified role."""
+        if key_name is None:
+            key_name = role_name
+        public_key_path = self.public_key_path(key_name=key_name)
+        if public_key_path.exists():
+            ssl_key = import_ed25519_publickey_from_file(
+                filepath=str(public_key_path)
+            )
+            getattr(self, role_name).append(ssl_key)
+            logger.debug(f'public key imported: {public_key_path}')
+        else:
+            logger.debug(f'file does not exist: {public_key_path}')
+
+    def create(self):
+        all_key_names = []
+        for key_list in self.key_map.values():
+            all_key_names.extend(key_list)
+        unique_key_names = set(all_key_names)
+        logger.debug(f'creating key-pairs: {unique_key_names}')
+        for key_name in unique_key_names:
+            default_private_key_path = self.private_key_path(key_name=key_name)
+            self.create_key_pair(
+                private_key_path=default_private_key_path,
+                encrypted=key_name in self.encrypted,
+            )
+        # import the newly created public keys
+        self.import_all_public_keys()
+
+    @staticmethod
+    def create_key_pair(
+            private_key_path: pathlib.Path, encrypted: bool
+    ) -> pathlib.Path:
+        if encrypted:
+            # encrypt private key
+            logger.debug(f'set encryption password for private key')
+            generate_keypair = generate_and_write_ed25519_keypair_with_prompt
+        else:
+            # do not encrypt private key (for automated signing)
+            generate_keypair = generate_and_write_unencrypted_ed25519_keypair
+        public_key_path = private_key_path.with_suffix(SUFFIX_PUB)
+        proceed = True
+        if public_key_path.exists():
+            logger.warning(f'Public key already exists: {public_key_path}')
+            proceed = input(f'Overwrite key pair? [n]/y') == 'y'
+        if proceed:
+            file_path_str = generate_keypair(filepath=str(private_key_path))
+            logger.info(f'key-pair created: {file_path_str}, {public_key_path}')
+        return public_key_path
+
+    def private_key_path(self, key_name: str) -> pathlib.Path:
+        return self.dir_path / self.filename_pattern.format(key_name=key_name)
+
+    def public_key_path(self, key_name: str) -> pathlib.Path:
+        return self.private_key_path(key_name=key_name).with_suffix(SUFFIX_PUB)
+
+    def public(self):
+        # return a dict that maps key ids to *public* key objects
+        return {
+            ssl_key['keyid']: SSlibKey.from_securesystemslib_key(key_dict=ssl_key)
+            for attr_name, ssl_keys in vars(self).items()
+            if attr_name in TOP_LEVEL_ROLE_NAMES
+            for ssl_key in ssl_keys
+        }
+
+    def roles(self):
+        # return a dict that maps role names to key ids and key thresholds
+        roles_map = dict()
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            ssl_keys = getattr(self, role_name)
+            role_keys = None
+            if ssl_keys:
+                unique_key_ids = list(set(ssl_key['keyid'] for ssl_key in ssl_keys))
+                role_keys = Role(
+                    keyids=unique_key_ids, threshold=self.thresholds[role_name]
+                )
+            roles_map[role_name] = role_keys
+        return roles_map
+
+    @classmethod
+    def find_private_key(cls, key_name: str, key_dirs: List[Union[pathlib.Path, str]]):
+        private_key_path = None
+        private_key_filename = cls.filename_pattern.format(key_name=key_name)
+        for key_dir in key_dirs:
+            key_dir = pathlib.Path(key_dir)  # ensure Path
+            for path in key_dir.iterdir():
+                if path.is_file() and path.name == private_key_filename:
+                    private_key_path = path
+                    break
+        return private_key_path
+
+
+class Roles(Base):
+    filename_pattern = '{version}{role_name}{suffix}'
+
+    def __init__(self, dir_path: Union[pathlib.Path, str, None] = None):
+        """
+        TUF roles
+
+        - root metadata tells us:
+            + all the known keys (key id and public key value)
+            + which keys belong to each role
+            + how many signatures are needed for each role
+        - targets metadata tells us:
+            + which target files are available (filename, size, hash)
+        - snapshots metatadata tells us:
+            + which version of the targets-metadata file to expect
+        - timestamp metadata tells us:
+            + which version of the snapshot-metadata file to expect
+
+        """
+        if dir_path is None:
+            dir_path = pathlib.Path.cwd() / DEFAULT_META_DIR_NAME
+        super().__init__(dir_path=dir_path)
+        # top-level roles
+        self.root: Optional[Metadata[Root]] = None
+        self.targets: Optional[Metadata[Targets]] = None
+        self.snapshot: Optional[Metadata[Snapshot]] = None
+        self.timestamp: Optional[Metadata[Timestamp]] = None
+        # import roles from dir_path, if it exists
+        self._import_roles(role_names=TOP_LEVEL_ROLE_NAMES)
+
+    def _import_roles(self, role_names: Iterable[str]):
+        """Import roles from metadata files."""
+        file_paths = []
+        if self.dir_path.exists():
+            file_paths = [p for p in self.dir_path.iterdir() if p.is_file()]
+        for role_name in role_names:
+            # exclude (root) filenames starting with a version
+            role_paths = [p for p in file_paths if p.name.startswith(role_name)]
+            if role_paths:
+                # there should be only one for each role
+                setattr(self, role_name, Metadata.from_file(str(role_paths[0])))
+
+    def initialize(
+            self, keys: Keys, expiration_days: Optional[RolesDict] = None
+    ):
+        if expiration_days is None:
+            expiration_days = DEFAULT_EXPIRATION_DAYS.copy()
+        # based on python-tuf basic_repo.py
+        common_kwargs = dict(version=1, spec_version=SPEC_VERSION)
+        # role-specific kwargs
+        initial_data = {
+            Root: dict(
+                expires=in_(expiration_days['root']),
+                keys=keys.public(),
+                roles=keys.roles(),
+                # repo is relatively static, no need for consistent snapshots
+                consistent_snapshot=False,
+            ),
+            Targets: dict(
+                expires=in_(expiration_days['targets']),
+                targets=dict(),
+            ),
+            Snapshot: dict(
+                expires=in_(expiration_days['snapshot']),
+                meta={FILENAME_TARGETS: MetaFile(version=1)},
+            ),
+            Timestamp: dict(
+                expires=in_(expiration_days['timestamp']),
+                snapshot_meta=MetaFile(version=1),
+            ),
+        }
+        for role_class, role_kwargs in initial_data.items():
+            attr_name = role_class.type
+            if getattr(self, attr_name) is None:
+                # intialize role only if there is no role yet
+                setattr(
+                    self,
+                    attr_name,
+                    Metadata(
+                        signed=role_class(**common_kwargs, **role_kwargs),
+                        signatures=dict(),
+                    ),
+                )
+
+    def add_or_update_target(
+            self,
+            local_path: Union[pathlib.Path, str],
+            url_path_segments: Optional[List[str]] = None,
+    ):
+        # based on python-tuf basic_repo.py
+        local_path = pathlib.Path(local_path)
+        # build url path
+        url_path_segments = url_path_segments or []
+        url_path_segments.append(local_path.name)
+        url_path = '/'.join(url_path_segments)
+        target_file_info = TargetFile.from_file(
+            target_file_path=url_path, local_path=str(local_path)
+        )
+        # note we assume self.targets has been initialized
+        self.targets.signed.targets[url_path] = target_file_info
+
+    def remove_target(self, local_path: Union[pathlib.Path, str]) -> bool:
+        removed = False
+        targets_dict = self.targets.signed.targets
+        for target_url in targets_dict:
+            # assume target filenames only occur once
+            if target_url.endswith(local_path.name):
+                removed = targets_dict.pop(target_url, None) is not None
+                break
+        if removed:
+            local_path.unlink()
+        return removed
+
+    def add_public_key(
+            self, role_name: str, public_key_path: Union[pathlib.Path, str]
+    ):
+        """Import a public key from file and add it to the specified role."""
+        # based on python-tuf basic_repo.py
+        ssl_key = import_ed25519_publickey_from_file(filepath=str(public_key_path))
+        self.root.signed.add_key(
+            role=role_name, key=SSlibKey.from_securesystemslib_key(ssl_key)
+        )
+
+    def set_signature_threshold(self, role_name: str, threshold: int):
+        self.root.signed.roles[role_name].threshold = threshold
+
+    def set_expiration_date(self, role_name: str, days: int):
+        role = getattr(self, role_name)
+        if hasattr(role, 'signed'):
+            role.signed.expires = in_(days)
+
+    def sign_role(
+            self, role_name: str, private_key_path: Union[pathlib.Path, str]
+    ):
+        """
+        Sign role using specified private key.
+
+        We sign off on the role.signed part, and the signature is added to
+        the role.signatures list.
+        """
+        # based on python-tuf basic_repo.py
+        try:
+            # assume unencrypted
+            ssl_key = import_ed25519_privatekey_from_file(
+                filepath=str(private_key_path), prompt=False
+            )
+        except CryptoError as e:
+            # possibly encrypted: try to import with password
+            logger.debug(f'private key import attempt without password failed: {e}')
+            ssl_key = import_ed25519_privatekey_from_file(
+                filepath=str(private_key_path), prompt=True
+            )
+        signer = SSlibSigner(ssl_key)
+        getattr(self, role_name).sign(signer, append=True)
+
+    def file_path(self, role_name: str, version: Optional[int] = None):
+        version_str = ''
+        if role_name == Root.type and version is not None:
+            # "... all released versions of root metadata files MUST always
+            # be provided so that outdated clients can update to the latest
+            # available root."
+            # https://theupdateframework.github.io/specification/latest/#writing-consistent-snapshots
+            version_str = f'{version}.'
+        return self.dir_path / self.filename_pattern.format(
+            version=version_str, role_name=role_name, suffix=SUFFIX_JSON
+        )
+
+    def file_exists(self, role_name: str):
+        """
+        Return True if any metadata file exists for the specified role,
+        ignoring any versions in the filename.
+        """
+        return any(
+            path.exists() for path in self.dir_path.iterdir()
+            if path.is_file() and role_name in path.name
+        )
+
+    def persist_role(self, role_name: str):
+        """
+        Save specified role to corresponding metadata file.
+
+        In case of root, make sure "root.json" always represents the latest
+        version (in addition to x.root.json).
+        """
+        # based on python-tuf basic_repo.py (but without consistent snapshots)
+        role = getattr(self, role_name)
+        file_path = self.file_path(
+            role_name=role_name, version=role.signed.version
+        )
+        role.to_file(
+            filename=str(file_path), serializer=JSONSerializer(compact=False)
+        )
+        if role_name == Root.type:
+            # Copy the latest root metadata to 'root.json' (without version),
+            # to use as trusted root metadata for distribution with the
+            # client. This is convenient, otherwise we would need to modify
+            # the version in the filename every time root is updated.
+            # Moreover, we can now easily access the latest root metadata,
+            # without having to check the version in the filename.
+            client_root_file_path = self.file_path(role_name=Root.type)
+            client_root_file_path.unlink(missing_ok=True)
+            shutil.copy(src=file_path, dst=client_root_file_path)
+
+    def get_latest_archive(self) -> Optional[TargetMeta]:
+        """
+        Returns TargetMeta for latest archive.
+
+        Note that all pre-release versions are always included: On the repo
+        side, there is no difference between final releases an pre-releases.
+        Pre-release specifiers are only used on the Client side, to filter
+        available updates).
+        """
+        # Note this is similar to the logic in Client._check_updates, but not
+        # exactly the same. Merging the implementations would overcomplicate
+        # things.
+        latest_archive = None
+        # sort by version
+        signed_targets = self.targets.signed.targets if self.targets else dict()
+        targets = sorted(
+            TargetMeta(key) for key in signed_targets.keys()
+        )
+        # extract only the archives
+        archives = [target for target in targets if target.is_archive]
+        if archives:
+            latest_archive = archives[-1]
+        return latest_archive
+
+
+class Repository(object):
+    """High-level tools for repository management."""
+    config_filename = '.tufup-repo-config'
+
+    def __init__(
+            self,
+            app_name: str,
+            app_version_attr: Optional[str] = None,
+            repo_dir: Union[pathlib.Path, str, None] = None,
+            keys_dir: Union[pathlib.Path, str, None] = None,
+            key_map: Optional[RolesDict] = None,
+            encrypted_keys: Optional[List[str]] = None,
+            expiration_days: Optional[RolesDict] = None,
+            thresholds: Optional[RolesDict] = None,
+    ):
+        if repo_dir is None:
+            repo_dir = pathlib.Path.cwd() / DEFAULT_REPO_DIR_NAME
+        if keys_dir is None:
+            keys_dir = pathlib.Path.cwd() / DEFAULT_KEYS_DIR_NAME
+        if key_map is None:
+            key_map = deepcopy(DEFAULT_KEY_MAP)
+        if encrypted_keys is None:
+            encrypted_keys = []
+        if expiration_days is None:
+            expiration_days = DEFAULT_EXPIRATION_DAYS.copy()
+        if thresholds is None:
+            thresholds = DEFAULT_THRESHOLDS.copy()
+        self.app_name = app_name
+        self.app_version_attr = app_version_attr
+        # force path object and resolve, in case of relative paths
+        self.repo_dir = pathlib.Path(repo_dir).resolve()
+        self.keys_dir = pathlib.Path(keys_dir).resolve()
+        self.key_map = key_map
+        self.encrypted_keys = encrypted_keys
+        self.expiration_days = expiration_days
+        self.thresholds = thresholds
+        # keys and roles
+        self.keys: Optional[Keys] = None
+        self.roles: Optional[Roles] = None
+        self.revoked_key_names = []
+
+    @property
+    def config_dict(self):
+        """dict to be saved to configuration file."""
+        # attributes matching __init__ arguments are stored as configuration
+        config_items = inspect.signature(self.__init__).parameters.keys()
+        return {item: getattr(self, item) for item in config_items}
+
+    @property
+    def metadata_dir(self) -> pathlib.Path:
+        return self.repo_dir / DEFAULT_META_DIR_NAME
+
+    @property
+    def targets_dir(self) -> pathlib.Path:
+        return self.repo_dir / DEFAULT_TARGETS_DIR_NAME
+
+    @property
+    def app_version(self) -> str:
+        # read version from specified module attribute without importing
+        version = ''
+        if self.app_version_attr:
+            version = str(
+                setuptools.config.expand.read_attr(self.app_version_attr)  # noqa
+            )
+        return version
+
+    @classmethod
+    def get_config_file_path(cls) -> pathlib.Path:
+        return pathlib.Path.cwd() / cls.config_filename
+
+    def save_config(self):
+        """Save current configuration."""
+        # todo: write directories relative to config file dir?
+        file_path = self.get_config_file_path()
+        file_path.write_text(
+            data=json.dumps(
+                self.config_dict, default=str, sort_keys=True, indent=4
+            ),
+            encoding='utf-8',
+        )
+
+    @classmethod
+    def load_config(cls) -> dict:
+        """Load configuration dict from file."""
+        file_path = cls.get_config_file_path()
+        config_dict = dict()
+        try:
+            config_dict = json.loads(file_path.read_text())
+        except FileNotFoundError:
+            logger.warning(f'config file not found: {file_path}')
+        except json.JSONDecodeError:
+            logger.warning(f'config file invalid: {file_path}')
+        return config_dict
+
+    @classmethod
+    def from_config(cls):
+        """Create Repository instance from configuration file."""
+        instance = cls(**cls.load_config())
+        instance._load_keys_and_roles(create_keys=False)
+        return instance
+
+    def initialize(self):
+        """
+        Initialize (or update) the local repository.
+
+        This includes:
+
+        - create directories if they do not exist
+        - import public keys from existing files, or create new key pairs
+        - import roles from existing metadata files
+        - create root metadata file if it does not exist
+
+        Safe to call for existing keys and roles.
+        """
+        # Ensure dirs exist
+        for path in [self.keys_dir, self.metadata_dir, self.targets_dir]:
+            path.mkdir(parents=True, exist_ok=True)
+
+        # Load keys and roles
+        self._load_keys_and_roles(create_keys=True)
+
+        # Publish root metadata (save 1.root.json and copy to root.json)
+        if not self.roles.file_path('root').exists():
+            self.publish_changes(private_key_dirs=[self.keys_dir])
+
+    def refresh_expiration_date(self, role_name: str, days: Optional[int] = None):
+        if days is None:
+            days = self.expiration_days.get(role_name)
+        self.roles.set_expiration_date(role_name=role_name, days=days)
+
+    def replace_key(
+            self,
+            old_key_name: str,
+            new_public_key_path: Union[pathlib.Path, str],
+            new_private_key_encrypted: bool,
+    ):
+        """
+        Replace an existing key by a new one, e.g. after a key compromise.
+
+        Note the changes are not published yet: call publish_changes() for that.
+        """
+        self.revoked_key_names = []
+        # Load old public key from file to obtain its key_id
+        public_key_path = self.keys.public_key_path(key_name=old_key_name)
+        old_key_id = import_ed25519_publickey_from_file(
+            filepath=str(public_key_path)
+        )['keyid']
+        # Get new key name from public key path
+        new_public_key_path = pathlib.Path(new_public_key_path)  # force path
+        # A key may be used for multiple roles, so we check the key id for
+        # all roles.
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            try:
+                # remove old key_id from roles dict, if found, and remove key
+                # from keys dict if it is no longer used by any roles
+                self.roles.root.signed.revoke_key(
+                    role=role_name, keyid=old_key_id
+                )
+                # move old key name from key_map to revoked_key_map
+                self.key_map[role_name].remove(old_key_name)
+                # to ensure continuity, changes to root must be signed both
+                # with the new key and the old key (in addition to unmodified
+                # keys), so we keep track of revoked keys until signed
+                self.revoked_key_names.append(old_key_name)
+                logger.debug(f'Key revoked for {role_name}: {old_key_name}')
+            except ValueError:
+                logger.debug(f'{role_name} does not have key {old_key_name}')
+            else:
+                # add new key_id
+                self.add_key(
+                    role_name=role_name,
+                    public_key_path=new_public_key_path,
+                    encrypted=new_private_key_encrypted,
+                )
+
+    def add_key(
+            self,
+            role_name: str,
+            public_key_path: Union[pathlib.Path, str],
+            encrypted: bool,
+    ):
+        """
+        Register a new public key for the specified role.
+
+        Note the changes are not published yet: call publish_changes() for that.
+        """
+        public_key_path = pathlib.Path(public_key_path)
+        # add new key to metadata
+        self.roles.add_public_key(
+            role_name=role_name, public_key_path=public_key_path
+        )
+        # add new key to key map
+        key_name = public_key_path.with_suffix('').name
+        if key_name not in self.key_map[role_name]:
+            self.key_map[role_name].append(key_name)
+        # add new key to encrypted keys if necessary
+        already_present = key_name in self.encrypted_keys
+        if encrypted and not already_present:
+            self.encrypted_keys.append(key_name)
+
+    def add_bundle(
+            self,
+            new_bundle_dir: Union[pathlib.Path, str],
+            new_version: Optional[str] = None,
+            skip_patch: bool = False,
+    ):
+        """
+        Adds a new application bundle to the local repository.
+
+        An archive file is created from the app bundle, and this file is
+        added to the tuf repository. If a previous archive version is found,
+        a patch file is also created and added to the repository, unless
+        `skip_patch` is True.
+
+        Note the changes are not published yet: call `publish_changes()` for
+        that.
+        """
+        # enforce path object
+        new_bundle_dir = pathlib.Path(new_bundle_dir)
+        # determine new version
+        if new_version is None:
+            # todo: should we check for a valid version string?
+            new_version = self.app_version
+        # create archive from latest app bundle
+        logger.info(f'Creating new archive from bundle: {new_bundle_dir}')
+        new_archive = make_gztar_archive(
+            src_dir=new_bundle_dir,
+            dst_dir=self.targets_dir,
+            app_name=self.app_name,
+            version=new_version,
+        )
+        logger.info(f'Archive ready: {new_archive}')
+        # check latest archive before registering the new one
+        latest_archive = self.roles.get_latest_archive()
+        if not latest_archive or latest_archive.version < new_archive.version:
+            # register new archive
+            self.roles.add_or_update_target(local_path=new_archive.path)
+            # create patch, if possible, and register that too
+            if latest_archive and not skip_patch:
+                patch_path = Patcher.create_patch(
+                    src_path=self.targets_dir / latest_archive.path,
+                    dst_path=self.targets_dir / new_archive.path,
+                )
+                self.roles.add_or_update_target(local_path=patch_path)
+
+    def remove_latest_bundle(self):
+        """
+        Removes the *latest* app bundle from the local repository.
+
+        This deletes the bundle's archive file and corresponding patch file
+        from the targets directory, and updates the tuf repository metadata
+        accordingly.
+
+        Note the changes are not published yet: call publish_changes() for that
+        """
+        # Get latest archive
+        latest_archive = self.roles.get_latest_archive()
+        if latest_archive:
+            # remove latest archive and corresponding patch
+            archive_path = self.targets_dir / latest_archive.target_path_str
+            patch_path = archive_path.with_suffix('').with_suffix(SUFFIX_PATCH)
+            for target_path in [archive_path, patch_path]:
+                removed = self.roles.remove_target(local_path=target_path)
+                logger.info(
+                    f'target {"removed" if removed else "not found"}: {target_path}'
+                )
+
+    def publish_changes(self, private_key_dirs: List[Union[pathlib.Path, str]]):
+        """
+        Publish all modified roles. That is, if a role has changed w.r.t. to
+        the version on disk:
+
+        - update expiration date (if not yet updated)
+        - bump version (if not yet bumped)
+        - sign
+        - save to disk
+
+        If a role has not been modified, it is skipped.
+        """
+        # todo: implement custom Metadata subclass with extra methods:
+        #  modified, set_expiration_date, sign, persist, etc. So we can do
+        #  e.g role.set_expiration_date(days=1) instead of passing the
+        #  role_name around
+        for role_name in ['root', 'targets', 'snapshot', 'timestamp']:
+            role = getattr(self.roles, role_name)
+            # filename without version is always the latest version
+            latest_file_path = self.roles.file_path(
+                role_name=role_name, version=None
+            )
+            # if the file does not exist yet, the role is considered modified,
+            # and we don't want to bump version and expiration date again
+            modified = True
+            expires_bumped = True
+            version_bumped = True
+            if latest_file_path.exists():
+                latest_role = Metadata.from_file(filename=str(latest_file_path))
+                modified = role.signed != latest_role.signed
+                expires_bumped = role.signed.expires != latest_role.signed.expires
+                version_bumped = role.signed.version > latest_role.signed.version
+            if modified:
+                # set new expiration date
+                if not expires_bumped:
+                    self.roles.set_expiration_date(
+                        role_name=role_name,
+                        days=self.expiration_days.get(role_name),
+                    )
+                # bump version
+                if not version_bumped:
+                    role.signed.version += 1
+                # sign metadata and persist changes
+                role.signatures.clear()
+                self.threshold_sign(
+                    role_name=role_name, private_key_dirs=private_key_dirs
+                )
+                # update version in dependent metadata
+                dependent = None
+                if role_name == 'root':
+                    # Not all changes to root require a re-sign of the other
+                    # metadata files (e.g. we could just add some additional
+                    # valid keys). However, to be on the safe side,
+                    # we'll force a re-sign cascade by bumping the targets
+                    # version. Note this may cause a double version bump for
+                    # targets, but that should not matter.
+                    if self.roles.file_path(
+                            role_name='targets', version=None
+                    ).exists():
+                        self.roles.targets.signed.version += 1
+                elif role_name == 'targets':
+                    dependent = self.roles.snapshot.signed.meta[FILENAME_TARGETS]
+                elif role_name == 'snapshot':
+                    dependent = self.roles.timestamp.signed.snapshot_meta
+                if dependent:
+                    dependent.version = role.signed.version
+                logger.info(f'Published changes for {role_name}.')
+            else:
+                logger.info(f'No changes detected for {role_name}.')
+                # Check if signature count meets threshold
+                threshold = self.roles.root.signed.roles[role_name].threshold
+                if len(role.signatures) < threshold:
+                    logger.info(
+                        f'{role_name} threshold not met. Trying to sign...'
+                    )
+                    signature_count = self.threshold_sign(
+                        role_name=role_name, private_key_dirs=private_key_dirs
+                    )
+                    logger.info(f'Added {signature_count} signatures.')
+        # update config if key_map has changed
+        if self.config_dict != self.load_config():
+            self.save_config()
+            logger.info('Config file updated.')
+
+    def threshold_sign(
+            self,
+            role_name: str,
+            private_key_dirs: List[Union[pathlib.Path, str]],
+    ) -> int:
+        """
+        Sign the metadata file for a specific role, and save changes to disk.
+
+        Use this to sign and save without making any changes to the actual
+        signed metadata.
+
+        In case of root key rotation, both the old private key and the new
+        private key are required.
+
+        Returns the number of signatures created.
+        """
+        signature_count = 0
+        # sign role with all required keys that can be found
+        key_names = set(self.key_map.get(role_name, []))
+        if role_name == 'root':
+            # set ensures uniqueness
+            key_names = key_names.union(self.revoked_key_names)
+        for key_name in key_names:
+            private_key_path = self.keys.find_private_key(
+                key_name=key_name, key_dirs=private_key_dirs
+            )
+            if private_key_path:
+                self.roles.sign_role(
+                    role_name=role_name,
+                    private_key_path=private_key_path,
+                )
+                signature_count += 1
+                if key_name in self.revoked_key_names:
+                    self.revoked_key_names.remove(key_name)
+                    if key_name in self.encrypted_keys:
+                        self.encrypted_keys.remove(key_name)
+            else:
+                logger.warning(f'Private key not found: {key_name}')
+        if not signature_count:
+            raise Exception(f'No private keys found for {role_name}.')
+        # save changes to disk
+        self.roles.persist_role(role_name=role_name)
+        return signature_count
+
+    def _load_keys_and_roles(self, create_keys: bool = False):
+        # todo: make public, rename load_keys_and_metadata
+        if self.keys is None:
+            logger.info('Importing public keys...')
+            self.keys = Keys(
+                dir_path=self.keys_dir,
+                encrypted=self.encrypted_keys,
+                key_map=self.key_map,
+                thresholds=self.thresholds,
+            )
+            if create_keys:
+                # safe to call if keys exist
+                self.keys.create()
+            logger.info('Public keys imported.')
+        if self.roles is None:
+            logger.info('Importing metadata...')
+            self.roles = Roles(dir_path=self.metadata_dir)
+            self.roles.initialize(
+                keys=self.keys, expiration_days=self.expiration_days
+            )
+            logger.info('Metadata imported.')
```

### Comparing `tufup-0.4.9/src/tufup/utils/__init__.py` & `tufup-0.5.0/src/tufup/utils/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-import logging
-import pathlib
-import shutil
-import sys
-from typing import List, Optional, Union
-
-utils_logger = logging.getLogger(__name__)
-
-_INPUT_SEPARATOR = ' '
-
-
-def remove_path(path: Union[pathlib.Path, str]) -> bool:
-    """
-    Recursively remove directory or file at specified path.
-
-    If you want to remove directory contents but keep the directory itself:
-
-        for path in my_dir_path.iterdir():
-            remove_path(path)
-    """
-    # enforce pathlib.Path
-    path = pathlib.Path(path)
-    try:
-        if path.is_dir():
-            shutil.rmtree(path=path)
-            utils_logger.debug(f'Removed directory {path}')
-        elif path.is_file():
-            path.unlink()
-            utils_logger.debug(f'Removed file {path}')
-    except Exception as e:
-        utils_logger.error(f'Failed to remove {path}: {e}')
-        return False
-    return True
-
-
-def log_print(message: str, logger: logging.Logger, level: int = logging.INFO):
-    """
-    Log message with specified level.
-
-    Print message too, if logger is not enabled for specified level,
-    or if logger does not have a handler that streams to stdout.
-    """
-    # log normally
-    logger.log(level=level, msg=message)
-    # print if necessary
-    message_logged_to_stdout = False
-    current_logger = logger
-    while current_logger and not message_logged_to_stdout:
-        is_enabled = current_logger.isEnabledFor(level)
-        logs_to_stdout = any(
-            getattr(handler, 'stream', None) == sys.stdout
-            for handler in current_logger.handlers
-        )
-        message_logged_to_stdout = is_enabled and logs_to_stdout
-        if not current_logger.propagate:
-            current_logger = None
-        else:
-            current_logger = current_logger.parent
-    if not message_logged_to_stdout:
-        print(message)
-
-
-def input_bool(prompt: str, default: bool) -> bool:
-    true_inputs = ['y']
-    default_str = ' (y/[n])'
-    if default:
-        default_str = ' ([y]/n)'
-        true_inputs.append('')
-    prompt += default_str + _INPUT_SEPARATOR
-    answer = input(prompt)
-    utils_logger.debug(f'{prompt}: {answer}')
-    return answer in true_inputs
-
-
-def input_list(
-        prompt: str, default: List[str], item_default: Optional[str] = None
-) -> List[str]:
-    new_list = []
-    log_print(message=prompt, level=logging.DEBUG, logger=utils_logger)
-    # handle existing items
-    for existing_item in default or []:
-        if input_bool(f'{existing_item}\nKeep this item?', default=True):
-            new_list.append(existing_item)
-    # add new items
-    while input_bool(prompt='Add a new item?', default=False):
-        new_list.append(input_text(prompt='Enter item:', default=item_default))
-    # return unique list (use dict keys instead of set(), to preserve order)
-    return list(dict.fromkeys(new_list))
-
-
-def input_numeric(prompt: str, default: int) -> int:
-    answer = 'not empty, not numeric'
-    default_str = f' (default: {default})'
-    prompt += default_str + _INPUT_SEPARATOR
-    while answer and not answer.isnumeric():
-        answer = input(prompt)
-        utils_logger.debug(f'{prompt}: {answer}')
-    if answer:
-        return int(answer)
-    else:
-        return default
-
-
-def input_text(
-        prompt: str, default: Optional[str], optional: bool = False
-) -> Optional[str]:
-    answer = None
-    prompt += f' (default: {default})'
-    prompt += ' [optional]' if optional else ''
-    prompt += _INPUT_SEPARATOR
-    while not answer:
-        answer = input(prompt) or default
-        utils_logger.debug(f'{prompt}: {answer}')
-        if optional:
-            break
-    return answer
+import logging
+import pathlib
+import shutil
+import sys
+from typing import List, Optional, Union
+
+utils_logger = logging.getLogger(__name__)
+
+_INPUT_SEPARATOR = ' '
+
+
+def remove_path(path: Union[pathlib.Path, str]) -> bool:
+    """
+    Recursively remove directory or file at specified path.
+
+    If you want to remove directory contents but keep the directory itself:
+
+        for path in my_dir_path.iterdir():
+            remove_path(path)
+    """
+    # enforce pathlib.Path
+    path = pathlib.Path(path)
+    try:
+        if path.is_dir():
+            shutil.rmtree(path=path)
+            utils_logger.debug(f'Removed directory {path}')
+        elif path.is_file():
+            path.unlink()
+            utils_logger.debug(f'Removed file {path}')
+    except Exception as e:
+        utils_logger.error(f'Failed to remove {path}: {e}')
+        return False
+    return True
+
+
+def log_print(message: str, logger: logging.Logger, level: int = logging.INFO):
+    """
+    Log message with specified level.
+
+    Print message too, if logger is not enabled for specified level,
+    or if logger does not have a handler that streams to stdout.
+    """
+    # log normally
+    logger.log(level=level, msg=message)
+    # print if necessary
+    message_logged_to_stdout = False
+    current_logger = logger
+    while current_logger and not message_logged_to_stdout:
+        is_enabled = current_logger.isEnabledFor(level)
+        logs_to_stdout = any(
+            getattr(handler, 'stream', None) == sys.stdout
+            for handler in current_logger.handlers
+        )
+        message_logged_to_stdout = is_enabled and logs_to_stdout
+        if not current_logger.propagate:
+            current_logger = None
+        else:
+            current_logger = current_logger.parent
+    if not message_logged_to_stdout:
+        print(message)
+
+
+def input_bool(prompt: str, default: bool) -> bool:
+    true_inputs = ['y']
+    default_str = ' (y/[n])'
+    if default:
+        default_str = ' ([y]/n)'
+        true_inputs.append('')
+    prompt += default_str + _INPUT_SEPARATOR
+    answer = input(prompt)
+    utils_logger.debug(f'{prompt}: {answer}')
+    return answer in true_inputs
+
+
+def input_list(
+        prompt: str, default: List[str], item_default: Optional[str] = None
+) -> List[str]:
+    new_list = []
+    log_print(message=prompt, level=logging.DEBUG, logger=utils_logger)
+    # handle existing items
+    for existing_item in default or []:
+        if input_bool(f'{existing_item}\nKeep this item?', default=True):
+            new_list.append(existing_item)
+    # add new items
+    while input_bool(prompt='Add a new item?', default=False):
+        new_list.append(input_text(prompt='Enter item:', default=item_default))
+    # return unique list (use dict keys instead of set(), to preserve order)
+    return list(dict.fromkeys(new_list))
+
+
+def input_numeric(prompt: str, default: int) -> int:
+    answer = 'not empty, not numeric'
+    default_str = f' (default: {default})'
+    prompt += default_str + _INPUT_SEPARATOR
+    while answer and not answer.isnumeric():
+        answer = input(prompt)
+        utils_logger.debug(f'{prompt}: {answer}')
+    if answer:
+        return int(answer)
+    else:
+        return default
+
+
+def input_text(
+        prompt: str, default: Optional[str], optional: bool = False
+) -> Optional[str]:
+    answer = None
+    prompt += f' (default: {default})'
+    prompt += ' [optional]' if optional else ''
+    prompt += _INPUT_SEPARATOR
+    while not answer:
+        answer = input(prompt) or default
+        utils_logger.debug(f'{prompt}: {answer}')
+        if optional:
+            break
+    return answer
```

### Comparing `tufup-0.4.9/src/tufup/utils/platform_specific.py` & `tufup-0.5.0/src/tufup/utils/platform_specific.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-import logging
-import pathlib
-import platform
-import shutil
-import subprocess
-import sys
-from tempfile import NamedTemporaryFile
-from typing import List, Optional, Union
-
-from tufup.utils import remove_path
-
-logger = logging.getLogger(__name__)
-
-CURRENT_PLATFORM = platform.system()
-ON_WINDOWS = CURRENT_PLATFORM == 'Windows'
-ON_MAC = CURRENT_PLATFORM == 'Darwin'
-PLATFORM_SUPPORTED = ON_WINDOWS or ON_MAC
-
-
-def install_update(
-        src_dir: Union[pathlib.Path, str],
-        dst_dir: Union[pathlib.Path, str],
-        purge_dst_dir: bool = False,
-        exclude_from_purge: Optional[List[Union[pathlib.Path, str]]] = None,
-        **kwargs,
-):
-    """
-    Installs update files using platform specific installation script. The
-    actual installation script copies the files and folders from `src_dir` to
-    `dst_dir`.
-
-    If `purge_dst_dir` is `True`, *ALL* files and folders are deleted from
-    `dst_dir` before copying.
-
-    **DANGER**:
-
-    ONLY use `purge_dst_dir=True` if your app is properly installed in its
-    own *separate* directory, such as %PROGRAMFILES%\MyApp.
-
-    DO NOT use `purge_dst_dir=True` if your app executable is running
-    directly from a folder that also contains unrelated files or folders,
-    such as the Desktop folder or the Downloads folder, because this
-    unrelated content would be then also be deleted.
-
-    Individual files and folders can be excluded from purge using e.g.
-
-        exclude_from_purge=['path\\to\\file1', r'"path to\file2"', ...]
-
-    If `purge_dst_dir` is `False`, the `exclude_from_purge` argument is
-    ignored.
-    """
-    if ON_WINDOWS:
-        _install_update = _install_update_win
-    elif ON_MAC:
-        _install_update = _install_update_mac
-    else:
-        raise RuntimeError('This platform is not supported.')
-    return _install_update(
-        src_dir=src_dir,
-        dst_dir=dst_dir,
-        purge_dst_dir=purge_dst_dir,
-        exclude_from_purge=exclude_from_purge,
-        **kwargs,
-    )
-
-
-# Note that robocopy itself also has an option to create a log file,
-# viz. `/log:<filename>`, as well as a `/tee` option, but we want to log *all*
-# output from the batch file, not just output from the robocopy command.
-WIN_LOG_LINES = """
-call :log > "{log_file_path}" 2>&1
-:log
-"""
-WIN_ROBOCOPY_OVERWRITE = (
-    '/e',  # include subdirectories, even if empty
-    '/move',  # deletes files and dirs from source dir after they've been copied
-    '/v',  # verbose (show what is going on)
-    '/w:2',  # set retry-timeout (default is 30 seconds)
-)
-WIN_ROBOCOPY_PURGE = '/purge'  # delete all files and dirs in destination folder
-WIN_ROBOCOPY_EXCLUDE_FROM_PURGE = '/xf'  # exclude specified paths from purge
-# makes batch file delete itself when done (https://stackoverflow.com/a/20333575)
-WIN_BATCH_DELETE_SELF = '(goto) 2>nul & del "%~f0"'
-
-# _install_update_win makes sure the following variables are available for
-# batch templates:
-# {log_lines}, {src_dir}, {dst_dir}, {robocopy_options}, {delete_self}
-WIN_BATCH_TEMPLATE = """@echo off
-{log_lines}
-echo Moving app files...
-robocopy "{src_dir}" "{dst_dir}" {robocopy_options}
-echo Done.
-{delete_self}
-"""
-WIN_BATCH_PREFIX = 'tufup'
-WIN_BATCH_SUFFIX = '.bat'
-
-
-def run_bat_as_admin(file_path: Union[pathlib.Path, str]):
-    """
-    Request elevation for windows command interpreter (opens UAC prompt) and
-    then run the specified .bat file.
-
-    Returns True if successfully started, does not block, can continue after
-    calling process exits.
-    """
-    from ctypes import windll
-    # https://docs.microsoft.com/en-us/windows/win32/api/shellapi/nf-shellapi-shellexecutew
-    result = windll.shell32.ShellExecuteW(
-        None,  # handle to parent window
-        'runas',  # verb
-        'cmd.exe',  # file on which verb acts
-        ' '.join(['/c', str(file_path)]),  # parameters
-        None,  # working directory (default is cwd)
-        1,  # show window normally
-    )
-    return result > 32
-
-
-def _install_update_win(
-        src_dir: Union[pathlib.Path, str],
-        dst_dir: Union[pathlib.Path, str],
-        purge_dst_dir: bool,
-        exclude_from_purge: List[Union[pathlib.Path, str]],
-        as_admin: bool = False,
-        batch_template: str = WIN_BATCH_TEMPLATE,
-        batch_template_extra_kwargs: Optional[dict] = None,
-        log_file_name: Optional[str] = None,
-        robocopy_options_override: Optional[List[str]] = None,
-):
-    """
-    Create a batch script that moves files from src to dst, then run the
-    script in a new console, and exit the current process.
-
-    The script is created in a default temporary directory, and deletes
-    itself when done.
-
-    The `as_admin` options allows installation as admin (opens UAC dialog).
-
-    The `batch_template` option allows specification of custom batch-file
-    content. This may be in the form of a template string, as in the default
-    `WIN_BATCH_TEMPLATE`, or it may be a ready-made string without any
-    template variables. The following default template variables are
-    available for use in the custom template, although their use is optional:
-    {log_lines}, {src_dir}, {dst_dir}, {robocopy_options}, {delete_self}.
-    Custom template variables can be used as well, in which case you'll need
-    to specify `batch_template_extra_kwargs`.
-
-    The `batch_template_extra_kwargs` options allows specification of
-    *custom* template variables (in addition to the default ones, which are
-    always available). It accepts a dict, with keys matching the *custom*
-    template variable names specified in the `batch_template`.
-
-    The `log_file_name` option will log the output of the install script to a
-    file in the `dst_dir`.
-
-    The `robocopy_options_override` option allows options for [robocopy][1]
-    to be overridden completely. It accepts a list of option strings. This
-    will cause the purge arguments to be ignored as well.
-
-    [1]: https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/robocopy
-    """
-    if batch_template_extra_kwargs is None:
-        batch_template_extra_kwargs = dict()
-    # collect robocopy options
-    if robocopy_options_override is None:
-        robocopy_options = list(WIN_ROBOCOPY_OVERWRITE)
-        if purge_dst_dir:
-            robocopy_options.append(WIN_ROBOCOPY_PURGE)
-            if exclude_from_purge:
-                robocopy_options.append(WIN_ROBOCOPY_EXCLUDE_FROM_PURGE)
-                robocopy_options.extend(exclude_from_purge)
-    else:
-        # empty list [] simply clears all options
-        robocopy_options = robocopy_options_override
-    options_str = ' '.join(robocopy_options)
-    # handle batch file output logging
-    log_lines = ''
-    if log_file_name:
-        log_file_path = pathlib.Path(dst_dir) / log_file_name
-        log_lines = WIN_LOG_LINES.format(log_file_path=log_file_path)
-        logger.info(f'logging install script output to {log_file_path}')
-    # write temporary batch file (NOTE: The file is placed in the system
-    # default temporary dir, but the file is not removed automatically. So,
-    # either the batch file should self-delete when done, or it should be
-    # deleted by some other means, because windows does not clean the temp
-    # dir automatically.)
-    script_content = batch_template.format(
-        src_dir=src_dir,
-        dst_dir=dst_dir,
-        robocopy_options=options_str,
-        log_lines=log_lines,
-        delete_self=WIN_BATCH_DELETE_SELF,
-        **batch_template_extra_kwargs,
-    )
-    logger.debug(f'writing windows batch script:\n{script_content}')
-    with NamedTemporaryFile(
-            mode='w', prefix=WIN_BATCH_PREFIX, suffix=WIN_BATCH_SUFFIX, delete=False
-    ) as temp_file:
-        temp_file.write(script_content)
-    logger.debug(f'temporary batch script created: {temp_file.name}')
-    script_path = pathlib.Path(temp_file.name).resolve()
-    logger.debug(f'starting script in new console: {script_path}')
-    # start the script in a separate process, non-blocking
-    if as_admin:
-        run_bat_as_admin(file_path=script_path)
-    else:
-        # we use Popen() instead of run(), because the latter blocks execution
-        subprocess.Popen(
-            [script_path], creationflags=subprocess.CREATE_NEW_CONSOLE
-        )
-    logger.debug('exiting')
-    # exit current process
-    sys.exit(0)
-
-
-def _install_update_mac(
-        src_dir: Union[pathlib.Path, str],
-        dst_dir: Union[pathlib.Path, str],
-        purge_dst_dir: bool,
-        exclude_from_purge: List[Union[pathlib.Path, str]],
-        **kwargs,
-):
-    # todo: implement as_admin and debug kwargs for mac
-    logger.debug(f'Kwargs not used: {kwargs}')
-    if purge_dst_dir:
-        exclude_from_purge = [  # enforce path objects
-            pathlib.Path(item) for item in exclude_from_purge
-        ] if exclude_from_purge else []
-        logger.debug(f'Purging content of {dst_dir}')
-        for path in pathlib.Path(dst_dir).iterdir():
-            if path not in exclude_from_purge:
-                remove_path(path=path)
-    logger.debug(f'Moving content of {src_dir} to {dst_dir}.')
-    shutil.copytree(src_dir, dst_dir, dirs_exist_ok=True)
-    # Note: the src_dir is typically a temporary directory, but we'll clear
-    # it anyway just to be consistent with the windows implementation
-    for path in pathlib.Path(src_dir).iterdir():
-        remove_path(path=path)
-    logger.debug(f'Restarting application, running {sys.executable}.')
-    subprocess.Popen(sys.executable, shell=True)  # nosec
-    sys.exit(0)
+import logging
+import pathlib
+import platform
+import shutil
+import subprocess
+import sys
+from tempfile import NamedTemporaryFile
+from typing import List, Optional, Union
+
+from tufup.utils import remove_path
+
+logger = logging.getLogger(__name__)
+
+CURRENT_PLATFORM = platform.system()
+ON_WINDOWS = CURRENT_PLATFORM == 'Windows'
+ON_MAC = CURRENT_PLATFORM == 'Darwin'
+PLATFORM_SUPPORTED = ON_WINDOWS or ON_MAC
+
+
+def install_update(
+        src_dir: Union[pathlib.Path, str],
+        dst_dir: Union[pathlib.Path, str],
+        purge_dst_dir: bool = False,
+        exclude_from_purge: Optional[List[Union[pathlib.Path, str]]] = None,
+        **kwargs,
+):
+    """
+    Installs update files using platform specific installation script. The
+    actual installation script copies the files and folders from `src_dir` to
+    `dst_dir`.
+
+    If `purge_dst_dir` is `True`, *ALL* files and folders are deleted from
+    `dst_dir` before copying.
+
+    **DANGER**:
+
+    ONLY use `purge_dst_dir=True` if your app is properly installed in its
+    own *separate* directory, such as %PROGRAMFILES%\MyApp.
+
+    DO NOT use `purge_dst_dir=True` if your app executable is running
+    directly from a folder that also contains unrelated files or folders,
+    such as the Desktop folder or the Downloads folder, because this
+    unrelated content would be then also be deleted.
+
+    Individual files and folders can be excluded from purge using e.g.
+
+        exclude_from_purge=['path\\to\\file1', r'"path to\file2"', ...]
+
+    If `purge_dst_dir` is `False`, the `exclude_from_purge` argument is
+    ignored.
+    """
+    if ON_WINDOWS:
+        _install_update = _install_update_win
+    elif ON_MAC:
+        _install_update = _install_update_mac
+    else:
+        raise RuntimeError('This platform is not supported.')
+    return _install_update(
+        src_dir=src_dir,
+        dst_dir=dst_dir,
+        purge_dst_dir=purge_dst_dir,
+        exclude_from_purge=exclude_from_purge,
+        **kwargs,
+    )
+
+
+# Note that robocopy itself also has an option to create a log file,
+# viz. `/log:<filename>`, as well as a `/tee` option, but we want to log *all*
+# output from the batch file, not just output from the robocopy command.
+WIN_LOG_LINES = """
+call :log > "{log_file_path}" 2>&1
+:log
+"""
+WIN_ROBOCOPY_OVERWRITE = (
+    '/e',  # include subdirectories, even if empty
+    '/move',  # deletes files and dirs from source dir after they've been copied
+    '/v',  # verbose (show what is going on)
+    '/w:2',  # set retry-timeout (default is 30 seconds)
+)
+WIN_ROBOCOPY_PURGE = '/purge'  # delete all files and dirs in destination folder
+WIN_ROBOCOPY_EXCLUDE_FROM_PURGE = '/xf'  # exclude specified paths from purge
+# makes batch file delete itself when done (https://stackoverflow.com/a/20333575)
+WIN_BATCH_DELETE_SELF = '(goto) 2>nul & del "%~f0"'
+
+# _install_update_win makes sure the following variables are available for
+# batch templates:
+# {log_lines}, {src_dir}, {dst_dir}, {robocopy_options}, {delete_self}
+WIN_BATCH_TEMPLATE = """@echo off
+{log_lines}
+echo Moving app files...
+robocopy "{src_dir}" "{dst_dir}" {robocopy_options}
+echo Done.
+{delete_self}
+"""
+WIN_BATCH_PREFIX = 'tufup'
+WIN_BATCH_SUFFIX = '.bat'
+
+
+def run_bat_as_admin(file_path: Union[pathlib.Path, str]):
+    """
+    Request elevation for windows command interpreter (opens UAC prompt) and
+    then run the specified .bat file.
+
+    Returns True if successfully started, does not block, can continue after
+    calling process exits.
+    """
+    from ctypes import windll
+    # https://docs.microsoft.com/en-us/windows/win32/api/shellapi/nf-shellapi-shellexecutew
+    result = windll.shell32.ShellExecuteW(
+        None,  # handle to parent window
+        'runas',  # verb
+        'cmd.exe',  # file on which verb acts
+        ' '.join(['/c', str(file_path)]),  # parameters
+        None,  # working directory (default is cwd)
+        1,  # show window normally
+    )
+    return result > 32
+
+
+def _install_update_win(
+        src_dir: Union[pathlib.Path, str],
+        dst_dir: Union[pathlib.Path, str],
+        purge_dst_dir: bool,
+        exclude_from_purge: List[Union[pathlib.Path, str]],
+        as_admin: bool = False,
+        batch_template: str = WIN_BATCH_TEMPLATE,
+        batch_template_extra_kwargs: Optional[dict] = None,
+        log_file_name: Optional[str] = None,
+        robocopy_options_override: Optional[List[str]] = None,
+):
+    """
+    Create a batch script that moves files from src to dst, then run the
+    script in a new console, and exit the current process.
+
+    The script is created in a default temporary directory, and deletes
+    itself when done.
+
+    The `as_admin` options allows installation as admin (opens UAC dialog).
+
+    The `batch_template` option allows specification of custom batch-file
+    content. This may be in the form of a template string, as in the default
+    `WIN_BATCH_TEMPLATE`, or it may be a ready-made string without any
+    template variables. The following default template variables are
+    available for use in the custom template, although their use is optional:
+    {log_lines}, {src_dir}, {dst_dir}, {robocopy_options}, {delete_self}.
+    Custom template variables can be used as well, in which case you'll need
+    to specify `batch_template_extra_kwargs`.
+
+    The `batch_template_extra_kwargs` options allows specification of
+    *custom* template variables (in addition to the default ones, which are
+    always available). It accepts a dict, with keys matching the *custom*
+    template variable names specified in the `batch_template`.
+
+    The `log_file_name` option will log the output of the install script to a
+    file in the `dst_dir`.
+
+    The `robocopy_options_override` option allows options for [robocopy][1]
+    to be overridden completely. It accepts a list of option strings. This
+    will cause the purge arguments to be ignored as well.
+
+    [1]: https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/robocopy
+    """
+    if batch_template_extra_kwargs is None:
+        batch_template_extra_kwargs = dict()
+    # collect robocopy options
+    if robocopy_options_override is None:
+        robocopy_options = list(WIN_ROBOCOPY_OVERWRITE)
+        if purge_dst_dir:
+            robocopy_options.append(WIN_ROBOCOPY_PURGE)
+            if exclude_from_purge:
+                robocopy_options.append(WIN_ROBOCOPY_EXCLUDE_FROM_PURGE)
+                robocopy_options.extend(exclude_from_purge)
+    else:
+        # empty list [] simply clears all options
+        robocopy_options = robocopy_options_override
+    options_str = ' '.join(robocopy_options)
+    # handle batch file output logging
+    log_lines = ''
+    if log_file_name:
+        log_file_path = pathlib.Path(dst_dir) / log_file_name
+        log_lines = WIN_LOG_LINES.format(log_file_path=log_file_path)
+        logger.info(f'logging install script output to {log_file_path}')
+    # write temporary batch file (NOTE: The file is placed in the system
+    # default temporary dir, but the file is not removed automatically. So,
+    # either the batch file should self-delete when done, or it should be
+    # deleted by some other means, because windows does not clean the temp
+    # dir automatically.)
+    script_content = batch_template.format(
+        src_dir=src_dir,
+        dst_dir=dst_dir,
+        robocopy_options=options_str,
+        log_lines=log_lines,
+        delete_self=WIN_BATCH_DELETE_SELF,
+        **batch_template_extra_kwargs,
+    )
+    logger.debug(f'writing windows batch script:\n{script_content}')
+    with NamedTemporaryFile(
+            mode='w', prefix=WIN_BATCH_PREFIX, suffix=WIN_BATCH_SUFFIX, delete=False
+    ) as temp_file:
+        temp_file.write(script_content)
+    logger.debug(f'temporary batch script created: {temp_file.name}')
+    script_path = pathlib.Path(temp_file.name).resolve()
+    logger.debug(f'starting script in new console: {script_path}')
+    # start the script in a separate process, non-blocking
+    if as_admin:
+        run_bat_as_admin(file_path=script_path)
+    else:
+        # we use Popen() instead of run(), because the latter blocks execution
+        subprocess.Popen(
+            [script_path], creationflags=subprocess.CREATE_NEW_CONSOLE
+        )
+    logger.debug('exiting')
+    # exit current process
+    sys.exit(0)
+
+
+def _install_update_mac(
+        src_dir: Union[pathlib.Path, str],
+        dst_dir: Union[pathlib.Path, str],
+        purge_dst_dir: bool,
+        exclude_from_purge: List[Union[pathlib.Path, str]],
+        **kwargs,
+):
+    # todo: implement as_admin and debug kwargs for mac
+    logger.debug(f'Kwargs not used: {kwargs}')
+    if purge_dst_dir:
+        exclude_from_purge = [  # enforce path objects
+            pathlib.Path(item) for item in exclude_from_purge
+        ] if exclude_from_purge else []
+        logger.debug(f'Purging content of {dst_dir}')
+        for path in pathlib.Path(dst_dir).iterdir():
+            if path not in exclude_from_purge:
+                remove_path(path=path)
+    logger.debug(f'Moving content of {src_dir} to {dst_dir}.')
+    shutil.copytree(src_dir, dst_dir, dirs_exist_ok=True)
+    # Note: the src_dir is typically a temporary directory, but we'll clear
+    # it anyway just to be consistent with the windows implementation
+    for path in pathlib.Path(src_dir).iterdir():
+        remove_path(path=path)
+    logger.debug(f'Restarting application, running {sys.executable}.')
+    subprocess.Popen(sys.executable, shell=True)  # nosec
+    sys.exit(0)
```

### Comparing `tufup-0.4.9/src/tufup.egg-info/PKG-INFO` & `tufup-0.5.0/src/tufup.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,246 +1,246 @@
-Metadata-Version: 2.1
-Name: tufup
-Version: 0.4.9
-Summary: Automated updates for stand-alone Python applications, built upon python-tuf.
-Author-email: dennisvang <djvg@protonmail.com>
-License: MIT License
-        
-        Copyright (c) 2022 Dennis
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: source, https://github.com/dennisvang/tufup
-Project-URL: documentation, https://tufup.readthedocs.io/en/latest/
-Project-URL: issues, https://github.com/dennisvang/tufup/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# tufup
-
-![Build](https://github.com/dennisvang/tufup/actions/workflows/python-package.yml/badge.svg)
-[![PyPI](https://img.shields.io/pypi/v/tufup)](https://pypi.org/project/tufup/)
-[![Documentation Status](https://readthedocs.org/projects/tufup/badge/?version=latest)](https://tufup.readthedocs.io/en/latest/?badge=latest)
-
-A simple software updater for stand-alone Python *applications*.
-
-## Application updates and TUF
-
-A basic update-cycle for a [self-updating application][15] could look like this: 
-
-1. the app's development team create a new release, and make it available on a server
-2. an older version of the app, out in the wild, contacts the server to check for updates
-3. the old app finds the new release, downloads it, and installs it
-4. goto 1.
-
-The principle is relatively simple, as long as you don't consider the security risks involved.
-
-Unfortunately, in the real world, [security cannot be neglected][16]: You don't want to install untrusted software on your system.
-
-So, how can we make sure our update-cycle is secure? This is where things get quite complicated.
-
-Luckily, [python-tuf][1], the reference implementation for [TUF][2] (The Update Framework) takes care of this complexity. If used properly, TUF ensures a high level of security for your update system.
-
-That's why the `tufup` package is built on top of `python-tuf`.
-
-It is highly advisable to read the [TUF documentation][11] before proceeding. 
-
-
-## Quickstart
-
-The easiest way to understand how `tufup` works is by example. A minimal example of an application that uses `tufup` can be found in the companion repository: 
-**[tufup-example][10]**
-
-The example repository shows how to integrate the `tufup` client into your app, and it shows you how to set up a `tufup` update-repository.
-
->NOTE: Although the tufup-example repository uses PyInstaller to bundle an application, `tufup` can be used with ***any*** type of application bundle, even plain python scripts.  
-
-## Questions and Issues
-
-If you have questions about `tufup`, or need help getting started, please post a question on [Stack Overflow][13], add a `tufup` tag, and we will help you there.
-
-If you encounter bugs or other problems that are likely to affect other users, please create a [new issue][14] here.
-
-## Some background
-
-The `tufup` package was inspired by [PyUpdater][3], and uses a general approach to updating that is directly based on PyUpdater's implementation.
-
-> NOTE: `tufup` is completely *independent* of PyUpdater. In fact, `tufup` was created as a replacement for PyUpdater, given the fact that [PyUpdater has been archived and is no longer maintained][17]. 
-
-However, whereas PyUpdater implements a *custom* security mechanism to ensure authenticity (and integrity) of downloaded update files, `tufup` is built on top of the security mechanisms implemented in the [python-tuf][1] package, a.k.a. `tuf`.
-By entrusting the design of security measures to the security professionals, `tufup` can focus on high-level tools.
-
-Although `tuf` supports highly complex security infrastructures, see e.g. [PEP458][5], it also offers sufficient flexibility to allow *application* developers to tailor the security level to their use case.
-For details and best practices, refer to the [tuf docs][2].
-
-Based on the intended use, the `tufup` package supports only the top-level roles offered by `tuf`. At this time we do not support delegations.
-
->NOTE: Whereas PyUpdater is tightly integrated with PyInstaller, `tufup` is completely *independent* of the type of packaging solution.
-> At its core, `tufup` simply moves bundles of files from A to B, securely, regardless of how these bundles were created. 
-> A bundle may consist of a simple python script, a PyInstaller bundle, a PEX package, or any other collection of files and folders. 
-
-## Overview
-
-Borrowing TUF terminology, we distinguish between a *repo*-side (repository) and a *client*-side (application).
-
-Below you'll find a list of the basic steps that occur in an application update cycle. 
-Steps covered by `tufup` are **highlighted**.
-
-On the *repo*-side, the app *developer*
-
-- modifies the application code
-- **creates a new application archive file and corresponding patch file**
-- **signs the resulting files cryptographically**
-- deploys these files to a server
-
-On the *client*-side, the *application*
-
-- **checks for updates**
-- **downloads update files**
-- **applies the update files (i.e. installation)**
-
-The `tuf` package is used under the hood to check for updates and download update files in a secure manner, so `tufup` can safely apply the update.
-See the [tuf docs][4] for more information.
-
-## Archives and patches
-
-*Internally*, `tufup` works with *archives* (gzipped bundles of files and folders) and *patches* (binary differences between subsequent archives).
-Each archive, except the first one, has a corresponding patch file.
-
-Archive filenames and patch filenames follow the pattern
-
-`<name>-<version><suffix>` 
-
-where `name` is a short string that may contain alphanumeric characters, underscores, and hyphens, `version` is a version string according to the [PEP440][6] specification, and `suffix` is either `'.tar.gz'` or `'.patch'`.
-
-Patches are typically smaller than archives, so the tufup *client* will always attempt to update using one or more patches.
-However, if the total amount of patch data is greater than the desired full archive file, a full update will be performed.
-
-If this sounds confusing, don't worry: it is all handled internally.
-
-## How updates are created (repo-side)
-
-When a new release of your application is ready, the following steps need to be taken to enable clients to update to that new release:
-
-1. Create an application archive for the new release.
-2. Create a patch from the current archive to the new archive.
-3. Add hashes for the newly created archive file and patch file to the `tuf` metadata.
-4. Sign the modified `tuf` metadata files.
-5. Upload the new target files, i.e. archive and patch, and the updated metadata files, to the update server.
-
-The `tufup.repo` module and the `tufup` CLI provide convenient ways to streamline steps 1 to 4, based on the `tuf` [basic repo example][7].
-Step 5 is not covered by `tufup`, as it depends on the implementation.
-
-The signed metadata and hashes ensure both authenticity and integrity of the update files (see [tuf docs][2]).
-In order to sign the metadata, we need access to the private key files for the applicable `tuf` roles.
-
-## How updates are applied (client-side)
-
-By default, updates are applied by copying all files and folders from the latest archive to the current app installation directory.
-
-Here's what happens during the update process:
-
-- The latest archive is either downloaded in full, as described above, or it is derived from the current archive by applying one or more downloaded patches.
-- Once the latest archive is available on disk, it is decompressed to a temporary directory.
-- A default install script is then started, which copies the new files and folders from the temporary directory to the current app installation directory. On Windows, this script is started in a new process, after which the currently running process will exit.
-- Alternatively, you can specify a custom install script to do whatever you want with the new files.
-
-The default install script accepts an optional `purge_dst_dir` argument, which will cause *ALL* files and folders to be deleted from the app installation directory, before moving the new files into place.
-This is a convenient way to remove any stale files and folders from the app installation directory.
-
->**WARNING**: The `purge_dst_dir` option should *only* be used if the app is properly installed in its *own separate* directory.
-If this is not the case, for example if the app is running from the Windows `Desktop` directory, any *unrelated* files or folders in this directory will also be deleted! 
-
-## App versions and release channels
-
-When adding an application bundle to your `tufup` repository, you need to specify an app version string.
-This version string is used in the archive filename, and must be [PEP440][18] compliant (internally we use [`packaging.version.Version`][20]).
-
-The `tufup` client inspects these version strings to determine if updates are available.
-
-By default, when the `tufup` client looks for updates, it only includes final releases.
-Pre-releases are filtered out, unless you explicitly specify a "pre-release" channel.
-Refer to the [`Client.check_for_updates()`][21] method for details:
-
-> If `pre` is specified, pre-releases are included, down to the specified level. 
-> Pre-release identifiers follow the PEP440 specification, i.e. `'a'`, `'b'`, or `'rc'`, for alpha, beta, and release candidate, respectively.
-
-For example, suppose your latest final-release is `1.3.0`, and your latest pre-release is `2.0.0a3`. 
-An app in the field still has old version `1.0.0`. 
-If this app checks either the default channel, the release-candidate (`'rc'`) channel, or the beta (`'b'`) channel, it finds version `1.3.0` available.
-If the app checks the alpha channel (`'a'`), it finds `2.0.0a3`.
-
-Just to be clear: `tufup` assumes a typical linear release history without branching, so
-
-```none
-0.0 < 0.1a < 0.1b < 0.1rc < 0.1rc0 < 0.1rc1 < 0.1 < ...
-```
-
-## Migrating from other update frameworks
-
-Here's one way to migrate from another update framework, such as `pyupdater`, to `tufup`:
-
-1. Add `tufup` to your main application environment as a core dependency, and move `pyupdater` from core dependencies to development dependencies.
-2. Replace all `pyupdater` client code (and configuration) in your application by the `tufup` client.
-3. Initialize the `tufup` repository, so the root metadata file `root.json` exists.
-4. Modify your PyInstaller `.spec` file (from PyUpdater) to ensure that the `root.json` file is included in your package.
-5. Build, package, and sign using `pyupdater`, and deploy to your server, as usual. 
-This ensures that your `pyupdater` clients currently in the field will be able to update to the new `tufup` client.
-6. From here on, new updates will be deployed using `tufup`.
-7. If you want to enable a patch update from the `pyupdater` version to the new `tufup` version, extract the latest PyUpdater archive and add the resulting bundle to the `tufup` repository. 
-8. To skip patch creation, just create a new app bundle and add that to the `tufup` repository. 
-9. BEWARE: Keep the `pyupdater` repository in place as long as necessary to allow all clients to update.
-10. From now on, build, package, sign and deploy using `tufup`, as described elsewhere in this document.
-
-## Platform support
-
-The `tufup.client` tools are aimed primarily at **Windows** and **macOS** applications, whereas the `tufup.repo` tools are platform independent, as `tufup.repo` is just a thin layer on top of `python-tuf`. 
-
-Although `tufup.client` could also be used for Linux applications, those are probably better off using native packaging solutions, or solutions such as Flatpak or Snapcraft. 
-Read the [Python packaging overview][8] for more information.
-
-Platform dependence for `tufup.client` is related to file handling and process handling during the installation procedure, as can be seen in [tufup.utils.platform_specific][12].
-A custom, platform *de*pendent, installation procedure can be specified via the optional `install` argument for the `Client.update()` method.
-
-
-
-[1]: https://github.com/theupdateframework/python-tuf
-[2]: https://theupdateframework.io/
-[3]: https://github.com/Digital-Sapphire/PyUpdater/
-[4]: https://theupdateframework.io/overview/#software-updates-101
-[5]: https://peps.python.org/pep-0458/
-[6]: https://peps.python.org/pep-0440/
-[7]: https://github.com/theupdateframework/python-tuf/blob/develop/examples/repo_example/basic_repo.py
-[8]: https://packaging.python.org/en/latest/overview/
-[9]: https://pythonhosted.org/not-so-tuf/
-[10]: https://github.com/dennisvang/tufup-example
-[11]: https://theupdateframework.io/metadata/
-[12]: https://github.com/dennisvang/tufup/blob/master/src/tufup/utils/platform_specific.py
-[13]: https://stackoverflow.com/questions/ask
-[14]: https://github.com/dennisvang/tufup/issues
-[15]: https://theupdateframework.io/overview/#software-updates-101
-[16]: https://theupdateframework.io/security/
-[17]: https://github.com/Digital-Sapphire/PyUpdater#this-is-the-end
-[18]: https://peps.python.org/pep-0440/
-[19]: https://peps.python.org/pep-0440/#public-version-identifiers
-[20]: https://packaging.pypa.io/en/stable/version.html#packaging.version.Version
-[21]: https://github.com/dennisvang/tufup/blob/master/src/tufup/client.py
+Metadata-Version: 2.1
+Name: tufup
+Version: 0.5.0
+Summary: Automated updates for stand-alone Python applications, built upon python-tuf.
+Author-email: dennisvang <djvg@protonmail.com>
+License: MIT License
+        
+        Copyright (c) 2022 Dennis
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: source, https://github.com/dennisvang/tufup
+Project-URL: documentation, https://tufup.readthedocs.io/en/latest/
+Project-URL: issues, https://github.com/dennisvang/tufup/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# tufup
+
+![Build](https://github.com/dennisvang/tufup/actions/workflows/python-package.yml/badge.svg)
+[![PyPI](https://img.shields.io/pypi/v/tufup)](https://pypi.org/project/tufup/)
+[![Documentation Status](https://readthedocs.org/projects/tufup/badge/?version=latest)](https://tufup.readthedocs.io/en/latest/?badge=latest)
+
+A simple software updater for stand-alone Python *applications*.
+
+## Application updates and TUF
+
+A basic update-cycle for a [self-updating application][15] could look like this: 
+
+1. the app's development team create a new release, and make it available on a server
+2. an older version of the app, out in the wild, contacts the server to check for updates
+3. the old app finds the new release, downloads it, and installs it
+4. goto 1.
+
+The principle is relatively simple, as long as you don't consider the security risks involved.
+
+Unfortunately, in the real world, [security cannot be neglected][16]: You don't want to install untrusted software on your system.
+
+So, how can we make sure our update-cycle is secure? This is where things get quite complicated.
+
+Luckily, [python-tuf][1], the reference implementation for [TUF][2] (The Update Framework) takes care of this complexity. If used properly, TUF ensures a high level of security for your update system.
+
+That's why the `tufup` package is built on top of `python-tuf`.
+
+It is highly advisable to read the [TUF documentation][11] before proceeding. 
+
+
+## Quickstart
+
+The easiest way to understand how `tufup` works is by example. A minimal example of an application that uses `tufup` can be found in the companion repository: 
+**[tufup-example][10]**
+
+The example repository shows how to integrate the `tufup` client into your app, and it shows you how to set up a `tufup` update-repository.
+
+>NOTE: Although the tufup-example repository uses PyInstaller to bundle an application, `tufup` can be used with ***any*** type of application bundle, even plain python scripts.  
+
+## Questions and Issues
+
+If you have questions about `tufup`, or need help getting started, please post a question on [Stack Overflow][13], add a `tufup` tag, and we will help you there.
+
+If you encounter bugs or other problems that are likely to affect other users, please create a [new issue][14] here.
+
+## Some background
+
+The `tufup` package was inspired by [PyUpdater][3], and uses a general approach to updating that is directly based on PyUpdater's implementation.
+
+> NOTE: `tufup` is completely *independent* of PyUpdater. In fact, `tufup` was created as a replacement for PyUpdater, given the fact that [PyUpdater has been archived and is no longer maintained][17]. 
+
+However, whereas PyUpdater implements a *custom* security mechanism to ensure authenticity (and integrity) of downloaded update files, `tufup` is built on top of the security mechanisms implemented in the [python-tuf][1] package, a.k.a. `tuf`.
+By entrusting the design of security measures to the security professionals, `tufup` can focus on high-level tools.
+
+Although `tuf` supports highly complex security infrastructures, see e.g. [PEP458][5], it also offers sufficient flexibility to allow *application* developers to tailor the security level to their use case.
+For details and best practices, refer to the [tuf docs][2].
+
+Based on the intended use, the `tufup` package supports only the top-level roles offered by `tuf`. At this time we do not support delegations.
+
+>NOTE: Whereas PyUpdater is tightly integrated with PyInstaller, `tufup` is completely *independent* of the type of packaging solution.
+> At its core, `tufup` simply moves bundles of files from A to B, securely, regardless of how these bundles were created. 
+> A bundle may consist of a simple python script, a PyInstaller bundle, a PEX package, or any other collection of files and folders. 
+
+## Overview
+
+Borrowing TUF terminology, we distinguish between a *repo*-side (repository) and a *client*-side (application).
+
+Below you'll find a list of the basic steps that occur in an application update cycle. 
+Steps covered by `tufup` are **highlighted**.
+
+On the *repo*-side, the app *developer*
+
+- modifies the application code
+- **creates a new application archive file and corresponding patch file**
+- **signs the resulting files cryptographically**
+- deploys these files to a server
+
+On the *client*-side, the *application*
+
+- **checks for updates**
+- **downloads update files**
+- **applies the update files (i.e. installation)**
+
+The `tuf` package is used under the hood to check for updates and download update files in a secure manner, so `tufup` can safely apply the update.
+See the [tuf docs][4] for more information.
+
+## Archives and patches
+
+*Internally*, `tufup` works with *archives* (gzipped bundles of files and folders) and *patches* (binary differences between subsequent archives).
+Each archive, except the first one, has a corresponding patch file.
+
+Archive filenames and patch filenames follow the pattern
+
+`<name>-<version><suffix>` 
+
+where `name` is a short string that may contain alphanumeric characters, underscores, and hyphens, `version` is a version string according to the [PEP440][6] specification, and `suffix` is either `'.tar.gz'` or `'.patch'`.
+
+Patches are typically smaller than archives, so the tufup *client* will always attempt to update using one or more patches.
+However, if the total amount of patch data is greater than the desired full archive file, a full update will be performed.
+
+If this sounds confusing, don't worry: it is all handled internally.
+
+## How updates are created (repo-side)
+
+When a new release of your application is ready, the following steps need to be taken to enable clients to update to that new release:
+
+1. Create an application archive for the new release.
+2. Create a patch from the current archive to the new archive.
+3. Add hashes for the newly created archive file and patch file to the `tuf` metadata.
+4. Sign the modified `tuf` metadata files.
+5. Upload the new target files, i.e. archive and patch, and the updated metadata files, to the update server.
+
+The `tufup.repo` module and the `tufup` CLI provide convenient ways to streamline steps 1 to 4, based on the `tuf` [basic repo example][7].
+Step 5 is not covered by `tufup`, as it depends on the implementation.
+
+The signed metadata and hashes ensure both authenticity and integrity of the update files (see [tuf docs][2]).
+In order to sign the metadata, we need access to the private key files for the applicable `tuf` roles.
+
+## How updates are applied (client-side)
+
+By default, updates are applied by copying all files and folders from the latest archive to the current app installation directory.
+
+Here's what happens during the update process:
+
+- The latest archive is either downloaded in full, as described above, or it is derived from the current archive by applying one or more downloaded patches.
+- Once the latest archive is available on disk, it is decompressed to a temporary directory.
+- A default install script is then started, which copies the new files and folders from the temporary directory to the current app installation directory. On Windows, this script is started in a new process, after which the currently running process will exit.
+- Alternatively, you can specify a custom install script to do whatever you want with the new files.
+
+The default install script accepts an optional `purge_dst_dir` argument, which will cause *ALL* files and folders to be deleted from the app installation directory, before moving the new files into place.
+This is a convenient way to remove any stale files and folders from the app installation directory.
+
+>**WARNING**: The `purge_dst_dir` option should *only* be used if the app is properly installed in its *own separate* directory.
+If this is not the case, for example if the app is running from the Windows `Desktop` directory, any *unrelated* files or folders in this directory will also be deleted! 
+
+## App versions and release channels
+
+When adding an application bundle to your `tufup` repository, you need to specify an app version string.
+This version string is used in the archive filename, and must be [PEP440][18] compliant (internally we use [`packaging.version.Version`][20]).
+
+The `tufup` client inspects these version strings to determine if updates are available.
+
+By default, when the `tufup` client looks for updates, it only includes final releases.
+Pre-releases are filtered out, unless you explicitly specify a "pre-release" channel.
+Refer to the [`Client.check_for_updates()`][21] method for details:
+
+> If `pre` is specified, pre-releases are included, down to the specified level. 
+> Pre-release identifiers follow the PEP440 specification, i.e. `'a'`, `'b'`, or `'rc'`, for alpha, beta, and release candidate, respectively.
+
+For example, suppose your latest final-release is `1.3.0`, and your latest pre-release is `2.0.0a3`. 
+An app in the field still has old version `1.0.0`. 
+If this app checks either the default channel, the release-candidate (`'rc'`) channel, or the beta (`'b'`) channel, it finds version `1.3.0` available.
+If the app checks the alpha channel (`'a'`), it finds `2.0.0a3`.
+
+Just to be clear: `tufup` assumes a typical linear release history without branching, so
+
+```none
+0.0 < 0.1a < 0.1b < 0.1rc < 0.1rc0 < 0.1rc1 < 0.1 < ...
+```
+
+## Migrating from other update frameworks
+
+Here's one way to migrate from another update framework, such as `pyupdater`, to `tufup`:
+
+1. Add `tufup` to your main application environment as a core dependency, and move `pyupdater` from core dependencies to development dependencies.
+2. Replace all `pyupdater` client code (and configuration) in your application by the `tufup` client.
+3. Initialize the `tufup` repository, so the root metadata file `root.json` exists.
+4. Modify your PyInstaller `.spec` file (from PyUpdater) to ensure that the `root.json` file is included in your package.
+5. Build, package, and sign using `pyupdater`, and deploy to your server, as usual. 
+This ensures that your `pyupdater` clients currently in the field will be able to update to the new `tufup` client.
+6. From here on, new updates will be deployed using `tufup`.
+7. If you want to enable a patch update from the `pyupdater` version to the new `tufup` version, extract the latest PyUpdater archive and add the resulting bundle to the `tufup` repository. 
+8. To skip patch creation, just create a new app bundle and add that to the `tufup` repository. 
+9. BEWARE: Keep the `pyupdater` repository in place as long as necessary to allow all clients to update.
+10. From now on, build, package, sign and deploy using `tufup`, as described elsewhere in this document.
+
+## Platform support
+
+The `tufup.client` tools are aimed primarily at **Windows** and **macOS** applications, whereas the `tufup.repo` tools are platform independent, as `tufup.repo` is just a thin layer on top of `python-tuf`. 
+
+Although `tufup.client` could also be used for Linux applications, those are probably better off using native packaging solutions, or solutions such as Flatpak or Snapcraft. 
+Read the [Python packaging overview][8] for more information.
+
+Platform dependence for `tufup.client` is related to file handling and process handling during the installation procedure, as can be seen in [tufup.utils.platform_specific][12].
+A custom, platform *de*pendent, installation procedure can be specified via the optional `install` argument for the `Client.update()` method.
+
+
+
+[1]: https://github.com/theupdateframework/python-tuf
+[2]: https://theupdateframework.io/
+[3]: https://github.com/Digital-Sapphire/PyUpdater/
+[4]: https://theupdateframework.io/overview/#software-updates-101
+[5]: https://peps.python.org/pep-0458/
+[6]: https://peps.python.org/pep-0440/
+[7]: https://github.com/theupdateframework/python-tuf/blob/develop/examples/repo_example/basic_repo.py
+[8]: https://packaging.python.org/en/latest/overview/
+[9]: https://pythonhosted.org/not-so-tuf/
+[10]: https://github.com/dennisvang/tufup-example
+[11]: https://theupdateframework.io/metadata/
+[12]: https://github.com/dennisvang/tufup/blob/master/src/tufup/utils/platform_specific.py
+[13]: https://stackoverflow.com/questions/ask
+[14]: https://github.com/dennisvang/tufup/issues
+[15]: https://theupdateframework.io/overview/#software-updates-101
+[16]: https://theupdateframework.io/security/
+[17]: https://github.com/Digital-Sapphire/PyUpdater#this-is-the-end
+[18]: https://peps.python.org/pep-0440/
+[19]: https://peps.python.org/pep-0440/#public-version-identifiers
+[20]: https://packaging.pypa.io/en/stable/version.html#packaging.version.Version
+[21]: https://github.com/dennisvang/tufup/blob/master/src/tufup/client.py
```

### Comparing `tufup-0.4.9/src/tufup.egg-info/SOURCES.txt` & `tufup-0.5.0/src/tufup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tufup-0.4.9/tests/test_client.py` & `tufup-0.5.0/tests/test_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,313 +1,315 @@
-import logging
-import os
-import pathlib
-import shutil
-from typing import Optional
-import unittest
-from unittest.mock import Mock, patch
-
-from requests.auth import HTTPBasicAuth
-import tuf.api.exceptions
-from tuf.api.metadata import TargetFile
-
-from tests import TempDirTestCase, TEST_REPO_DIR
-from tufup.client import AuthRequestsFetcher, Client
-from tufup.common import TargetMeta
-
-ROOT_FILENAME = 'root.json'
-TARGETS_FILENAME = 'targets.json'
-SNAPSHOT_FILENAME = 'snapshot.json'
-TIMESTAMP_FILENAME = 'timestamp.json'
-ON_GITHUB = os.getenv('GITHUB_ACTIONS')
-
-
-class ClientTests(TempDirTestCase):
-    def setUp(self) -> None:
-        super().setUp()
-        # directory where the parent application is installed (e.g.
-        # %PROGRAMFILES%\MyApp or %LOCALAPPDATA%\Programs\MyApp on Windows 10)
-        # https://docs.microsoft.com/en-us/windows/win32/msi/installation-context
-        self.app_install_dir = self.temp_dir_path / 'programs' / 'example'
-        self.app_install_dir.mkdir(parents=True)
-        # directories must be created by parent application
-        self.metadata_dir = self.temp_dir_path / 'metadata'
-        self.target_dir = self.temp_dir_path / 'targets'
-        self.metadata_dir.mkdir()
-        self.target_dir.mkdir()
-        # parent application must be shipped with root metadata, and must
-        # ensure it is placed in the metadata_dir (without version in filename)
-        shutil.copy(
-            src=TEST_REPO_DIR / 'metadata' / ('1.' + ROOT_FILENAME),
-            dst=self.metadata_dir / ROOT_FILENAME,
-        )
-        # kwargs for client initializer
-        self.client_kwargs = dict(
-            app_name='example_app',
-            app_install_dir=self.app_install_dir,
-            current_version='1.0',
-            metadata_dir=self.metadata_dir,
-            metadata_base_url='http://localhost:8000/metadata/',
-            target_dir=self.target_dir,
-            target_base_url='http://localhost:8000/targets/',
-            session_auth={'http://localhost:8000': ('username', 'password')}
-        )
-
-    def mock_download_metadata(
-            self, rolename: str, length: int, version: Optional[int] = None
-    ) -> bytes:
-        if rolename == 'root':
-            # indicate current root is newest version
-            raise tuf.api.exceptions.DownloadHTTPError(status_code=404, message='')
-        # read from the test repo dir, instead of actually downloading
-        filename = f'{rolename}.json'
-        if version:
-            filename = f'{version}.{filename}'
-        file_path = TEST_REPO_DIR / 'metadata' / filename
-        return file_path.read_bytes()
-
-    def get_refreshed_client(self):
-        # refresh to load targets metadata (mock to prevent actual download)
-        client = Client(**self.client_kwargs)
-        with patch.object(client, '_download_metadata', self.mock_download_metadata):
-            client.refresh()
-        # ensure current archive exists (dummy)
-        shutil.copy(
-            src=TEST_REPO_DIR / 'targets' / client.current_archive.path.name,
-            dst=client.current_archive_local_path,
-        )
-        return client
-
-    def test_init_no_metadata(self):
-        # cannot initialize without root metadata file
-        (self.metadata_dir / ROOT_FILENAME).unlink()
-        with self.assertRaises(FileNotFoundError):
-            Client(**self.client_kwargs)
-
-    def test_init(self):
-        client = Client(**self.client_kwargs)
-        # Client is a subclass of tuf.ngclient.Updater, so it automatically
-        # loads and verifies the local root metadata file
-        self.assertTrue(client._trusted_set.root)
-        # other metadata is not available yet
-        for role_name in ['targets', 'snapshot', 'timestamp']:
-            self.assertIsNone(getattr(client._trusted_set, role_name))
-
-    def test_trusted_target_metas(self):
-        client = self.get_refreshed_client()
-        self.assertTrue(client.trusted_target_metas)
-
-    def test_get_targetinfo(self):
-        client = self.get_refreshed_client()
-        target_path_str = 'example_app-1.0.tar.gz'
-        target_meta = TargetMeta(target_path=target_path_str)
-        for target_path in [target_path_str, target_meta]:
-            target_info = client.get_targetinfo(target_path=target_path)
-            with self.subTest(msg=target_path):
-                self.assertIsInstance(target_info, TargetFile)
-
-    def test_updates_available(self):
-        client = Client(**self.client_kwargs)
-        # test check_for_updates not called
-        with self.assertLogs(logger='tufup.client', level=logging.WARNING) as cm:
-            self.assertFalse(client.updates_available)
-        self.assertIn('check_for_updates', cm.output[0])
-        # test check_for_updates called and update available
-        client.new_targets = {'dummy': None}
-        self.assertTrue(client.updates_available)
-
-    def test_download_and_apply_update(self):
-        # just for completeness...
-        mock_download = Mock(return_value=True)
-        mock_apply = Mock(return_value=True)
-        mock_install = Mock()
-        with patch.multiple(
-                Client, _download_updates=mock_download, _apply_updates=mock_apply
-        ):
-            client = self.get_refreshed_client()
-            client.new_targets = {'dummy': None}
-            client.download_and_apply_update(install=mock_install)
-        self.assertTrue(mock_download.called)
-        self.assertTrue(mock_apply.called)
-        self.assertIn(mock_install, mock_apply.call_args.kwargs.values())
-
-    def test_check_for_updates(self):
-        # expectations (based on targets in tests/data/repository):
-        # - pre=None: only full releases are included, so finds 2.0 patch
-        # - pre='a': finds all, but total patch size exceeds archive size
-        # - pre='b': there is no 'b' release, so this finds same as 'rc'
-        # - pre='rc': finds 2.0 and 3.0rc0, total patch size smaller than archive
-        client = self.get_refreshed_client()
-        with patch.object(client, 'refresh', Mock()):
-            for pre, expected in [(None, 1), ('a', 1), ('b', 2), ('rc', 2)]:
-                with self.subTest(msg=pre):
-                    self.assertTrue(client.check_for_updates(pre=pre))
-                    self.assertEqual(expected, len(client.new_targets))
-                    if pre == 'a':
-                        self.assertTrue(all(
-                            item.is_archive for item in
-                            client.new_targets.keys())
-                        )
-                    else:
-                        self.assertTrue(all(
-                            item.is_patch for item in client.new_targets.keys())
-                        )
-
-    def test_check_for_updates_already_up_to_date(self):
-        self.client_kwargs['current_version'] = '4.0a0'
-        client = self.get_refreshed_client()
-        with patch.object(client, 'refresh', Mock()):
-            self.assertFalse(client.check_for_updates(pre='a'))
-
-    def test_check_for_updates_current_archive_missing(self):
-        client = self.get_refreshed_client()
-        # remove current archive dummy
-        client.current_archive_local_path.unlink()
-        with patch.object(client, 'refresh', Mock()):
-            for pre in [None, 'a', 'b', 'rc']:
-                self.assertTrue(client.check_for_updates(pre=pre))
-                target_meta = next(iter(client.new_targets.keys()))
-                self.assertTrue(target_meta.is_archive)
-
-    def test__download_updates(self):
-        client = Client(**self.client_kwargs)
-        client.new_targets = {Mock(): Mock()}
-        for cached_path, downloaded_path in [('cached', None), (None, 'downloaded')]:
-            with patch.multiple(
-                    client,
-                    find_cached_target=Mock(return_value=cached_path),
-                    download_target=Mock(return_value=downloaded_path),
-            ):
-                self.assertTrue(client._download_updates(progress_hook=None))
-                local_path = next(iter(client.downloaded_target_files.values()))
-                if cached_path:
-                    self.assertEqual(cached_path, str(local_path))
-                else:
-                    self.assertEqual(downloaded_path, str(local_path))
-
-    def test__apply_updates(self):
-        client = self.get_refreshed_client()
-        # directly use target files from test repo as downloaded files
-        client.downloaded_target_files = {
-            target_meta: TEST_REPO_DIR / 'targets' / str(target_meta)
-            for target_meta in client.trusted_target_metas
-            if target_meta.is_patch
-            and str(target_meta.version) in ['2.0', '3.0rc0']
-        }
-        # specify new archive (normally done in _check_updates)
-        archives = [
-            tp for tp in client.trusted_target_metas
-            if tp.is_archive and str(tp.version) == '3.0rc0'
-        ]
-        client.new_archive_info = client.get_targetinfo(archives[-1])
-        client.new_archive_local_path = pathlib.Path(
-            client.target_dir, client.new_archive_info.path
-        )
-        # test confirmation
-        mock_install = Mock()
-        with patch('builtins.input', Mock(return_value='y')):
-            client._apply_updates(install=mock_install, skip_confirmation=False)
-        self.assertTrue(any(client.extract_dir.iterdir()))
-        self.assertTrue(mock_install.called)
-        # test skip confirmation
-        mock_install = Mock()
-        client._apply_updates(install=mock_install, skip_confirmation=True)
-        mock_install.assert_called()
-
-
-class AuthRequestsFetcherTests(unittest.TestCase):
-    def setUp(self) -> None:
-        self.session_auth = {
-            'https://example.net': None,
-            'https://example.com': ('username', 'password'),
-            'https://example.org': HTTPBasicAuth(username='x', password='y'),
-            'http://localhost:8000': ('username', 'password'),
-        }
-
-    def test_init(self):
-        # drop-in replacement for default RequestsFetcher, without args
-        self.assertTrue(AuthRequestsFetcher())
-        # if authentication is required, specify arg
-        fetcher = AuthRequestsFetcher(session_auth=self.session_auth)
-        self.assertEqual(self.session_auth, fetcher.session_auth)
-
-    def test__get_session(self):
-        fetcher = AuthRequestsFetcher(session_auth=self.session_auth)
-        for scheme_and_server, auth in self.session_auth.items():
-            url = scheme_and_server + '/some/path?query=something'
-            with self.subTest(msg=url):
-                session = fetcher._get_session(url=url)
-                self.assertEqual(auth, session.auth)
-
-    @unittest.skipIf(condition=ON_GITHUB, reason='external dependency')
-    def test_fetch_basic_auth(self):
-        # kind of an integration test, as it connects to an external server...
-        scheme_and_server = 'https://httpbin.org'
-        user = 'me'
-        passwd = 'mypassword'
-        url = f'{scheme_and_server}/basic-auth/{user}/{passwd}'
-        session_auth = {
-            scheme_and_server: HTTPBasicAuth(username=user, password=passwd)
-        }
-        fetcher = AuthRequestsFetcher(session_auth=session_auth)
-        # we don't have direct access to the response, so we'll just check
-        # that RequestsFetcher.fetch() doesn't raise an error, such as a
-        # status "401 Unauthorized" or "403 Forbidden"
-        try:
-            fetcher.fetch(url=url)
-        except tuf.api.exceptions.DownloadHTTPError as e:
-            self.fail(msg=f'fetch() raised unexpected HTTPError: {e}')
-
-    def test_attach_progress_hook(self):
-        mock_hook = Mock()
-        bytes_expected = 10
-        fetcher = AuthRequestsFetcher()
-        fetcher.attach_progress_hook(
-            hook=mock_hook, bytes_expected=bytes_expected
-        )
-        bytes_new = 1
-        bytes_downloaded = 0
-        while bytes_downloaded < bytes_expected:
-            bytes_downloaded += bytes_new
-            fetcher._progress(bytes_new=bytes_new)
-            mock_hook.assert_called_with(
-                bytes_downloaded=bytes_downloaded, bytes_expected=bytes_expected
-            )
-
-    def test__chunks_without_progress_hook(self):
-        chunk_size = 10
-        chunk_count = 10
-        chunks = [b'x' * chunk_size] * chunk_count
-
-        def mock_iter_content(*args):
-            yield from chunks
-
-        mock_response = Mock(iter_content=mock_iter_content, close=Mock())
-        fetcher = AuthRequestsFetcher()
-        fetcher.chunk_size = chunk_size
-        # _chunks should work even if attach_progress_hook was not called
-        try:
-            for __ in fetcher._chunks(response=mock_response):
-                pass
-        except Exception as e:
-            self.fail(msg=f'_chunks raised an unexpected exception: {e}')
-
-    def test__chunks_with_progress_hook(self):
-        chunk_size = 10
-        chunk_count = 10
-        chunks = [b'x' * chunk_size] * chunk_count
-
-        def mock_iter_content(*args):
-            yield from chunks
-
-        mock_response = Mock(iter_content=mock_iter_content, close=Mock())
-        fetcher = AuthRequestsFetcher()
-        fetcher.chunk_size = chunk_size
-        # test custom progress hook
-        mock_hook = Mock()
-        bytes_expected = chunk_size * chunk_count
-        fetcher.attach_progress_hook(
-            hook=mock_hook, bytes_expected=bytes_expected
-        )
-        for __ in fetcher._chunks(response=mock_response):
-            pass
-        self.assertEqual(chunk_count, mock_hook.call_count)
+import logging
+import os
+import pathlib
+import shutil
+from typing import Optional
+import unittest
+from unittest.mock import Mock, patch
+
+from requests.auth import HTTPBasicAuth
+import tuf.api.exceptions
+from tuf.ngclient import TargetFile
+
+from tests import TempDirTestCase, TEST_REPO_DIR
+from tufup.client import AuthRequestsFetcher, Client
+from tufup.common import TargetMeta
+
+ROOT_FILENAME = 'root.json'
+TARGETS_FILENAME = 'targets.json'
+SNAPSHOT_FILENAME = 'snapshot.json'
+TIMESTAMP_FILENAME = 'timestamp.json'
+ON_GITHUB = os.getenv('GITHUB_ACTIONS')
+
+
+class ClientTests(TempDirTestCase):
+    def setUp(self) -> None:
+        super().setUp()
+        # directory where the parent application is installed (e.g.
+        # %PROGRAMFILES%\MyApp or %LOCALAPPDATA%\Programs\MyApp on Windows 10)
+        # https://docs.microsoft.com/en-us/windows/win32/msi/installation-context
+        self.app_install_dir = self.temp_dir_path / 'programs' / 'example'
+        self.app_install_dir.mkdir(parents=True)
+        # directories must be created by parent application
+        self.metadata_dir = self.temp_dir_path / 'metadata'
+        self.target_dir = self.temp_dir_path / 'targets'
+        self.metadata_dir.mkdir()
+        self.target_dir.mkdir()
+        # parent application must be shipped with root metadata, and must
+        # ensure it is placed in the metadata_dir (without version in filename)
+        shutil.copy(
+            src=TEST_REPO_DIR / 'metadata' / ('1.' + ROOT_FILENAME),
+            dst=self.metadata_dir / ROOT_FILENAME,
+        )
+        # kwargs for client initializer
+        self.client_kwargs = dict(
+            app_name='example_app',
+            app_install_dir=self.app_install_dir,
+            current_version='1.0',
+            metadata_dir=self.metadata_dir,
+            metadata_base_url='http://localhost:8000/metadata/',
+            target_dir=self.target_dir,
+            target_base_url='http://localhost:8000/targets/',
+            session_auth={'http://localhost:8000': ('username', 'password')}
+        )
+
+    def mock_download_metadata(
+            self, rolename: str, length: int, version: Optional[int] = None
+    ) -> bytes:
+        if rolename == 'root':
+            # indicate current root is newest version
+            raise tuf.api.exceptions.DownloadHTTPError(status_code=404, message='')
+        # read from the test repo dir, instead of actually downloading
+        filename = f'{rolename}.json'
+        if version:
+            filename = f'{version}.{filename}'
+        file_path = TEST_REPO_DIR / 'metadata' / filename
+        return file_path.read_bytes()
+
+    def get_refreshed_client(self):
+        # refresh to load targets metadata (mock to prevent actual download)
+        client = Client(**self.client_kwargs)
+        with patch.object(client, '_download_metadata', self.mock_download_metadata):
+            client.refresh()
+        # ensure current archive exists (dummy)
+        shutil.copy(
+            src=TEST_REPO_DIR / 'targets' / client.current_archive.path.name,
+            dst=client.current_archive_local_path,
+        )
+        return client
+
+    def test_init_no_metadata(self):
+        # cannot initialize without root metadata file
+        (self.metadata_dir / ROOT_FILENAME).unlink()
+        with self.assertRaises(FileNotFoundError):
+            Client(**self.client_kwargs)
+
+    def test_init(self):
+        client = Client(**self.client_kwargs)
+        # Client is a subclass of tuf.ngclient.Updater, so it automatically
+        # loads and verifies the local root metadata file
+        self.assertTrue(client._trusted_set.root)
+        # other metadata is not available yet
+        for role_name in ['targets', 'snapshot', 'timestamp']:
+            # see python-tuf #2250
+            self.assertNotIn(role_name, client._trusted_set)
+
+    def test_trusted_target_metas(self):
+        client = self.get_refreshed_client()
+        self.assertTrue(client.trusted_target_metas)
+
+    def test_get_targetinfo(self):
+        client = self.get_refreshed_client()
+        target_path_str = 'example_app-1.0.tar.gz'
+        target_meta = TargetMeta(target_path=target_path_str)
+        for target_path in [target_path_str, target_meta]:
+            target_info = client.get_targetinfo(target_path=target_path)
+            with self.subTest(msg=target_path):
+                self.assertIsInstance(target_info, TargetFile)
+
+    def test_updates_available(self):
+        client = Client(**self.client_kwargs)
+        # test check_for_updates not called
+        with self.assertLogs(logger='tufup.client', level=logging.WARNING) as cm:
+            self.assertFalse(client.updates_available)
+        self.assertIn('check_for_updates', cm.output[0])
+        # test check_for_updates called and update available
+        client.new_targets = {'dummy': None}
+        self.assertTrue(client.updates_available)
+
+    def test_download_and_apply_update(self):
+        # just for completeness...
+        mock_download = Mock(return_value=True)
+        mock_apply = Mock(return_value=True)
+        mock_install = Mock()
+        with patch.multiple(
+                Client, _download_updates=mock_download, _apply_updates=mock_apply
+        ):
+            client = self.get_refreshed_client()
+            client.new_targets = {'dummy': None}
+            client.download_and_apply_update(install=mock_install)
+        self.assertTrue(mock_download.called)
+        self.assertTrue(mock_apply.called)
+        self.assertIn(mock_install, mock_apply.call_args.kwargs.values())
+
+    def test_check_for_updates(self):
+        # expectations (based on targets in tests/data/repository):
+        # - pre=None: only full releases are included, so finds 2.0 patch
+        # - pre='a': finds all, but total patch size exceeds archive size
+        # - pre='b': there is no 'b' release, so this finds same as 'rc'
+        # - pre='rc': finds 2.0 and 3.0rc0, total patch size smaller than archive
+        client = self.get_refreshed_client()
+        with patch.object(client, 'refresh', Mock()):
+            for pre, expected in [(None, 1), ('a', 1), ('b', 2), ('rc', 2)]:
+                with self.subTest(msg=pre):
+                    self.assertTrue(client.check_for_updates(pre=pre))
+                    self.assertEqual(expected, len(client.new_targets))
+                    if pre == 'a':
+                        self.assertTrue(all(
+                            item.is_archive for item in
+                            client.new_targets.keys())
+                        )
+                    else:
+                        self.assertTrue(all(
+                            item.is_patch for item in client.new_targets.keys())
+                        )
+
+    def test_check_for_updates_already_up_to_date(self):
+        self.client_kwargs['current_version'] = '4.0a0'
+        client = self.get_refreshed_client()
+        with patch.object(client, 'refresh', Mock()):
+            self.assertFalse(client.check_for_updates(pre='a'))
+
+    def test_check_for_updates_current_archive_missing(self):
+        client = self.get_refreshed_client()
+        # remove current archive dummy
+        client.current_archive_local_path.unlink()
+        with patch.object(client, 'refresh', Mock()):
+            for pre in [None, 'a', 'b', 'rc']:
+                self.assertTrue(client.check_for_updates(pre=pre))
+                target_meta = next(iter(client.new_targets.keys()))
+                self.assertTrue(target_meta.is_archive)
+
+    def test__download_updates(self):
+        client = Client(**self.client_kwargs)
+        client.new_targets = {Mock(): Mock()}
+        for cached_path, downloaded_path in [('cached', None), (None, 'downloaded')]:
+            with patch.multiple(
+                    client,
+                    find_cached_target=Mock(return_value=cached_path),
+                    download_target=Mock(return_value=downloaded_path),
+            ):
+                self.assertTrue(client._download_updates(progress_hook=None))
+                local_path = next(iter(client.downloaded_target_files.values()))
+                if cached_path:
+                    self.assertEqual(cached_path, str(local_path))
+                else:
+                    self.assertEqual(downloaded_path, str(local_path))
+
+    def test__apply_updates(self):
+        client = self.get_refreshed_client()
+        # directly use target files from test repo as downloaded files
+        client.downloaded_target_files = {
+            target_meta: TEST_REPO_DIR / 'targets' / str(target_meta)
+            for target_meta in client.trusted_target_metas
+            if target_meta.is_patch
+            and str(target_meta.version) in ['2.0', '3.0rc0']
+        }
+        # specify new archive (normally done in _check_updates)
+        archives = [
+            tp for tp in client.trusted_target_metas
+            if tp.is_archive and str(tp.version) == '3.0rc0'
+        ]
+        client.new_archive_info = client.get_targetinfo(archives[-1])
+        client.new_archive_local_path = pathlib.Path(
+            client.target_dir, client.new_archive_info.path
+        )
+        # test confirmation
+        mock_install = Mock()
+        with patch('builtins.input', Mock(return_value='y')):
+            client._apply_updates(install=mock_install, skip_confirmation=False)
+        self.assertTrue(any(client.extract_dir.iterdir()))
+        self.assertTrue(mock_install.called)
+        # test skip confirmation
+        mock_install = Mock()
+        client._apply_updates(install=mock_install, skip_confirmation=True)
+        mock_install.assert_called()
+
+
+class AuthRequestsFetcherTests(unittest.TestCase):
+    def setUp(self) -> None:
+        self.session_auth = {
+            'https://example.net': None,
+            'https://example.com': ('username', 'password'),
+            'https://example.org': HTTPBasicAuth(username='x', password='y'),
+            'http://localhost:8000': ('username', 'password'),
+        }
+
+    def test_init(self):
+        # drop-in replacement for default RequestsFetcher, without args
+        self.assertTrue(AuthRequestsFetcher())
+        # if authentication is required, specify arg
+        fetcher = AuthRequestsFetcher(session_auth=self.session_auth)
+        self.assertEqual(self.session_auth, fetcher.session_auth)
+
+    def test__get_session(self):
+        fetcher = AuthRequestsFetcher(session_auth=self.session_auth)
+        for scheme_and_server, auth in self.session_auth.items():
+            url = scheme_and_server + '/some/path?query=something'
+            with self.subTest(msg=url):
+                session = fetcher._get_session(url=url)
+                self.assertEqual(auth, session.auth)
+
+    @unittest.skipIf(condition=ON_GITHUB, reason='external dependency')
+    def test_fetch_basic_auth(self):
+        # kind of an integration test, as it connects to an external server...
+        scheme_and_server = 'https://httpbin.org'
+        user = 'me'
+        passwd = 'mypassword'
+        url = f'{scheme_and_server}/basic-auth/{user}/{passwd}'
+        session_auth = {
+            scheme_and_server: HTTPBasicAuth(username=user, password=passwd)
+        }
+        fetcher = AuthRequestsFetcher(session_auth=session_auth)
+        fetcher.socket_timeout = 30  # in case httpbin.org is slow to respond
+        # we don't have direct access to the response, so we'll just check
+        # that RequestsFetcher.fetch() doesn't raise an error, such as a
+        # status "401 Unauthorized" or "403 Forbidden"
+        try:
+            fetcher.fetch(url=url)
+        except tuf.api.exceptions.DownloadHTTPError as e:
+            self.fail(msg=f'fetch() raised unexpected HTTPError: {e}')
+
+    def test_attach_progress_hook(self):
+        mock_hook = Mock()
+        bytes_expected = 10
+        fetcher = AuthRequestsFetcher()
+        fetcher.attach_progress_hook(
+            hook=mock_hook, bytes_expected=bytes_expected
+        )
+        bytes_new = 1
+        bytes_downloaded = 0
+        while bytes_downloaded < bytes_expected:
+            bytes_downloaded += bytes_new
+            fetcher._progress(bytes_new=bytes_new)
+            mock_hook.assert_called_with(
+                bytes_downloaded=bytes_downloaded, bytes_expected=bytes_expected
+            )
+
+    def test__chunks_without_progress_hook(self):
+        chunk_size = 10
+        chunk_count = 10
+        chunks = [b'x' * chunk_size] * chunk_count
+
+        def mock_iter_content(*args):
+            yield from chunks
+
+        mock_response = Mock(iter_content=mock_iter_content, close=Mock())
+        fetcher = AuthRequestsFetcher()
+        fetcher.chunk_size = chunk_size
+        # _chunks should work even if attach_progress_hook was not called
+        try:
+            for __ in fetcher._chunks(response=mock_response):
+                pass
+        except Exception as e:
+            self.fail(msg=f'_chunks raised an unexpected exception: {e}')
+
+    def test__chunks_with_progress_hook(self):
+        chunk_size = 10
+        chunk_count = 10
+        chunks = [b'x' * chunk_size] * chunk_count
+
+        def mock_iter_content(*args):
+            yield from chunks
+
+        mock_response = Mock(iter_content=mock_iter_content, close=Mock())
+        fetcher = AuthRequestsFetcher()
+        fetcher.chunk_size = chunk_size
+        # test custom progress hook
+        mock_hook = Mock()
+        bytes_expected = chunk_size * chunk_count
+        fetcher.attach_progress_hook(
+            hook=mock_hook, bytes_expected=bytes_expected
+        )
+        for __ in fetcher._chunks(response=mock_response):
+            pass
+        self.assertEqual(chunk_count, mock_hook.call_count)
```

### Comparing `tufup-0.4.9/tests/test_common.py` & `tufup-0.5.0/tests/test_common.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-import pathlib
-
-import bsdiff4
-from packaging.version import Version
-
-from tests import TempDirTestCase
-from tufup.common import Patcher, TargetMeta
-
-
-class TestTargetMeta(TempDirTestCase):
-    def test_eq_ne(self):
-        target_meta = TargetMeta()
-        self.assertEqual(target_meta, TargetMeta())
-        self.assertNotEqual(target_meta, TargetMeta(target_path='something'))
-        # two ways to initialize a TargetMeta instance:
-        self.assertEqual(
-            TargetMeta(target_path='my-app-1.2.3a0.patch'),
-            TargetMeta(name='my-app', version='1.2.3a0', is_archive=False),
-        )
-
-    def test_repr(self):
-        # https://docs.python.org/3/reference/datamodel.html#object.__repr__
-        target_meta = TargetMeta(target_path='some.file')
-        # the input to eval is known and trusted, so that should be safe, right?
-        self.assertEqual(eval(repr(target_meta)), target_meta)
-
-    def test_str(self):
-        # see issue #3
-        for target_path in ['str_path', pathlib.Path('pathlib_path')]:
-            with self.subTest(msg=target_path):
-                self.assertIsInstance(
-                    TargetMeta(target_path=target_path).__str__(), str
-                )
-
-    def test_hashable(self):
-        obj = TargetMeta()
-        self.assertEqual(obj.__hash__(), hash(tuple(vars(obj).items())))
-        # we can use the obj as a set member or as dict key
-        self.assertEqual({obj, obj}, {obj})
-
-    def test_sortable(self):
-        version_1 = TargetMeta(target_path='my-app-win-1.0.tar.gz')
-        version_2 = TargetMeta(target_path='my-app-win-2.0.tar.gz')
-        info_list = [version_2, version_1]
-        self.assertEqual([version_1, version_2], sorted(info_list))
-
-    def test_filename(self):
-        target_path = 'url/path/somefile'
-        target_meta = TargetMeta(target_path=target_path)
-        self.assertEqual('somefile', target_meta.filename)
-
-    def test_name(self):
-        target_meta = TargetMeta(target_path='url/path/my-app-1.0.tar.gz')
-        self.assertEqual('my-app', target_meta.name)
-
-    def test_version(self):
-        for version_str in ['1.2.3a4', '']:
-            expected = Version(version_str) if version_str else None
-            with self.subTest(msg=version_str):
-                target_meta = TargetMeta(target_path=f'x-{version_str}.tar.gz')
-                self.assertEqual(expected, target_meta.version)
-
-    def test_suffix(self):
-        valid_suffixes = ['.tar.gz', '.patch']
-        for suffix in ['', '.zip', '.tar.gz', '.patch']:
-            with self.subTest(msg=suffix):
-                target_meta = TargetMeta(target_path=f'my-app-1.2.3a4{suffix}')
-                if suffix in valid_suffixes:
-                    self.assertEqual(suffix, target_meta.suffix)
-                else:
-                    self.assertIsNone(target_meta.suffix)
-
-    def test_is_archive(self):
-        self.assertTrue(TargetMeta(target_path='my-app-1.0.tar.gz').is_archive)
-        self.assertFalse(TargetMeta(target_path='my-app-1.0.patch').is_archive)
-        self.assertFalse(TargetMeta(target_path='my-app-1.0.zip').is_archive)
-
-    def test_is_patch(self):
-        self.assertTrue(TargetMeta(target_path='my-app-1.0.patch').is_patch)
-        self.assertFalse(TargetMeta(target_path='my-app-1.0.tar.gz').is_patch)
-        self.assertFalse(TargetMeta(target_path='my-app-1.0.zip').is_patch)
-
-    def test_is_other(self):
-        self.assertTrue(TargetMeta(target_path='my-app-1.0.zip').is_other)
-        self.assertFalse(TargetMeta(target_path='my-app-1.0.patch').is_other)
-        self.assertFalse(TargetMeta(target_path='my-app-1.0.tar.gz').is_other)
-
-    def test_parse_filename(self):
-        cases = [
-            # PEP440 versions are allowed (we do not parse them here...)
-            ('app-1.patch', ('app', '1', '.patch')),
-            ('app-1.tar.gz', ('app', '1', '.tar.gz')),
-            ('app-1.2.tar.gz', ('app', '1.2', '.tar.gz')),
-            ('app-1.2.3.tar.gz', ('app', '1.2.3', '.tar.gz')),
-            ('app-1a.tar.gz', ('app', '1a', '.tar.gz')),
-            ('app-1b.tar.gz', ('app', '1b', '.tar.gz')),
-            ('app-1rc.tar.gz', ('app', '1rc', '.tar.gz')),
-            ('app-1rc0.tar.gz', ('app', '1rc0', '.tar.gz')),
-            ('app-2022.0.tar.gz', ('app', '2022.0', '.tar.gz')),
-            # we don't impose a specific version format at this point (that
-            # is deferred to packaging.Version)
-            ('app-invalidversion.tar.gz', ('app', 'invalidversion', '.tar.gz')),
-            # underscores, dashes, capitals, etc.
-            ('app-name---1.tar.gz', ('app-name--', '1', '.tar.gz')),
-            ('CAPS-1.tar.gz', ('CAPS', '1', '.tar.gz')),
-            ('un_der_scores-1.0.tar.gz', ('un_der_scores', '1.0', '.tar.gz')),
-            # invalid filenames
-            ('sp ac es-1.zip', ()),
-            ('app-1.gz', ()),
-            ('app-1.xz', ()),
-            ('anything', ()),
-        ]
-        for filename, expected in cases:
-            match_dict = TargetMeta.parse_filename(filename=filename)
-            with self.subTest(msg=filename):
-                self.assertEqual(expected, tuple(match_dict.values()))
-
-    def test_compose_filename(self):
-        filename = TargetMeta.compose_filename(
-            name='app', version='1.0', is_archive=True
-        )
-        self.assertEqual('app-1.0.tar.gz', filename)
-
-
-class PatcherTests(TempDirTestCase):
-    def setUp(self) -> None:
-        super().setUp()
-        # dummy paths
-        self.old_archive_path = self.temp_dir_path / 'my_app-1.0.tar.gz'
-        self.new_archive_path = self.temp_dir_path / 'my_app-2.0.tar.gz'
-        self.new_patch_path = self.temp_dir_path / 'my_app-2.0.patch'
-        # write dummy archive data to files
-        self.old_archive_path.write_bytes(b'old archive data')
-        self.new_archive_data = b'new archive data'
-        self.new_archive_path.write_bytes(self.new_archive_data)
-        # create patch file (see Patcher.create_patch)
-        bsdiff4.file_diff(
-            src_path=self.old_archive_path,
-            dst_path=self.new_archive_path,
-            patch_path=self.new_patch_path,
-        )
-        self.new_patch_data = self.new_patch_path.read_bytes()
-
-    def test_create_patch(self):
-        # remove existing patch file, just to be sure
-        self.new_patch_path.unlink()
-        # test
-        new_patch_path = Patcher.create_patch(
-            src_path=self.old_archive_path, dst_path=self.new_archive_path
-        )
-        self.assertTrue(new_patch_path.exists())
-        self.assertEqual(self.new_patch_data, new_patch_path.read_bytes())
-
-    def test_apply_patch(self):
-        # remove existing "new archive" file, just to be sure
-        self.new_archive_path.unlink()
-        # test
-        new_archive_path = Patcher.apply_patch(
-            src_path=self.old_archive_path, patch_path=self.new_patch_path
-        )
-        self.assertTrue(new_archive_path.exists())
-        self.assertEqual(self.new_archive_data, new_archive_path.read_bytes())
+import pathlib
+
+import bsdiff4
+from packaging.version import Version
+
+from tests import TempDirTestCase
+from tufup.common import Patcher, TargetMeta
+
+
+class TestTargetMeta(TempDirTestCase):
+    def test_eq_ne(self):
+        target_meta = TargetMeta()
+        self.assertEqual(target_meta, TargetMeta())
+        self.assertNotEqual(target_meta, TargetMeta(target_path='something'))
+        # two ways to initialize a TargetMeta instance:
+        self.assertEqual(
+            TargetMeta(target_path='my-app-1.2.3a0.patch'),
+            TargetMeta(name='my-app', version='1.2.3a0', is_archive=False),
+        )
+
+    def test_repr(self):
+        # https://docs.python.org/3/reference/datamodel.html#object.__repr__
+        target_meta = TargetMeta(target_path='some.file')
+        # the input to eval is known and trusted, so that should be safe, right?
+        self.assertEqual(eval(repr(target_meta)), target_meta)
+
+    def test_str(self):
+        # see issue #3
+        for target_path in ['str_path', pathlib.Path('pathlib_path')]:
+            with self.subTest(msg=target_path):
+                self.assertIsInstance(
+                    TargetMeta(target_path=target_path).__str__(), str
+                )
+
+    def test_hashable(self):
+        obj = TargetMeta()
+        self.assertEqual(obj.__hash__(), hash(tuple(vars(obj).items())))
+        # we can use the obj as a set member or as dict key
+        self.assertEqual({obj, obj}, {obj})
+
+    def test_sortable(self):
+        version_1 = TargetMeta(target_path='my-app-win-1.0.tar.gz')
+        version_2 = TargetMeta(target_path='my-app-win-2.0.tar.gz')
+        info_list = [version_2, version_1]
+        self.assertEqual([version_1, version_2], sorted(info_list))
+
+    def test_filename(self):
+        target_path = 'url/path/somefile'
+        target_meta = TargetMeta(target_path=target_path)
+        self.assertEqual('somefile', target_meta.filename)
+
+    def test_name(self):
+        target_meta = TargetMeta(target_path='url/path/my-app-1.0.tar.gz')
+        self.assertEqual('my-app', target_meta.name)
+
+    def test_version(self):
+        for version_str in ['1.2.3a4', '']:
+            expected = Version(version_str) if version_str else None
+            with self.subTest(msg=version_str):
+                target_meta = TargetMeta(target_path=f'x-{version_str}.tar.gz')
+                self.assertEqual(expected, target_meta.version)
+
+    def test_suffix(self):
+        valid_suffixes = ['.tar.gz', '.patch']
+        for suffix in ['', '.zip', '.tar.gz', '.patch']:
+            with self.subTest(msg=suffix):
+                target_meta = TargetMeta(target_path=f'my-app-1.2.3a4{suffix}')
+                if suffix in valid_suffixes:
+                    self.assertEqual(suffix, target_meta.suffix)
+                else:
+                    self.assertIsNone(target_meta.suffix)
+
+    def test_is_archive(self):
+        self.assertTrue(TargetMeta(target_path='my-app-1.0.tar.gz').is_archive)
+        self.assertFalse(TargetMeta(target_path='my-app-1.0.patch').is_archive)
+        self.assertFalse(TargetMeta(target_path='my-app-1.0.zip').is_archive)
+
+    def test_is_patch(self):
+        self.assertTrue(TargetMeta(target_path='my-app-1.0.patch').is_patch)
+        self.assertFalse(TargetMeta(target_path='my-app-1.0.tar.gz').is_patch)
+        self.assertFalse(TargetMeta(target_path='my-app-1.0.zip').is_patch)
+
+    def test_is_other(self):
+        self.assertTrue(TargetMeta(target_path='my-app-1.0.zip').is_other)
+        self.assertFalse(TargetMeta(target_path='my-app-1.0.patch').is_other)
+        self.assertFalse(TargetMeta(target_path='my-app-1.0.tar.gz').is_other)
+
+    def test_parse_filename(self):
+        cases = [
+            # PEP440 versions are allowed (we do not parse them here...)
+            ('app-1.patch', ('app', '1', '.patch')),
+            ('app-1.tar.gz', ('app', '1', '.tar.gz')),
+            ('app-1.2.tar.gz', ('app', '1.2', '.tar.gz')),
+            ('app-1.2.3.tar.gz', ('app', '1.2.3', '.tar.gz')),
+            ('app-1a.tar.gz', ('app', '1a', '.tar.gz')),
+            ('app-1b.tar.gz', ('app', '1b', '.tar.gz')),
+            ('app-1rc.tar.gz', ('app', '1rc', '.tar.gz')),
+            ('app-1rc0.tar.gz', ('app', '1rc0', '.tar.gz')),
+            ('app-2022.0.tar.gz', ('app', '2022.0', '.tar.gz')),
+            # we don't impose a specific version format at this point (that
+            # is deferred to packaging.Version)
+            ('app-invalidversion.tar.gz', ('app', 'invalidversion', '.tar.gz')),
+            # underscores, dashes, capitals, etc.
+            ('app-name---1.tar.gz', ('app-name--', '1', '.tar.gz')),
+            ('CAPS-1.tar.gz', ('CAPS', '1', '.tar.gz')),
+            ('un_der_scores-1.0.tar.gz', ('un_der_scores', '1.0', '.tar.gz')),
+            # invalid filenames
+            ('sp ac es-1.zip', ()),
+            ('app-1.gz', ()),
+            ('app-1.xz', ()),
+            ('anything', ()),
+        ]
+        for filename, expected in cases:
+            match_dict = TargetMeta.parse_filename(filename=filename)
+            with self.subTest(msg=filename):
+                self.assertEqual(expected, tuple(match_dict.values()))
+
+    def test_compose_filename(self):
+        filename = TargetMeta.compose_filename(
+            name='app', version='1.0', is_archive=True
+        )
+        self.assertEqual('app-1.0.tar.gz', filename)
+
+
+class PatcherTests(TempDirTestCase):
+    def setUp(self) -> None:
+        super().setUp()
+        # dummy paths
+        self.old_archive_path = self.temp_dir_path / 'my_app-1.0.tar.gz'
+        self.new_archive_path = self.temp_dir_path / 'my_app-2.0.tar.gz'
+        self.new_patch_path = self.temp_dir_path / 'my_app-2.0.patch'
+        # write dummy archive data to files
+        self.old_archive_path.write_bytes(b'old archive data')
+        self.new_archive_data = b'new archive data'
+        self.new_archive_path.write_bytes(self.new_archive_data)
+        # create patch file (see Patcher.create_patch)
+        bsdiff4.file_diff(
+            src_path=self.old_archive_path,
+            dst_path=self.new_archive_path,
+            patch_path=self.new_patch_path,
+        )
+        self.new_patch_data = self.new_patch_path.read_bytes()
+
+    def test_create_patch(self):
+        # remove existing patch file, just to be sure
+        self.new_patch_path.unlink()
+        # test
+        new_patch_path = Patcher.create_patch(
+            src_path=self.old_archive_path, dst_path=self.new_archive_path
+        )
+        self.assertTrue(new_patch_path.exists())
+        self.assertEqual(self.new_patch_data, new_patch_path.read_bytes())
+
+    def test_apply_patch(self):
+        # remove existing "new archive" file, just to be sure
+        self.new_archive_path.unlink()
+        # test
+        new_archive_path = Patcher.apply_patch(
+            src_path=self.old_archive_path, patch_path=self.new_patch_path
+        )
+        self.assertTrue(new_archive_path.exists())
+        self.assertEqual(self.new_archive_data, new_archive_path.read_bytes())
```

### Comparing `tufup-0.4.9/tests/test_repo.py` & `tufup-0.5.0/tests/test_repo.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,873 +1,873 @@
-import copy
-from datetime import date, datetime, timedelta
-import json
-import logging
-import pathlib
-from tempfile import TemporaryDirectory
-from time import sleep
-from unittest.mock import Mock, patch
-
-from securesystemslib.interface import (
-    generate_and_write_unencrypted_ed25519_keypair,
-    generate_and_write_ed25519_keypair,
-    import_ed25519_publickey_from_file,
-)
-from tuf.api.metadata import (
-    Metadata,
-    Role,
-    Root,
-    Targets,
-    Snapshot,
-    Timestamp,
-    TargetFile,
-    TOP_LEVEL_ROLE_NAMES
-)
-
-from tests import TempDirTestCase, TEST_REPO_DIR
-from tufup.common import TargetMeta
-import tufup.repo  # for patching
-from tufup.repo import (
-    Base, in_, Keys, make_gztar_archive, Repository, Roles, SUFFIX_PUB, SUFFIX_PATCH
-)
-
-
-mock_input = Mock(return_value='')
-
-DUMMY_SSL_KEY = {
-    'keytype': 'ed25519',
-    'scheme': 'ed25519',
-    'keyid': '22f7c6046e29cfb0205a1c07941a5a57da39a6859b844f8c347f622a57ff82c8',
-    'keyid_hash_algorithms': ['sha256', 'sha512'],
-    'keyval': {'public': '93032b5804ba40a725145171193782bdfa30038584715546aea3228ea8018e46'},
-}
-DUMMY_ROOT = Root(
-    version=1,
-    spec_version='1.0',
-    expires=datetime.now() + timedelta(days=1),
-    keys=dict(),
-    roles={
-        role_name: Role(keyids=[], threshold=1)
-        for role_name in TOP_LEVEL_ROLE_NAMES
-    },
-    consistent_snapshot=False,
-)
-DUMMY_EXPIRATION_DAYS = dict(root=1000, targets=100, snapshot=10, timestamp=1)
-DUMMY_PRIVATE_KEY_PATHS = dict(
-    (role_name, [pathlib.Path('dummy', role_name)])
-    for role_name in TOP_LEVEL_ROLE_NAMES
-)
-DUMMY_KEY_MAP = dict(
-    root=['root_one', 'root_two'],
-    targets=['targets'],
-    snapshot=['snapshot'],
-    timestamp=['timestamp'],
-)
-DUMMY_THRESHOLDS = dict(root=4, targets=3, snapshot=2, timestamp=1)
-
-
-class ModuleTests(TempDirTestCase):
-    def test_in_(self):
-        self.assertIsInstance(in_(days=1), datetime)
-
-    def test_make_gztar_archive(self):
-        app_name = 'test'
-        version = '1.2.3'
-        # prepare
-        sub_dir = self.temp_dir_path / 'sub'
-        sub_file = sub_dir / 'sub.txt'
-        root_file = self.temp_dir_path / 'root.txt'
-        sub_dir.mkdir()
-        sub_file.touch()
-        root_file.touch()
-        # test
-        mock_input_no = Mock(return_value='n')
-        for exists in [False, True]:
-            with patch('builtins.input', mock_input_no):
-                archive = make_gztar_archive(
-                    src_dir=self.temp_dir_path,
-                    dst_dir=self.temp_dir_path,
-                    app_name=app_name,
-                    version=version,
-                    base_dir='.',  # this kwarg is allowed
-                    root_dir='some path',  # this kwarg is removed
-                )
-            self.assertIsInstance(archive, TargetMeta)
-            self.assertEqual(exists, mock_input_no.called)
-            self.assertTrue(archive.path.exists())
-            self.assertTrue(app_name in str(archive.path))
-            self.assertTrue(version in str(archive.path))
-
-
-class BaseTests(TempDirTestCase):
-    def test_init(self):
-        with patch('builtins.input', mock_input):
-            # dir exists
-            base = Base(dir_path=self.temp_dir_path)
-            self.assertTrue(base.dir_path.exists())
-            # dir does not exist yet
-            base = Base(dir_path=self.temp_dir_path / 'new')
-            self.assertTrue(base.dir_path.exists())
-
-
-class KeysTests(TempDirTestCase):
-    def test_init_no_key_files(self):
-        # no public key files exist yet
-        keys = Keys(dir_path=self.temp_dir_path)
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            self.assertFalse(getattr(keys, role_name))
-
-    def test_init_and_import_all_public_keys(self):
-        # create some key files
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            private_key_filename = Keys.filename_pattern.format(key_name=role_name)
-            file_path = self.temp_dir_path / private_key_filename
-            generate_and_write_unencrypted_ed25519_keypair(filepath=str(file_path))
-        # test
-        keys = Keys(dir_path=self.temp_dir_path)
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            self.assertIsInstance(getattr(keys, role_name)[0], dict)
-
-    def test_init_and_import_all_public_keys_with_key_map(self):
-        # create a single key-pair
-        key_name = 'single'
-        private_key_filename = Keys.filename_pattern.format(key_name=key_name)
-        file_path = self.temp_dir_path / private_key_filename
-        generate_and_write_unencrypted_ed25519_keypair(filepath=str(file_path))
-        key_map = {role_name: [key_name] for role_name in TOP_LEVEL_ROLE_NAMES}
-        # test
-        keys = Keys(dir_path=self.temp_dir_path, key_map=key_map)
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            self.assertIsInstance(getattr(keys, role_name)[0], dict)
-            # all keys should be equal
-            self.assertEqual(keys.root, getattr(keys, role_name))
-
-    def test_import_all_public_keys(self):
-        # note: import_all_public_keys is also (implicitly) tested via __init__
-        keys = Keys(dir_path=self.temp_dir_path)
-        # create some key files
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            private_key_filename = Keys.filename_pattern.format(
-                key_name=role_name)
-            file_path = self.temp_dir_path / private_key_filename
-            generate_and_write_unencrypted_ed25519_keypair(
-                filepath=str(file_path))
-        # test
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            self.assertFalse(getattr(keys, role_name))
-        keys.import_all_public_keys()
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            self.assertIsInstance(getattr(keys, role_name)[0], dict)
-
-    def test_import_public_key(self):
-        # create dummy key with name differing from role name
-        key_name = 'test'
-        role_name = 'targets'
-        private_key_filename = Keys.filename_pattern.format(key_name=key_name)
-        file_path = self.temp_dir_path / private_key_filename
-        generate_and_write_unencrypted_ed25519_keypair(filepath=str(file_path))
-        # test
-        keys = Keys(dir_path=self.temp_dir_path)
-        keys.import_public_key(role_name=role_name, key_name=key_name)
-        self.assertTrue(keys.targets)
-
-    def test_create(self):
-        with patch('getpass.getpass', mock_input):
-            keys = Keys(dir_path=self.temp_dir_path, encrypted=['root'])
-            keys.create()
-            # key pair files should now exist
-            filenames = [item.name for item in keys.dir_path.iterdir()]
-            for role_name in TOP_LEVEL_ROLE_NAMES:
-                private_key_filename = Keys.filename_pattern.format(key_name=role_name)
-                public_key_filename = private_key_filename + SUFFIX_PUB
-                self.assertIn(private_key_filename, filenames)
-                self.assertIn(public_key_filename, filenames)
-            # and the public keys should have been imported
-            self.assertTrue(all(getattr(keys, n) for n in TOP_LEVEL_ROLE_NAMES))
-
-    def test_create_with_key_map(self):
-        # prepare
-        keys = Keys(dir_path=self.temp_dir_path, key_map=DUMMY_KEY_MAP)
-        expected_key_names = [
-            key_name
-            for key_names in DUMMY_KEY_MAP.values()
-            for key_name in key_names
-        ]
-        # test
-        keys.create()
-        # we should now have five key-pairs (one for each, but two for root)
-        filenames = [item.name for item in keys.dir_path.iterdir()]
-        self.assertEqual(2*len(expected_key_names), len(filenames))
-        for key_name in expected_key_names:
-            self.assertIn(key_name, filenames)
-            self.assertIn(key_name + SUFFIX_PUB, filenames)
-        # and the public keys should have been imported
-        for role_name, key_names in DUMMY_KEY_MAP.items():
-            self.assertEqual(len(key_names), len(getattr(keys, role_name)))
-
-    def test_create_key_pair(self):
-        public_key_path = Keys.create_key_pair(
-            private_key_path=self.temp_dir_path / 'key_name', encrypted=False
-        )
-        self.assertTrue(public_key_path.exists())
-
-    def test_create_key_pair_do_not_overwrite(self):
-        # create dummy key pair
-        key_name = 'dummy'
-        private_key_filename = Keys.filename_pattern.format(key_name=key_name)
-        private_key_path = self.temp_dir_path / private_key_filename
-        generate_and_write_unencrypted_ed25519_keypair(
-            filepath=str(private_key_path)
-        )
-        original_private_key = private_key_path.read_bytes()
-        with patch('builtins.input', Mock(return_value='n')):
-            Keys.create_key_pair(
-                private_key_path=private_key_path, encrypted=False
-            )
-        self.assertEqual(original_private_key, private_key_path.read_bytes())
-
-    def test_public(self):
-        keys = Keys(dir_path=self.temp_dir_path)
-        # test empty
-        self.assertFalse(keys.public())
-        # set a dummy key value
-        keys.root = [DUMMY_SSL_KEY]
-        # test
-        self.assertIn(DUMMY_SSL_KEY['keyid'], keys.public().keys())
-
-    def test_roles(self):
-        keys = Keys(dir_path=self.temp_dir_path)
-        # test empty
-        self.assertSetEqual(set(TOP_LEVEL_ROLE_NAMES), set(keys.roles().keys()))
-        # set a dummy key value
-        keys.root = [DUMMY_SSL_KEY]
-        # test
-        self.assertIn('root', keys.roles().keys())
-
-    def test_roles_thresholds(self):
-        # prepare
-        keys = Keys(dir_path=self.temp_dir_path, thresholds=DUMMY_THRESHOLDS)
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            setattr(keys, role_name, [DUMMY_SSL_KEY])
-        # test
-        roles = keys.roles()
-        for key, value in roles.items():
-            self.assertEqual(DUMMY_THRESHOLDS[key], value.threshold)
-
-    def test_find_private_key(self):
-        # create dummy private key files in separate folders
-        key_names = [
-            ('online', [Snapshot.type, Timestamp.type]),
-            ('offline', [Root.type, Targets.type]),
-        ]
-        key_dirs = []
-        for dir_name, role_names  in key_names:
-            dir_path = self.temp_dir_path / dir_name
-            dir_path.mkdir()
-            key_dirs.append(dir_path)
-            for role_name in role_names:
-                filename = Keys.filename_pattern.format(key_name=role_name)
-                (dir_path / filename).touch()
-        # test
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            key_path = Keys.find_private_key(key_name=role_name, key_dirs=key_dirs)
-            self.assertIn(role_name, str(key_path))
-            self.assertTrue(key_path.exists())
-
-
-class RolesTests(TempDirTestCase):
-    def test_init(self):
-        self.assertTrue(Roles(dir_path=self.temp_dir_path))
-
-    def test_init_import_roles(self):
-        def mock_from_file(filename, *args, **kwargs):
-            file_path = pathlib.Path(filename)
-            assert file_path.exists()
-            return file_path.stem
-
-        # create dummy metadata files
-        for role_name in TOP_LEVEL_ROLE_NAMES:
-            filenames = [f'{role_name}.json']
-            if role_name == 'root':
-                filenames.extend(f'{v}.{role_name}.json' for v in [1, 2, 3])
-            for filename in filenames:
-                (self.temp_dir_path / filename).touch()
-        # test
-        with patch.object(tufup.repo.Metadata, 'from_file', mock_from_file):
-            roles = Roles(dir_path=self.temp_dir_path)
-            for role_name in TOP_LEVEL_ROLE_NAMES:
-                self.assertEqual(role_name, getattr(roles, role_name))
-
-    def test_initialize_empty(self):
-        # prepare
-        mock_keys = Mock()
-        mock_keys.public = Mock()
-        mock_keys.roles = Mock(
-            return_value={name: None for name in TOP_LEVEL_ROLE_NAMES}
-        )
-        roles = Roles(dir_path=self.temp_dir_path)
-        # test
-        roles.initialize(keys=mock_keys)
-        self.assertTrue(
-            all(
-                isinstance(getattr(roles, n), Metadata)
-                for n in TOP_LEVEL_ROLE_NAMES
-            )
-        )
-        # files do not exist yet, because the roles still need to be populated
-        self.assertFalse(any(roles.dir_path.iterdir()))
-
-    def test_initialize_existing_root(self):
-        # prepare
-        mock_keys = Mock()
-        mock_keys.public = Mock()
-        mock_keys.roles = Mock(return_value={n: None for n in TOP_LEVEL_ROLE_NAMES})
-        roles = Roles(dir_path=self.temp_dir_path)
-        # set existing root role
-        mock_root_role = Mock()
-        roles.root = mock_root_role
-        # test
-        roles.initialize(keys=mock_keys)
-        # ensure the existing role has not been replaced
-        self.assertEqual(mock_root_role, roles.root)
-
-    def test_add_or_update_target(self):
-        # prepare
-        roles = Roles(dir_path=self.temp_dir_path)
-        roles.targets = Mock(signed=Mock(targets=dict()))
-        # test
-        filename = 'my_app.tar.gz'
-        local_target_path = self.temp_dir_path / filename
-        # path must exist
-        with self.assertRaises(FileNotFoundError):
-            roles.add_or_update_target(local_path=local_target_path)
-        local_target_path.write_bytes(b'some bytes')
-        # test
-        for segments, expected_url_path in [
-            (None, filename), ([], filename), (['a', 'b'], 'a/b/' + filename)
-        ]:
-            roles.add_or_update_target(
-                local_path=local_target_path, url_path_segments=segments
-            )
-            with self.subTest(msg=segments):
-                self.assertIsInstance(
-                    roles.targets.signed.targets[expected_url_path], TargetFile
-                )
-
-    def test_remove_target(self):
-        # prepare
-        filename = 'my_app-1.0.tar.gz'
-        dirname = 'subdir'
-        url_path = f'{dirname}/{filename}'
-        subdir = self.temp_dir_path / dirname
-        subdir.mkdir()
-        local_target_path = subdir / filename
-        local_target_path.touch()
-        roles = Roles(dir_path=self.temp_dir_path)
-        roles.targets = Mock(signed=Mock(targets={url_path: Mock()}))
-        original_targets_signed = copy.deepcopy(roles.targets.signed)
-        # test
-        self.assertTrue(local_target_path.exists())
-        roles.remove_target(local_path=local_target_path)
-        self.assertNotIn(filename, roles.targets.signed.targets)
-        self.assertFalse(local_target_path.exists())
-        self.assertNotEqual(original_targets_signed, roles.targets.signed)
-        # cannot remove non-existent target
-        self.assertFalse(roles.remove_target(local_path=local_target_path))
-
-    def test_add_public_key(self):
-        # prepare
-        roles = Roles(dir_path=self.temp_dir_path)
-        roles.root = Mock(signed=Mock(roles=dict(), add_key=Mock()))
-        public_key_path = self.temp_dir_path / 'targets_key.pub'
-        public_key_path.write_text(json.dumps(DUMMY_SSL_KEY))
-        # test
-        role_name = 'targets'
-        roles.add_public_key(role_name=role_name, public_key_path=public_key_path)
-        self.assertTrue(roles.root.signed.add_key.called)
-
-    def test_set_signature_threshold(self):
-        # prepare
-        role_name = 'targets'
-        threshold = 2
-        roles = Roles(dir_path=self.temp_dir_path)
-        roles.root = Mock(signed=Mock(roles={role_name: Mock(threshold=1)}))
-        # test
-        roles.set_signature_threshold(role_name=role_name, threshold=threshold)
-        self.assertEqual(threshold, roles.root.signed.roles[role_name].threshold)
-
-    def test_sign_role(self):
-        # prepare
-        roles = Roles(dir_path=self.temp_dir_path)
-        roles.root = Metadata(signed=DUMMY_ROOT, signatures=dict())
-        role_name = 'root'
-        signature_count = 2
-        password = 'mock-password'
-        with patch('getpass.getpass', Mock(return_value=password)):
-            for index in range(signature_count):
-                private_key_path = self.temp_dir_path / f'{index}.{role_name}'
-                # create key pair
-                if index == 0:
-                    generate_and_write_unencrypted_ed25519_keypair(
-                        filepath=str(private_key_path)
-                    )
-                else:
-                    generate_and_write_ed25519_keypair(
-                        password=password, filepath=str(private_key_path)
-                    )
-                # test
-                roles.sign_role(
-                    role_name=role_name, private_key_path=private_key_path
-                )
-        self.assertEqual(signature_count, len(roles.root.signatures))
-
-    def test_file_path(self):
-        # prepare
-        roles = Roles(dir_path=self.temp_dir_path)
-        # test
-        self.assertEqual(
-            self.temp_dir_path / '1.root.json',
-            roles.file_path(role_name='root', version=1),
-        )
-        self.assertEqual(
-            self.temp_dir_path / 'root.json',
-            roles.file_path(role_name='root'),
-        )
-        self.assertEqual(
-            self.temp_dir_path / 'targets.json',
-            roles.file_path(role_name='targets', version=1),
-        )
-
-    def test_file_exists(self):
-        # prepare
-        roles = Roles(dir_path=self.temp_dir_path)
-        (self.temp_dir_path / '1.root.json').touch()
-        # test
-        self.assertTrue(roles.file_exists(role_name='root'))
-        self.assertFalse(roles.file_exists(role_name='targets'))
-
-    def test_persist_role(self):
-        # prepare
-        roles = Roles(dir_path=self.temp_dir_path)
-        roles.root = Metadata(signed=DUMMY_ROOT, signatures=dict())
-        expected_filenames = [f'{DUMMY_ROOT.version}.root.json', 'root.json']
-        # test
-        roles.persist_role(role_name='root')
-        for filename in expected_filenames:
-            with self.subTest(msg=filename):
-                self.assertTrue((self.temp_dir_path / filename).exists())
-
-    def test_get_latest_archive(self):
-        roles = Roles(dir_path=TEST_REPO_DIR / 'metadata')
-        expected_filename = 'example_app-4.0a0.tar.gz'
-        latest_archive = roles.get_latest_archive()
-        self.assertEqual(expected_filename, latest_archive.path.name)
-
-    def test_get_latest_archive_empty(self):
-        roles = Roles(dir_path=self.temp_dir_path)
-        self.assertIsNone(roles.get_latest_archive())
-
-
-class RepositoryTests(TempDirTestCase):
-    @classmethod
-    def setUpClass(cls) -> None:
-        logging.basicConfig(level=logging.DEBUG)
-
-    def test_defaults(self):
-        self.assertTrue(Repository(app_name='test'))
-
-    def test_config_dict(self):
-        app_name = 'test'
-        repo = Repository(app_name=app_name)
-        expected_config_dict = {
-            'app_name': app_name,
-            'app_version_attr': None,
-            'encrypted_keys': None,
-            'expiration_days': None,
-            'key_map': None,
-            'keys_dir': None,
-            'repo_dir': None,
-            'thresholds': None,
-        }
-        self.assertEqual(set(expected_config_dict), set(repo.config_dict))
-
-    def test_app_version(self):
-        # for convenience we use the notosotuf version attribute here,
-        # but normally this would point to an external app version e.g.
-        # 'my_app.__version__'
-        app_version_attr = 'tufup.__version__'
-        repo = Repository(app_name='test', app_version_attr=app_version_attr)
-        self.assertEqual(str(tufup.__version__), repo.app_version)
-
-    def test_get_config_file_path(self):
-        self.assertTrue(Repository.get_config_file_path())
-
-    def test_save_config(self):
-        # prepare
-        repo = Repository(app_name='test')
-        # test
-        repo.save_config()
-        self.assertTrue(repo.get_config_file_path().exists())
-        print(repo.get_config_file_path().read_text())
-
-    def test_load_config(self):
-        # file does not exist
-        self.assertEqual(dict(), Repository.load_config())
-        # file exists but invalid
-        Repository.get_config_file_path().touch()
-        # test
-        self.assertEqual(dict(), Repository.load_config())
-
-    def test_from_config(self):
-        temp_dir = self.temp_dir_path.resolve()
-        # prepare
-        config_data = dict(
-            app_name='test',
-            app_version_attr='my_app.__version__',
-            repo_dir=temp_dir / 'repo',
-            keys_dir=temp_dir / 'keystore',
-            key_map=dict(),
-            encrypted_keys=[],
-            expiration_days=dict(),
-            thresholds=dict(),
-        )
-        Repository.get_config_file_path().write_text(
-            json.dumps(config_data, default=str)
-        )
-        mock_load_keys_and_roles = Mock()
-        # test
-        with patch.object(
-                Repository, '_load_keys_and_roles', mock_load_keys_and_roles,
-        ):
-            repo = Repository.from_config()
-        self.assertEqual(
-            config_data,
-            {item: getattr(repo, item) for item in config_data.keys()},
-        )
-        self.assertTrue(mock_load_keys_and_roles.called)
-
-    def test_initialize(self):
-        # prepare
-        repo = Repository(
-            app_name='test',
-            keys_dir=self.temp_dir_path / 'keystore',
-            repo_dir=self.temp_dir_path / 'repo',
-            expiration_days=DUMMY_EXPIRATION_DAYS,
-        )
-        # test
-        repo.initialize()
-        self.assertTrue(any(repo.keys_dir.iterdir()))
-        self.assertTrue(any(repo.metadata_dir.iterdir()))
-        self.assertTrue(
-            all(getattr(repo.roles, name) for name in TOP_LEVEL_ROLE_NAMES)
-        )
-        self.assertEqual(
-            date.today() + timedelta(days=DUMMY_EXPIRATION_DAYS['root']),
-            repo.roles.root.signed.expires.date(),
-        )
-
-    def test_refresh_expiration_date(self):
-        repo = Repository(
-            app_name='test',
-            keys_dir=self.temp_dir_path / 'keystore',
-            repo_dir=self.temp_dir_path / 'repo',
-        )
-        repo.initialize()  # todo: make test independent...
-        days = 999
-        repo.refresh_expiration_date(role_name='root', days=days)
-        self.assertEqual(
-            date.today() + timedelta(days=days),
-            repo.roles.root.signed.expires.date(),
-        )
-
-    def test_replace_key(self):
-        role_name = 'root'
-        # prepare
-        new_key_name = 'new_key'
-        old_key_name = 'old-key'
-        key_map = {name: [name] for name in TOP_LEVEL_ROLE_NAMES}
-        key_map['root'].append(old_key_name)
-        key_map['targets'] = [old_key_name]
-        repo = Repository(
-            app_name='test',
-            keys_dir=self.temp_dir_path / 'keystore',
-            repo_dir=self.temp_dir_path / 'repo',
-            key_map=key_map,
-        )
-        repo.initialize()  # todo: make test independent...
-        old_key_id = repo.roles.root.signed.roles['targets'].keyids[0]
-        # create new key pair to replace old one
-        new_private_key_path = repo.keys_dir / new_key_name
-        new_public_key_path = Keys.create_key_pair(
-            private_key_path=new_private_key_path, encrypted=False
-        )
-        new_key_id = import_ed25519_publickey_from_file(
-            filepath=str(new_public_key_path)
-        )['keyid']
-        # test
-        expected_key_count = len(key_map[role_name])
-        repo.replace_key(
-            old_key_name=old_key_name,
-            new_public_key_path=new_public_key_path,
-            new_private_key_encrypted=True,  # pretend the key is encrypted
-        )
-        self.assertEqual(
-            expected_key_count,
-            len(repo.roles.root.signed.roles[role_name].keyids),
-        )
-        # old key removed?
-        self.assertNotIn(
-            old_key_id, repo.roles.root.signed.roles[role_name].keyids
-        )
-        self.assertNotIn(old_key_name, repo.key_map[role_name])
-        self.assertIn(old_key_name, repo.revoked_key_names)
-        # new key added?
-        self.assertIn(
-            new_key_id, repo.roles.root.signed.roles[role_name].keyids
-        )
-        self.assertIn(new_key_name, repo.key_map[role_name])
-        self.assertIn(new_key_name, repo.encrypted_keys)
-        # no duplicates in encrypted_keys?
-        self.assertEqual(1, len(repo.encrypted_keys))
-        # other keys still in key map?
-        self.assertEqual(expected_key_count, len(repo.key_map[role_name]))
-        # keys replaced for all roles?
-        self.assertIn(new_key_name, repo.key_map['targets'])
-
-    def test_add_key(self):
-        repo = Repository(
-            app_name='test',
-            keys_dir=self.temp_dir_path / 'keystore',
-            repo_dir=self.temp_dir_path / 'repo',
-        )
-        repo.initialize()  # todo: make test independent...
-        # create new key pair to add
-        new_key_name = 'new-key'
-        new_private_key_path = repo.keys_dir / new_key_name
-        new_public_key_path = Keys.create_key_pair(
-            private_key_path=new_private_key_path, encrypted=False
-        )
-        new_key_id = import_ed25519_publickey_from_file(
-            filepath=str(new_public_key_path)
-        )['keyid']
-        # test
-        role_name = 'root'
-        repo.add_key(
-            role_name=role_name,
-            public_key_path=new_public_key_path,
-            encrypted=True,  # pretend the key is encrypted
-        )
-        # new key added?
-        self.assertEqual(2, len(repo.roles.root.signed.roles[role_name].keyids))
-        self.assertIn(
-            new_key_id, repo.roles.root.signed.roles[role_name].keyids
-        )
-        self.assertIn(new_key_name, repo.key_map[role_name])
-        self.assertIn(new_key_name, repo.encrypted_keys)
-
-    def test_add_bundle(self):
-        # prepare
-        bundle_dir = self.temp_dir_path / 'dist' / 'test_app'
-        bundle_dir.mkdir(parents=True)
-        bundle_file = bundle_dir / 'dummy.exe'
-        bundle_file.touch()
-        repo = Repository(
-            app_name='test',
-            keys_dir=self.temp_dir_path / 'keystore',
-            repo_dir=self.temp_dir_path / 'repo',
-        )
-        repo.initialize()  # todo: make test independent...
-        # test
-        repo.add_bundle(new_version='1.0', new_bundle_dir=bundle_dir)
-        self.assertTrue((repo.metadata_dir / 'targets.json').exists())
-
-    def test_add_bundle_no_patch(self):
-        # prepare
-        bundle_dir = self.temp_dir_path / 'dist' / 'test_app'
-        bundle_dir.mkdir(parents=True)
-        bundle_file = bundle_dir / 'dummy.exe'
-        bundle_file.write_text('this is version 1')
-        repo = Repository(
-            app_name='test',
-            keys_dir=self.temp_dir_path / 'keystore',
-            repo_dir=self.temp_dir_path / 'repo',
-        )
-        repo.initialize()  # todo: make test independent...
-        repo.add_bundle(new_version='1.0', new_bundle_dir=bundle_dir)
-        # test
-        bundle_file.write_text('much has changed in version 2')
-        repo.add_bundle(
-            new_version='2.0', new_bundle_dir=bundle_dir, skip_patch=True
-        )
-        self.assertTrue((repo.metadata_dir / 'targets.json').exists())
-        target_keys = list(repo.roles.targets.signed.targets.keys())
-        self.assertEqual(2, len(target_keys))
-        self.assertFalse(any(key.endswith(SUFFIX_PATCH) for key in target_keys))
-
-    def test_remove_latest_bundle(self):
-        # prepare
-        bundle_dir = self.temp_dir_path / 'dist' / 'test_app'
-        bundle_dir.mkdir(parents=True)
-        bundle_file = bundle_dir / 'dummy.exe'
-        bundle_file.touch()
-        repo = Repository(
-            app_name='test',
-            keys_dir=self.temp_dir_path / 'keystore',
-            repo_dir=self.temp_dir_path / 'repo',
-        )
-        repo.initialize()  # todo: make test independent...
-        v1 = '1.0'
-        v2 = '2.0'
-        repo.add_bundle(new_version=v1, new_bundle_dir=bundle_dir)
-        repo.add_bundle(new_version=v2, new_bundle_dir=bundle_dir)
-        # test
-        repo.remove_latest_bundle()
-        remaining_target_keys = list(repo.roles.targets.signed.targets.keys())
-        self.assertEqual(1, len(remaining_target_keys))
-        self.assertIn(v1, remaining_target_keys[0])
-        remaining_target_filenames = [p.name for p in repo.targets_dir.iterdir()]
-        self.assertEqual(1, len(remaining_target_filenames))
-        self.assertIn(remaining_target_keys[0], remaining_target_filenames)
-
-    def test_threshold_sign(self):
-        # prepare
-        role_name = 'root'
-        keys_dir = self.temp_dir_path / 'keystore'
-        repo = Repository(
-            app_name='test',
-            keys_dir=keys_dir,
-            repo_dir=self.temp_dir_path / 'repo',
-        )
-        repo.initialize()  # todo: make test independent...
-        # create dummy "revoked key" and pretend it is encrypted
-        revoked_key_name = 'revoked'
-        repo.keys.create_key_pair(
-            private_key_path=keys_dir / revoked_key_name, encrypted=False
-        )
-        repo.revoked_key_names.append(revoked_key_name)
-        repo.encrypted_keys.append(revoked_key_name)
-        # dummy modification
-        repo.roles.root.signed.spec_version = 'x'
-        versioned_file_path = repo.metadata_dir / f'1.{role_name}.json'
-        non_versioned_file_path = repo.metadata_dir / f'{role_name}.json'
-        versioned_last_modified = versioned_file_path.stat().st_mtime_ns
-        non_versioned_last_modified = non_versioned_file_path.stat().st_mtime_ns
-        # test
-        sleep(0.1)  # enforce different modification time
-        count = repo.threshold_sign(
-            role_name=role_name, private_key_dirs=[repo.keys_dir]
-        )
-        self.assertEqual(2, count)  # existing key and revoked key
-        self.assertFalse(repo.revoked_key_names)
-        self.assertFalse(repo.encrypted_keys)
-        # files should have been modified
-        self.assertGreater(
-            versioned_file_path.stat().st_mtime_ns, versioned_last_modified
-        )
-        self.assertGreater(
-            non_versioned_file_path.stat().st_mtime_ns, non_versioned_last_modified
-        )
-        # if no signatures found
-        for path in repo.keys_dir.iterdir():
-            path.unlink()
-        with self.assertRaises(Exception):
-            repo.threshold_sign(
-                role_name=role_name, private_key_dirs=[repo.keys_dir]
-            )
-
-    def test__load_keys_and_roles(self):
-        # prepare
-        keys_dir = self.temp_dir_path / 'keystore'
-        repo = Repository(
-            app_name='test',
-            keys_dir=keys_dir,
-            repo_dir=self.temp_dir_path / 'repo',
-        )
-        # test
-        with patch('builtins.input', Mock(return_value='y')):
-            repo._load_keys_and_roles(create_keys=True)
-        self.assertTrue(
-            all(getattr(repo.roles, name) for name in TOP_LEVEL_ROLE_NAMES)
-        )
-        self.assertTrue(
-            all((keys_dir / name).exists() for name in TOP_LEVEL_ROLE_NAMES)
-        )
-
-    def test_publish_changes_no_change(self):
-        # prepare
-        repo = Repository(
-            app_name='test',
-            keys_dir=self.temp_dir_path / 'keystore',
-            repo_dir=self.temp_dir_path / 'repo',
-        )
-        # note that initialize() already calls publish_changes...
-        repo.initialize()  # todo: make test independent...
-        # test
-        repo.publish_changes(private_key_dirs=[repo.keys_dir])
-        for role_name in ['root', 'targets', 'snapshot', 'timestamp']:
-            role = getattr(repo.roles, role_name)
-            with self.subTest(msg=role_name):
-                self.assertEqual(1, role.signed.version)
-                self.assertTrue(role.signatures)
-
-    def test_publish_changes_threshold(self):
-        # prepare
-        repo = Repository(
-            app_name='test',
-            keys_dir=self.temp_dir_path / 'keystore',
-            repo_dir=self.temp_dir_path / 'repo',
-        )
-        # note that initialize() already calls publish_changes...
-        repo.initialize()  # todo: make test independent...
-        # remove the root signature
-        repo.roles.root.signatures = {}
-        # test
-        repo.publish_changes(private_key_dirs=[repo.keys_dir])
-        for role_name in ['root', 'targets', 'snapshot', 'timestamp']:
-            with self.subTest(msg=role_name):
-                role = getattr(repo.roles, role_name)
-                self.assertEqual(
-                    repo.thresholds[role_name], len(role.signatures)
-                )
-
-    def test_publish_changes(self):
-        days = 999
-        role_names = ['root', 'targets', 'snapshot', 'timestamp']
-        for test_role_name in role_names.copy():
-            # use a fresh temporary dir and repo
-            with TemporaryDirectory() as temp_dir:
-                temp_dir_path = pathlib.Path(temp_dir)
-                repo = Repository(
-                    app_name='test',
-                    keys_dir=temp_dir_path / 'keystore',
-                    repo_dir=temp_dir_path / 'repo',
-                )
-                # note that initialize() already calls publish_changes...
-                repo.initialize()  # todo: make test independent...
-                # make a change to metadata (in memory)
-                repo.roles.set_expiration_date(
-                    role_name=test_role_name, days=days
-                )
-                # make a change to config
-                config_change = 'dummy'
-                repo.encrypted_keys.append(config_change)
-                # test
-                repo.publish_changes(private_key_dirs=[repo.keys_dir])
-                for role_name in role_names:
-                    role = getattr(repo.roles, role_name)
-                    with self.subTest(msg=f'{test_role_name}: {role_name}'):
-                        self.assertEqual(2, role.signed.version)
-                        self.assertTrue(role.signatures)
-                role_names.remove(test_role_name)
-                #  re-load from file to verify change
-                root = Metadata.from_file(
-                    repo.roles.file_path(role_name=test_role_name)
-                )
-                self.assertEqual(
-                    date.today() + timedelta(days=days),
-                    root.signed.expires.date(),
-                )
-                # verify change in config
-                config_from_disk = repo.load_config()
-                self.assertIn(
-                    config_change, config_from_disk['encrypted_keys']
-                )
+import copy
+from datetime import date, datetime, timedelta
+import json
+import logging
+import pathlib
+from tempfile import TemporaryDirectory
+from time import sleep
+from unittest.mock import Mock, patch
+
+from securesystemslib.interface import (
+    generate_and_write_unencrypted_ed25519_keypair,
+    generate_and_write_ed25519_keypair,
+    import_ed25519_publickey_from_file,
+)
+from tuf.api.metadata import (
+    Metadata,
+    Role,
+    Root,
+    Targets,
+    Snapshot,
+    Timestamp,
+    TargetFile,
+    TOP_LEVEL_ROLE_NAMES
+)
+
+from tests import TempDirTestCase, TEST_REPO_DIR
+from tufup.common import TargetMeta
+import tufup.repo  # for patching
+from tufup.repo import (
+    Base, in_, Keys, make_gztar_archive, Repository, Roles, SUFFIX_PUB, SUFFIX_PATCH
+)
+
+
+mock_input = Mock(return_value='')
+
+DUMMY_SSL_KEY = {
+    'keytype': 'ed25519',
+    'scheme': 'ed25519',
+    'keyid': '22f7c6046e29cfb0205a1c07941a5a57da39a6859b844f8c347f622a57ff82c8',
+    'keyid_hash_algorithms': ['sha256', 'sha512'],
+    'keyval': {'public': '93032b5804ba40a725145171193782bdfa30038584715546aea3228ea8018e46'},
+}
+DUMMY_ROOT = Root(
+    version=1,
+    spec_version='1.0',
+    expires=datetime.now() + timedelta(days=1),
+    keys=dict(),
+    roles={
+        role_name: Role(keyids=[], threshold=1)
+        for role_name in TOP_LEVEL_ROLE_NAMES
+    },
+    consistent_snapshot=False,
+)
+DUMMY_EXPIRATION_DAYS = dict(root=1000, targets=100, snapshot=10, timestamp=1)
+DUMMY_PRIVATE_KEY_PATHS = dict(
+    (role_name, [pathlib.Path('dummy', role_name)])
+    for role_name in TOP_LEVEL_ROLE_NAMES
+)
+DUMMY_KEY_MAP = dict(
+    root=['root_one', 'root_two'],
+    targets=['targets'],
+    snapshot=['snapshot'],
+    timestamp=['timestamp'],
+)
+DUMMY_THRESHOLDS = dict(root=4, targets=3, snapshot=2, timestamp=1)
+
+
+class ModuleTests(TempDirTestCase):
+    def test_in_(self):
+        self.assertIsInstance(in_(days=1), datetime)
+
+    def test_make_gztar_archive(self):
+        app_name = 'test'
+        version = '1.2.3'
+        # prepare
+        sub_dir = self.temp_dir_path / 'sub'
+        sub_file = sub_dir / 'sub.txt'
+        root_file = self.temp_dir_path / 'root.txt'
+        sub_dir.mkdir()
+        sub_file.touch()
+        root_file.touch()
+        # test
+        mock_input_no = Mock(return_value='n')
+        for exists in [False, True]:
+            with patch('builtins.input', mock_input_no):
+                archive = make_gztar_archive(
+                    src_dir=self.temp_dir_path,
+                    dst_dir=self.temp_dir_path,
+                    app_name=app_name,
+                    version=version,
+                    base_dir='.',  # this kwarg is allowed
+                    root_dir='some path',  # this kwarg is removed
+                )
+            self.assertIsInstance(archive, TargetMeta)
+            self.assertEqual(exists, mock_input_no.called)
+            self.assertTrue(archive.path.exists())
+            self.assertTrue(app_name in str(archive.path))
+            self.assertTrue(version in str(archive.path))
+
+
+class BaseTests(TempDirTestCase):
+    def test_init(self):
+        with patch('builtins.input', mock_input):
+            # dir exists
+            base = Base(dir_path=self.temp_dir_path)
+            self.assertTrue(base.dir_path.exists())
+            # dir does not exist yet
+            base = Base(dir_path=self.temp_dir_path / 'new')
+            self.assertTrue(base.dir_path.exists())
+
+
+class KeysTests(TempDirTestCase):
+    def test_init_no_key_files(self):
+        # no public key files exist yet
+        keys = Keys(dir_path=self.temp_dir_path)
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            self.assertFalse(getattr(keys, role_name))
+
+    def test_init_and_import_all_public_keys(self):
+        # create some key files
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            private_key_filename = Keys.filename_pattern.format(key_name=role_name)
+            file_path = self.temp_dir_path / private_key_filename
+            generate_and_write_unencrypted_ed25519_keypair(filepath=str(file_path))
+        # test
+        keys = Keys(dir_path=self.temp_dir_path)
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            self.assertIsInstance(getattr(keys, role_name)[0], dict)
+
+    def test_init_and_import_all_public_keys_with_key_map(self):
+        # create a single key-pair
+        key_name = 'single'
+        private_key_filename = Keys.filename_pattern.format(key_name=key_name)
+        file_path = self.temp_dir_path / private_key_filename
+        generate_and_write_unencrypted_ed25519_keypair(filepath=str(file_path))
+        key_map = {role_name: [key_name] for role_name in TOP_LEVEL_ROLE_NAMES}
+        # test
+        keys = Keys(dir_path=self.temp_dir_path, key_map=key_map)
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            self.assertIsInstance(getattr(keys, role_name)[0], dict)
+            # all keys should be equal
+            self.assertEqual(keys.root, getattr(keys, role_name))
+
+    def test_import_all_public_keys(self):
+        # note: import_all_public_keys is also (implicitly) tested via __init__
+        keys = Keys(dir_path=self.temp_dir_path)
+        # create some key files
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            private_key_filename = Keys.filename_pattern.format(
+                key_name=role_name)
+            file_path = self.temp_dir_path / private_key_filename
+            generate_and_write_unencrypted_ed25519_keypair(
+                filepath=str(file_path))
+        # test
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            self.assertFalse(getattr(keys, role_name))
+        keys.import_all_public_keys()
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            self.assertIsInstance(getattr(keys, role_name)[0], dict)
+
+    def test_import_public_key(self):
+        # create dummy key with name differing from role name
+        key_name = 'test'
+        role_name = 'targets'
+        private_key_filename = Keys.filename_pattern.format(key_name=key_name)
+        file_path = self.temp_dir_path / private_key_filename
+        generate_and_write_unencrypted_ed25519_keypair(filepath=str(file_path))
+        # test
+        keys = Keys(dir_path=self.temp_dir_path)
+        keys.import_public_key(role_name=role_name, key_name=key_name)
+        self.assertTrue(keys.targets)
+
+    def test_create(self):
+        with patch('getpass.getpass', mock_input):
+            keys = Keys(dir_path=self.temp_dir_path, encrypted=['root'])
+            keys.create()
+            # key pair files should now exist
+            filenames = [item.name for item in keys.dir_path.iterdir()]
+            for role_name in TOP_LEVEL_ROLE_NAMES:
+                private_key_filename = Keys.filename_pattern.format(key_name=role_name)
+                public_key_filename = private_key_filename + SUFFIX_PUB
+                self.assertIn(private_key_filename, filenames)
+                self.assertIn(public_key_filename, filenames)
+            # and the public keys should have been imported
+            self.assertTrue(all(getattr(keys, n) for n in TOP_LEVEL_ROLE_NAMES))
+
+    def test_create_with_key_map(self):
+        # prepare
+        keys = Keys(dir_path=self.temp_dir_path, key_map=DUMMY_KEY_MAP)
+        expected_key_names = [
+            key_name
+            for key_names in DUMMY_KEY_MAP.values()
+            for key_name in key_names
+        ]
+        # test
+        keys.create()
+        # we should now have five key-pairs (one for each, but two for root)
+        filenames = [item.name for item in keys.dir_path.iterdir()]
+        self.assertEqual(2*len(expected_key_names), len(filenames))
+        for key_name in expected_key_names:
+            self.assertIn(key_name, filenames)
+            self.assertIn(key_name + SUFFIX_PUB, filenames)
+        # and the public keys should have been imported
+        for role_name, key_names in DUMMY_KEY_MAP.items():
+            self.assertEqual(len(key_names), len(getattr(keys, role_name)))
+
+    def test_create_key_pair(self):
+        public_key_path = Keys.create_key_pair(
+            private_key_path=self.temp_dir_path / 'key_name', encrypted=False
+        )
+        self.assertTrue(public_key_path.exists())
+
+    def test_create_key_pair_do_not_overwrite(self):
+        # create dummy key pair
+        key_name = 'dummy'
+        private_key_filename = Keys.filename_pattern.format(key_name=key_name)
+        private_key_path = self.temp_dir_path / private_key_filename
+        generate_and_write_unencrypted_ed25519_keypair(
+            filepath=str(private_key_path)
+        )
+        original_private_key = private_key_path.read_bytes()
+        with patch('builtins.input', Mock(return_value='n')):
+            Keys.create_key_pair(
+                private_key_path=private_key_path, encrypted=False
+            )
+        self.assertEqual(original_private_key, private_key_path.read_bytes())
+
+    def test_public(self):
+        keys = Keys(dir_path=self.temp_dir_path)
+        # test empty
+        self.assertFalse(keys.public())
+        # set a dummy key value
+        keys.root = [DUMMY_SSL_KEY]
+        # test
+        self.assertIn(DUMMY_SSL_KEY['keyid'], keys.public().keys())
+
+    def test_roles(self):
+        keys = Keys(dir_path=self.temp_dir_path)
+        # test empty
+        self.assertSetEqual(set(TOP_LEVEL_ROLE_NAMES), set(keys.roles().keys()))
+        # set a dummy key value
+        keys.root = [DUMMY_SSL_KEY]
+        # test
+        self.assertIn('root', keys.roles().keys())
+
+    def test_roles_thresholds(self):
+        # prepare
+        keys = Keys(dir_path=self.temp_dir_path, thresholds=DUMMY_THRESHOLDS)
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            setattr(keys, role_name, [DUMMY_SSL_KEY])
+        # test
+        roles = keys.roles()
+        for key, value in roles.items():
+            self.assertEqual(DUMMY_THRESHOLDS[key], value.threshold)
+
+    def test_find_private_key(self):
+        # create dummy private key files in separate folders
+        key_names = [
+            ('online', [Snapshot.type, Timestamp.type]),
+            ('offline', [Root.type, Targets.type]),
+        ]
+        key_dirs = []
+        for dir_name, role_names  in key_names:
+            dir_path = self.temp_dir_path / dir_name
+            dir_path.mkdir()
+            key_dirs.append(dir_path)
+            for role_name in role_names:
+                filename = Keys.filename_pattern.format(key_name=role_name)
+                (dir_path / filename).touch()
+        # test
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            key_path = Keys.find_private_key(key_name=role_name, key_dirs=key_dirs)
+            self.assertIn(role_name, str(key_path))
+            self.assertTrue(key_path.exists())
+
+
+class RolesTests(TempDirTestCase):
+    def test_init(self):
+        self.assertTrue(Roles(dir_path=self.temp_dir_path))
+
+    def test_init_import_roles(self):
+        def mock_from_file(filename, *args, **kwargs):
+            file_path = pathlib.Path(filename)
+            assert file_path.exists()
+            return file_path.stem
+
+        # create dummy metadata files
+        for role_name in TOP_LEVEL_ROLE_NAMES:
+            filenames = [f'{role_name}.json']
+            if role_name == 'root':
+                filenames.extend(f'{v}.{role_name}.json' for v in [1, 2, 3])
+            for filename in filenames:
+                (self.temp_dir_path / filename).touch()
+        # test
+        with patch.object(tufup.repo.Metadata, 'from_file', mock_from_file):
+            roles = Roles(dir_path=self.temp_dir_path)
+            for role_name in TOP_LEVEL_ROLE_NAMES:
+                self.assertEqual(role_name, getattr(roles, role_name))
+
+    def test_initialize_empty(self):
+        # prepare
+        mock_keys = Mock()
+        mock_keys.public = Mock()
+        mock_keys.roles = Mock(
+            return_value={name: None for name in TOP_LEVEL_ROLE_NAMES}
+        )
+        roles = Roles(dir_path=self.temp_dir_path)
+        # test
+        roles.initialize(keys=mock_keys)
+        self.assertTrue(
+            all(
+                isinstance(getattr(roles, n), Metadata)
+                for n in TOP_LEVEL_ROLE_NAMES
+            )
+        )
+        # files do not exist yet, because the roles still need to be populated
+        self.assertFalse(any(roles.dir_path.iterdir()))
+
+    def test_initialize_existing_root(self):
+        # prepare
+        mock_keys = Mock()
+        mock_keys.public = Mock()
+        mock_keys.roles = Mock(return_value={n: None for n in TOP_LEVEL_ROLE_NAMES})
+        roles = Roles(dir_path=self.temp_dir_path)
+        # set existing root role
+        mock_root_role = Mock()
+        roles.root = mock_root_role
+        # test
+        roles.initialize(keys=mock_keys)
+        # ensure the existing role has not been replaced
+        self.assertEqual(mock_root_role, roles.root)
+
+    def test_add_or_update_target(self):
+        # prepare
+        roles = Roles(dir_path=self.temp_dir_path)
+        roles.targets = Mock(signed=Mock(targets=dict()))
+        # test
+        filename = 'my_app.tar.gz'
+        local_target_path = self.temp_dir_path / filename
+        # path must exist
+        with self.assertRaises(FileNotFoundError):
+            roles.add_or_update_target(local_path=local_target_path)
+        local_target_path.write_bytes(b'some bytes')
+        # test
+        for segments, expected_url_path in [
+            (None, filename), ([], filename), (['a', 'b'], 'a/b/' + filename)
+        ]:
+            roles.add_or_update_target(
+                local_path=local_target_path, url_path_segments=segments
+            )
+            with self.subTest(msg=segments):
+                self.assertIsInstance(
+                    roles.targets.signed.targets[expected_url_path], TargetFile
+                )
+
+    def test_remove_target(self):
+        # prepare
+        filename = 'my_app-1.0.tar.gz'
+        dirname = 'subdir'
+        url_path = f'{dirname}/{filename}'
+        subdir = self.temp_dir_path / dirname
+        subdir.mkdir()
+        local_target_path = subdir / filename
+        local_target_path.touch()
+        roles = Roles(dir_path=self.temp_dir_path)
+        roles.targets = Mock(signed=Mock(targets={url_path: Mock()}))
+        original_targets_signed = copy.deepcopy(roles.targets.signed)
+        # test
+        self.assertTrue(local_target_path.exists())
+        roles.remove_target(local_path=local_target_path)
+        self.assertNotIn(filename, roles.targets.signed.targets)
+        self.assertFalse(local_target_path.exists())
+        self.assertNotEqual(original_targets_signed, roles.targets.signed)
+        # cannot remove non-existent target
+        self.assertFalse(roles.remove_target(local_path=local_target_path))
+
+    def test_add_public_key(self):
+        # prepare
+        roles = Roles(dir_path=self.temp_dir_path)
+        roles.root = Mock(signed=Mock(roles=dict(), add_key=Mock()))
+        public_key_path = self.temp_dir_path / 'targets_key.pub'
+        public_key_path.write_text(json.dumps(DUMMY_SSL_KEY))
+        # test
+        role_name = 'targets'
+        roles.add_public_key(role_name=role_name, public_key_path=public_key_path)
+        self.assertTrue(roles.root.signed.add_key.called)
+
+    def test_set_signature_threshold(self):
+        # prepare
+        role_name = 'targets'
+        threshold = 2
+        roles = Roles(dir_path=self.temp_dir_path)
+        roles.root = Mock(signed=Mock(roles={role_name: Mock(threshold=1)}))
+        # test
+        roles.set_signature_threshold(role_name=role_name, threshold=threshold)
+        self.assertEqual(threshold, roles.root.signed.roles[role_name].threshold)
+
+    def test_sign_role(self):
+        # prepare
+        roles = Roles(dir_path=self.temp_dir_path)
+        roles.root = Metadata(signed=DUMMY_ROOT, signatures=dict())
+        role_name = 'root'
+        signature_count = 2
+        password = 'mock-password'
+        with patch('getpass.getpass', Mock(return_value=password)):
+            for index in range(signature_count):
+                private_key_path = self.temp_dir_path / f'{index}.{role_name}'
+                # create key pair
+                if index == 0:
+                    generate_and_write_unencrypted_ed25519_keypair(
+                        filepath=str(private_key_path)
+                    )
+                else:
+                    generate_and_write_ed25519_keypair(
+                        password=password, filepath=str(private_key_path)
+                    )
+                # test
+                roles.sign_role(
+                    role_name=role_name, private_key_path=private_key_path
+                )
+        self.assertEqual(signature_count, len(roles.root.signatures))
+
+    def test_file_path(self):
+        # prepare
+        roles = Roles(dir_path=self.temp_dir_path)
+        # test
+        self.assertEqual(
+            self.temp_dir_path / '1.root.json',
+            roles.file_path(role_name='root', version=1),
+        )
+        self.assertEqual(
+            self.temp_dir_path / 'root.json',
+            roles.file_path(role_name='root'),
+        )
+        self.assertEqual(
+            self.temp_dir_path / 'targets.json',
+            roles.file_path(role_name='targets', version=1),
+        )
+
+    def test_file_exists(self):
+        # prepare
+        roles = Roles(dir_path=self.temp_dir_path)
+        (self.temp_dir_path / '1.root.json').touch()
+        # test
+        self.assertTrue(roles.file_exists(role_name='root'))
+        self.assertFalse(roles.file_exists(role_name='targets'))
+
+    def test_persist_role(self):
+        # prepare
+        roles = Roles(dir_path=self.temp_dir_path)
+        roles.root = Metadata(signed=DUMMY_ROOT, signatures=dict())
+        expected_filenames = [f'{DUMMY_ROOT.version}.root.json', 'root.json']
+        # test
+        roles.persist_role(role_name='root')
+        for filename in expected_filenames:
+            with self.subTest(msg=filename):
+                self.assertTrue((self.temp_dir_path / filename).exists())
+
+    def test_get_latest_archive(self):
+        roles = Roles(dir_path=TEST_REPO_DIR / 'metadata')
+        expected_filename = 'example_app-4.0a0.tar.gz'
+        latest_archive = roles.get_latest_archive()
+        self.assertEqual(expected_filename, latest_archive.path.name)
+
+    def test_get_latest_archive_empty(self):
+        roles = Roles(dir_path=self.temp_dir_path)
+        self.assertIsNone(roles.get_latest_archive())
+
+
+class RepositoryTests(TempDirTestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        logging.basicConfig(level=logging.DEBUG)
+
+    def test_defaults(self):
+        self.assertTrue(Repository(app_name='test'))
+
+    def test_config_dict(self):
+        app_name = 'test'
+        repo = Repository(app_name=app_name)
+        expected_config_dict = {
+            'app_name': app_name,
+            'app_version_attr': None,
+            'encrypted_keys': None,
+            'expiration_days': None,
+            'key_map': None,
+            'keys_dir': None,
+            'repo_dir': None,
+            'thresholds': None,
+        }
+        self.assertEqual(set(expected_config_dict), set(repo.config_dict))
+
+    def test_app_version(self):
+        # for convenience we use the notosotuf version attribute here,
+        # but normally this would point to an external app version e.g.
+        # 'my_app.__version__'
+        app_version_attr = 'tufup.__version__'
+        repo = Repository(app_name='test', app_version_attr=app_version_attr)
+        self.assertEqual(str(tufup.__version__), repo.app_version)
+
+    def test_get_config_file_path(self):
+        self.assertTrue(Repository.get_config_file_path())
+
+    def test_save_config(self):
+        # prepare
+        repo = Repository(app_name='test')
+        # test
+        repo.save_config()
+        self.assertTrue(repo.get_config_file_path().exists())
+        print(repo.get_config_file_path().read_text())
+
+    def test_load_config(self):
+        # file does not exist
+        self.assertEqual(dict(), Repository.load_config())
+        # file exists but invalid
+        Repository.get_config_file_path().touch()
+        # test
+        self.assertEqual(dict(), Repository.load_config())
+
+    def test_from_config(self):
+        temp_dir = self.temp_dir_path.resolve()
+        # prepare
+        config_data = dict(
+            app_name='test',
+            app_version_attr='my_app.__version__',
+            repo_dir=temp_dir / 'repo',
+            keys_dir=temp_dir / 'keystore',
+            key_map=dict(),
+            encrypted_keys=[],
+            expiration_days=dict(),
+            thresholds=dict(),
+        )
+        Repository.get_config_file_path().write_text(
+            json.dumps(config_data, default=str)
+        )
+        mock_load_keys_and_roles = Mock()
+        # test
+        with patch.object(
+                Repository, '_load_keys_and_roles', mock_load_keys_and_roles,
+        ):
+            repo = Repository.from_config()
+        self.assertEqual(
+            config_data,
+            {item: getattr(repo, item) for item in config_data.keys()},
+        )
+        self.assertTrue(mock_load_keys_and_roles.called)
+
+    def test_initialize(self):
+        # prepare
+        repo = Repository(
+            app_name='test',
+            keys_dir=self.temp_dir_path / 'keystore',
+            repo_dir=self.temp_dir_path / 'repo',
+            expiration_days=DUMMY_EXPIRATION_DAYS,
+        )
+        # test
+        repo.initialize()
+        self.assertTrue(any(repo.keys_dir.iterdir()))
+        self.assertTrue(any(repo.metadata_dir.iterdir()))
+        self.assertTrue(
+            all(getattr(repo.roles, name) for name in TOP_LEVEL_ROLE_NAMES)
+        )
+        self.assertEqual(
+            date.today() + timedelta(days=DUMMY_EXPIRATION_DAYS['root']),
+            repo.roles.root.signed.expires.date(),
+        )
+
+    def test_refresh_expiration_date(self):
+        repo = Repository(
+            app_name='test',
+            keys_dir=self.temp_dir_path / 'keystore',
+            repo_dir=self.temp_dir_path / 'repo',
+        )
+        repo.initialize()  # todo: make test independent...
+        days = 999
+        repo.refresh_expiration_date(role_name='root', days=days)
+        self.assertEqual(
+            date.today() + timedelta(days=days),
+            repo.roles.root.signed.expires.date(),
+        )
+
+    def test_replace_key(self):
+        role_name = 'root'
+        # prepare
+        new_key_name = 'new_key'
+        old_key_name = 'old-key'
+        key_map = {name: [name] for name in TOP_LEVEL_ROLE_NAMES}
+        key_map['root'].append(old_key_name)
+        key_map['targets'] = [old_key_name]
+        repo = Repository(
+            app_name='test',
+            keys_dir=self.temp_dir_path / 'keystore',
+            repo_dir=self.temp_dir_path / 'repo',
+            key_map=key_map,
+        )
+        repo.initialize()  # todo: make test independent...
+        old_key_id = repo.roles.root.signed.roles['targets'].keyids[0]
+        # create new key pair to replace old one
+        new_private_key_path = repo.keys_dir / new_key_name
+        new_public_key_path = Keys.create_key_pair(
+            private_key_path=new_private_key_path, encrypted=False
+        )
+        new_key_id = import_ed25519_publickey_from_file(
+            filepath=str(new_public_key_path)
+        )['keyid']
+        # test
+        expected_key_count = len(key_map[role_name])
+        repo.replace_key(
+            old_key_name=old_key_name,
+            new_public_key_path=new_public_key_path,
+            new_private_key_encrypted=True,  # pretend the key is encrypted
+        )
+        self.assertEqual(
+            expected_key_count,
+            len(repo.roles.root.signed.roles[role_name].keyids),
+        )
+        # old key removed?
+        self.assertNotIn(
+            old_key_id, repo.roles.root.signed.roles[role_name].keyids
+        )
+        self.assertNotIn(old_key_name, repo.key_map[role_name])
+        self.assertIn(old_key_name, repo.revoked_key_names)
+        # new key added?
+        self.assertIn(
+            new_key_id, repo.roles.root.signed.roles[role_name].keyids
+        )
+        self.assertIn(new_key_name, repo.key_map[role_name])
+        self.assertIn(new_key_name, repo.encrypted_keys)
+        # no duplicates in encrypted_keys?
+        self.assertEqual(1, len(repo.encrypted_keys))
+        # other keys still in key map?
+        self.assertEqual(expected_key_count, len(repo.key_map[role_name]))
+        # keys replaced for all roles?
+        self.assertIn(new_key_name, repo.key_map['targets'])
+
+    def test_add_key(self):
+        repo = Repository(
+            app_name='test',
+            keys_dir=self.temp_dir_path / 'keystore',
+            repo_dir=self.temp_dir_path / 'repo',
+        )
+        repo.initialize()  # todo: make test independent...
+        # create new key pair to add
+        new_key_name = 'new-key'
+        new_private_key_path = repo.keys_dir / new_key_name
+        new_public_key_path = Keys.create_key_pair(
+            private_key_path=new_private_key_path, encrypted=False
+        )
+        new_key_id = import_ed25519_publickey_from_file(
+            filepath=str(new_public_key_path)
+        )['keyid']
+        # test
+        role_name = 'root'
+        repo.add_key(
+            role_name=role_name,
+            public_key_path=new_public_key_path,
+            encrypted=True,  # pretend the key is encrypted
+        )
+        # new key added?
+        self.assertEqual(2, len(repo.roles.root.signed.roles[role_name].keyids))
+        self.assertIn(
+            new_key_id, repo.roles.root.signed.roles[role_name].keyids
+        )
+        self.assertIn(new_key_name, repo.key_map[role_name])
+        self.assertIn(new_key_name, repo.encrypted_keys)
+
+    def test_add_bundle(self):
+        # prepare
+        bundle_dir = self.temp_dir_path / 'dist' / 'test_app'
+        bundle_dir.mkdir(parents=True)
+        bundle_file = bundle_dir / 'dummy.exe'
+        bundle_file.touch()
+        repo = Repository(
+            app_name='test',
+            keys_dir=self.temp_dir_path / 'keystore',
+            repo_dir=self.temp_dir_path / 'repo',
+        )
+        repo.initialize()  # todo: make test independent...
+        # test
+        repo.add_bundle(new_version='1.0', new_bundle_dir=bundle_dir)
+        self.assertTrue((repo.metadata_dir / 'targets.json').exists())
+
+    def test_add_bundle_no_patch(self):
+        # prepare
+        bundle_dir = self.temp_dir_path / 'dist' / 'test_app'
+        bundle_dir.mkdir(parents=True)
+        bundle_file = bundle_dir / 'dummy.exe'
+        bundle_file.write_text('this is version 1')
+        repo = Repository(
+            app_name='test',
+            keys_dir=self.temp_dir_path / 'keystore',
+            repo_dir=self.temp_dir_path / 'repo',
+        )
+        repo.initialize()  # todo: make test independent...
+        repo.add_bundle(new_version='1.0', new_bundle_dir=bundle_dir)
+        # test
+        bundle_file.write_text('much has changed in version 2')
+        repo.add_bundle(
+            new_version='2.0', new_bundle_dir=bundle_dir, skip_patch=True
+        )
+        self.assertTrue((repo.metadata_dir / 'targets.json').exists())
+        target_keys = list(repo.roles.targets.signed.targets.keys())
+        self.assertEqual(2, len(target_keys))
+        self.assertFalse(any(key.endswith(SUFFIX_PATCH) for key in target_keys))
+
+    def test_remove_latest_bundle(self):
+        # prepare
+        bundle_dir = self.temp_dir_path / 'dist' / 'test_app'
+        bundle_dir.mkdir(parents=True)
+        bundle_file = bundle_dir / 'dummy.exe'
+        bundle_file.touch()
+        repo = Repository(
+            app_name='test',
+            keys_dir=self.temp_dir_path / 'keystore',
+            repo_dir=self.temp_dir_path / 'repo',
+        )
+        repo.initialize()  # todo: make test independent...
+        v1 = '1.0'
+        v2 = '2.0'
+        repo.add_bundle(new_version=v1, new_bundle_dir=bundle_dir)
+        repo.add_bundle(new_version=v2, new_bundle_dir=bundle_dir)
+        # test
+        repo.remove_latest_bundle()
+        remaining_target_keys = list(repo.roles.targets.signed.targets.keys())
+        self.assertEqual(1, len(remaining_target_keys))
+        self.assertIn(v1, remaining_target_keys[0])
+        remaining_target_filenames = [p.name for p in repo.targets_dir.iterdir()]
+        self.assertEqual(1, len(remaining_target_filenames))
+        self.assertIn(remaining_target_keys[0], remaining_target_filenames)
+
+    def test_threshold_sign(self):
+        # prepare
+        role_name = 'root'
+        keys_dir = self.temp_dir_path / 'keystore'
+        repo = Repository(
+            app_name='test',
+            keys_dir=keys_dir,
+            repo_dir=self.temp_dir_path / 'repo',
+        )
+        repo.initialize()  # todo: make test independent...
+        # create dummy "revoked key" and pretend it is encrypted
+        revoked_key_name = 'revoked'
+        repo.keys.create_key_pair(
+            private_key_path=keys_dir / revoked_key_name, encrypted=False
+        )
+        repo.revoked_key_names.append(revoked_key_name)
+        repo.encrypted_keys.append(revoked_key_name)
+        # dummy modification
+        repo.roles.root.signed.spec_version = 'x'
+        versioned_file_path = repo.metadata_dir / f'1.{role_name}.json'
+        non_versioned_file_path = repo.metadata_dir / f'{role_name}.json'
+        versioned_last_modified = versioned_file_path.stat().st_mtime_ns
+        non_versioned_last_modified = non_versioned_file_path.stat().st_mtime_ns
+        # test
+        sleep(0.1)  # enforce different modification time
+        count = repo.threshold_sign(
+            role_name=role_name, private_key_dirs=[repo.keys_dir]
+        )
+        self.assertEqual(2, count)  # existing key and revoked key
+        self.assertFalse(repo.revoked_key_names)
+        self.assertFalse(repo.encrypted_keys)
+        # files should have been modified
+        self.assertGreater(
+            versioned_file_path.stat().st_mtime_ns, versioned_last_modified
+        )
+        self.assertGreater(
+            non_versioned_file_path.stat().st_mtime_ns, non_versioned_last_modified
+        )
+        # if no signatures found
+        for path in repo.keys_dir.iterdir():
+            path.unlink()
+        with self.assertRaises(Exception):
+            repo.threshold_sign(
+                role_name=role_name, private_key_dirs=[repo.keys_dir]
+            )
+
+    def test__load_keys_and_roles(self):
+        # prepare
+        keys_dir = self.temp_dir_path / 'keystore'
+        repo = Repository(
+            app_name='test',
+            keys_dir=keys_dir,
+            repo_dir=self.temp_dir_path / 'repo',
+        )
+        # test
+        with patch('builtins.input', Mock(return_value='y')):
+            repo._load_keys_and_roles(create_keys=True)
+        self.assertTrue(
+            all(getattr(repo.roles, name) for name in TOP_LEVEL_ROLE_NAMES)
+        )
+        self.assertTrue(
+            all((keys_dir / name).exists() for name in TOP_LEVEL_ROLE_NAMES)
+        )
+
+    def test_publish_changes_no_change(self):
+        # prepare
+        repo = Repository(
+            app_name='test',
+            keys_dir=self.temp_dir_path / 'keystore',
+            repo_dir=self.temp_dir_path / 'repo',
+        )
+        # note that initialize() already calls publish_changes...
+        repo.initialize()  # todo: make test independent...
+        # test
+        repo.publish_changes(private_key_dirs=[repo.keys_dir])
+        for role_name in ['root', 'targets', 'snapshot', 'timestamp']:
+            role = getattr(repo.roles, role_name)
+            with self.subTest(msg=role_name):
+                self.assertEqual(1, role.signed.version)
+                self.assertTrue(role.signatures)
+
+    def test_publish_changes_threshold(self):
+        # prepare
+        repo = Repository(
+            app_name='test',
+            keys_dir=self.temp_dir_path / 'keystore',
+            repo_dir=self.temp_dir_path / 'repo',
+        )
+        # note that initialize() already calls publish_changes...
+        repo.initialize()  # todo: make test independent...
+        # remove the root signature
+        repo.roles.root.signatures = {}
+        # test
+        repo.publish_changes(private_key_dirs=[repo.keys_dir])
+        for role_name in ['root', 'targets', 'snapshot', 'timestamp']:
+            with self.subTest(msg=role_name):
+                role = getattr(repo.roles, role_name)
+                self.assertEqual(
+                    repo.thresholds[role_name], len(role.signatures)
+                )
+
+    def test_publish_changes(self):
+        days = 999
+        role_names = ['root', 'targets', 'snapshot', 'timestamp']
+        for test_role_name in role_names.copy():
+            # use a fresh temporary dir and repo
+            with TemporaryDirectory() as temp_dir:
+                temp_dir_path = pathlib.Path(temp_dir)
+                repo = Repository(
+                    app_name='test',
+                    keys_dir=temp_dir_path / 'keystore',
+                    repo_dir=temp_dir_path / 'repo',
+                )
+                # note that initialize() already calls publish_changes...
+                repo.initialize()  # todo: make test independent...
+                # make a change to metadata (in memory)
+                repo.roles.set_expiration_date(
+                    role_name=test_role_name, days=days
+                )
+                # make a change to config
+                config_change = 'dummy'
+                repo.encrypted_keys.append(config_change)
+                # test
+                repo.publish_changes(private_key_dirs=[repo.keys_dir])
+                for role_name in role_names:
+                    role = getattr(repo.roles, role_name)
+                    with self.subTest(msg=f'{test_role_name}: {role_name}'):
+                        self.assertEqual(2, role.signed.version)
+                        self.assertTrue(role.signatures)
+                role_names.remove(test_role_name)
+                #  re-load from file to verify change
+                root = Metadata.from_file(
+                    repo.roles.file_path(role_name=test_role_name)
+                )
+                self.assertEqual(
+                    date.today() + timedelta(days=days),
+                    root.signed.expires.date(),
+                )
+                # verify change in config
+                config_from_disk = repo.load_config()
+                self.assertIn(
+                    config_change, config_from_disk['encrypted_keys']
+                )
```

### Comparing `tufup-0.4.9/tests/test_repo_cli.py` & `tufup-0.5.0/tests/test_repo_cli.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,226 +1,226 @@
-import argparse
-import unittest
-from unittest.mock import Mock, patch
-
-import tufup
-import tufup.repo.cli
-import tufup.utils
-from tests import TempDirTestCase
-
-
-class ParserTests(unittest.TestCase):
-    def test_get_parser(self):
-        parser = tufup.repo.cli.get_parser()
-        for cmd in [
-            'init',
-            'init --debug',
-            'targets add 1.0 c:\\my_bundle_dir c:\\private_keys',
-            'targets -d add 1.0 c:\\my_bundle_dir c:\\private_keys',
-            'targets -d add -s 1.0 c:\\my_bundle_dir c:\\private_keys',
-            'targets remove-latest c:\\private_keys',
-            'keys my-key-name -c -e',
-            'keys my-key-name add root c:\\private_keys d:\\more_private_keys',
-            'keys my-key-name -c -e add root c:\\private_keys',
-            'keys my-key-name replace old-key-name c:\\private_keys',
-            'keys my-key-name -c -e replace old-key-name c:\\private_keys',
-            'sign root c:\\private_keys d:\\other_private_keys',
-            'sign root c:\\private_keys -e',
-            'sign root c:\\private_keys -e 100',
-        ]:
-            with self.subTest(msg=cmd):
-                args = cmd.split()
-                options = parser.parse_args(args)
-                expected_func_name = '_cmd_' + args[0]
-                self.assertEqual(expected_func_name, options.func.__name__)
-
-
-class CommandTests(TempDirTestCase):
-    def setUp(self) -> None:
-        super().setUp()
-        role_names = ['root', 'targets', 'snapshot', 'timestamp']
-        self.config = dict(
-            app_name='my-app',
-            repo_dir=self.temp_dir_path / 'repo',
-            keys_dir=self.temp_dir_path / 'keys',
-            key_map={name: [name] for name in role_names},
-            encrypted_keys=[],
-            expiration_days={name: 1 for name in role_names},
-        )
-        mock_return_config = Mock(return_value=self.config)
-        mock_keys = Mock()
-        mock_keys.create_key_pair = Mock()
-        mock_repo = Mock(keys=mock_keys, **self.config)
-        mock_repo.save_config = Mock()
-        mock_repo.initialize = Mock()
-        mock_repo.add_bundle = Mock()
-        mock_repo.remove_latest_bundle = Mock()
-        mock_repo.add_key = Mock()
-        mock_repo.replace_key = Mock()
-        mock_repo.refresh_expiration_date = Mock()
-        mock_repo.threshold_sign = Mock()
-        mock_repo.publish_changes = Mock()
-        MockRepository = Mock(return_value=mock_repo)  # noqa
-        MockRepository.load_config = mock_return_config
-        MockRepository.from_config = Mock(return_value=mock_repo)
-        self.mock_repo = mock_repo
-        self.mock_repo_class = MockRepository
-
-    def test__cmd_init(self):
-        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
-            with patch('tufup.repo.cli.input_bool', Mock(return_value=True)):
-                with patch(
-                        'tufup.repo.cli._get_config_from_user',
-                        self.mock_repo_class.load_config,
-                ):
-                    tufup.repo.cli._cmd_init(options=argparse.Namespace())
-        self.mock_repo.initialize.assert_called()
-
-    def test__cmd_keys_create(self):
-        options = argparse.Namespace(
-            new_key_name='test', encrypted=True, create=True
-        )
-        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
-            tufup.repo.cli._cmd_keys(options=options)
-        self.mock_repo.keys.create_key_pair.assert_called()
-
-    def test__cmd_keys_create_and_add_key(self):
-        options = argparse.Namespace(
-            create=True,
-            encrypted=True,
-            key_dirs=['c:\\my_private_keys'],
-            new_key_name='test',
-            role_name='root',
-        )
-        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
-            tufup.repo.cli._cmd_keys(options=options)
-        self.mock_repo.keys.create_key_pair.assert_called()
-        self.mock_repo.add_key.assert_called()
-        self.mock_repo.publish_changes.assert_called()
-
-    def test__cmd_keys_replace_key(self):
-        options = argparse.Namespace(
-            create=True,
-            encrypted=False,
-            key_dirs=['c:\\my_private_keys'],
-            new_key_name='some new key to be created',
-            old_key_name='some old key name',
-        )
-        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
-            tufup.repo.cli._cmd_keys(options=options)
-        self.mock_repo.replace_key.assert_called()
-        self.mock_repo.keys.create_key_pair.assert_called()
-        self.mock_repo.publish_changes.assert_called()
-
-    def test__cmd_targets_add(self):
-        version = '1.0'
-        bundle_dir = 'dummy'
-        key_dirs = ['c:\\my_private_keys']
-        skip_patch = True
-        options = argparse.Namespace(
-            app_version=version,
-            bundle_dir=bundle_dir,
-            key_dirs=key_dirs,
-            skip_patch=skip_patch,
-        )
-        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
-            tufup.repo.cli._cmd_targets(options=options)
-        self.mock_repo.add_bundle.assert_called_with(
-            new_version=version, new_bundle_dir=bundle_dir, skip_patch=skip_patch,
-        )
-        self.mock_repo.publish_changes.assert_called_with(
-            private_key_dirs=key_dirs
-        )
-
-    def test__cmd_targets_remove_latest(self):
-        key_dirs = ['c:\\my_private_keys']
-        options = argparse.Namespace(key_dirs=key_dirs)
-        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
-            tufup.repo.cli._cmd_targets(options=options)
-        self.mock_repo.remove_latest_bundle.assert_called()
-
-    def test__cmd_sign_threshold(self):
-        role_name = 'root'
-        key_dirs = ['c:\\my_private_keys']
-        options = argparse.Namespace(
-            role_name=role_name, key_dirs=key_dirs, expiration_days=None
-        )
-        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
-            tufup.repo.cli._cmd_sign(options=options)
-        self.mock_repo.threshold_sign.assert_called_with(
-            role_name=role_name, private_key_dirs=key_dirs
-        )
-
-    def test__cmd_sign_expired(self):
-        role_name = 'root'
-        key_dirs = ['c:\\my_private_keys']
-        options = argparse.Namespace(
-            role_name=role_name,
-            key_dirs=key_dirs,
-            expiration_days='default',  # i.e. specify -e without a value
-        )
-        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
-            tufup.repo.cli._cmd_sign(options=options)
-        self.mock_repo.refresh_expiration_date.assert_called_with(
-            role_name=role_name, days=self.config['expiration_days'][role_name]
-        )
-        self.mock_repo.publish_changes.assert_called_with(
-            private_key_dirs=key_dirs
-        )
-
-    def test__get_config_from_user_no_kwargs(self):
-        default = ''
-        yes = 'y'
-        no = 'n'
-        user_inputs = iter(
-            [
-                'my-app',  # app name
-                'my_app.__version__',  # app version
-                'repo/dir',  # repo dir
-                'keys/dir',  # keys dir
-                yes,  # keep default root key name
-                yes,  # add another root key name
-                'root-2',  # key name
-                no,  # add another root key name
-                default,  # encrypt 'root' key
-                yes,  # encrypt 'root-2' key
-                '365',  # expiration days
-                '2',  # signature threshold
-                default,  # keep default targets key name
-                default,  # add another targets key name
-                default,  # encrypt 'targets' key
-                '30',  # expiration days
-                '1',  # signature threshold
-                default,  # keep default snapshot key name
-                default,  # add another snapshot key name
-                default,  # encrypt 'snapshot' key
-                '7',  # expiration days
-                '1',  # signature threshold
-                default,  # keep default timestamp key name
-                default,  # add another timestamp key name
-                default,  # encrypt 'timestamp' key
-                '1',  # expiration days
-                '1',  # signature threshold
-            ]
-        )
-        with patch('builtins.input', lambda *_, **__: next(user_inputs)):
-            config_kwargs = tufup.repo.cli._get_config_from_user()
-        self.assertTrue(config_kwargs)
-
-    def test__get_config_from_user_with_kwargs(self):
-        role_names = ['root', 'targets', 'snapshot', 'timestamp']
-        original_kwargs = dict(
-            app_name='my-app',
-            app_version_attr='my_app.__version__',
-            repo_dir='repo/dir',
-            keys_dir='keys/dir',
-            key_map={name: [name] for name in role_names},
-            encrypted_keys=['root'],
-            expiration_days={name: 1 for name in role_names},
-            thresholds={name: 1 for name in role_names},
-        )
-        default = ''
-        with patch('builtins.input', Mock(return_value=default)):
-            config_kwargs = tufup.repo.cli._get_config_from_user(
-                **original_kwargs
-            )
-        self.assertEqual(config_kwargs, original_kwargs)
+import argparse
+import unittest
+from unittest.mock import Mock, patch
+
+import tufup
+import tufup.repo.cli
+import tufup.utils
+from tests import TempDirTestCase
+
+
+class ParserTests(unittest.TestCase):
+    def test_get_parser(self):
+        parser = tufup.repo.cli.get_parser()
+        for cmd in [
+            'init',
+            'init --debug',
+            'targets add 1.0 c:\\my_bundle_dir c:\\private_keys',
+            'targets -d add 1.0 c:\\my_bundle_dir c:\\private_keys',
+            'targets -d add -s 1.0 c:\\my_bundle_dir c:\\private_keys',
+            'targets remove-latest c:\\private_keys',
+            'keys my-key-name -c -e',
+            'keys my-key-name add root c:\\private_keys d:\\more_private_keys',
+            'keys my-key-name -c -e add root c:\\private_keys',
+            'keys my-key-name replace old-key-name c:\\private_keys',
+            'keys my-key-name -c -e replace old-key-name c:\\private_keys',
+            'sign root c:\\private_keys d:\\other_private_keys',
+            'sign root c:\\private_keys -e',
+            'sign root c:\\private_keys -e 100',
+        ]:
+            with self.subTest(msg=cmd):
+                args = cmd.split()
+                options = parser.parse_args(args)
+                expected_func_name = '_cmd_' + args[0]
+                self.assertEqual(expected_func_name, options.func.__name__)
+
+
+class CommandTests(TempDirTestCase):
+    def setUp(self) -> None:
+        super().setUp()
+        role_names = ['root', 'targets', 'snapshot', 'timestamp']
+        self.config = dict(
+            app_name='my-app',
+            repo_dir=self.temp_dir_path / 'repo',
+            keys_dir=self.temp_dir_path / 'keys',
+            key_map={name: [name] for name in role_names},
+            encrypted_keys=[],
+            expiration_days={name: 1 for name in role_names},
+        )
+        mock_return_config = Mock(return_value=self.config)
+        mock_keys = Mock()
+        mock_keys.create_key_pair = Mock()
+        mock_repo = Mock(keys=mock_keys, **self.config)
+        mock_repo.save_config = Mock()
+        mock_repo.initialize = Mock()
+        mock_repo.add_bundle = Mock()
+        mock_repo.remove_latest_bundle = Mock()
+        mock_repo.add_key = Mock()
+        mock_repo.replace_key = Mock()
+        mock_repo.refresh_expiration_date = Mock()
+        mock_repo.threshold_sign = Mock()
+        mock_repo.publish_changes = Mock()
+        MockRepository = Mock(return_value=mock_repo)  # noqa
+        MockRepository.load_config = mock_return_config
+        MockRepository.from_config = Mock(return_value=mock_repo)
+        self.mock_repo = mock_repo
+        self.mock_repo_class = MockRepository
+
+    def test__cmd_init(self):
+        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
+            with patch('tufup.repo.cli.input_bool', Mock(return_value=True)):
+                with patch(
+                        'tufup.repo.cli._get_config_from_user',
+                        self.mock_repo_class.load_config,
+                ):
+                    tufup.repo.cli._cmd_init(options=argparse.Namespace())
+        self.mock_repo.initialize.assert_called()
+
+    def test__cmd_keys_create(self):
+        options = argparse.Namespace(
+            new_key_name='test', encrypted=True, create=True
+        )
+        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
+            tufup.repo.cli._cmd_keys(options=options)
+        self.mock_repo.keys.create_key_pair.assert_called()
+
+    def test__cmd_keys_create_and_add_key(self):
+        options = argparse.Namespace(
+            create=True,
+            encrypted=True,
+            key_dirs=['c:\\my_private_keys'],
+            new_key_name='test',
+            role_name='root',
+        )
+        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
+            tufup.repo.cli._cmd_keys(options=options)
+        self.mock_repo.keys.create_key_pair.assert_called()
+        self.mock_repo.add_key.assert_called()
+        self.mock_repo.publish_changes.assert_called()
+
+    def test__cmd_keys_replace_key(self):
+        options = argparse.Namespace(
+            create=True,
+            encrypted=False,
+            key_dirs=['c:\\my_private_keys'],
+            new_key_name='some new key to be created',
+            old_key_name='some old key name',
+        )
+        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
+            tufup.repo.cli._cmd_keys(options=options)
+        self.mock_repo.replace_key.assert_called()
+        self.mock_repo.keys.create_key_pair.assert_called()
+        self.mock_repo.publish_changes.assert_called()
+
+    def test__cmd_targets_add(self):
+        version = '1.0'
+        bundle_dir = 'dummy'
+        key_dirs = ['c:\\my_private_keys']
+        skip_patch = True
+        options = argparse.Namespace(
+            app_version=version,
+            bundle_dir=bundle_dir,
+            key_dirs=key_dirs,
+            skip_patch=skip_patch,
+        )
+        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
+            tufup.repo.cli._cmd_targets(options=options)
+        self.mock_repo.add_bundle.assert_called_with(
+            new_version=version, new_bundle_dir=bundle_dir, skip_patch=skip_patch,
+        )
+        self.mock_repo.publish_changes.assert_called_with(
+            private_key_dirs=key_dirs
+        )
+
+    def test__cmd_targets_remove_latest(self):
+        key_dirs = ['c:\\my_private_keys']
+        options = argparse.Namespace(key_dirs=key_dirs)
+        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
+            tufup.repo.cli._cmd_targets(options=options)
+        self.mock_repo.remove_latest_bundle.assert_called()
+
+    def test__cmd_sign_threshold(self):
+        role_name = 'root'
+        key_dirs = ['c:\\my_private_keys']
+        options = argparse.Namespace(
+            role_name=role_name, key_dirs=key_dirs, expiration_days=None
+        )
+        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
+            tufup.repo.cli._cmd_sign(options=options)
+        self.mock_repo.threshold_sign.assert_called_with(
+            role_name=role_name, private_key_dirs=key_dirs
+        )
+
+    def test__cmd_sign_expired(self):
+        role_name = 'root'
+        key_dirs = ['c:\\my_private_keys']
+        options = argparse.Namespace(
+            role_name=role_name,
+            key_dirs=key_dirs,
+            expiration_days='default',  # i.e. specify -e without a value
+        )
+        with patch('tufup.repo.cli.Repository', self.mock_repo_class):
+            tufup.repo.cli._cmd_sign(options=options)
+        self.mock_repo.refresh_expiration_date.assert_called_with(
+            role_name=role_name, days=self.config['expiration_days'][role_name]
+        )
+        self.mock_repo.publish_changes.assert_called_with(
+            private_key_dirs=key_dirs
+        )
+
+    def test__get_config_from_user_no_kwargs(self):
+        default = ''
+        yes = 'y'
+        no = 'n'
+        user_inputs = iter(
+            [
+                'my-app',  # app name
+                'my_app.__version__',  # app version
+                'repo/dir',  # repo dir
+                'keys/dir',  # keys dir
+                yes,  # keep default root key name
+                yes,  # add another root key name
+                'root-2',  # key name
+                no,  # add another root key name
+                default,  # encrypt 'root' key
+                yes,  # encrypt 'root-2' key
+                '365',  # expiration days
+                '2',  # signature threshold
+                default,  # keep default targets key name
+                default,  # add another targets key name
+                default,  # encrypt 'targets' key
+                '30',  # expiration days
+                '1',  # signature threshold
+                default,  # keep default snapshot key name
+                default,  # add another snapshot key name
+                default,  # encrypt 'snapshot' key
+                '7',  # expiration days
+                '1',  # signature threshold
+                default,  # keep default timestamp key name
+                default,  # add another timestamp key name
+                default,  # encrypt 'timestamp' key
+                '1',  # expiration days
+                '1',  # signature threshold
+            ]
+        )
+        with patch('builtins.input', lambda *_, **__: next(user_inputs)):
+            config_kwargs = tufup.repo.cli._get_config_from_user()
+        self.assertTrue(config_kwargs)
+
+    def test__get_config_from_user_with_kwargs(self):
+        role_names = ['root', 'targets', 'snapshot', 'timestamp']
+        original_kwargs = dict(
+            app_name='my-app',
+            app_version_attr='my_app.__version__',
+            repo_dir='repo/dir',
+            keys_dir='keys/dir',
+            key_map={name: [name] for name in role_names},
+            encrypted_keys=['root'],
+            expiration_days={name: 1 for name in role_names},
+            thresholds={name: 1 for name in role_names},
+        )
+        default = ''
+        with patch('builtins.input', Mock(return_value=default)):
+            config_kwargs = tufup.repo.cli._get_config_from_user(
+                **original_kwargs
+            )
+        self.assertEqual(config_kwargs, original_kwargs)
```

### Comparing `tufup-0.4.9/tests/test_tests.py` & `tufup-0.5.0/tests/test_tests.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import pathlib
-from unittest import TestCase
-
-from tests import _create_cwd_change_generator, TempDirTestCase
-
-
-class CreateToggleGeneratorTests(TestCase):
-    def test__create_toggle_cwd_generator(self):
-        original_cwd = pathlib.Path.cwd()
-        toggle_generator = _create_cwd_change_generator()
-        # switch to temporary dir
-        temp_dir = next(toggle_generator)
-        self.assertNotEqual(original_cwd, temp_dir)
-        self.assertNotEqual(original_cwd, pathlib.Path.cwd())
-        self.assertTrue(pathlib.Path(temp_dir).exists())
-        # switch back to original dir
-        try:
-            next(toggle_generator)
-        except StopIteration:
-            pass
-        self.assertEqual(original_cwd, pathlib.Path.cwd())
-        self.assertFalse(pathlib.Path(temp_dir).exists())
-
-
-class TempDirTestCaseTests(TempDirTestCase):
-    def setUp(self) -> None:
-        self.original_cwd = pathlib.Path.cwd()
-        super().setUp()
-
-    def test_temporary_cwd(self):
-        current_cwd = pathlib.Path.cwd()
-        self.assertNotIn('tests', str(current_cwd))
-        self.assertNotEqual(self.original_cwd, current_cwd)
-        self.assertEqual(self.temp_dir_path.resolve(), current_cwd.resolve())
+import pathlib
+from unittest import TestCase
+
+from tests import _create_cwd_change_generator, TempDirTestCase
+
+
+class CreateToggleGeneratorTests(TestCase):
+    def test__create_toggle_cwd_generator(self):
+        original_cwd = pathlib.Path.cwd()
+        toggle_generator = _create_cwd_change_generator()
+        # switch to temporary dir
+        temp_dir = next(toggle_generator)
+        self.assertNotEqual(original_cwd, temp_dir)
+        self.assertNotEqual(original_cwd, pathlib.Path.cwd())
+        self.assertTrue(pathlib.Path(temp_dir).exists())
+        # switch back to original dir
+        try:
+            next(toggle_generator)
+        except StopIteration:
+            pass
+        self.assertEqual(original_cwd, pathlib.Path.cwd())
+        self.assertFalse(pathlib.Path(temp_dir).exists())
+
+
+class TempDirTestCaseTests(TempDirTestCase):
+    def setUp(self) -> None:
+        self.original_cwd = pathlib.Path.cwd()
+        super().setUp()
+
+    def test_temporary_cwd(self):
+        current_cwd = pathlib.Path.cwd()
+        self.assertNotIn('tests', str(current_cwd))
+        self.assertNotEqual(self.original_cwd, current_cwd)
+        self.assertEqual(self.temp_dir_path.resolve(), current_cwd.resolve())
```

### Comparing `tufup-0.4.9/tests/test_utils.py` & `tufup-0.5.0/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import pathlib
-import unittest
-from unittest.mock import Mock, patch
-
-import tufup.utils
-from tests import TempDirTestCase
-
-
-class RemovePathTests(TempDirTestCase):
-    def test_remove_path(self):
-        for arg_type in [str, pathlib.Path]:
-            # create a directory and subdirectory with dummy files
-            dir_path = self.temp_dir_path / 'dir'
-            subdir_path = dir_path / 'subdir'
-            subdir_path.mkdir(parents=True)
-            for file in [dir_path / 'file.in.dir', subdir_path / 'file.in.subdir']:
-                file.touch()
-            # just to be sure
-            self.assertEqual(2, len(list(dir_path.iterdir())))
-            self.assertEqual(1, len(list(subdir_path.iterdir())))
-            # test
-            with self.subTest(msg=arg_type):
-                self.assertTrue(
-                    tufup.utils.remove_path(path=arg_type(dir_path))
-                )
-                self.assertFalse(dir_path.exists())
-
-
-class InputTests(unittest.TestCase):
-    def test_input_bool(self):
-        inputs = [('', None), ('y', True), ('n', False), ('anything', False)]
-        for default in [True, False]:
-            for user_input, expected in inputs:
-                if expected is None:
-                    expected = default
-                with patch('builtins.input', Mock(return_value=user_input)):
-                    self.assertEqual(
-                        expected,
-                        tufup.utils.input_bool(prompt='', default=default),
-                    )
-
-    def test_input_list(self):
-        default = ['existing item']
-        item_default = 'default item'
-        new_item = 'new item'
-        bool_inputs = iter([True, True, True, False])
-        text_inputs = iter(['', new_item])
-        # we use iterators to simulate sequences of user inputs
-        with patch.object(
-                tufup.utils, 'input_bool', lambda *_, **__: next(bool_inputs)
-        ):
-            with patch.object(
-                    tufup.utils,
-                    'input_text',
-                    lambda *_, **__: next(text_inputs) or item_default,
-            ):
-                expected = default + [item_default, new_item]
-                self.assertEqual(
-                    expected,
-                    tufup.utils.input_list(
-                        prompt='', default=default, item_default=item_default
-                    )
-                )
-
-    def test_input_numeric(self):
-        default = 1
-        answer = 0
-        user_inputs = iter(['not numeric', str(answer)])
-        # we use an iterator to simulate a sequence of user inputs,
-        # and return '' instead of raising StopIteration
-        with patch('builtins.input', lambda *_: next(user_inputs, '')):
-            self.assertEqual(
-                answer, tufup.utils.input_numeric(prompt='', default=default)
-            )
-            # iterator exhausted, so next user input is ''
-            self.assertEqual(
-                default, tufup.utils.input_numeric(prompt='', default=default)
-            )
-
-    def test_input_text(self):
-        answer = 'something'
-        user_inputs = iter(['', answer])
-        with patch('builtins.input', lambda *_: next(user_inputs, '')):
-            # this should iterate until we get a non-empty answer
-            self.assertEqual(
-                answer, tufup.utils.input_text(prompt='', default='')
-            )
-            # iterator exhausted, so next user input is ''
-            self.assertEqual(
-                answer, tufup.utils.input_text(prompt='', default=answer)
-            )
-
-    def test_input_text_optional(self):
-        with patch('builtins.input', Mock(return_value='')):
-            self.assertIsNone(
-                tufup.utils.input_text(
-                    prompt='', default=None, optional=True
-                )
-            )
+import pathlib
+import unittest
+from unittest.mock import Mock, patch
+
+import tufup.utils
+from tests import TempDirTestCase
+
+
+class RemovePathTests(TempDirTestCase):
+    def test_remove_path(self):
+        for arg_type in [str, pathlib.Path]:
+            # create a directory and subdirectory with dummy files
+            dir_path = self.temp_dir_path / 'dir'
+            subdir_path = dir_path / 'subdir'
+            subdir_path.mkdir(parents=True)
+            for file in [dir_path / 'file.in.dir', subdir_path / 'file.in.subdir']:
+                file.touch()
+            # just to be sure
+            self.assertEqual(2, len(list(dir_path.iterdir())))
+            self.assertEqual(1, len(list(subdir_path.iterdir())))
+            # test
+            with self.subTest(msg=arg_type):
+                self.assertTrue(
+                    tufup.utils.remove_path(path=arg_type(dir_path))
+                )
+                self.assertFalse(dir_path.exists())
+
+
+class InputTests(unittest.TestCase):
+    def test_input_bool(self):
+        inputs = [('', None), ('y', True), ('n', False), ('anything', False)]
+        for default in [True, False]:
+            for user_input, expected in inputs:
+                if expected is None:
+                    expected = default
+                with patch('builtins.input', Mock(return_value=user_input)):
+                    self.assertEqual(
+                        expected,
+                        tufup.utils.input_bool(prompt='', default=default),
+                    )
+
+    def test_input_list(self):
+        default = ['existing item']
+        item_default = 'default item'
+        new_item = 'new item'
+        bool_inputs = iter([True, True, True, False])
+        text_inputs = iter(['', new_item])
+        # we use iterators to simulate sequences of user inputs
+        with patch.object(
+                tufup.utils, 'input_bool', lambda *_, **__: next(bool_inputs)
+        ):
+            with patch.object(
+                    tufup.utils,
+                    'input_text',
+                    lambda *_, **__: next(text_inputs) or item_default,
+            ):
+                expected = default + [item_default, new_item]
+                self.assertEqual(
+                    expected,
+                    tufup.utils.input_list(
+                        prompt='', default=default, item_default=item_default
+                    )
+                )
+
+    def test_input_numeric(self):
+        default = 1
+        answer = 0
+        user_inputs = iter(['not numeric', str(answer)])
+        # we use an iterator to simulate a sequence of user inputs,
+        # and return '' instead of raising StopIteration
+        with patch('builtins.input', lambda *_: next(user_inputs, '')):
+            self.assertEqual(
+                answer, tufup.utils.input_numeric(prompt='', default=default)
+            )
+            # iterator exhausted, so next user input is ''
+            self.assertEqual(
+                default, tufup.utils.input_numeric(prompt='', default=default)
+            )
+
+    def test_input_text(self):
+        answer = 'something'
+        user_inputs = iter(['', answer])
+        with patch('builtins.input', lambda *_: next(user_inputs, '')):
+            # this should iterate until we get a non-empty answer
+            self.assertEqual(
+                answer, tufup.utils.input_text(prompt='', default='')
+            )
+            # iterator exhausted, so next user input is ''
+            self.assertEqual(
+                answer, tufup.utils.input_text(prompt='', default=answer)
+            )
+
+    def test_input_text_optional(self):
+        with patch('builtins.input', Mock(return_value='')):
+            self.assertIsNone(
+                tufup.utils.input_text(
+                    prompt='', default=None, optional=True
+                )
+            )
```

### Comparing `tufup-0.4.9/tests/test_utils_platform_specific.py` & `tufup-0.5.0/tests/test_utils_platform_specific.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-import pathlib
-from getpass import getuser
-import os
-import subprocess
-import sys
-import tempfile
-import textwrap
-from time import sleep
-import unittest
-
-from tests import BASE_DIR, TempDirTestCase
-from tufup.utils.platform_specific import (
-    ON_WINDOWS,
-    PLATFORM_SUPPORTED,
-    run_bat_as_admin,
-    WIN_BATCH_PREFIX,
-    WIN_BATCH_SUFFIX,
-)
-
-_reason_platform_not_supported = (
-    'install_update() is only actively supported on windows and mac'
-)
-
-DUMMY_APP_CONTENT = f"""
-import sys
-sys.path.append('{(BASE_DIR.parent / 'src').as_posix()}')
-from tufup.utils.platform_specific import install_update
-install_update(src_dir=sys.argv[1], dst_dir=sys.argv[2], {{extra_kwargs_str}})
-"""
-
-ON_GITHUB = os.getenv('GITHUB_ACTIONS')
-TEST_RUNAS = os.getenv('TEST_RUNAS')
-
-
-class UtilsTests(TempDirTestCase):
-    def setUp(self) -> None:
-        super().setUp()
-        # create src dir with dummy app file, and dst dir with stale subdir
-        # and a file that must be excluded from purge
-        test_dir = self.temp_dir_path / 'tufup_tests'
-        self.src_dir = test_dir / 'src'
-        self.src_subdir = self.src_dir / 'new'
-        self.src_subdir.mkdir(parents=True)
-        self.dst_dir = test_dir / 'dst'
-        self.dst_subdir = self.dst_dir / 'stale'
-        self.dst_subdir.mkdir(parents=True)
-        (self.dst_subdir / 'stale.file').touch()
-        self.keep_file_path = self.dst_dir / 'keep.file'
-        self.keep_file_path.touch()
-        self.keep_file_str = str(self.keep_file_path).replace('\\', '\\\\')
-        self.src_file_name = 'dummy_app.py'
-        self.src_file_path = self.src_dir / self.src_file_name
-
-    def run_dummy_app(self, extra_kwargs_strings):
-        # write dummy app content to file
-        dummy_app_content = DUMMY_APP_CONTENT.format(
-            extra_kwargs_str=', '.join(extra_kwargs_strings),
-        )
-        print(dummy_app_content)
-        self.src_file_path.write_text(dummy_app_content)
-        # run the dummy app in a separate process, which, in turn, will run
-        # another process that moves the file
-        completed_process = subprocess.run(
-            [sys.executable, self.src_file_path, self.src_dir, self.dst_dir]
-        )
-        print(sys.executable)
-        completed_process.check_returncode()
-        if ON_WINDOWS:
-            # allow some time for the batch file to complete (the batch file
-            # waits a few seconds, so we have to wait longer)
-            sleep(3)
-
-    @unittest.skipIf(
-        condition=ON_GITHUB or not TEST_RUNAS or not ON_WINDOWS,
-        reason='windows only, requires user interaction',
-    )
-    def test_run_bat_as_admin(self):
-        output_path = self.temp_dir_path / 'output.txt'
-        bat_path = self.temp_dir_path / 'tell_me_who_i_am.bat'
-        bat_path.write_text(f'whoami > "{output_path}"\ntimeout /t -1')
-        # NOTE: this will open a UAC prompt (User Access Control)
-        self.assertTrue(run_bat_as_admin(file_path=bat_path))
-        # doesn't block, so we'll pause for a while
-        sleep(1)
-        self.assertTrue(output_path.exists())
-        output = output_path.read_text()
-        current_user = getuser()
-        print(f'bat file runs as: {output}')
-        print(f'current user: {current_user}')
-        self.assertTrue(len(output))
-        self.assertNotIn(current_user, output)
-
-    @unittest.skipIf(
-        condition=not PLATFORM_SUPPORTED, reason=_reason_platform_not_supported
-    )
-    def test_install_update_no_purge(self):
-        extra_kwargs_strings = []
-        if ON_WINDOWS:
-            extra_kwargs_strings.extend(['as_admin=False', 'log_file_name=None'])
-        # run the dummy app in a separate process
-        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
-        # ensure file has been moved from src to dst
-        self.assertTrue(any(self.dst_dir.iterdir()))
-        self.assertTrue((self.dst_dir / self.src_file_name).exists())
-        # new empty subdir has been moved as well
-        self.assertTrue((self.dst_dir / self.src_subdir.name).exists())
-        # original src file no longer exists
-        self.assertFalse(self.src_file_path.exists())
-        # stale dst content must still be present
-        self.assertTrue(self.dst_subdir.exists())
-        # file to keep must still be present
-        self.assertTrue(self.keep_file_path.exists())
-        # the batch file itself should have been removed
-        self.assertFalse(batch_file_exists())
-
-    @unittest.skipIf(
-        condition=not PLATFORM_SUPPORTED, reason=_reason_platform_not_supported
-    )
-    def test_install_update_purge(self):
-        extra_kwargs_strings = [
-            'purge_dst_dir=True', f'exclude_from_purge=["{self.keep_file_str}"]'
-        ]
-        if ON_WINDOWS:
-            extra_kwargs_strings.extend(['as_admin=False', 'log_file_name=None'])
-        # run the dummy app in a separate process
-        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
-        # ensure file has been moved from src to dst
-        self.assertTrue(any(self.dst_dir.iterdir()))
-        self.assertTrue((self.dst_dir / self.src_file_name).exists())
-        # new empty subdir has been moved as well
-        self.assertTrue((self.dst_dir / self.src_subdir.name).exists())
-        # original src file no longer exists
-        self.assertFalse(self.src_file_path.exists())
-        # stale dst content has been removed (robocopy /purge)
-        self.assertFalse(self.dst_subdir.exists())
-        # file to keep must still be present
-        self.assertTrue(self.keep_file_path.exists())
-
-    @unittest.skipIf(condition=not ON_WINDOWS, reason='robocopy is windows only')
-    def test_install_update_robocopy_options_override(self):
-        extra_kwargs_strings = [
-            'as_admin=False', 'log_file_name=None', 'robocopy_options_override=[]'
-        ]
-        # run the dummy app in a separate process
-        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
-        # ensure file has been copied from src to dst
-        self.assertTrue(any(self.dst_dir.iterdir()))
-        self.assertTrue((self.dst_dir / self.src_file_name).exists())
-        # new subdir has not been copied
-        self.assertFalse((self.dst_dir / self.src_subdir.name).exists())
-        # original src file still exists
-        self.assertTrue(self.src_file_path.exists())
-        # stale dst content must still be present
-        self.assertTrue(self.dst_subdir.exists())
-        # file to keep must still be present
-        self.assertTrue(self.keep_file_path.exists())
-
-    @unittest.skipIf(
-        condition=not ON_WINDOWS, reason='install.log file is windows only'
-    )
-    def test_install_update_log_file(self):
-        log_file_name = 'install.log'
-        extra_kwargs_strings = [
-            'as_admin=False',
-            f'log_file_name="{log_file_name}"',
-            'robocopy_options_override=[]',
-        ]
-        # run the dummy app in a separate process
-        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
-        # a log file should exist
-        log_file_path = self.dst_dir / log_file_name
-        self.assertTrue(log_file_path.exists())
-        log_file_content = log_file_path.read_text()
-        self.assertTrue(log_file_content)
-
-    @unittest.skipIf(
-        condition=not ON_WINDOWS, reason='windows batch files are windows only'
-    )
-    def test_install_update_custom_batch_template(self):
-        custom_content = 'some custom text'
-        custom_file_path = self.temp_dir_path / 'test.txt'
-        # a custom batch template that ignores most of the default template
-        # variables and adds some custom variables
-        custom_batch_template = textwrap.dedent(
-            """
-            echo {custom_content}> "{custom_file_path}"
-            {delete_self}
-            """
-        )
-        extra_kwargs_strings = [
-            f'batch_template="""{custom_batch_template}"""',
-            f'batch_template_extra_kwargs=dict(custom_content="{custom_content}", custom_file_path=r"{custom_file_path}")',
-        ]
-        # run the dummy app in a separate process
-        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
-        # batch file should have created a file with specified content
-        self.assertTrue(custom_file_path.exists())
-        custom_file_content = custom_file_path.read_text()
-        self.assertIn(custom_content, custom_file_content)
-        # the batch file itself should have been removed
-        self.assertFalse(batch_file_exists())
-
-
-def batch_file_exists():
-    """
-    Checks if any tufup batch files remain in the system temporary directory.
-
-    BEWARE: If a batch file does not remove itself successfully even once,
-    this function will keep returning True, until the batch file is removed
-    manually from the system temp dir (see print statement below). Windows
-    does not clear the temp dirs automatically.
-    """
-    system_temp_dir = pathlib.Path(tempfile.gettempdir())
-    print(f'system temp dir: {system_temp_dir}')
-    return any(
-        path.name.startswith(WIN_BATCH_PREFIX) and path.name.endswith(WIN_BATCH_SUFFIX)
-        for path in system_temp_dir.iterdir()
-        if path.is_file()
-    )
+import pathlib
+from getpass import getuser
+import os
+import subprocess
+import sys
+import tempfile
+import textwrap
+from time import sleep
+import unittest
+
+from tests import BASE_DIR, TempDirTestCase
+from tufup.utils.platform_specific import (
+    ON_WINDOWS,
+    PLATFORM_SUPPORTED,
+    run_bat_as_admin,
+    WIN_BATCH_PREFIX,
+    WIN_BATCH_SUFFIX,
+)
+
+_reason_platform_not_supported = (
+    'install_update() is only actively supported on windows and mac'
+)
+
+DUMMY_APP_CONTENT = f"""
+import sys
+sys.path.append('{(BASE_DIR.parent / 'src').as_posix()}')
+from tufup.utils.platform_specific import install_update
+install_update(src_dir=sys.argv[1], dst_dir=sys.argv[2], {{extra_kwargs_str}})
+"""
+
+ON_GITHUB = os.getenv('GITHUB_ACTIONS')
+TEST_RUNAS = os.getenv('TEST_RUNAS')
+
+
+class UtilsTests(TempDirTestCase):
+    def setUp(self) -> None:
+        super().setUp()
+        # create src dir with dummy app file, and dst dir with stale subdir
+        # and a file that must be excluded from purge
+        test_dir = self.temp_dir_path / 'tufup_tests'
+        self.src_dir = test_dir / 'src'
+        self.src_subdir = self.src_dir / 'new'
+        self.src_subdir.mkdir(parents=True)
+        self.dst_dir = test_dir / 'dst'
+        self.dst_subdir = self.dst_dir / 'stale'
+        self.dst_subdir.mkdir(parents=True)
+        (self.dst_subdir / 'stale.file').touch()
+        self.keep_file_path = self.dst_dir / 'keep.file'
+        self.keep_file_path.touch()
+        self.keep_file_str = str(self.keep_file_path).replace('\\', '\\\\')
+        self.src_file_name = 'dummy_app.py'
+        self.src_file_path = self.src_dir / self.src_file_name
+
+    def run_dummy_app(self, extra_kwargs_strings):
+        # write dummy app content to file
+        dummy_app_content = DUMMY_APP_CONTENT.format(
+            extra_kwargs_str=', '.join(extra_kwargs_strings),
+        )
+        print(dummy_app_content)
+        self.src_file_path.write_text(dummy_app_content)
+        # run the dummy app in a separate process, which, in turn, will run
+        # another process that moves the file
+        completed_process = subprocess.run(
+            [sys.executable, self.src_file_path, self.src_dir, self.dst_dir]
+        )
+        print(sys.executable)
+        completed_process.check_returncode()
+        if ON_WINDOWS:
+            # allow some time for the batch file to complete (the batch file
+            # waits a few seconds, so we have to wait longer)
+            sleep(3)
+
+    @unittest.skipIf(
+        condition=ON_GITHUB or not TEST_RUNAS or not ON_WINDOWS,
+        reason='windows only, requires user interaction',
+    )
+    def test_run_bat_as_admin(self):
+        output_path = self.temp_dir_path / 'output.txt'
+        bat_path = self.temp_dir_path / 'tell_me_who_i_am.bat'
+        bat_path.write_text(f'whoami > "{output_path}"\ntimeout /t -1')
+        # NOTE: this will open a UAC prompt (User Access Control)
+        self.assertTrue(run_bat_as_admin(file_path=bat_path))
+        # doesn't block, so we'll pause for a while
+        sleep(1)
+        self.assertTrue(output_path.exists())
+        output = output_path.read_text()
+        current_user = getuser()
+        print(f'bat file runs as: {output}')
+        print(f'current user: {current_user}')
+        self.assertTrue(len(output))
+        self.assertNotIn(current_user, output)
+
+    @unittest.skipIf(
+        condition=not PLATFORM_SUPPORTED, reason=_reason_platform_not_supported
+    )
+    def test_install_update_no_purge(self):
+        extra_kwargs_strings = []
+        if ON_WINDOWS:
+            extra_kwargs_strings.extend(['as_admin=False', 'log_file_name=None'])
+        # run the dummy app in a separate process
+        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
+        # ensure file has been moved from src to dst
+        self.assertTrue(any(self.dst_dir.iterdir()))
+        self.assertTrue((self.dst_dir / self.src_file_name).exists())
+        # new empty subdir has been moved as well
+        self.assertTrue((self.dst_dir / self.src_subdir.name).exists())
+        # original src file no longer exists
+        self.assertFalse(self.src_file_path.exists())
+        # stale dst content must still be present
+        self.assertTrue(self.dst_subdir.exists())
+        # file to keep must still be present
+        self.assertTrue(self.keep_file_path.exists())
+        # the batch file itself should have been removed
+        self.assertFalse(batch_file_exists())
+
+    @unittest.skipIf(
+        condition=not PLATFORM_SUPPORTED, reason=_reason_platform_not_supported
+    )
+    def test_install_update_purge(self):
+        extra_kwargs_strings = [
+            'purge_dst_dir=True', f'exclude_from_purge=["{self.keep_file_str}"]'
+        ]
+        if ON_WINDOWS:
+            extra_kwargs_strings.extend(['as_admin=False', 'log_file_name=None'])
+        # run the dummy app in a separate process
+        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
+        # ensure file has been moved from src to dst
+        self.assertTrue(any(self.dst_dir.iterdir()))
+        self.assertTrue((self.dst_dir / self.src_file_name).exists())
+        # new empty subdir has been moved as well
+        self.assertTrue((self.dst_dir / self.src_subdir.name).exists())
+        # original src file no longer exists
+        self.assertFalse(self.src_file_path.exists())
+        # stale dst content has been removed (robocopy /purge)
+        self.assertFalse(self.dst_subdir.exists())
+        # file to keep must still be present
+        self.assertTrue(self.keep_file_path.exists())
+
+    @unittest.skipIf(condition=not ON_WINDOWS, reason='robocopy is windows only')
+    def test_install_update_robocopy_options_override(self):
+        extra_kwargs_strings = [
+            'as_admin=False', 'log_file_name=None', 'robocopy_options_override=[]'
+        ]
+        # run the dummy app in a separate process
+        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
+        # ensure file has been copied from src to dst
+        self.assertTrue(any(self.dst_dir.iterdir()))
+        self.assertTrue((self.dst_dir / self.src_file_name).exists())
+        # new subdir has not been copied
+        self.assertFalse((self.dst_dir / self.src_subdir.name).exists())
+        # original src file still exists
+        self.assertTrue(self.src_file_path.exists())
+        # stale dst content must still be present
+        self.assertTrue(self.dst_subdir.exists())
+        # file to keep must still be present
+        self.assertTrue(self.keep_file_path.exists())
+
+    @unittest.skipIf(
+        condition=not ON_WINDOWS, reason='install.log file is windows only'
+    )
+    def test_install_update_log_file(self):
+        log_file_name = 'install.log'
+        extra_kwargs_strings = [
+            'as_admin=False',
+            f'log_file_name="{log_file_name}"',
+            'robocopy_options_override=[]',
+        ]
+        # run the dummy app in a separate process
+        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
+        # a log file should exist
+        log_file_path = self.dst_dir / log_file_name
+        self.assertTrue(log_file_path.exists())
+        log_file_content = log_file_path.read_text()
+        self.assertTrue(log_file_content)
+
+    @unittest.skipIf(
+        condition=not ON_WINDOWS, reason='windows batch files are windows only'
+    )
+    def test_install_update_custom_batch_template(self):
+        custom_content = 'some custom text'
+        custom_file_path = self.temp_dir_path / 'test.txt'
+        # a custom batch template that ignores most of the default template
+        # variables and adds some custom variables
+        custom_batch_template = textwrap.dedent(
+            """
+            echo {custom_content}> "{custom_file_path}"
+            {delete_self}
+            """
+        )
+        extra_kwargs_strings = [
+            f'batch_template="""{custom_batch_template}"""',
+            f'batch_template_extra_kwargs=dict(custom_content="{custom_content}", custom_file_path=r"{custom_file_path}")',
+        ]
+        # run the dummy app in a separate process
+        self.run_dummy_app(extra_kwargs_strings=extra_kwargs_strings)
+        # batch file should have created a file with specified content
+        self.assertTrue(custom_file_path.exists())
+        custom_file_content = custom_file_path.read_text()
+        self.assertIn(custom_content, custom_file_content)
+        # the batch file itself should have been removed
+        self.assertFalse(batch_file_exists())
+
+
+def batch_file_exists():
+    """
+    Checks if any tufup batch files remain in the system temporary directory.
+
+    BEWARE: If a batch file does not remove itself successfully even once,
+    this function will keep returning True, until the batch file is removed
+    manually from the system temp dir (see print statement below). Windows
+    does not clear the temp dirs automatically.
+    """
+    system_temp_dir = pathlib.Path(tempfile.gettempdir())
+    print(f'system temp dir: {system_temp_dir}')
+    return any(
+        path.name.startswith(WIN_BATCH_PREFIX) and path.name.endswith(WIN_BATCH_SUFFIX)
+        for path in system_temp_dir.iterdir()
+        if path.is_file()
+    )
```

