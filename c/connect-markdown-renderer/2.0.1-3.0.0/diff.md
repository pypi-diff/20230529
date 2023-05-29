# Comparing `tmp/connect-markdown-renderer-2.0.1.tar.gz` & `tmp/connect_markdown_renderer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect-markdown-renderer-2.0.1.tar", max compression
+gzip compressed data, was "connect_markdown_renderer-3.0.0.tar", max compression
```

## Comparing `connect-markdown-renderer-2.0.1.tar` & `connect_markdown_renderer-3.0.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2022-05-17 10:20:13.762820 connect-markdown-renderer-2.0.1/LICENSE
--rw-r--r--   0        0        0     2370 2022-05-17 10:20:13.762820 connect-markdown-renderer-2.0.1/README.md
--rw-r--r--   0        0        0       59 2022-05-17 10:20:13.762820 connect-markdown-renderer-2.0.1/cmr/__init__.py
--rw-r--r--   0        0        0      428 2022-05-17 10:20:13.762820 connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/__init__.py
--rw-r--r--   0        0        0     3574 2022-05-17 10:20:13.762820 connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/components.py
--rw-r--r--   0        0        0     1929 2022-05-17 10:20:13.762820 connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/emoji.py
--rw-r--r--   0        0        0     2034 2022-05-17 10:20:13.762820 connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/node.py
--rw-r--r--   0        0        0     5375 2022-05-17 10:20:13.762820 connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/renderer.py
--rw-r--r--   0        0        0      831 2022-05-17 10:20:13.762820 connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/theme.py
--rw-r--r--   0        0        0     1411 2022-05-17 10:21:01.531317 connect-markdown-renderer-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3172 2022-05-17 10:21:02.084550 connect-markdown-renderer-2.0.1/setup.py
--rw-r--r--   0        0        0     3182 2022-05-17 10:21:02.084941 connect-markdown-renderer-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-29 15:30:08.264581 connect_markdown_renderer-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2370 2023-05-29 15:30:08.264581 connect_markdown_renderer-3.0.0/README.md
+-rw-r--r--   0        0        0       59 2023-05-29 15:30:08.264581 connect_markdown_renderer-3.0.0/cmr/__init__.py
+-rw-r--r--   0        0        0      428 2023-05-29 15:30:08.264581 connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/__init__.py
+-rw-r--r--   0        0        0     3574 2023-05-29 15:30:08.264581 connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/components.py
+-rw-r--r--   0        0        0     1929 2023-05-29 15:30:08.264581 connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/emoji.py
+-rw-r--r--   0        0        0     2034 2023-05-29 15:30:08.264581 connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/node.py
+-rw-r--r--   0        0        0     5375 2023-05-29 15:30:08.264581 connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/renderer.py
+-rw-r--r--   0        0        0      831 2023-05-29 15:30:08.264581 connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/theme.py
+-rw-r--r--   0        0        0     2073 2023-05-29 15:30:31.661360 connect_markdown_renderer-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3179 1970-01-01 00:00:00.000000 connect_markdown_renderer-3.0.0/PKG-INFO
```

### Comparing `connect-markdown-renderer-2.0.1/LICENSE` & `connect_markdown_renderer-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connect-markdown-renderer-2.0.1/README.md` & `connect_markdown_renderer-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/components.py` & `connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/components.py`

 * *Files identical despite different names*

### Comparing `connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/emoji.py` & `connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/emoji.py`

 * *Files identical despite different names*

### Comparing `connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/node.py` & `connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/node.py`

 * *Files identical despite different names*

### Comparing `connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/renderer.py` & `connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/renderer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+from markdown_it import MarkdownIt
 from rich.emoji import Emoji, NoEmoji
 from rich.markdown import (
     BlockQuote,
     CodeBlock,
     HorizontalRule,
     ImageItem,
     ListElement,
     MarkdownContext,
     Paragraph,
     UnknownElement,
 )
 from rich.segment import Segment
 from rich.style import Style
