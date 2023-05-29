# Comparing `tmp/ansible_doctor-2.0.4.tar.gz` & `tmp/ansible_doctor-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_doctor-2.0.4.tar", max compression
+gzip compressed data, was "ansible_doctor-2.0.5.tar", max compression
```

## Comparing `ansible_doctor-2.0.4.tar` & `ansible_doctor-2.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    32460 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/LICENSE
--rw-r--r--   0        0        0     2754 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/README.md
--rw-r--r--   0        0        0       58 2023-04-05 12:37:04.679567 ansible_doctor-2.0.4/ansibledoctor/__init__.py
--rw-r--r--   0        0        0     6263 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/annotation.py
--rw-r--r--   0        0        0     4041 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/cli.py
--rw-r--r--   0        0        0    11842 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/config.py
--rw-r--r--   0        0        0      120 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/contstants.py
--rw-r--r--   0        0        0     7210 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/doc_generator.py
--rw-r--r--   0        0        0     5952 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/doc_parser.py
--rw-r--r--   0        0        0      472 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/exception.py
--rw-r--r--   0        0        0     1734 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/file_registry.py
--rw-r--r--   0        0        0      377 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/_meta.j2
--rw-r--r--   0        0        0      173 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/_requirements.j2
--rw-r--r--   0        0        0      318 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/_tag.j2
--rw-r--r--   0        0        0      371 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/_toc.j2
--rw-r--r--   0        0        0      583 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/_todo.j2
--rw-r--r--   0        0        0      935 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/_vars.j2
--rw-r--r--   0        0        0      847 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/index.md.j2
--rw-r--r--   0        0        0      696 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/readme/README.md.j2
--rw-r--r--   0        0        0      691 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/readme/_meta.j2
--rw-r--r--   0        0        0      173 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/readme/_requirements.j2
--rw-r--r--   0        0        0      365 2023-04-05 12:36:49.239652 ansible_doctor-2.0.4/ansibledoctor/templates/readme/_tag.j2
--rw-r--r--   0        0        0      434 2023-04-05 12:36:49.243652 ansible_doctor-2.0.4/ansibledoctor/templates/readme/_toc.j2
--rw-r--r--   0        0        0      583 2023-04-05 12:36:49.243652 ansible_doctor-2.0.4/ansibledoctor/templates/readme/_todo.j2
--rw-r--r--   0        0        0      935 2023-04-05 12:36:49.243652 ansible_doctor-2.0.4/ansibledoctor/templates/readme/_vars.j2
--rw-r--r--   0        0        0     9272 2023-04-05 12:36:49.243652 ansible_doctor-2.0.4/ansibledoctor/utils.py
--rw-r--r--   0        0        0     3372 2023-04-05 12:37:04.675567 ansible_doctor-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     4758 1970-01-01 00:00:00.000000 ansible_doctor-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0    32460 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/LICENSE
+-rw-r--r--   0        0        0     2754 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/README.md
+-rw-r--r--   0        0        0       58 2023-05-29 20:03:30.783262 ansible_doctor-2.0.5/ansibledoctor/__init__.py
+-rw-r--r--   0        0        0     6263 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/annotation.py
+-rw-r--r--   0        0        0     4038 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/cli.py
+-rw-r--r--   0        0        0    11842 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/config.py
+-rw-r--r--   0        0        0      120 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/contstants.py
+-rw-r--r--   0        0        0     7204 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/doc_generator.py
+-rw-r--r--   0        0        0     5952 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/doc_parser.py
+-rw-r--r--   0        0        0      472 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/exception.py
+-rw-r--r--   0        0        0     1734 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/file_registry.py
+-rw-r--r--   0        0        0      377 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_meta.j2
+-rw-r--r--   0        0        0      173 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_requirements.j2
+-rw-r--r--   0        0        0      318 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_tag.j2
+-rw-r--r--   0        0        0      371 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_toc.j2
+-rw-r--r--   0        0        0      583 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_todo.j2
+-rw-r--r--   0        0        0      935 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_vars.j2
+-rw-r--r--   0        0        0      847 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/index.md.j2
+-rw-r--r--   0        0        0      696 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/README.md.j2
+-rw-r--r--   0        0        0      691 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_meta.j2
+-rw-r--r--   0        0        0      173 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_requirements.j2
+-rw-r--r--   0        0        0      365 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_tag.j2
+-rw-r--r--   0        0        0      434 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_toc.j2
+-rw-r--r--   0        0        0      583 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_todo.j2
+-rw-r--r--   0        0        0      935 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_vars.j2
+-rw-r--r--   0        0        0     9272 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/utils.py
+-rw-r--r--   0        0        0     3359 2023-05-29 20:03:30.783262 ansible_doctor-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 ansible_doctor-2.0.5/PKG-INFO
```

### Comparing `ansible_doctor-2.0.4/LICENSE` & `ansible_doctor-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/README.md` & `ansible_doctor-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/annotation.py` & `ansible_doctor-2.0.5/ansibledoctor/annotation.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/cli.py` & `ansible_doctor-2.0.5/ansibledoctor/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         for item in walkdirs:
             os.chdir(item)
 
             self.config.set_config(base_dir=os.getcwd())
             try:
                 self.log.set_level(self.config.config["logging"]["level"])
             except ValueError as e:
