# Comparing `tmp/valgrind_codequality-1.1.0.tar.gz` & `tmp/valgrind_codequality-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valgrind_codequality-1.1.0.tar", max compression
+gzip compressed data, was "valgrind_codequality-1.2.0.tar", max compression
```

## Comparing `valgrind_codequality-1.1.0.tar` & `valgrind_codequality-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1105 2023-02-03 17:45:59.054645 valgrind_codequality-1.1.0/LICENSE
--rwxr-xr-x   0        0        0     3620 2023-02-19 15:08:29.098497 valgrind_codequality-1.1.0/README.md
--rwxr-xr-x   0        0        0     1616 2023-03-02 07:11:14.335223 valgrind_codequality-1.1.0/pyproject.toml
--rwxr-xr-x   0        0        0    11340 2023-03-02 07:11:14.352224 valgrind_codequality-1.1.0/valgrind_codequality/__init__.py
--rwxr-xr-x   0        0        0     4282 2023-03-02 07:11:14.360222 valgrind_codequality-1.1.0/valgrind_codequality/__main__.py
--rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 valgrind_codequality-1.1.0/setup.py
--rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 valgrind_codequality-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1105 2023-02-03 17:45:59.054645 valgrind_codequality-1.2.0/LICENSE
+-rwxr-xr-x   0        0        0     3526 2023-05-01 13:06:47.846935 valgrind_codequality-1.2.0/README.md
+-rwxr-xr-x   0        0        0     1617 2023-05-29 12:54:37.862882 valgrind_codequality-1.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0    13258 2023-05-29 12:54:37.880938 valgrind_codequality-1.2.0/valgrind_codequality/__init__.py
+-rwxr-xr-x   0        0        0     4535 2023-05-29 12:37:31.605726 valgrind_codequality-1.2.0/valgrind_codequality/__main__.py
+-rw-r--r--   0        0        0     4448 1970-01-01 00:00:00.000000 valgrind_codequality-1.2.0/setup.py
+-rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 valgrind_codequality-1.2.0/PKG-INFO
```

### Comparing `valgrind_codequality-1.1.0/LICENSE` & `valgrind_codequality-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valgrind_codequality-1.1.0/README.md` & `valgrind_codequality-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,22 +63,20 @@
   artifacts:
     reports:
       codequality: valgrind.json
 ```
 
 ### Contributing
 
-* Sign the contributor agreement (coming soon)
 * Format with [black](https://pypi.org/project/black/)
 * Check with [pylint](https://pypi.org/project/pylint/)
 
 ### Credits & Trademarks
 
 valgrind is an open-source project with a GPL v3.0 license.
-* http://valgrind.sourceforge.net
-* https://github.com/danmar/valgrind
+* https://valgrind.org/
 
 "GitLab" is a trademark of GitLab B.V.
 * https://gitlab.com
 * https://docs.gitlab.com/ee/user/project/merge_requests/code_quality.html
 
 All other trademarks belong to their respective owners.
```

