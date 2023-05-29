# Comparing `tmp/git_batch-2.0.8.tar.gz` & `tmp/git_batch-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_batch-2.0.8.tar", max compression
+gzip compressed data, was "git_batch-2.0.9.tar", max compression
```

## Comparing `git_batch-2.0.8.tar` & `git_batch-2.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1123 2022-11-25 12:22:03.292616 git_batch-2.0.8/LICENSE
--rw-r--r--   0        0        0     1768 2022-11-25 12:22:03.292616 git_batch-2.0.8/README.md
--rw-r--r--   0        0        0       46 2022-11-25 12:22:45.717800 git_batch-2.0.8/gitbatch/__init__.py
--rw-r--r--   0        0        0     6650 2022-11-25 12:22:03.292616 git_batch-2.0.8/gitbatch/cli.py
--rw-r--r--   0        0        0     5820 2022-11-25 12:22:03.292616 git_batch-2.0.8/gitbatch/logging.py
--rw-r--r--   0        0        0      568 2022-11-25 12:22:03.292616 git_batch-2.0.8/gitbatch/utils.py
--rw-r--r--   0        0        0     2541 2022-11-25 12:22:45.717800 git_batch-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 git_batch-2.0.8/setup.py
--rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 git_batch-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-02-12 13:58:47.166700 git_batch-2.0.9/LICENSE
+-rw-r--r--   0        0        0     1768 2023-02-12 13:58:47.170699 git_batch-2.0.9/README.md
+-rw-r--r--   0        0        0       46 2023-02-12 13:59:06.654632 git_batch-2.0.9/gitbatch/__init__.py
+-rw-r--r--   0        0        0     6554 2023-02-12 13:58:47.170699 git_batch-2.0.9/gitbatch/cli.py
+-rw-r--r--   0        0        0     5766 2023-02-12 13:58:47.170699 git_batch-2.0.9/gitbatch/logging.py
+-rw-r--r--   0        0        0      571 2023-02-12 13:58:47.170699 git_batch-2.0.9/gitbatch/utils.py
+-rw-r--r--   0        0        0     3326 2023-02-12 13:59:06.650632 git_batch-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 git_batch-2.0.9/setup.py
+-rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 git_batch-2.0.9/PKG-INFO
```

### Comparing `git_batch-2.0.8/LICENSE` & `git_batch-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `git_batch-2.0.8/README.md` & `git_batch-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `git_batch-2.0.8/gitbatch/cli.py` & `git_batch-2.0.9/gitbatch/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 from pathlib import Path
 from urllib.parse import urlparse
 
 import git
 
 from gitbatch import __version__
 from gitbatch.logging import SingleLog
-from gitbatch.utils import normalize_path
-from gitbatch.utils import to_bool
+from gitbatch.utils import normalize_path, to_bool
 
 
 class GitBatch:
     """Handles git operations."""
 
     def __init__(self):
         self.log = SingleLog()
@@ -27,17 +26,15 @@
         self.config = self._config()
         self.run()
 
     def _cli_args(self):
         parser = argparse.ArgumentParser(
             description=("Clone single branch from all repositories listed in a file")
         )
-        parser.add_argument(
-            "--version", action="version", version="%(prog)s {}".format(__version__)
-        )
+        parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
         parser.add_argument(
             "-v", dest="logging.level", action="append_const", const=-1, help="increase log level"
         )
         parser.add_argument(
             "-q", dest="logging.level", action="append_const", const=1, help="decrease log level"
         )
 
@@ -61,22 +58,22 @@
         config["ignore_existing"] = to_bool(os.environ.get("GIT_BATCH_IGNORE_EXISTING", True))
         config["ignore_missing"] = to_bool(os.environ.get("GIT_BATCH_IGNORE_MISSING_REMOTE", True))
 
         return config
 
     def _repos_from_file(self, src):
         repos = []