-                self.log.sysexit_with_message(f"Can not set log level.\n{str(e)}")
+                self.log.sysexit_with_message(f"Can not set log level.\n{e!s}")
             self.logger.info(f"Using config file: {self.config.config_file}")
 
             self.logger.debug(f"Using working dir: {item}")
 
             if self.config.config["role_detection"]:
                 if self.config.is_role:
                     self.logger.info(f"Ansible role detected: {self.config.config['role_name']}")
```

### Comparing `ansible_doctor-2.0.4/ansibledoctor/config.py` & `ansible_doctor-2.0.5/ansibledoctor/config.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/doc_generator.py` & `ansible_doctor-2.0.5/ansibledoctor/doc_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         header_content = ""
         if bool(header_file):
             role_data["internal"]["append"] = True
             try:
                 with open(header_file) as a:
                     header_content = a.read()
             except FileNotFoundError as e:
-                self.log.sysexit_with_message(f"Can not open custom header file\n{str(e)}")
+                self.log.sysexit_with_message(f"Can not open custom header file\n{e!s}")
 
         if (
             len(files_to_overwite) > 0 and self.config.config.get("force_overwrite") is False
             and not self.config.config["dry_run"]
         ):
             files_to_overwite_string = "\n".join(files_to_overwite)
             self.logger.warning(f"This files will be overwritten:\n{files_to_overwite_string}")
@@ -138,15 +138,15 @@
                             self.log.sysexit_with_message(
                                 "Jinja2 templating error while loading file: '{}'\n{}".format(
                                     file, str(e)
                                 )
                             )
                         except UnicodeEncodeError as e:
                             self.log.sysexit_with_message(
-                                f"Unable to print special characters\n{str(e)}"
+                                f"Unable to print special characters\n{e!s}"
                             )
 
     def _to_nice_yaml(self, a, indent=4, **kw):
         """Make verbose, human readable yaml."""
         yaml = ruamel.yaml.YAML()
         yaml.indent(mapping=indent, sequence=(indent * 2), offset=indent)
         stream = ruamel.yaml.compat.StringIO()
```

### Comparing `ansible_doctor-2.0.4/ansibledoctor/doc_parser.py` & `ansible_doctor-2.0.5/ansibledoctor/doc_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/file_registry.py` & `ansible_doctor-2.0.5/ansibledoctor/file_registry.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/_todo.j2` & `ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_todo.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/_vars.j2` & `ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_vars.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/templates/hugo-book/index.md.j2` & `ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/index.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/templates/readme/README.md.j2` & `ansible_doctor-2.0.5/ansibledoctor/templates/readme/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/templates/readme/_meta.j2` & `ansible_doctor-2.0.5/ansibledoctor/templates/readme/_meta.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/templates/readme/_todo.j2` & `ansible_doctor-2.0.5/ansibledoctor/templates/readme/_todo.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/templates/readme/_vars.j2` & `ansible_doctor-2.0.5/ansibledoctor/templates/readme/_vars.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/ansibledoctor/utils.py` & `ansible_doctor-2.0.5/ansibledoctor/utils.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.4/pyproject.toml` & `ansible_doctor-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,47 +29,47 @@
 license = "GPL-3.0-only"
 name = "ansible-doctor"
 packages = [
   {include = "ansibledoctor"},
 ]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/ansible-doctor/"
-version = "2.0.4"
+version = "2.0.5"
 
 [tool.poetry.dependencies]
 Jinja2 = "3.1.2"
 anyconfig = "0.13.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
 environs = "9.5.0"
 jsonschema = "4.17.3"
 nested-lookup = "0.2.25"
 pathspec = "0.11.1"
 python = "^3.7.0"
 python-json-logger = "2.0.7"
-"ruamel.yaml" = "0.17.21"
+"ruamel.yaml" = "0.17.28"
 
 [tool.poetry.scripts]
 ansible-doctor = "ansibledoctor.cli:main"
 
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
 
 [tool.pytest.ini_options]
-addopts = "ansibledoctor --cov=ansibledoctor --cov-report=xml:coverage.xml --cov-report=term --cov-append --no-cov-on-fail"
+addopts = "ansibledoctor --cov=ansibledoctor --cov-report=xml:coverage.xml --cov-report=term --no-cov-on-fail"
 filterwarnings = [
   "ignore::FutureWarning",
   "ignore::DeprecationWarning",
   "ignore:.*pep8.*:FutureWarning",
 ]
 
 [tool.coverage.run]
```

### Comparing `ansible_doctor-2.0.4/PKG-INFO` & `ansible_doctor-2.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-doctor
-Version: 2.0.4
+Version: 2.0.5
 Summary: Generate documentation from annotated Ansible roles using templates.
 Home-page: https://ansible-doctor.geekdocs.de/
 License: GPL-3.0-only
 Keywords: ansible,role,documentation
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.7.0,<4.0.0
@@ -18,33 +18,27 @@
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
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Requires-Dist: Jinja2 (==3.1.2)
 Requires-Dist: anyconfig (==0.13.0)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: environs (==9.5.0)
 Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: nested-lookup (==0.2.25)
 Requires-Dist: pathspec (==0.11.1)
 Requires-Dist: python-json-logger (==2.0.7)
-Requires-Dist: ruamel.yaml (==0.17.21)
+Requires-Dist: ruamel.yaml (==0.17.28)
 Project-URL: Documentation, https://ansible-doctor.geekdocs.de/
 Project-URL: Repository, https://github.com/thegeeklab/ansible-doctor/
 Description-Content-Type: text/markdown
 
 # ansible-doctor
 
 Annotation based documentation for your Ansible roles
```

