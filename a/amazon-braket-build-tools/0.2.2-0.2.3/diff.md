# Comparing `tmp/amazon-braket-build-tools-0.2.2.tar.gz` & `tmp/amazon-braket-build-tools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-build-tools-0.2.2.tar", last modified: Tue May 23 16:06:24 2023, max compression
+gzip compressed data, was "amazon-braket-build-tools-0.2.3.tar", last modified: Mon May 29 16:04:11 2023, max compression
```

## Comparing `amazon-braket-build-tools-0.2.2.tar` & `amazon-braket-build-tools-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.759700 amazon-braket-build-tools-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-23 16:06:24.759700 amazon-braket-build-tools-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 16:06:24.759700 amazon-braket-build-tools-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 16:06:24.000000 amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/braket/_build_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/src/braket/_build_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:06:24.755700 amazon-braket-build-tools-0.2.2/src/braket/flake8_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-05-23 16:06:15.000000 amazon-braket-build-tools-0.2.2/src/braket/flake8_plugins/braket_checkstyle_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.720320 amazon-braket-build-tools-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.720320 amazon-braket-build-tools-0.2.3/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/src/braket/_build_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/src/braket/_build_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/src/braket/flake8_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/src/braket/flake8_plugins/braket_checkstyle_plugin.py
```

### Comparing `amazon-braket-build-tools-0.2.2/LICENSE` & `amazon-braket-build-tools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.2/PKG-INFO` & `amazon-braket-build-tools-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-build-tools
-Version: 0.2.2
+Version: 0.2.3
 Summary: A set of build tools for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-build-tools
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-build-tools-0.2.2/README.md` & `amazon-braket-build-tools-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.2/setup.cfg` & `amazon-braket-build-tools-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.2/setup.py` & `amazon-braket-build-tools-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.2/src/amazon_braket_build_tools.egg-info/PKG-INFO` & `amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-build-tools
-Version: 0.2.2
+Version: 0.2.3
 Summary: A set of build tools for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-build-tools
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-build-tools-0.2.2/src/braket/_build_tools/_version.py` & `amazon-braket-build-tools-0.2.3/src/braket/_build_tools/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # language governing permissions and limitations under the License.
 
 """Version information.
 
 Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
```

### Comparing `amazon-braket-build-tools-0.2.2/src/braket/flake8_plugins/braket_checkstyle_plugin.py` & `amazon-braket-build-tools-0.2.3/src/braket/flake8_plugins/braket_checkstyle_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,32 +34,33 @@
     This is the context object for parsing the function definition. We record all the information
     we need about the function and the current state of parsing.
     """
 
     found_args: bool = False
     found_return: bool = False
     found_description: bool = False
+    in_sub_list: bool = False
     current_section: DocSection = DocSection.DESCRIPTION
     current_arg: int = 0
     found_arg_list: Set = None
     args_indent: int = 0
     return_indent: int = 0
     invalid_indents: int = 0
     first_invalid_indent_line: str = None
 
 
 class _Visitor(ast.NodeVisitor):
     ARGS_REGEX = re.compile(r"^(\s*)Args\s*:\s*$")
     RETURN_REGEX = re.compile(r"^(\s*)(Returns|Yields)\s*:\s*$")
     MISC_REGEX = re.compile(
-        r"^(\s*)(Throws|Raises|See Also|Note|Example|Examples|Warnings)\s*:\s*$"
+        r"^(\s*)(Throws|Raises|See Also|Note|Example|Examples|Warnings)( \(.+\))?:\s*$"
     )
-    ARG_INFO_REGEX = re.compile(r"^(\s*)(`?\*{0,2}\w*`?)\s*(\([^:]*\))?\s*:\s*(.*)")
+    ARG_INFO_REGEX = re.compile(r"^(\s*)`{0,2}(\*{0,2}\w*)`{0,2}\s*(\([^:]*\))?\s*:\s*(.*)")
     RETURN_INFO_REGEX = re.compile(r"^(\s*)([^:]*)\s*(:)?\s*(.*)")
-    INDENT_REGEX = re.compile(r"^(\s*)\S+.*")
+    INDENT_REGEX = re.compile(r"^(\s*)(\S+.*)")
     RESERVED_ARGS = {"self", "cls"}
 
     MESSAGES = {
         "BCS001": "Argument '%s' is missing a type hint.",
         "BCS002": "Function '%s' is missing a type hint for the return value.",
         "BCS003": "Function '%s' is missing documentation.",
         "BCS004": "Argument '%s' documentation is missing the type hint.",
@@ -170,31 +171,30 @@
     def _check_doc_section(self, doc_line: str, context: DocContext, node: ast.FunctionDef) -> None:
         if context.current_section == DocSection.DESCRIPTION:
             if len(doc_line.strip()) > 1:
                 context.found_description = True
         elif context.current_section == DocSection.ARGUMENTS:
             matches = self.ARG_INFO_REGEX.match(doc_line)
             if matches:
+                context.in_sub_list = False
                 self._check_argument_info(matches, context, node)
             else:
                 self._check_indent(context.args_indent + 4, doc_line, context)
         elif context.current_section == DocSection.RETURN_FIRST_LINE:
             matches = self.RETURN_INFO_REGEX.match(doc_line)
             self._check_return_info(matches, context, node)
+            context.in_sub_list = False
             context.current_section = DocSection.RETURN_REST
         elif context.current_section == DocSection.RETURN_REST:
             self._check_indent(context.return_indent, doc_line, context)
 
     def _check_argument_info(
         self, regex_matches: re.Match, context: DocContext, node: ast.FunctionDef
     ) -> None:
-        arg_indent = regex_matches.group(1)
-        arg_name = regex_matches.group(2).strip("`") if regex_matches.group(2) else None
-        arg_type = regex_matches.group(3) if regex_matches.group(3) else None
-        arg_description = regex_matches.group(4)
+        arg_indent, arg_name, arg_type, arg_description = regex_matches.groups()
         arg_index = _get_argument_with_name(arg_name, node)
         self._check_argument_indent(arg_indent, arg_name, arg_index, context, node)
         if arg_index is None:
             return
         self._check_argument_docs(arg_name, arg_type, arg_description, arg_index, context, node)
         context.current_arg = arg_index + 1
 
@@ -353,17 +353,23 @@
             if args.arg not in self.RESERVED_ARGS:
                 return True
         return False
 
     def _check_indent(self, expected_indent: int, line: str, context: DocContext) -> None:
         match = self.INDENT_REGEX.match(line)
         if match:
-            indent = match.groups()[0]
-            if indent is not None and len(indent) != expected_indent:
-                _invalid_indent_found(line, context)
+            groups = match.groups()
+            indent = groups[0]
+            text = groups[1]
+            ind_len = len(indent)
+            if indent is not None and ind_len != expected_indent:
+                if text.startswith("-") and ind_len in [expected_indent - 2, expected_indent + 2]:
+                    context.in_sub_list = True
+                elif not context.in_sub_list:
+                    _invalid_indent_found(line, context)
 
 
 class BraketCheckstylePlugin:
     name = __name__
     version = build_tools_version.__version__
     off_by_default = True
```