-        with open(src, "r") as f:
+        with open(src) as f:
             for num, line in enumerate(f, start=1):
                 repo = {}
                 line = line.strip()
                 if line and not line.startswith("#"):
                     try:
-                        url, src, dest = [x.strip() for x in line.split(";")]
-                        branch, *_ = [x.strip() for x in src.split(":")]
+                        url, src, dest = (x.strip() for x in line.split(";"))
+                        branch, *_ = (x.strip() for x in src.split(":"))
 
                         path = None
                         if len(_) > 0:
                             path = Path(_[0])
                             path = path.relative_to(path.anchor)
 
                     except ValueError as e:
@@ -96,17 +93,15 @@
                         repo["rel_dest"] = dest
                         repo["dest"] = normalize_path(dest) or normalize_path(
                             "./{}".format(repo["name"])
                         )
 
                         repos.append(repo)
                     else:
-                        self.log.sysexit_with_message(
-                            "Repository Url is not set on line {line_num}".format(line_num=num)
-                        )
+                        self.log.sysexit_with_message(f"Repository Url is not set on line {num}")
         return repos
 
     def _repos_clone(self, repos):
         for repo in repos:
             with tempfile.TemporaryDirectory(prefix="gitbatch_") as tmp:
                 try:
                     options = ["--branch={}".format(repo["branch"]), "--single-branch"]
@@ -116,17 +111,19 @@
                     skip = False
                     err_raw = e.stderr.strip().splitlines()[:-1]
                     err = [
                         x.split(":", 1)[1].strip().replace(repo["dest"], repo["rel_dest"])
                         for x in err_raw
                     ]
 
-                    if any(["could not find remote branch" in item for item in err]):
-                        if self.config["ignore_missing"]:
-                            skip = True
+                    if (
+                        any(["could not find remote branch" in item for item in err])
+                        and self.config["ignore_missing"]
+                    ):
+                        skip = True
                     if not skip:
                         self.log.sysexit_with_message("Error: {}".format("\n".join(err)))
                 except FileExistsError:
                     self._file_exist_handler()
 
                 try:
                     path = tmp
```

### Comparing `git_batch-2.0.8/gitbatch/logging.py` & `git_batch-2.0.9/gitbatch/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import logging
 import os
 import sys
 
 import colorama
 from pythonjsonlogger import jsonlogger
 
-from gitbatch.utils import Singleton
-from gitbatch.utils import to_bool
+from gitbatch.utils import Singleton, to_bool
 
 CONSOLE_FORMAT = "{}[%(levelname)s]{} %(message)s"
 JSON_FORMAT = "%(asctime)s %(levelname)s %(message)s"
 
 
 def _should_do_markup():
     py_colors = os.environ.get("PY_COLORS", None)
@@ -22,15 +21,15 @@
 
     return sys.stdout.isatty() and os.environ.get("TERM") != "dumb"
 
 
 colorama.init(autoreset=True, strip=not _should_do_markup())
 
 
-class LogFilter(object):
+class LogFilter:
     """A custom log filter which excludes log messages above the logged level."""
 
     def __init__(self, level):
         """
         Initialize a new custom log filter.
 
         :param level: Log level limit
@@ -44,15 +43,15 @@
         return logRecord.levelno <= self.__level
 
 
 class MultilineFormatter(logging.Formatter):
     """Logging Formatter to reset color after newline characters."""
 
     def format(self, record):  # noqa
-        record.msg = record.msg.replace("\n", "\n{}... ".format(colorama.Style.RESET_ALL))
+        record.msg = record.msg.replace("\n", f"\n{colorama.Style.RESET_ALL}... ")
         return logging.Formatter.format(self, record)
 
 
 class MultilineJsonFormatter(jsonlogger.JsonFormatter):
     """Logging Formatter to remove newline characters."""
 
     def format(self, record):  # noqa
@@ -178,15 +177,15 @@
         Colorize strings.
 
         :param color: colorama color settings
         :param msg: string to colorize
         :returns: string
 
         """
