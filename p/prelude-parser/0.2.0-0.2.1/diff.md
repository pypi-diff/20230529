# Comparing `tmp/prelude_parser-0.2.0.tar.gz` & `tmp/prelude_parser-0.2.1.tar.gz`

## Comparing `prelude_parser-0.2.0.tar` & `prelude_parser-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 prelude_parser-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      439 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/dependabot.yml
--rw-r--r--   0     1001      123      539 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/release-draft-template.yml
--rw-r--r--   0     1001      123     2599 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0     1001      123      309 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/workflows/release-drafter.yml
--rw-r--r--   0     1001      123     1884 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/workflows/testing.yml
--rw-r--r--   0     1001      123      686 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.gitignore
--rw-r--r--   0     1001      123      640 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     7889 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1080 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/LICENSE
--rw-r--r--   0     1001      123     1499 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/README.md
--rw-r--r--   0     1001      123      585 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/justfile
--rw-r--r--   0     1001      123      115 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/__init__.py
--rw-r--r--   0     1001      123      399 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/_prelude_parser.pyi
--rw-r--r--   0     1001      123      911 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/pandas.py
--rw-r--r--   0     1001      123     2325 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/parser.py
--rw-r--r--   0     1001      123      901 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/polars.py
--rw-r--r--   0     1001      123        0 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/py.typed
--rw-r--r--   0     1001      123     1845 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      147 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/requirements-dev.txt
--rw-r--r--   0     1001      123     6082 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/__init__.py
--rw-r--r--   0     1001      123     1304 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/assets/test1.xml
--rw-r--r--   0     1001      123     1839 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/assets/test2.xml
--rw-r--r--   0     1001      123     2122 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/assets/test3.xml
--rw-r--r--   0     1001      123      312 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/conftest.py
--rw-r--r--   0     1001      123      942 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/test_pandas.py
--rw-r--r--   0     1001      123     8042 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/test_parser.py
--rw-r--r--   0     1001      123     1004 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/test_polars.py
--rw-r--r--   0     1001      123     8093 2023-05-19 16:42:55.000000 prelude_parser-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     2710 1970-01-01 00:00:00.000000 prelude_parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 prelude_parser-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123      439 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/dependabot.yml
+-rw-r--r--   0     1001      123      539 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/release-draft-template.yml
+-rw-r--r--   0     1001      123     2599 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0     1001      123      309 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0     1001      123     1889 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/workflows/testing.yml
+-rw-r--r--   0     1001      123      686 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.gitignore
+-rw-r--r--   0     1001      123      640 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     7889 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1080 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/LICENSE
+-rw-r--r--   0     1001      123     2801 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/README.md
+-rw-r--r--   0     1001      123      595 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/justfile
+-rw-r--r--   0     1001      123      115 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/__init__.py
+-rw-r--r--   0     1001      123      399 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/_prelude_parser.pyi
+-rw-r--r--   0     1001      123      911 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/pandas.py
+-rw-r--r--   0     1001      123     1753 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/parser.py
+-rw-r--r--   0     1001      123      901 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/polars.py
+-rw-r--r--   0     1001      123        0 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/py.typed
+-rw-r--r--   0     1001      123     1876 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123      132 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/requirements-dev.txt
+-rw-r--r--   0     1001      123    10754 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/__init__.py
+-rw-r--r--   0     1001      123     1304 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/assets/test1.xml
+-rw-r--r--   0     1001      123     1839 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/assets/test2.xml
+-rw-r--r--   0     1001      123     2122 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/assets/test3.xml
+-rw-r--r--   0     1001      123      312 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/conftest.py
+-rw-r--r--   0     1001      123      942 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/test_pandas.py
+-rw-r--r--   0     1001      123     8018 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/test_parser.py
+-rw-r--r--   0     1001      123     1004 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/test_polars.py
+-rw-r--r--   0     1001      123    15614 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     4012 1970-01-01 00:00:00.000000 prelude_parser-0.2.1/PKG-INFO
```

### Comparing `prelude_parser-0.2.0/Cargo.toml` & `prelude_parser-0.2.1/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [package]
 name = "prelude-parser"
-version = "0.2.0"
+version = "0.2.1"
 description = "Parses XML files exported from Prelude EDC into formats usable by Python."
 edition = "2021"
 license = "MIT"
 homepage = "https://github.com/pbs-data-solutions/prelude-parser"
 repository = "https://github.com/pbs-data-solutions/prelude-parser"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "_prelude_parser"
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.18.2", features = ["extension-module", "abi3-py38"] }
+chrono = "0.4.24"
+pyo3 = { version = "0.18.3", features = ["extension-module", "abi3-py38"] }
 roxmltree = "0.18.0"