-from markdown_it import MarkdownIt
 
 from connect.utils.terminal.markdown.components import (
     Heading,
     Link,
     ListItem,
     TableCellElement,
     TableElement,
```

### Comparing `connect-markdown-renderer-2.0.1/connect/utils/terminal/markdown/theme.py` & `connect_markdown_renderer-3.0.0/connect/utils/terminal/markdown/theme.py`

 * *Files identical despite different names*

### Comparing `connect-markdown-renderer-2.0.1/pyproject.toml` & `connect_markdown_renderer-3.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 [tool.poetry]
 name = "connect-markdown-renderer"
-version = "2.0.1"
+version = "3.0.0"
 description = "Connect Markdown Renderer"
 authors = ["CloudBlue"]
 license = "Apache-2.0"
 packages = [
     { include = "connect" },
     { include = "cmr" }
 ]
 readme = "./README.md"
 documentation = "https://github.com/cloudblue/connect-markdown-renderer"
 homepage = "https://connect.cloudblue.com"
 repository = "https://github.com/cloudblue/connect-markdown-renderer"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4"
-rich = "^12.4.1"
-markdown-it-py = "^2.1.0"
-
-[tool.poetry.dev-dependencies]
-pytest = "^6.1.2"
-pytest-cov = "^2.10.1"
-pytest-mock = "^3.3.1"
-coverage = {extras = ["toml"], version = "^5.3"}
-flake8 = "~3.8"
-flake8-bugbear = "~20"
+python = ">=3.8,<4"
+rich = ">=12.4.4,<13"
+markdown-it-py = "^2.2.0"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3"
+pytest-cov = "^4.1"
+pytest-mock = "^3.10"
+coverage = {extras = ["toml"], version = "^7.2"}
+flake8 = ">=3.8,<6"
+flake8-bugbear = "~22"
 flake8-cognitive-complexity = "^0.1"
-flake8-commas = "~2.0"
+flake8-commas = "^2.1.0"
 flake8-future-import = "~0.4"
-flake8-import-order = "~0.18"
-flake8-broken-line = "~0.3"
+flake8-broken-line = "~0.6"
+flake8-isort = "^6.0.0"
+flake8-pyproject = "^1.2.3"
+
+[tool.poetry.group.docs.dependencies]
 Sphinx = "^4.5.0"
 sphinx-copybutton = "^0.5.0"
 m2r2 = "^0.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools>=42"]
 build-backend = "poetry.core.masonry.api"
@@ -51,8 +54,39 @@
 
 exclude_lines = [
     "pragma: no cover",
     "def __str__",
     "def __repr__",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
-]
+]
+
+[tool.isort]
+src_paths = "*"
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
+group_by_package = true
+multi_line_output = 3
+force_grid_wrap = 4
+combine_as_imports = true
+use_parentheses = true
+include_trailing_comma = true
+line_length = 100
+lines_after_imports = 2
+
+[tool.flake8]
+exclude = [
+    ".idea",
+    ".vscode",
+    ".git",
+    "pg_data",
+    "venv",
+    "*.eggs",
+    "*.egg",
+    "tests/fixtures",
+    "setup.py",
+    "resources",
+    "docs/*",
+]
+show-source = true
+max-line-length = 100
+max-cognitive-complexity = 20
+ignore = ["FI1", "I100", "W503"]
```

### Comparing `connect-markdown-renderer-2.0.1/PKG-INFO` & `connect_markdown_renderer-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: connect-markdown-renderer
-Version: 2.0.1
+Version: 3.0.0
 Summary: Connect Markdown Renderer
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Author: CloudBlue
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: markdown-it-py (>=2.1.0,<3.0.0)
-Requires-Dist: rich (>=12.4.1,<13.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: markdown-it-py (>=2.2.0,<3.0.0)
+Requires-Dist: rich (>=12.4.4,<13)
 Project-URL: Documentation, https://github.com/cloudblue/connect-markdown-renderer
 Project-URL: Repository, https://github.com/cloudblue/connect-markdown-renderer
 Description-Content-Type: text/markdown
 
 # CloudBlue Connect Markdown Renderer
```

