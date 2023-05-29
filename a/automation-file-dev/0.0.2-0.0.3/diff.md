# Comparing `tmp/automation_file_dev-0.0.2.tar.gz` & `tmp/automation_file_dev-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file_dev-0.0.2.tar", last modified: Sat May 27 05:08:15 2023, max compression
+gzip compressed data, was "automation_file_dev-0.0.3.tar", last modified: Mon May 29 02:19:48 2023, max compression
```

## Comparing `automation_file_dev-0.0.2.tar` & `automation_file_dev-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.761092 automation_file_dev-0.0.2/
--rw-rw-rw-   0        0        0     1084 2023-04-29 15:33:58.000000 automation_file_dev-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1376 2023-05-27 05:08:15.760095 automation_file_dev-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-05-26 18:14:27.000000 automation_file_dev-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.739946 automation_file_dev-0.0.2/automation_file_dev.egg-info/
--rw-rw-rw-   0        0        0     1376 2023-05-27 05:08:15.000000 automation_file_dev-0.0.2/automation_file_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-05-27 05:08:15.000000 automation_file_dev-0.0.2/automation_file_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 05:08:15.000000 automation_file_dev-0.0.2/automation_file_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-27 05:08:15.000000 automation_file_dev-0.0.2/automation_file_dev.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.740894 automation_file_dev-0.0.2/file_automation/
--rw-rw-rw-   0        0        0      712 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.744066 automation_file_dev-0.0.2/file_automation/dir/
--rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/dir/__init__.py
--rw-rw-rw-   0        0        0     1230 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/dir/dir_process.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.748059 automation_file_dev-0.0.2/file_automation/file/
--rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/file/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/file/file_process.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.750053 automation_file_dev-0.0.2/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-04-29 16:59:14.000000 automation_file_dev-0.0.2/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.756105 automation_file_dev-0.0.2/file_automation/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/utils/exception/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      165 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.758100 automation_file_dev-0.0.2/file_automation/zip/
--rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/zip/__init__.py
--rw-rw-rw-   0        0        0     2383 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/zip/zip_process.py
--rw-rw-rw-   0        0        0      877 2023-05-27 05:07:53.000000 automation_file_dev-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 05:08:15.761092 automation_file_dev-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.081762 automation_file_dev-0.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file_dev-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1376 2023-05-29 02:19:48.080760 automation_file_dev-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      749 2023-05-29 01:54:01.000000 automation_file_dev-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.021777 automation_file_dev-0.0.3/automation_file_dev.egg-info/
+-rw-rw-rw-   0        0        0     1376 2023-05-29 02:19:47.000000 automation_file_dev-0.0.3/automation_file_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-05-29 02:19:47.000000 automation_file_dev-0.0.3/automation_file_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 02:19:47.000000 automation_file_dev-0.0.3/automation_file_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-29 02:19:47.000000 automation_file_dev-0.0.3/automation_file_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.024779 automation_file_dev-0.0.3/file_automation/
+-rw-rw-rw-   0        0        0      325 2023-05-29 02:05:27.000000 automation_file_dev-0.0.3/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.027778 automation_file_dev-0.0.3/file_automation/local/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file_dev-0.0.3/file_automation/local/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.037787 automation_file_dev-0.0.3/file_automation/local/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file_dev-0.0.3/file_automation/local/dir/__init__.py
+-rw-rw-rw-   0        0        0     1230 2023-05-19 07:13:21.000000 automation_file_dev-0.0.3/file_automation/local/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.045806 automation_file_dev-0.0.3/file_automation/local/file/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file_dev-0.0.3/file_automation/local/file/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-05-19 06:44:49.000000 automation_file_dev-0.0.3/file_automation/local/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.055532 automation_file_dev-0.0.3/file_automation/local/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file_dev-0.0.3/file_automation/local/zip/__init__.py
+-rw-rw-rw-   0        0        0     2383 2023-05-19 09:53:23.000000 automation_file_dev-0.0.3/file_automation/local/zip/zip_process.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.058532 automation_file_dev-0.0.3/file_automation/remote/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file_dev-0.0.3/file_automation/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.061531 automation_file_dev-0.0.3/file_automation/remote/google_drive/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file_dev-0.0.3/file_automation/remote/google_drive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.065532 automation_file_dev-0.0.3/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file_dev-0.0.3/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:19:48.075761 automation_file_dev-0.0.3/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file_dev-0.0.3/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:25.000000 automation_file_dev-0.0.3/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      165 2023-05-19 07:56:11.000000 automation_file_dev-0.0.3/file_automation/utils/exception/exceptions.py
+-rw-rw-rw-   0        0        0      877 2023-05-29 02:17:59.000000 automation_file_dev-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 02:19:48.081762 automation_file_dev-0.0.3/setup.cfg
```

### Comparing `automation_file_dev-0.0.2/LICENSE` & `automation_file_dev-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `automation_file_dev-0.0.2/PKG-INFO` & `automation_file_dev-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_file_dev
-Version: 0.0.2
+Version: 0.0.3
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file_dev-0.0.2/automation_file_dev.egg-info/PKG-INFO` & `automation_file_dev-0.0.3/automation_file_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-file-dev
-Version: 0.0.2
+Version: 0.0.3
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file_dev-0.0.2/automation_file_dev.egg-info/SOURCES.txt` & `automation_file_dev-0.0.3/automation_file_dev.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 README.md
 pyproject.toml
 automation_file_dev.egg-info/PKG-INFO
 automation_file_dev.egg-info/SOURCES.txt
 automation_file_dev.egg-info/dependency_links.txt
 automation_file_dev.egg-info/top_level.txt
 file_automation/__init__.py
-file_automation/dir/__init__.py
-file_automation/dir/dir_process.py
-file_automation/file/__init__.py
-file_automation/file/file_process.py
+file_automation/local/__init__.py
+file_automation/local/dir/__init__.py
+file_automation/local/dir/dir_process.py
+file_automation/local/file/__init__.py
+file_automation/local/file/file_process.py
+file_automation/local/zip/__init__.py
+file_automation/local/zip/zip_process.py
+file_automation/remote/__init__.py
+file_automation/remote/google_drive/__init__.py
 file_automation/utils/__init__.py
 file_automation/utils/exception/__init__.py
 file_automation/utils/exception/exception_tags.py
-file_automation/utils/exception/exceptions.py
-file_automation/zip/__init__.py
-file_automation/zip/zip_process.py
+file_automation/utils/exception/exceptions.py
```

### Comparing `automation_file_dev-0.0.2/file_automation/dir/dir_process.py` & `automation_file_dev-0.0.3/file_automation/local/dir/dir_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.2/file_automation/file/file_process.py` & `automation_file_dev-0.0.3/file_automation/local/file/file_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.2/file_automation/zip/zip_process.py` & `automation_file_dev-0.0.3/file_automation/local/zip/zip_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.2/pyproject.toml` & `automation_file_dev-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file_dev"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = ""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