```

### Comparing `prelude_parser-0.2.0/.github/release-draft-template.yml` & `prelude_parser-0.2.1/.github/release-draft-template.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/.github/workflows/pypi_publish.yml` & `prelude_parser-0.2.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/.github/workflows/testing.yml` & `prelude_parser-0.2.1/.github/workflows/testing.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     - uses: actions-rs/toolchain@v1
       with:
         profile: minimal
         toolchain: stable
         override: true
         components: clippy
     - name: Cache dependencies
-      uses: Swatinem/rust-cache@v2.3.0
+      uses: Swatinem/rust-cache@v2.4.0
     - name: Run cargo clippy
       uses: actions-rs/cargo@v1
       with:
         command: clippy
         args: --all-targets -- --deny warnings
   fmt:
     name: Rustfmt
@@ -35,15 +35,15 @@
     - uses: actions-rs/toolchain@v1
       with:
         profile: minimal
         toolchain: stable
         override: true
         components: rustfmt
     - name: Cache dependencies
-      uses: Swatinem/rust-cache@v2.3.0
+      uses: Swatinem/rust-cache@v2.4.0
     - name: Run cargo fmt
       run: cargo fmt --all -- --check
   test:
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
@@ -56,15 +56,15 @@
       with:
         python-version: ${{ matrix.python-version }}
         cache: "pip"
     - name: Install dependencies
       run: |
         pip install -U pip
         pip install -r requirements-dev.txt
-        pip install -e .
+        pip install -e .[all]
         maturin build --out dist
         pip install --no-index --find-links=dist/ prelude-parser
     - name: Run tests
       run: pytest --cov=prelude_parser --cov-report=xml
     - name: Upload coverage
       uses: codecov/codecov-action@v3
       with:
```

### Comparing `prelude_parser-0.2.0/.gitignore` & `prelude_parser-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/.pre-commit-config.yaml` & `prelude_parser-0.2.1/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -15,11 +15,11 @@
       language_version: python3
       args: [--line-length=100]
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
     - id: mypy
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.267
+    rev: v0.0.269
     hooks:
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `prelude_parser-0.2.0/CONTRIBUTING.md` & `prelude_parser-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/LICENSE` & `prelude_parser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/prelude_parser/pandas.py` & `prelude_parser-0.2.1/prelude_parser/pandas.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/prelude_parser/polars.py` & `prelude_parser-0.2.1/prelude_parser/polars.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/pyproject.toml` & `prelude_parser-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["maturin>=0.15"]
+requires = ["maturin>=1.0.0"]
 build-backend = "maturin"
 
 [project]
 name = "prelude-parser"
 requires-python = ">=3.8"
 description = "Parses XML files exported from Prelude EDC into formats usable by Python."
 authors = [{name = "Paul Sanders", email = "paul@pbsdatasolutions.com"}]
@@ -65,11 +65,12 @@
 disallow_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
 
 [tool.ruff]
-select=["E", "F", "T201", "T203", "I001"]
+select=["E", "F", "UP", "I001", "T201", "T203"]
 ignore=["E501"]
 line-length = 100
+target-version = "py38"
 fix = true
```

### Comparing `prelude_parser-0.2.0/tests/assets/test1.xml` & `prelude_parser-0.2.1/tests/assets/test1.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/tests/assets/test2.xml` & `prelude_parser-0.2.1/tests/assets/test2.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/tests/assets/test3.xml` & `prelude_parser-0.2.1/tests/assets/test3.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/tests/test_pandas.py` & `prelude_parser-0.2.1/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/tests/test_parser.py` & `prelude_parser-0.2.1/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+from datetime import date
 
 import pytest
 
 from prelude_parser import parse_to_classes, parse_to_dict
 from prelude_parser._prelude_parser import FileNotFoundError, InvalidFileTypeError, ParsingError
 
 
@@ -24,15 +24,15 @@
 
 
 def test_parse_to_classes_with_float(test_file_2):
     result = parse_to_classes(test_file_2)
     assert len(result) == 2
     assert result[0].__name__ == "Demographics"
     assert result[0].weight == 80.2
-    assert result[0].dob == datetime(2020, 4, 15)
+    assert result[0].dob == date(2020, 4, 15)
 
 
 def test_parse_to_classes_i_form(test_file_3):
     result = parse_to_classes(test_file_3)
     assert len(result) == 3
     assert result[0].__name__ == "ICommunicationsDetails"
     assert result[0].study_name == "PBS"
