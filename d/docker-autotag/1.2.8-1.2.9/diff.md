# Comparing `tmp/docker_autotag-1.2.8.tar.gz` & `tmp/docker_autotag-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_autotag-1.2.8.tar", max compression
+gzip compressed data, was "docker_autotag-1.2.9.tar", max compression
```

## Comparing `docker_autotag-1.2.8.tar` & `docker_autotag-1.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1123 2023-03-20 13:11:00.566913 docker_autotag-1.2.8/LICENSE
--rw-r--r--   0        0        0     3596 2023-03-20 13:11:00.566913 docker_autotag-1.2.8/README.md
--rw-r--r--   0        0        0       46 2023-03-20 13:11:20.326209 docker_autotag-1.2.8/dockerautotag/__init__.py
--rw-r--r--   0        0        0     3756 2023-03-20 13:11:00.566913 docker_autotag-1.2.8/dockerautotag/cli.py
--rw-r--r--   0        0        0     5748 2023-03-20 13:11:00.566913 docker_autotag-1.2.8/dockerautotag/logging.py
--rw-r--r--   0        0        0      713 2023-03-20 13:11:00.566913 docker_autotag-1.2.8/dockerautotag/utils.py
--rw-r--r--   0        0        0     3404 2023-03-20 13:11:20.322209 docker_autotag-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     5278 1970-01-01 00:00:00.000000 docker_autotag-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-05-29 20:13:22.969835 docker_autotag-1.2.9/LICENSE
+-rw-r--r--   0        0        0     3596 2023-05-29 20:13:22.969835 docker_autotag-1.2.9/README.md
+-rw-r--r--   0        0        0       46 2023-05-29 20:13:35.813742 docker_autotag-1.2.9/dockerautotag/__init__.py
+-rw-r--r--   0        0        0     3753 2023-05-29 20:13:22.969835 docker_autotag-1.2.9/dockerautotag/cli.py
+-rw-r--r--   0        0        0     5748 2023-05-29 20:13:22.969835 docker_autotag-1.2.9/dockerautotag/logging.py
+-rw-r--r--   0        0        0      713 2023-05-29 20:13:22.969835 docker_autotag-1.2.9/dockerautotag/utils.py
+-rw-r--r--   0        0        0     3376 2023-05-29 20:13:35.813742 docker_autotag-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 docker_autotag-1.2.9/PKG-INFO
```

### Comparing `docker_autotag-1.2.8/LICENSE` & `docker_autotag-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_autotag-1.2.8/README.md` & `docker_autotag-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `docker_autotag-1.2.8/dockerautotag/cli.py` & `docker_autotag-1.2.9/dockerautotag/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,12 +119,12 @@
         v = self._tag_extra(v, config["extra"])
 
         if config["file"]:
             try:
                 with open(config["file"], "w") as f:
                     f.write(",".join(v))
             except OSError as e:
-                self.logger.error(f"Unable to write file: {str(e)}")
+                self.logger.error(f"Unable to write file: {e!s}")
 
 
 def main():
     Autotag()
```

### Comparing `docker_autotag-1.2.8/dockerautotag/logging.py` & `docker_autotag-1.2.9/dockerautotag/logging.py`

 * *Files identical despite different names*

### Comparing `docker_autotag-1.2.8/dockerautotag/utils.py` & `docker_autotag-1.2.9/dockerautotag/utils.py`

 * *Files identical despite different names*

### Comparing `docker_autotag-1.2.8/pyproject.toml` & `docker_autotag-1.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,50 +28,50 @@
 license = "MIT"
 name = "docker-autotag"
 packages = [
   {include = "dockerautotag"},
 ]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/docker-autotag/"
-version = "1.2.8"
+version = "1.2.9"
 
 [tool.poetry.dependencies]
 colorama = "0.4.6"
 python = "^3.7.0"
 python-json-logger = "2.0.7"
 semantic-version = "2.10.0"
 
 [tool.poetry.scripts]
 docker-autotag = "dockerautotag.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.0.257"
-pytest = "7.2.2"
+ruff = "0.0.270"
+pytest = "7.3.1"
 pytest-mock = "3.10.0"
-pytest-cov = "4.0.0"
+pytest-cov = "4.1.0"
 toml = "0.10.2"
-yapf = "0.32.0"
+yapf = "0.33.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
 
 [tool.isort]
 default_section = "THIRDPARTY"
 force_single_line = true
 line_length = 99
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 skip_glob = ["**/.env*", "**/env/*", "**/.venv/*", "**/docs/*"]
 
 [tool.pytest.ini_options]
-addopts = "dockerautotag --cov=dockerautotag --cov-report=xml:coverage.xml --cov-report=term --cov-append --no-cov-on-fail"
+addopts = "dockerautotag --cov=dockerautotag --cov-report=xml:coverage.xml --cov-report=term --no-cov-on-fail"
 filterwarnings = [
   "ignore::FutureWarning",
-  "ignore:.*collections.*:DeprecationWarning",
+  "ignore::DeprecationWarning",
   "ignore:.*pep8.*:FutureWarning",
 ]
 
 [tool.coverage.run]
 omit = ["**/test/*"]
 
 [build-system]
```

### Comparing `docker_autotag-1.2.8/PKG-INFO` & `docker_autotag-1.2.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-autotag
-Version: 1.2.8
+Version: 1.2.9
 Summary: Creates a list of docker tags from a given version string.
 Home-page: https://github.com/thegeeklab/docker-autotag/
 License: MIT
 Keywords: docker,versioning,automation,ci
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.7.0,<4.0.0
@@ -18,20 +18,14 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: python-json-logger (==2.0.7)
 Requires-Dist: semantic-version (==2.10.0)
 Project-URL: Documentation, https://github.com/thegeeklab/docker-autotag/
 Project-URL: Repository, https://github.com/thegeeklab/docker-autotag/
```