-        return "{}{}{}".format(color, msg, colorama.Style.RESET_ALL)
+        return f"{color}{msg}{colorama.Style.RESET_ALL}"
 
     def sysexit(self, code=1):
         sys.exit(code)
 
     def sysexit_with_message(self, msg, code=1):
         self.logger.critical(str(msg))
         self.sysexit(code)
```

### Comparing `git_batch-2.0.8/gitbatch/utils.py` & `git_batch-2.0.9/gitbatch/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 from distutils.util import strtobool
 
 
 def normalize_path(path):
     if path:
         return os.path.abspath(os.path.expanduser(os.path.expandvars(path)))
 
+    return None
+
 
 def to_bool(string):
     return bool(strtobool(str(string)))
 
 
 class Singleton(type):
     """Meta singleton class."""
 
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
-            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
+            cls._instances[cls] = super().__call__(*args, **kwargs)
         return cls._instances[cls]
```

### Comparing `git_batch-2.0.8/pyproject.toml` & `git_batch-2.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -28,47 +28,33 @@
 license = "MIT"
 name = "git-batch"
 packages = [
   {include = "gitbatch"},
 ]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/git-batch/"
-version = "2.0.8"
+version = "2.0.9"
 
 [tool.poetry.dependencies]
-GitPython = "3.1.29"
+GitPython = "3.1.30"
 colorama = "0.4.6"
 python = "^3.7.0"
 python-json-logger = "2.0.4"
 
-[tool.poetry.dev-dependencies]
-bandit = "1.7.4"
-flake8 = "5.0.4"
-flake8-blind-except = "0.2.1"
-flake8-builtins = "2.0.1"
-flake8-docstrings = "1.6.0"
-flake8-eradicate = "1.4.0"
-flake8-isort = "5.0.3"
-flake8-logging-format = "0.8.1"
-flake8-pep3101 = "2.0.0"
-flake8-polyfill = "1.0.2"
-flake8-quotes = "3.3.1"
-pdoc3 = "0.10.0"
-pep8-naming = "0.13.2"
-pydocstyle = "6.1.1"
-pytest = "7.2.0"
-pytest-cov = "4.0.0"
-pytest-mock = "3.10.0"
-requests-mock = "1.10.0"
-yapf = "0.32.0"
-toml = "0.10.2"
-
 [tool.poetry.scripts]
 git-batch = "gitbatch.cli:main"
 
+[tool.poetry.group.dev.dependencies]
+ruff = "0.0.243"
+pytest = "7.2.1"
+pytest-mock = "3.10.0"
+pytest-cov = "4.0.0"
+toml = "0.10.2"
+yapf = "0.32.0"
+
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
 
 [tool.isort]
 default_section = "THIRDPARTY"