@@ -111,15 +111,15 @@
 def test_parse_to_dict_with_float(test_file_2):
     result = parse_to_dict(test_file_2)
     expected = {
         "demographics": [
             {
                 "base_form": "day.0.form.name.demographics",
                 "breed": "Labrador",
-                "dob": datetime(2020, 4, 15),
+                "dob": date(2020, 4, 15),
                 "first_name": "Imma",
                 "form_group": "Day 0",
                 "form_number": None,
                 "form_state": "In-Work",
                 "form_title": "Demographics",
                 "gender": "Female Spayed",
                 "last_name": "Dog",
@@ -127,21 +127,21 @@
                 "patient_name": "ABC-001",
                 "screening_number": 1,
                 "site_id": 1681574834910,
                 "site_name": "Some Site",
                 "site_type": "Live",
                 "study_name": "PBS",
                 "subject_id": "ABC-001",
-                "visit_date": datetime(2023, 4, 15),
+                "visit_date": date(2023, 4, 15),
                 "weight": 80.2,
             },
             {
                 "base_form": "day.0.form.name.demographics",
                 "breed": "Golden",
-                "dob": datetime(2019, 4, 9),
+                "dob": date(2019, 4, 9),
                 "first_name": "Arthur",
                 "form_group": "Day 0",
                 "form_number": None,
                 "form_state": "In-Work",
                 "form_title": "Demographics",
                 "gender": "Male Neutered",
                 "last_name": "Dent",
@@ -149,15 +149,15 @@
                 "patient_name": "ABC-002",
                 "screening_number": 2,
                 "site_id": 1681574834910,
                 "site_name": "Some Site",
                 "site_type": "Live",
                 "study_name": "PBS",
                 "subject_id": "ABC-002",
-                "visit_date": datetime(2023, 4, 15),
+                "visit_date": date(2023, 4, 15),
                 "weight": 40.5,
             },
         ]
     }
 
     result["demographics"] = [dict(sorted(x.items())) for x in result["demographics"]]
```

### Comparing `prelude_parser-0.2.0/tests/test_polars.py` & `prelude_parser-0.2.1/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.0/PKG-INFO` & `prelude_parser-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: prelude-parser
-Version: 0.2.0
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Typing :: Typed
-Requires-Dist: camel-converter >=3.0.0
-Requires-Dist: pandas >=2.0.1 ; extra == 'pandas'
-Requires-Dist: polars >=0.17.14 ; extra == 'polars'
-Requires-Dist: pandas >=2.0.1 ; extra == 'all'
-Requires-Dist: polars >=0.17.14 ; extra == 'all'
-Provides-Extra: pandas
-Provides-Extra: polars
-Provides-Extra: all
-License-File: LICENSE
-Summary: Parses XML files exported from Prelude EDC into formats usable by Python.
-Keywords: parser,prelude-edc,xml,pandas,polars
-Home-Page: https://github.com/pbs-data-solutions/prelude-parser
-Author-email: Paul Sanders <paul@pbsdatasolutions.com>
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source Code, https://github.com/pbs-data-solutions/prelude-parser
-
 # Prelude Parser
 
 [![Tests Status](https://github.com/pbs-data-solutions/prelude-parser/workflows/Testing/badge.svg?branch=main&event=push)](https://github.com/pbs-data-solutions/prelude-parser/actions?query=workflow%3ATesting+branch%3Amain+event%3Apush)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pbs-data-solutions/prelude-parser/main.svg)](https://results.pre-commit.ci/latest/github/pbs-data-solutions/prelude-parser/main)
 [![Coverage](https://codecov.io/github/pbs-data-solutions/prelude-parser/coverage.svg?branch=main)](https://codecov.io/gh/pbs-data-solutions/prelude-parser)
 [![PyPI version](https://badge.fury.io/py/prelude-parser.svg)](https://badge.fury.io/py/prelude-parser)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/prelude-parser?color=5cc141)](https://github.com/pbs-data-solutions/prelude-parser)
@@ -57,11 +28,46 @@
 
 All extras can be install with
 
 ```sh
 pip install prelude-parser[all]
 ```
 
+## Usage
+
+Parse a Prelude flat XML file to a Python dictionary.
+
+```py
+from prelude_parser import parse_to_dict
+data = parse_to_dict("physical_examination.xml")
+```
+
+Parse a Prelude flat XML file into a list of Python class. The name of the class is taken from the
+form name node in the XML file converted to pascal case. For example a <physical_examination> node
+will result in a PhysicalExamination class being created.
+
+```py
+from prelude_parser import parse_to_classes
+data = parse_to_classes("physical_examination.xml")
+```
+
+Parse a Prelude flat XML file into a Pandas DataFrame. This works for Prelude flat XML files that
+were exported with the "write tables to seperate files" option. In order to use this option
+`prelude-parser` either needs to be installed with the `pandas` extra or the `all` extras.
+
+```py
+from prelude_parser.pandas import to_dataframe
+df = to_dataframe("physical_examination.xml")
+```
+
+Parse a Prelude flat XML file into a Polars DataFrame. This works for Prelude flat XML files that
+were exported with the "write tables to seperate files" option. In order to use this option
+`prelude-parser` either needs to be installed with the `polars` extra or the `all` extras.
+
+```py
+from prelude_parser.polars import to_dataframe
+df = to_dataframe("physical_examination.xml")
+```
+
 ## Contributing
 
 Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
-
```

