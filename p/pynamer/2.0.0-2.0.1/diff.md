# Comparing `tmp/pynamer-2.0.0.tar.gz` & `tmp/pynamer-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.0.0.tar", last modified: Wed May 24 16:02:12 2023, max compression
+gzip compressed data, was "pynamer-2.0.1.tar", last modified: Mon May 29 09:39:59 2023, max compression
```

## Comparing `pynamer-2.0.0.tar` & `pynamer-2.0.1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.504706 pynamer-2.0.0/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.0.0/AUTHORS.md
--rw-rw-rw-   0        0        0     9599 2023-05-24 16:01:59.000000 pynamer-2.0.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.0.0/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    18662 2023-05-24 16:02:12.504706 pynamer-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    17081 2023-05-22 08:49:55.000000 pynamer-2.0.0/README.md
--rw-rw-rw-   0        0        0     2071 2023-05-21 12:45:00.000000 pynamer-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1893 2023-05-24 16:02:12.505710 pynamer-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.407715 pynamer-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.437711 pynamer-2.0.0/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.0.0/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1853 2023-05-24 16:02:00.000000 pynamer-2.0.0/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9660 2023-05-24 15:55:39.000000 pynamer-2.0.0/src/pynamer/builder.py
--rw-rw-rw-   0        0        0      754 2023-05-21 12:10:39.000000 pynamer-2.0.0/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.447708 pynamer-2.0.0/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.0.0/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0    15174 2023-05-24 09:27:39.000000 pynamer-2.0.0/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-05-24 15:24:28.000000 pynamer-2.0.0/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.0.0/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0     5781 2023-05-24 09:37:42.000000 pynamer-2.0.0/src/pynamer/utils.py
--rw-rw-rw-   0        0        0     6128 2023-05-24 15:55:39.000000 pynamer-2.0.0/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.445710 pynamer-2.0.0/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    18662 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 16:02:12.000000 pynamer-2.0.0/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 16:02:12.502708 pynamer-2.0.0/tests/
--rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1541 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     1721 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.0.0/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1671 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.0.0/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.348382 pynamer-2.0.1/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.0.1/AUTHORS.md
+-rw-rw-rw-   0        0        0     9767 2023-05-29 09:39:45.000000 pynamer-2.0.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    18779 2023-05-29 09:39:59.348382 pynamer-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    17196 2023-05-28 18:04:36.000000 pynamer-2.0.1/README.md
+-rw-rw-rw-   0        0        0     2287 2023-05-25 17:05:54.000000 pynamer-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1841 2023-05-29 09:39:59.348382 pynamer-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 09:39:58.957773 pynamer-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.067110 pynamer-2.0.1/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.0.1/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1853 2023-05-29 09:39:46.000000 pynamer-2.0.1/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9660 2023-05-24 15:55:39.000000 pynamer-2.0.1/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2210 2023-05-28 18:04:31.000000 pynamer-2.0.1/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      726 2023-05-25 17:08:55.000000 pynamer-2.0.1/src/pynamer/config.py
+-rw-rw-rw-   0        0        0       17 2023-05-28 17:55:42.000000 pynamer-2.0.1/src/pynamer/project_count.pickle
+drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.082723 pynamer-2.0.1/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.0.1/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7702 2023-05-28 17:35:56.000000 pynamer-2.0.1/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-05-24 15:24:28.000000 pynamer-2.0.1/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.0.1/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0     9563 2023-05-28 18:04:31.000000 pynamer-2.0.1/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0     7738 2023-05-28 18:04:31.000000 pynamer-2.0.1/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.082723 pynamer-2.0.1/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    18779 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1154 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.348382 pynamer-2.0.1/tests/
+-rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1541 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     1721 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1671 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_write_output_file.py
```

### Comparing `pynamer-2.0.0/CHANGELOG.md` & `pynamer-2.0.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.0.1 (2023-05-29)
+### Documentation
+* Final updates ([`6c85802`](https://github.com/Stephen-RA-King/pynamer/commit/6c85802a132e91586d8d21c0ceb6dcf8f011264d))
+
 ## v2.0.0 (2023-05-24)
 ### Documentation
 * Update citation ([`6cd655b`](https://github.com/Stephen-RA-King/pynamer/commit/6cd655bc1c9672fd5f64cbf63a78fc739a141328))
 
 ## v1.3.4 (2023-05-22)
 ### Documentation
 * Fix type ([`a0cc3e1`](https://github.com/Stephen-RA-King/pynamer/commit/a0cc3e1b63cc3d147dea05085f7c9ecc80944815))
```

### Comparing `pynamer-2.0.0/LICENSE` & `pynamer-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/PKG-INFO` & `pynamer-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.0.0
+Version: 2.0.1
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -76,15 +76,15 @@
     -   [Wiki](https://github.com/Stephen-RA-King/pynamer/wiki)
 -   [Planned Future improvements](#Planned-Future-improvements)
 
 ## Introduction
 
 ### Project Rationale
 
-Some of you may have reached the point where you want to publish a package on the PyPI python repository.
+Some of you may have reached the point where you want to publish a package in the PyPI python repository.
 The first step of which is to choose a unique name. Here lies the problem.
 
 A recent look at the PyPI repository revealed there were over 453,769 projects, so many names have already been taken.
 
 pip leaps to the rescue with its search utility... or does it?
 
 ```python
@@ -216,15 +216,15 @@
 
 Congratulations!
 
 # Usage
 
 ---
 
-Display the help menu with the -h argument
+Display the help menu with the `-h` argument
 
 ```bash
 ~ $ pynamer -h
 ```
 
 ```bash
 usage: pynamer [-h] [-r] [-v] [-g] [-m] [-w] [--version] [-f FILE] [-o OUTPUT] [projects ...]
@@ -253,39 +253,39 @@
 
 ```bash
 ~ $ pynamer ganymede europa callisto
 ```
 
 ## Using an input file
 
-You can use the -f argument to specify a file containing the a names of projects to analyze.
+You can use the `-f` argument to specify a file containing the a names of projects to analyze.
 You specify a space separated sequence of as many names as you like on as many lines as you like. e.g.
 
 'projects' file
 
 ```file
 ganymede europa
 IO callisto
 ```
 
-Then specify the -f argument
+Then specify the `-f` argument
 
 ```bash
 ~ $ pynamer -f projects
 ```
 
 You can use the input file with names from the command line. The names will be aggregated. e.g.
 
 ```bash
 ~ $ pynamer ersa pandia leda metis -f projects
 ```
 
 ## Saving the results to a file
 
-You can specify a file to write the result to by using the -o argument. e.g.
+You can specify a file to write the result to by using the `-o` argument. e.g.
 
 ```bash
 ~ $ pynamer ersa pandia leda -o results
 ```
 
 This will write a file e.g.
 
@@ -305,37 +305,37 @@
 leda            Not Found   Not Found   Not Found       Available
 ```
 
 Again you can use a combination of names from the command line and input file.
 
 ## Register the package name with PyPI
 
-You can optionally 'register' the name on PyPI by using the -r argument.
+You can optionally 'register' the name on PyPI by using the `-r` argument.
 If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
 to PyPI.
 
 The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
 You can also optionally choose to change the version and description.
 
 ![](assets/usage_register_first.png)
 
 This information will be retained and you will not be prompted to enter this information again. However, you can regenerate
-this meta data by using the -m argument along with the -r argument. You can just enter on the options you dont want to change.
+this meta data by using the `-m` argument along with the `-r` argument. You can just enter on the options you dont want to change.
 
 ![](assets/usage_register_meta.png)
 
 ```bash
 ~ $ pynamer agrajag -r
 ```
 
 ![](assets/usage_register.png)
 
 ## Verbose output
 
-ith the -v argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
+With the `-v` argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
 The algorithm that PyPI uses to select these in unknown but seems to be a mixture of names and other
 projects written by the same author.
 
 ```bash
 ~ $ pynamer pynamer -v
 ```
 
@@ -348,15 +348,15 @@
 The PyPI Simple Index is a plain text file that lists the names of all the packages available on PyPI.
 
 It is a simplified version of the PyPI index that makes it easier for users to browse and download packages.
 
 The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
 The Index is updated every few hours.
 
-Using the -g argument can be used to regenerate the local file contents.
+Using the `-g` argument can be used to regenerate the local file contents.
 
 ```bash
 ~ $ pynamer -g
 ```
 
 ![](assets/usage_generate.png)
 
@@ -394,15 +394,15 @@
 HTTPError: 400 Bad Request from https://test.pypi.org/legacy/
 The name 'yourpackage' is too similar to an existing project. See https://test.pypi.org/help/#project-name for more information-
 ```
 
 Using a name similar to to an existing package name is a security issue.
 
 Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
-e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found at GitHub: [warehouse](https://github.com/pypi/warehouse).
+e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found on GitHub: [warehouse](https://github.com/pypi/warehouse).
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
@@ -429,14 +429,16 @@
 
 Stephen R A King : [sking.github@gmail.com](sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
 
+[![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
+
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
```

### Comparing `pynamer-2.0.0/README.md` & `pynamer-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     -   [Wiki](https://github.com/Stephen-RA-King/pynamer/wiki)
 -   [Planned Future improvements](#Planned-Future-improvements)
 
 ## Introduction
 
 ### Project Rationale
 
-Some of you may have reached the point where you want to publish a package on the PyPI python repository.
+Some of you may have reached the point where you want to publish a package in the PyPI python repository.
 The first step of which is to choose a unique name. Here lies the problem.
 
 A recent look at the PyPI repository revealed there were over 453,769 projects, so many names have already been taken.
 
 pip leaps to the rescue with its search utility... or does it?
 
 ```python
@@ -187,15 +187,15 @@
 
 Congratulations!
 
 # Usage
 
 ---
 
-Display the help menu with the -h argument
+Display the help menu with the `-h` argument
 
 ```bash
 ~ $ pynamer -h
 ```
 
 ```bash
 usage: pynamer [-h] [-r] [-v] [-g] [-m] [-w] [--version] [-f FILE] [-o OUTPUT] [projects ...]
@@ -224,39 +224,39 @@
 
 ```bash
 ~ $ pynamer ganymede europa callisto
 ```
 
 ## Using an input file
 
-You can use the -f argument to specify a file containing the a names of projects to analyze.
+You can use the `-f` argument to specify a file containing the a names of projects to analyze.
 You specify a space separated sequence of as many names as you like on as many lines as you like. e.g.
 
 'projects' file
 
 ```file
 ganymede europa
 IO callisto
 ```
 
-Then specify the -f argument
+Then specify the `-f` argument
 
 ```bash
 ~ $ pynamer -f projects
 ```
 
 You can use the input file with names from the command line. The names will be aggregated. e.g.
 
 ```bash
 ~ $ pynamer ersa pandia leda metis -f projects
 ```
 
 ## Saving the results to a file
 
-You can specify a file to write the result to by using the -o argument. e.g.
+You can specify a file to write the result to by using the `-o` argument. e.g.
 
 ```bash
 ~ $ pynamer ersa pandia leda -o results
 ```
 
 This will write a file e.g.
 
@@ -276,37 +276,37 @@
 leda            Not Found   Not Found   Not Found       Available
 ```
 
 Again you can use a combination of names from the command line and input file.
 
 ## Register the package name with PyPI
 
-You can optionally 'register' the name on PyPI by using the -r argument.
+You can optionally 'register' the name on PyPI by using the `-r` argument.
 If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
 to PyPI.
 
 The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
 You can also optionally choose to change the version and description.
 
 ![](assets/usage_register_first.png)
 
 This information will be retained and you will not be prompted to enter this information again. However, you can regenerate
-this meta data by using the -m argument along with the -r argument. You can just enter on the options you dont want to change.
+this meta data by using the `-m` argument along with the `-r` argument. You can just enter on the options you dont want to change.
 
 ![](assets/usage_register_meta.png)
 
 ```bash
 ~ $ pynamer agrajag -r
 ```
 
 ![](assets/usage_register.png)
 
 ## Verbose output
 
-ith the -v argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
+With the `-v` argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
 The algorithm that PyPI uses to select these in unknown but seems to be a mixture of names and other
 projects written by the same author.
 
 ```bash
 ~ $ pynamer pynamer -v
 ```
 
@@ -319,15 +319,15 @@
 The PyPI Simple Index is a plain text file that lists the names of all the packages available on PyPI.
 
 It is a simplified version of the PyPI index that makes it easier for users to browse and download packages.
 
 The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
 The Index is updated every few hours.
 
-Using the -g argument can be used to regenerate the local file contents.
+Using the `-g` argument can be used to regenerate the local file contents.
 
 ```bash
 ~ $ pynamer -g
 ```
 
 ![](assets/usage_generate.png)
 
@@ -365,15 +365,15 @@
 HTTPError: 400 Bad Request from https://test.pypi.org/legacy/
 The name 'yourpackage' is too similar to an existing project. See https://test.pypi.org/help/#project-name for more information-
 ```
 
 Using a name similar to to an existing package name is a security issue.
 
 Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
-e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found at GitHub: [warehouse](https://github.com/pypi/warehouse).
+e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found on GitHub: [warehouse](https://github.com/pypi/warehouse).
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
@@ -400,14 +400,16 @@
 
 Stephen R A King : [sking.github@gmail.com](sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
 
+[![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
+
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
```

### Comparing `pynamer-2.0.0/pyproject.toml` & `pynamer-2.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,104 @@
-[build-system]
-requires = [
-    "setuptools",
-    "wheel"
-]
-build-backend = "setuptools.build_meta"
-
-[tool]
-[tool.black]
-line-length = 88
-
-[tool.cruft]
-skip = [
-    "tests/",
-    "src/",
-    "*/header.png",
-    ".pypirc",
-    "CHANGELOG.md",
-    "setup.cfg"
-]
-
-[tool.isort]
-import_heading_stdlib = "Core Library modules"
-import_heading_thirdparty = "Third party modules"
-import_heading_firstparty = "First party modules"
-import_heading_localfolder = "Local modules"
-include_trailing_comma = true
-indent = '    '
-known_third_party = [
-    "click",
-    "pytest",
-    "setuptools",
-    "pip-tools",
-    "pre-commit"
-]
-known_first_party = [
-    "pathmagic"
-]
-line_length = 80
-multi_line_output = 3
-force_grid_wrap = 0
-use_parentheses = true
-ensure_newline_before_comments = true
-balanced_wrapping = true
-combine_as_imports = true
-
-[tool.mypy]
-ignore_missing_imports = true
-check_untyped_defs = true
-disallow_untyped_defs = false
-warn_unused_ignores = true
-strict_optional = true
-warn_redundant_casts = true
-warn_unused_configs = true
-disallow_untyped_calls = false
-disallow_incomplete_defs = true
-follow_imports = "skip"
-html_report = "mypy-report"
-mypy_path = "typeshed/pyi:typeshed/imports"
-
-[tool.semantic_release]
-version_variable = [
-    "src/pynamer/__init__.py:__version__",
-    "docs/conf.py:version",
-]
-branch = "main"
-changelog_file = "CHANGELOG.md"
-build_command = "python -m build"
-dist_path = "dist/"
-upload_to_pypi = true
-upload_to_repository = true
-remove_dist = true
-version_source = "tag"
-commit_message = "chore: generate by PSR"
-
-[tool.flakeheaven]
-# base = "https://raw.githubusercontent.com/flakeheaven/flakeheaven/main/pyproject.toml"
-exclude = ["example.py"]
-format = "grouped"
-max_line_length = 80
-show_source = true
-
-[tool.flakeheaven.plugins]
-pyflakes = ["+*", "-F401"]
-"flake8-*" = ["+*"]
-mccabe = ["+*"]
-pep8-naming = ["+*"]
-pycodestyle = ["+*"]
-pylint = ["+F*", "+E*", "-E0611", "-E1101", "-E0401", "-E1102", "-E1123"]
-
-[tool.coverage.run]
-branch = true
-parallel = true
-
-[tool.coverage.report]
-show_missing = true
-precision = 2
-skip_empty = true
+[build-system]
+requires = [
+    "setuptools",
+    "wheel"
+]
+build-backend = "setuptools.build_meta"
+
+[tool]
+[tool.black]
+line-length = 88
+
+[tool.cruft]
+skip = [
+    "tests/",
+    "src/",
+    "*/header.png",
+    ".pypirc",
+    "CHANGELOG.md",
+    "setup.cfg"
+]
+
+[tool.isort]
+import_heading_stdlib = "Core Library modules"
+import_heading_thirdparty = "Third party modules"
+import_heading_firstparty = "First party modules"
+import_heading_localfolder = "Local modules"
+include_trailing_comma = true
+indent = '    '
+known_third_party = [
+    "click",
+    "pytest",
+    "setuptools",
+    "pip-tools",
+    "pre-commit"
+]
+known_first_party = [
+    "pathmagic"
+]
+line_length = 80
+multi_line_output = 3
+force_grid_wrap = 0
+use_parentheses = true
+ensure_newline_before_comments = true
+balanced_wrapping = true
+combine_as_imports = true
+
+[tool.mypy]
+ignore_missing_imports = true
+check_untyped_defs = true
+disallow_untyped_defs = false
+warn_unused_ignores = true
+strict_optional = true
+warn_redundant_casts = true
+warn_unused_configs = true
+disallow_untyped_calls = false
+disallow_incomplete_defs = true
+follow_imports = "skip"
+html_report = "reports/mypy"
+cache_dir = 'cache/.mypy_cache'
+mypy_path = "typeshed/pyi:typeshed/imports"
+exclude = [
+    '^tests/[\w]*.py$',
+    '^tools/[\w]*.py$',
+    '^tasks.py$'
+]
+
+[tool.semantic_release]
+version_variable = [
+    "src/pynamer/__init__.py:__version__",
+    "docs/conf.py:version",
+]
+branch = "main"
+changelog_file = "CHANGELOG.md"
+build_command = "python -m build"
+dist_path = "dist/"
+upload_to_pypi = true
+upload_to_repository = true
+remove_dist = true
+version_source = "tag"
+commit_message = "chore: generate by PSR"
+
+[tool.flakeheaven]
+# base = "https://raw.githubusercontent.com/flakeheaven/flakeheaven/main/pyproject.toml"
+exclude = ["example.py"]
+format = "grouped"
+max_line_length = 80
+show_source = true
+
+[tool.flakeheaven.plugins]
+pyflakes = ["+*", "-F401"]
+"flake8-*" = ["+*"]
+mccabe = ["+*"]
+pep8-naming = ["+*"]
+pycodestyle = ["+*"]
+pylint = ["+F*", "+E*", "-E0611", "-E1101", "-E0401", "-E1102", "-E1123"]
+
+[tool.coverage.run]
+branch = true
+parallel = true
+
+[tool.coverage.report]
+show_missing = true
+precision = 2
+skip_empty = true
```

### Comparing `pynamer-2.0.0/setup.cfg` & `pynamer-2.0.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -102,18 +102,15 @@
 00000650: 3d20 3838 0d0a 7365 6c65 6374 203d 2042  = 88..select = B
 00000660: 2c20 4239 2c20 432c 2044 2c20 452c 2046  , B9, C, D, E, F
 00000670: 2c20 4e2c 2057 0d0a 6578 636c 7564 6520  , N, W..exclude 
 00000680: 3d20 7465 7374 732f 2a2c 2e74 6f78 2f2a  = tests/*,.tox/*
 00000690: 2c2e 6e6f 782f 2a2c 646f 6373 2f2a 2c2e  ,.nox/*,docs/*,.
 000006a0: 6769 742f 2a2c 2e67 6974 6875 622f 2a0d  git/*,.github/*.
 000006b0: 0a69 676e 6f72 6520 3d20 0d0a 0945 3230  .ignore = ...E20
-000006c0: 332c 0d0a 0957 3530 332c 0d0a 0946 3430  3,...W503,...F40
-000006d0: 312c 0d0a 7065 722d 6669 6c65 2d69 676e  1,..per-file-ign
-000006e0: 6f72 6573 203d 200d 0a09 5f5f 696e 6974  ores = ...__init
-000006f0: 5f5f 2e70 793a 4634 3031 0d0a 0970 6174  __.py:F401...pat
-00000700: 686d 6167 6963 2e70 793a 4634 3031 0d0a  hmagic.py:F401..
-00000710: 0974 6573 745f 7079 6e61 6d65 722e 7079  .test_pynamer.py
-00000720: 3a46 3430 310d 0a09 7079 6e61 6d65 722e  :F401...pynamer.
-00000730: 7079 3a46 3430 310d 0a0d 0a5b 6567 675f  py:F401....[egg_
-00000740: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000750: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000760: 300d 0a0d 0a                             0....
+000006c0: 332c 0d0a 0957 3530 332c 0d0a 7065 722d  3,...W503,..per-
+000006d0: 6669 6c65 2d69 676e 6f72 6573 203d 200d  file-ignores = .
+000006e0: 0a09 7079 6e61 6d65 722e 7079 3a43 3930  ..pynamer.py:C90
+000006f0: 310d 0a09 6275 696c 6465 722e 7079 3a43  1...builder.py:C
+00000700: 3930 310d 0a0d 0a5b 6567 675f 696e 666f  901....[egg_info
+00000710: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000720: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000730: 0a                                       .
```

### Comparing `pynamer-2.0.0/src/pynamer/__init__.py` & `pynamer-2.0.1/src/pynamer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
```

### Comparing `pynamer-2.0.0/src/pynamer/builder.py` & `pynamer-2.0.1/src/pynamer/builder.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/src/pynamer/config.py` & `pynamer-2.0.1/src/pynamer/config.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-#!/usr/bin/env python3
-
-# Core Library modules
-import sys
-from pathlib import Path
-from typing import Optional
-
-# Local modules
-from . import project_count
-
-
-class Config:
-    """Configuration class"""
-
-    pypirc: Optional[Path] = None
-    original_project_name: str = "project_name"
-    no_cleanup: bool = False
-    project_count: int = project_count
-    package_version: str = "0.0.0"
-    description: str = "placeholder"
-    pypi_search_url: str = "https://pypi.org/search/"
-    pypi_project_url: str = "https://pypi.org/project/"
-    pypi_json_url: str = "https://pypi.org/pypi/"
-    pypi_simple_index_url: str = "https://pypi.org/simple/"
-    idlemode: int = 1 if "idlelib.run" in sys.modules else 0
-
-
-config = Config()
+#!/usr/bin/env python3
+
+# Core Library modules
+import sys
+from pathlib import Path
+from typing import Optional
+
+# Local modules
+from . import project_count
+
+
+class Config:
+    """Configuration class"""
+
+    pypirc: Optional[Path] = None
+    original_project_name: str = "project_name"
+    no_cleanup: bool = False
+    project_count: int = project_count
+    package_version: str = "0.0.0"
+    description: str = "placeholder"
+    pypi_search_url: str = "https://pypi.org/search/"
+    pypi_project_url: str = "https://pypi.org/project/"
+    pypi_json_url: str = "https://pypi.org/pypi/"
+    pypi_simple_index_url: str = "https://pypi.org/simple/"
+    idlemode: int = 1 if "idlelib.run" in sys.modules else 0
+
+
+config = Config()
```

### Comparing `pynamer-2.0.0/src/pynamer/validators.py` & `pynamer-2.0.1/src/pynamer/validators.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import string
 from datetime import datetime
 from typing import Any, Union
 
 # Third party modules
 import requests
 from bs4 import BeautifulSoup
+from rich.console import Console
+from rich.table import Table
 
 # Local modules
 from . import logger, pypi_index_file_trv
 from .config import config
 from .utils import _generate_pypi_index
 
 
@@ -45,15 +47,15 @@
 
     Raises:
         SystemExit:     If any requests.RequestException occurs.
     """
     url_project = "".join([config.pypi_project_url, project_name, "/"])
     logger.debug("attempting to get url %s", url_project)
     try:
-        project_ping = requests.get(url_project, timeout=10)
+        project_ping = requests.get(url_project, timeout=5)
     except requests.RequestException as e:
         logger.error("An error occurred: %s", e)
         raise SystemExit("An error occurred with an HTTP request")
     if project_ping.status_code == 200:
         logger.debug("%s FOUND in the project area of PyPI", project_name)
         return True
     logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
@@ -68,15 +70,15 @@
 
     Raises:
         SystemExit:     If any requests.RequestException occurs.
     """
     url_json = "".join([config.pypi_json_url, project_name, "/json"])
     logger.debug("attempting to get url %s", url_json)
     try:
-        project_json_raw = requests.get(url_json, timeout=10)
+        project_json_raw = requests.get(url_json, timeout=5)
     except requests.RequestException as e:
         logger.error("An error occurred: %s", e)
         raise SystemExit("An error occurred with an HTTP request")
     if project_json_raw.status_code == 200:
         project_json = json.loads(project_json_raw.content)
         result = "".join(
             [
@@ -171,7 +173,45 @@
             "".join([str(total), "+"])
             if total == 10000
             else (str(int(total) - len(match)))
         )
     else:
         others_total = "0"
     return match, others, others_total
+
+
+def _final_analysis(pattern: list[int]) -> None:
+    """Displays a rich console table displaying the conclusion of the test results
+
+    Args:
+        pattern:    A list of the test results:
+                    1 - A 'negative' result, indicating the project has been found.
+                    0 - A 'positive' result, indicating the project was not found.
+    """
+    table = Table(show_header=True)
+    table.add_column("FINAL ANALYSIS", style="bold cyan")
+    if pattern == [0, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "It can only be found by searching the simple index which is not available "
+            "through the interface"
+        )
+    elif pattern == [1, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "However if appears in the simple index and can be displayed by simply"
+            " browsing "
+            "to the projects URL"
+        )
+    elif sum(pattern) >= 1:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row("The package name was found in at least one place")
+    elif sum(pattern) == 0:
+        table.add_row("[green]AVAILABLE![/green]\n")
+        table.add_row("The package name was not found in any part of PyPI")
+
+    console = Console()
+    console.print(table)
```

### Comparing `pynamer-2.0.0/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.0.1/src/pynamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.0.0
+Version: 2.0.1
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -76,15 +76,15 @@
     -   [Wiki](https://github.com/Stephen-RA-King/pynamer/wiki)
 -   [Planned Future improvements](#Planned-Future-improvements)
 
 ## Introduction
 
 ### Project Rationale
 
-Some of you may have reached the point where you want to publish a package on the PyPI python repository.
+Some of you may have reached the point where you want to publish a package in the PyPI python repository.
 The first step of which is to choose a unique name. Here lies the problem.
 
 A recent look at the PyPI repository revealed there were over 453,769 projects, so many names have already been taken.
 
 pip leaps to the rescue with its search utility... or does it?
 
 ```python
@@ -216,15 +216,15 @@
 
 Congratulations!
 
 # Usage
 
 ---
 
-Display the help menu with the -h argument
+Display the help menu with the `-h` argument
 
 ```bash
 ~ $ pynamer -h
 ```
 
 ```bash
 usage: pynamer [-h] [-r] [-v] [-g] [-m] [-w] [--version] [-f FILE] [-o OUTPUT] [projects ...]
@@ -253,39 +253,39 @@
 
 ```bash
 ~ $ pynamer ganymede europa callisto
 ```
 
 ## Using an input file
 
-You can use the -f argument to specify a file containing the a names of projects to analyze.
+You can use the `-f` argument to specify a file containing the a names of projects to analyze.
 You specify a space separated sequence of as many names as you like on as many lines as you like. e.g.
 
 'projects' file
 
 ```file
 ganymede europa
 IO callisto
 ```
 
-Then specify the -f argument
+Then specify the `-f` argument
 
 ```bash
 ~ $ pynamer -f projects
 ```
 
 You can use the input file with names from the command line. The names will be aggregated. e.g.
 
 ```bash
 ~ $ pynamer ersa pandia leda metis -f projects
 ```
 
 ## Saving the results to a file
 
-You can specify a file to write the result to by using the -o argument. e.g.
+You can specify a file to write the result to by using the `-o` argument. e.g.
 
 ```bash
 ~ $ pynamer ersa pandia leda -o results
 ```
 
 This will write a file e.g.
 
@@ -305,37 +305,37 @@
 leda            Not Found   Not Found   Not Found       Available
 ```
 
 Again you can use a combination of names from the command line and input file.
 
 ## Register the package name with PyPI
 
-You can optionally 'register' the name on PyPI by using the -r argument.
+You can optionally 'register' the name on PyPI by using the `-r` argument.
 If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
 to PyPI.
 
 The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
 You can also optionally choose to change the version and description.
 
 ![](assets/usage_register_first.png)
 
 This information will be retained and you will not be prompted to enter this information again. However, you can regenerate
-this meta data by using the -m argument along with the -r argument. You can just enter on the options you dont want to change.
+this meta data by using the `-m` argument along with the `-r` argument. You can just enter on the options you dont want to change.
 
 ![](assets/usage_register_meta.png)
 
 ```bash
 ~ $ pynamer agrajag -r
 ```
 
 ![](assets/usage_register.png)
 
 ## Verbose output
 
-ith the -v argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
+With the `-v` argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
 The algorithm that PyPI uses to select these in unknown but seems to be a mixture of names and other
 projects written by the same author.
 
 ```bash
 ~ $ pynamer pynamer -v
 ```
 
@@ -348,15 +348,15 @@
 The PyPI Simple Index is a plain text file that lists the names of all the packages available on PyPI.
 
 It is a simplified version of the PyPI index that makes it easier for users to browse and download packages.
 
 The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
 The Index is updated every few hours.
 
-Using the -g argument can be used to regenerate the local file contents.
+Using the `-g` argument can be used to regenerate the local file contents.
 
 ```bash
 ~ $ pynamer -g
 ```
 
 ![](assets/usage_generate.png)
 
@@ -394,15 +394,15 @@
 HTTPError: 400 Bad Request from https://test.pypi.org/legacy/
 The name 'yourpackage' is too similar to an existing project. See https://test.pypi.org/help/#project-name for more information-
 ```
 
 Using a name similar to to an existing package name is a security issue.
 
 Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
-e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found at GitHub: [warehouse](https://github.com/pypi/warehouse).
+e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found on GitHub: [warehouse](https://github.com/pypi/warehouse).
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
@@ -429,14 +429,16 @@
 
 Stephen R A King : [sking.github@gmail.com](sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
 
+[![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
+
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
```

### Comparing `pynamer-2.0.0/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.0.1/src/pynamer.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/pynamer/README.md
 src/pynamer/__init__.py
 src/pynamer/builder.py
+src/pynamer/cli.py
 src/pynamer/config.py
+src/pynamer/project_count.pickle
 src/pynamer/pynamer.py
 src/pynamer/setup.txt
 src/pynamer/setup_base.txt
 src/pynamer/utils.py
 src/pynamer/validators.py
 src/pynamer.egg-info/PKG-INFO
 src/pynamer.egg-info/SOURCES.txt
```

### Comparing `pynamer-2.0.0/tests/test_args.py` & `pynamer-2.0.1/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_build_dist.py` & `pynamer-2.0.1/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_cleanup.py` & `pynamer-2.0.1/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_create_setup_file.py` & `pynamer-2.0.1/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_defaults.py` & `pynamer-2.0.1/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_delete_director.py` & `pynamer-2.0.1/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_feedback.py` & `pynamer-2.0.1/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_final_analysis.py` & `pynamer-2.0.1/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_find_pypirc_file.py` & `pynamer-2.0.1/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_generate_pypi_index.py` & `pynamer-2.0.1/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_ping_json.py` & `pynamer-2.0.1/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_ping_project.py` & `pynamer-2.0.1/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_process_input_file.py` & `pynamer-2.0.1/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_pypi_search.py` & `pynamer-2.0.1/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_pypi_search_index.py` & `pynamer-2.0.1/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_rename_project_dir.py` & `pynamer-2.0.1/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_upload_dist.py` & `pynamer-2.0.1/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_utils_version.py` & `pynamer-2.0.1/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.0/tests/test_write_output_file.py` & `pynamer-2.0.1/tests/test_write_output_file.py`

 * *Files identical despite different names*