### Comparing `valgrind_codequality-1.1.0/pyproject.toml` & `valgrind_codequality-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "valgrind-codequality"
-version = "1.1.0"
+version = "1.2.0"
 description = "Convert Valgrind XML to GitLab Code Quality JSON file."
 authors = ["Arnaud Moura <arnaudmoura@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "valgrind_codequality"}]
 
 [tool.poetry.urls]
@@ -48,11 +48,11 @@
 tox = ">=3.24.0"
 
 [tool.poetry.group.ci.dependencies]
 anybadge = "^1.0.0"
 pylint-exit = "^1.2.0"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 style = "semver"
 metadata = false
```

### Comparing `valgrind_codequality-1.1.0/valgrind_codequality/__init__.py` & `valgrind_codequality-1.2.0/valgrind_codequality/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,29 +27,29 @@
 import os
 import typing
 from copy import deepcopy
 
 # third-party
 import xmltodict
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 log = logging.getLogger(__name__)
 
 # Source: https://github.com/codeclimate/platform/blob/master/spec/analyzers/SPEC.md#data-types
 CODE_QUAL_ELEMENT = {
     "severity": "",
     "description": "",
     "fingerprint": "",
     "location": {"path": "", "lines": {"begin": -1}},
 }
 
 
 def _get_codeclimate_severity(valgrind_severity: str) -> str:
-    """Get Code Climate severity, from valgrind severity string
+    """Get Code Climate severity, from valgrind severity string.
 
     CodeQuality: info, minor, major, critical, blocker
     """
     severity = ""
     if "Leak_DefinitelyLost" == valgrind_severity:
         severity = "blocker"
     else:
@@ -84,28 +84,31 @@
 
 def convert_file(
     fname_in: str,
     fname_out: str,
     base_dirs: typing.List[str],
     file_concat: typing.Optional[str] = None,
     relative_dir: typing.Optional[str] = None,
+    exclude_list: typing.Optional[typing.List[str]] = None,
 ) -> int:
-    """Convert valgrind XML file to GitLab-compatible "Code Quality" JSON report
+    """Convert valgrind XML file to GitLab-compatible "Code Quality" JSON report.
 
     Args:
         fname_in (str):
           Input file path (valgrind XML). Like 'valgrind.xml'.
         fname_out (str):
           Output file path (code quality JSON). Like 'valgrind.json'.
         base_dirs (list):
           Base directories where source files with relative paths can be found.
         file_concat (str):
           File path (JSON) contains code quality informations from previous analyze.
         relative_dir (str):
           Absolute path to change absolute path to relative from this path.
+        exclude_list (list):
+          Folders name to exclude leaks from a folder containing these names.
 
     Returns:
         int: If processing failed, a negative value. If successful, number of
           valgrind issues processed.
     """
     fin = None
     dict_concat = None
@@ -136,14 +139,15 @@
     log.debug("Reading input file: %s", fname_in)
     with open(fname_in, mode="rt", encoding="utf-8", errors="backslashreplace") as fin:
         json_out_str, num_cq_issues_converted = _convert(
             fin.read(),
             base_dirs=base_dirs,
             relative_dir=relative_dir,
             dict_concat=dict_concat,
+            exclude_list=exclude_list,
         )
 
     log.debug("Writing output file: %s", fname_out)
     with open(fname_out, "w", encoding="utf-8") as f_out:
         f_out.write(json_out_str)
 
     return num_cq_issues_converted
@@ -172,17 +176,15 @@
     max_line_cnt = 0
     if line_number <= 0:
         return str(filename) + "<the whole file>"
 
     filename = os.path.abspath(filename)
     if not os.path.isfile(filename):
         raise FileNotFoundError(
-            "Source code file does not exist or cannot be opened. Missing a base directory?\n--> '{}'".format(
-                filename
-            )
+            f"Source code file does not exist or cannot be opened. Missing a base directory?\n--> '{filename}'"
         )
 
     with open(filename, mode="rt", encoding="utf-8", errors="backslashreplace") as fin:
         for i, line in enumerate(fin):
             if (i + 1) == line_number:
                 # log.debug("Extracted line %s:%d", filename, line_number)
                 return line
@@ -190,24 +192,25 @@
 
     log.warning(
         "Only %d lines in file. Can't read line %d from '%s'",
         max_line_cnt,
         line_number,
         filename,
     )
-    return "Can't read line {} from a {} line file".format(line_number, max_line_cnt)
+    return f"Can't read line {line_number} from a {max_line_cnt} line file"
 
 
 def _convert(
-    xml_input,
+    xml_input: str,
     base_dirs: typing.List[str],
     relative_dir: typing.Optional[str] = None,
     dict_concat: typing.Optional[typing.Dict[str, str]] = None,
+    exclude_list: typing.Optional[typing.List[str]] = None,
 ) -> typing.Tuple[str, int]:
-    """Convert valgrind XML to Code Climate JSON
+    """Convert valgrind XML to Code Climate JSON.
 
     Note:
         There isn't a great 1:1 conversion from valgrind's "severity" level, to
         the Code Climate's "categories." To prevent information loss, the
         original valgrind severity is appended to the category list.
 
         In the future, maybe this conversion can be made using valgrind's "id"
@@ -215,15 +218,18 @@
 
     Args:
         xml_input (str): Filename of the XML from valgrind
         base_dirs (list):
           Base directories where source files with relative paths can be found.
         relative_dir (str):
           Absolute path to change absolute path to relative from this path.
-        dict_concat: dictionnary contains code quality informations from previous analyze.
+        dict_concat:
+          Dictionnary contains code quality informations from previous analyze.
+        exclude_list (list):
+          Folders name to exclude leaks from a folder containing these names.
 
     Returns:
         Tuple, where the first element, a string, is the JSON conversion result
         and the second element, an int, is the number of issues converted.
     """
 
     dict_in = xmltodict.parse(xml_input=xml_input)
@@ -260,43 +266,21 @@
             log.info("No stack. Skipping the below issue:\n  %s", error["unique"])
             continue
 
         # Extract frames
         stacks = error["stack"]
         if not type(stacks) is list:
             stacks = [stacks]
+        if stacks[0] == None:
+            log.info("No frames. Skipping the below issue:\n  %s", error["unique"])
+            continue
+        (tmp_dict, kind) = _extract_frames(error)
 
-        tmp_dict = dict(CODE_QUAL_ELEMENT)
-        kind = error["kind"]
-        if "xwhat" in error:
-            tmp_dict["description"] = error["xwhat"]["text"]
-        else:
-            tmp_dict["description"] = error["what"]
-
-        tmp_dict["description"] = kind + ": " + tmp_dict["description"]
-        tmp_dict["severity"] = _get_codeclimate_severity(kind)
-
-        path = ""
-        line = -1
-        for index in range(len(stacks[0]["frame"])):
-            frame = stacks[0]["frame"][index]
-            log.debug("- Analyse frames -- %s", str(frame["ip"]))
-            if "dir" in frame and "file" in frame:
-                line = int(frame["line"])
-
-                # Check in base dirs
-                for d in base_dirs:
-                    if d in frame["dir"]:
-                        path = os.path.join(frame["dir"], frame["file"])
-                        break
-
-                if path == "":
-                    continue
-                else:
-                    break
+        # Extract error
+        (path, line) = _extract_error(stacks, base_dirs, exclude_list)
 
         # Path found
         if path != "":
             if relative_dir:
                 tmp_dict["location"]["path"] = os.path.relpath(path, relative_dir)
             else:
                 tmp_dict["location"]["path"] = path
@@ -328,14 +312,90 @@
                 fingerprints.append(fingerprint_str)
 
     if len(dict_out) == 0:
         log.warning("Result is empty")
     return (json.dumps(dict_out, indent=4), len(dict_out))
 
 
+def _extract_frames(error: dict):
+    """Extract frames from error.
+
+    Args:
+        error (str): Error where extract frames.
+
+    Returns:
+        Tuple, where the firs element, dictionary, with description and severity,
+        and the second element, an string, is the kind of error.
+    """
+    tmp_dict = dict(CODE_QUAL_ELEMENT)
+    kind = error["kind"]
+    if "xwhat" in error:
+        tmp_dict["description"] = error["xwhat"]["text"]
+    else:
+        tmp_dict["description"] = error["what"]
+
+    tmp_dict["description"] = kind + ": " + tmp_dict["description"]
+    tmp_dict["severity"] = _get_codeclimate_severity(kind)
+
+    return (tmp_dict, kind)
+
+
+def _extract_error(
+    stacks: list,
+    base_dirs: typing.List[str],
+    exclude_list: typing.Optional[typing.List[str]] = None,
+):
+    """Extract line and file path from error.
+
+    Args:
+        error (str): Error where extract line and path.
+
+    Returns:
+        Tuple, where the key element, a string, is the path
+        and the second element, an string, is the line.
+    """
+    line = -1
+    path = ""
+    for index in range(len(stacks[0]["frame"])):
+        frame = stacks[0]["frame"][index]
+        log.debug("- Analyse frames -- %s", str(frame["ip"]))
+
+        # Check if path in "obj" contains name to exclude
+        exclude_error = False
+        if exclude_list:
+            path_name = ""
+            path_analyse = ""
+            for path_name in exclude_list:
+                path_analyse = frame["obj"]
+                if path_name in path_analyse:
+                    exclude_error = True
+                if "dir" in frame:
+                    path_analyse = frame["dir"]
+                    if path_name in path_analyse:
+                        exclude_error = True
+            if exclude_error:
+                log.debug(f"- Exclude because '{path_name}' in {path_analyse}")
+                break
+
+        # Get line
+        if "dir" in frame and "file" in frame:
+            line = int(frame["line"])
+
+            # Check in base dirs
+            for d in base_dirs:
+                if d in frame["dir"]:
+                    path = os.path.join(frame["dir"], frame["file"])
+                    break
+
+            if path == "":
+                continue
+            break
+    return (path, line)
+
+
 if __name__ == "__main__":
     import warnings
 
     warnings.warn(
         "use 'python3 -m valgrind_codequality', not 'python3 -m valgrind_codequality.__init__'",
         DeprecationWarning,
     )
```

### Comparing `valgrind_codequality-1.1.0/valgrind_codequality/__main__.py` & `valgrind_codequality-1.2.0/valgrind_codequality/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,15 @@
         logging.getLogger("").addHandler(h_file)
 
 
 def _get_args() -> argparse.Namespace:
     """Parse CLI args with argparse"""
     # Make parser object
     parser = argparse.ArgumentParser(
-        description=__doc__,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter
     )
 
     parser.add_argument(
         "-i",
         "--input-file",
         metavar="INPUT_XML_FILE",
         dest="input_file",
@@ -95,29 +94,38 @@
         action="store_true",
         help="print version and exit",
     )
 
     parser.add_argument(
         "-b",
         "--base-dirs",
-        metavar="base_dirs",
+        metavar="BASE_DIRS",
         action="append",
         default=[],
         help="base directories where source code files can be found. (default: '%(default)s')",
     )
 
     parser.add_argument(
         "-r",
         "--relative-dir",
         metavar="RELATIVE_DIR",
         type=str,
         default=os.getcwd(),
         help="change absolute path to relative from this path. (default: '%(default)s')",
     )
 
+    parser.add_argument(
+        "-e",
+        "--exclude-dir",
+        metavar="EXCLUDE_NAME",
+        nargs="+",
+        type=str,
+        help="folders name to exclude leaks from a folder containing these names",
+    )
+
     return parser.parse_args()
 
 
 def main() -> int:
     """Convert a valgrind XML file to Code Climate JSON file, at the command line."""
 
     if sys.version_info < (3, 6, 0):
@@ -135,14 +143,15 @@
 
     ret = convert_file(
         fname_in=args.input_file,
         fname_out=args.output_file,
         file_concat=args.concatenate,
         base_dirs=[os.getcwd()] if len(args.base_dirs) == 0 else args.base_dirs,
         relative_dir=args.relative_dir,
+        exclude_list=args.exclude_dir,
     )
     if ret < 0:
         m_log.error("Conversion failed")
         return 1
 
     # Logging the total count.
     # Side note: In personal projects, I intent to `cat` the log file and extract
```

### Comparing `valgrind_codequality-1.1.0/setup.py` & `valgrind_codequality-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['valgrind-codequality = '
                      'valgrind_codequality.__main__:main']}
 
 setup_kwargs = {
     'name': 'valgrind-codequality',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': 'Convert Valgrind XML to GitLab Code Quality JSON file.',
-    'long_description': '# valgrind-codequality\n\n[![badge-pypi](https://img.shields.io/pypi/v/valgrind-codequality.svg?logo=pypi)](https://pypi.python.org/pypi/valgrind-codequality/)\n&nbsp;\n[![badge-pypi-downloads](https://img.shields.io/pypi/dm/valgrind-codequality)](https://pypi.org/project/valgrind-codequality/)\n\n\n[![badge-pipeline](https://gitlab.com/echopouet/valgrind-codequality/badges/main/pipeline.svg)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-coverage](https://gitlab.com/echopouet/valgrind-codequality/badges/main/coverage.svg)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-pylint](https://gitlab.com/echopouet/valgrind-codequality/-/jobs/artifacts/main/raw/badge.svg?job=pylint)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-formatting](https://gitlab.com/echopouet/valgrind-codequality/-/jobs/artifacts/main/raw/badge.svg?job=format_black)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-issues-cnt](https://img.shields.io/badge/dynamic/json?label=issues&query=statistics.counts.opened&url=https%3A%2F%2Fgitlab.com%2Fapi%2Fv4%2Fprojects%2F19114200%2Fissues_statistics%3Fscope%3Dall)](https://gitlab.com/echopouet/valgrind-codequality/-/issues)\n\n\n## About\n\nI wanted reports from [Valgrind](https://valgrind.org/) to appear in GitLab Merge Requests as [Code Quality reports](https://docs.gitlab.com/ee/user/project/merge_requests/code_quality.html#implementing-a-custom-tool), which is a JSON file defined by the Code Quality\'s GitLab.\n\nThat\'s all this does: convert Valgrind XML report to Code Quality JSON.\n\nContributions are welcome.\n\n[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/EchoPouet)\n\n### Usage\n\nIt is primarily used as a console script. As such, ensure you have Python 3\'s "scripts" directory in your `PATH` variable.\nFor example, on Linux, that might be `$HOME/.local/bin`.\n\nTo test, try the `--help` or `--version` flags:\n```bash\nvalgrind-codequality --help\n```\n\nThis script follows that example and provides similar command-line options.\nA typical workflow might look like this:\n\n```bash\n# Generate valgrind report as XML\nvalgrind --tool=memcheck --leak-check=full --show-leak-kinds=all --track-origins=yes --verbose --xml=yes --xml-file=valgrind_out.xml your_exe\n# Convert to a Code Climate JSON report\nvalgrind-codequality --input-file valgrind_out.xml --output-file valgrind.json\n```\n\nIf you wanted, you could invoke the script directly as a module, like this:\n\n```bash\n# Run as a module instead (note the underscore in the module name here)\npython -m valgrind_codequality --input-file=valgrind_out.xml --output-file=valgrind.json\n```\n\nNow, in your GitLab CI script, [upload this file](https://docs.gitlab.com/ee/ci/pipelines/job_artifacts.html#artifactsreportscodequality)\nas a Code Quality report.\n\n```yaml\nmy-code-quality:\n  script:\n    - [...]\n  artifacts:\n    reports:\n      codequality: valgrind.json\n```\n\n### Contributing\n\n* Sign the contributor agreement (coming soon)\n* Format with [black](https://pypi.org/project/black/)\n* Check with [pylint](https://pypi.org/project/pylint/)\n\n### Credits & Trademarks\n\nvalgrind is an open-source project with a GPL v3.0 license.\n* http://valgrind.sourceforge.net\n* https://github.com/danmar/valgrind\n\n"GitLab" is a trademark of GitLab B.V.\n* https://gitlab.com\n* https://docs.gitlab.com/ee/user/project/merge_requests/code_quality.html\n\nAll other trademarks belong to their respective owners.\n',
+    'long_description': '# valgrind-codequality\n\n[![badge-pypi](https://img.shields.io/pypi/v/valgrind-codequality.svg?logo=pypi)](https://pypi.python.org/pypi/valgrind-codequality/)\n&nbsp;\n[![badge-pypi-downloads](https://img.shields.io/pypi/dm/valgrind-codequality)](https://pypi.org/project/valgrind-codequality/)\n\n\n[![badge-pipeline](https://gitlab.com/echopouet/valgrind-codequality/badges/main/pipeline.svg)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-coverage](https://gitlab.com/echopouet/valgrind-codequality/badges/main/coverage.svg)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-pylint](https://gitlab.com/echopouet/valgrind-codequality/-/jobs/artifacts/main/raw/badge.svg?job=pylint)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-formatting](https://gitlab.com/echopouet/valgrind-codequality/-/jobs/artifacts/main/raw/badge.svg?job=format_black)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-issues-cnt](https://img.shields.io/badge/dynamic/json?label=issues&query=statistics.counts.opened&url=https%3A%2F%2Fgitlab.com%2Fapi%2Fv4%2Fprojects%2F19114200%2Fissues_statistics%3Fscope%3Dall)](https://gitlab.com/echopouet/valgrind-codequality/-/issues)\n\n\n## About\n\nI wanted reports from [Valgrind](https://valgrind.org/) to appear in GitLab Merge Requests as [Code Quality reports](https://docs.gitlab.com/ee/user/project/merge_requests/code_quality.html#implementing-a-custom-tool), which is a JSON file defined by the Code Quality\'s GitLab.\n\nThat\'s all this does: convert Valgrind XML report to Code Quality JSON.\n\nContributions are welcome.\n\n[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/EchoPouet)\n\n### Usage\n\nIt is primarily used as a console script. As such, ensure you have Python 3\'s "scripts" directory in your `PATH` variable.\nFor example, on Linux, that might be `$HOME/.local/bin`.\n\nTo test, try the `--help` or `--version` flags:\n```bash\nvalgrind-codequality --help\n```\n\nThis script follows that example and provides similar command-line options.\nA typical workflow might look like this:\n\n```bash\n# Generate valgrind report as XML\nvalgrind --tool=memcheck --leak-check=full --show-leak-kinds=all --track-origins=yes --verbose --xml=yes --xml-file=valgrind_out.xml your_exe\n# Convert to a Code Climate JSON report\nvalgrind-codequality --input-file valgrind_out.xml --output-file valgrind.json\n```\n\nIf you wanted, you could invoke the script directly as a module, like this:\n\n```bash\n# Run as a module instead (note the underscore in the module name here)\npython -m valgrind_codequality --input-file=valgrind_out.xml --output-file=valgrind.json\n```\n\nNow, in your GitLab CI script, [upload this file](https://docs.gitlab.com/ee/ci/pipelines/job_artifacts.html#artifactsreportscodequality)\nas a Code Quality report.\n\n```yaml\nmy-code-quality:\n  script:\n    - [...]\n  artifacts:\n    reports:\n      codequality: valgrind.json\n```\n\n### Contributing\n\n* Format with [black](https://pypi.org/project/black/)\n* Check with [pylint](https://pypi.org/project/pylint/)\n\n### Credits & Trademarks\n\nvalgrind is an open-source project with a GPL v3.0 license.\n* https://valgrind.org/\n\n"GitLab" is a trademark of GitLab B.V.\n* https://gitlab.com\n* https://docs.gitlab.com/ee/user/project/merge_requests/code_quality.html\n\nAll other trademarks belong to their respective owners.\n',
     'author': 'Arnaud Moura',
     'author_email': 'arnaudmoura@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `valgrind_codequality-1.1.0/PKG-INFO` & `valgrind_codequality-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valgrind-codequality
-Version: 1.1.0
+Version: 1.2.0
 Summary: Convert Valgrind XML to GitLab Code Quality JSON file.
 License: MIT
 Author: Arnaud Moura
 Author-email: arnaudmoura@gmail.com
 Requires-Python: >=3.6.8,<=3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -83,23 +83,21 @@
   artifacts:
     reports:
       codequality: valgrind.json
 ```
 
 ### Contributing
 
-* Sign the contributor agreement (coming soon)
 * Format with [black](https://pypi.org/project/black/)
 * Check with [pylint](https://pypi.org/project/pylint/)
 
 ### Credits & Trademarks
 
 valgrind is an open-source project with a GPL v3.0 license.
-* http://valgrind.sourceforge.net
-* https://github.com/danmar/valgrind
+* https://valgrind.org/
 
 "GitLab" is a trademark of GitLab B.V.
 * https://gitlab.com
 * https://docs.gitlab.com/ee/user/project/merge_requests/code_quality.html
 
 All other trademarks belong to their respective owners.
```