@@ -87,7 +73,73 @@
 
 [tool.coverage.run]
 omit = ["**/test/*"]
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+
+[tool.ruff]
+exclude = [
+    ".git",
+    "__pycache__",
+    "build",
+    "dist",
+    "test",
+    "*.pyc",
+    "*.egg-info",
+    ".cache",
+    ".eggs",
+    "env*",
+]
+# Explanation of errors
+#
+# D102: Missing docstring in public method
+# D103: Missing docstring in public function
+# D105: Missing docstring in magic method
+# D107: Missing docstring in __init__
+# D202: No blank lines allowed after function docstring
+# D203: One blank line required before class docstring
+# D212: Multi-line docstring summary should start at the first line
+ignore = [
+    "D102",
+    "D103",
+    "D105",
+    "D107",
+    "D202",
+    "D203",
+    "D212",
+]
+line-length = 99
+select = [
+    "D",
+    "E",
+    "F",
+    "Q",
+    "W",
+    "I",
+    "S",
+    "BLE",
+    "N",
+    "UP",
+    "B",
+    "A",
+    "C4",
+    "T20",
+    "SIM",
+    "RET",
+    "ARG",
+    "ERA",
+    "RUF",
+]
+
+[tool.ruff.flake8-quotes]
+inline-quotes = "double"
+
+[tool.yapf]
+based_on_style = "google"
+column_limit = 99
+dedent_closing_brackets = true
+coalesce_brackets = true
+split_before_logical_operator = true
+indent_dictionary_value = true
+allow_split_before_dict_value = false
```

### Comparing `git_batch-2.0.8/setup.py` & `git_batch-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['gitbatch']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['GitPython==3.1.29', 'colorama==0.4.6', 'python-json-logger==2.0.4']
+['GitPython==3.1.30', 'colorama==0.4.6', 'python-json-logger==2.0.4']
 
 entry_points = \
 {'console_scripts': ['git-batch = gitbatch.cli:main']}
 
 setup_kwargs = {
     'name': 'git-batch',
-    'version': '2.0.8',
+    'version': '2.0.9',
     'description': 'Clone single branch from all repositories listed in a file.',
     'long_description': '# git-batch\n\nAutomate cloning a single branch from a list of repositories\n\n[![Build Status](https://img.shields.io/drone/build/thegeeklab/git-batch?logo=drone&server=https%3A%2F%2Fdrone.thegeeklab.de)](https://drone.thegeeklab.de/thegeeklab/git-batch)\n[![Docker Hub](https://img.shields.io/badge/dockerhub-latest-blue.svg?logo=docker&logoColor=white)](https://hub.docker.com/r/thegeeklab/git-batch)\n[![Quay.io](https://img.shields.io/badge/quay-latest-blue.svg?logo=docker&logoColor=white)](https://quay.io/repository/thegeeklab/git-batch)\n[![Python Version](https://img.shields.io/pypi/pyversions/git-batch.svg)](https://pypi.org/project/git-batch/)\n[![PyPi Status](https://img.shields.io/pypi/status/git-batch.svg)](https://pypi.org/project/git-batch/)\n[![PyPi Release](https://img.shields.io/pypi/v/git-batch.svg)](https://pypi.org/project/git-batch/)\n[![GitHub contributors](https://img.shields.io/github/contributors/thegeeklab/git-batch)](https://github.com/thegeeklab/git-batch/graphs/contributors)\n[![Source: GitHub](https://img.shields.io/badge/source-github-blue.svg?logo=github&logoColor=white)](https://github.com/thegeeklab/git-batch)\n[![License: MIT](https://img.shields.io/github/license/thegeeklab/git-batch)](https://github.com/thegeeklab/git-batch/blob/main/LICENSE)\n\nSimple tool to automate cloning a single branch from a list of repositories.\n\n## Contributors\n\nSpecial thanks to all [contributors](https://github.com/thegeeklab/git-batch/graphs/contributors). If you would like to contribute,\nplease see the [instructions](https://github.com/thegeeklab/git-batch/blob/main/CONTRIBUTING.md).\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](https://github.com/thegeeklab/git-batch/blob/main/LICENSE) file for details.\n',
     'author': 'Robert Kaussow',
     'author_email': 'mail@thegeeklab.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/thegeeklab/git-batch/',
```

### Comparing `git_batch-2.0.8/PKG-INFO` & `git_batch-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-batch
-Version: 2.0.8
+Version: 2.0.9
 Summary: Clone single branch from all repositories listed in a file.
 Home-page: https://github.com/thegeeklab/git-batch/
 License: MIT
 Keywords: git,batch,automation
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.7.0,<4.0.0
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Dist: GitPython (==3.1.29)
+Requires-Dist: GitPython (==3.1.30)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: python-json-logger (==2.0.4)
 Project-URL: Documentation, https://github.com/thegeeklab/git-batch/
 Project-URL: Repository, https://github.com/thegeeklab/git-batch/
 Description-Content-Type: text/markdown
 
 # git-batch
```

