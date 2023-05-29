# Comparing `tmp/vigilant_kit-1.2.6.tar.gz` & `tmp/vigilant_kit-1.2.7.tar.gz`

## Comparing `vigilant_kit-1.2.6.tar` & `vigilant_kit-1.2.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/.vigilant.env.example
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/vigilant.json.example
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/bin/doc_generator.py
--rw-r--r--   0        0        0    30712 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/actions.md
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/browser_options.md
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/configuration.md
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/native_selenium.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/docs/vigilant_unittest.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/install_dev_kit_command.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/install_standalone_command.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/install_webdriver_command.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/run_selenium_command.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vgl_cli/vgl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0    13552 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/LICENSE
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 vigilant_kit-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/.vigilant.env.example
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/vigilant.json.example
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/bin/doc_generator.py
+-rw-r--r--   0        0        0    30712 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/actions.md
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/browser_options.md
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/configuration.md
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/native_selenium.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/install_dev_kit_command.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/install_standalone_command.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/install_webdriver_command.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/run_selenium_command.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/vgl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0    13552 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/LICENSE
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/PKG-INFO
```

### Comparing `vigilant_kit-1.2.6/bin/doc_generator.py` & `vigilant_kit-1.2.7/bin/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/docs/actions.md` & `vigilant_kit-1.2.7/docs/actions.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/docs/browser_options.md` & `vigilant_kit-1.2.7/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/docs/configuration.md` & `vigilant_kit-1.2.7/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/docs/native_selenium.md` & `vigilant_kit-1.2.7/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/docs/selenium_install.md` & `vigilant_kit-1.2.7/docs/selenium_install.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/docs/tutorial_pytest.md` & `vigilant_kit-1.2.7/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/docs/vigilant_pytest.md` & `vigilant_kit-1.2.7/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/docs/vigilant_unittest.md` & `vigilant_kit-1.2.7/docs/vigilant_unittest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vgl_cli/install_dev_kit_command.py` & `vigilant_kit-1.2.7/src/vgl_cli/install_dev_kit_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vgl_cli/install_standalone_command.py` & `vigilant_kit-1.2.7/src/vgl_cli/install_standalone_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vgl_cli/install_webdriver_command.py` & `vigilant_kit-1.2.7/src/vgl_cli/install_webdriver_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vgl_cli/run_selenium_command.py` & `vigilant_kit-1.2.7/src/vgl_cli/run_selenium_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vgl_cli/vgl.py` & `vigilant_kit-1.2.7/src/vgl_cli/vgl.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vigilant/actions/assertions.py` & `vigilant_kit-1.2.7/src/vigilant/actions/assertions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vigilant/actions/finder.py` & `vigilant_kit-1.2.7/src/vigilant/actions/finder.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vigilant/actions/vigilant_actions.py` & `vigilant_kit-1.2.7/src/vigilant/actions/vigilant_actions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vigilant/actions/waiter.py` & `vigilant_kit-1.2.7/src/vigilant/actions/waiter.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vigilant/driver/__init__.py` & `vigilant_kit-1.2.7/src/vigilant/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/src/vigilant/driver/vigilant_driver.py` & `vigilant_kit-1.2.7/src/vigilant/driver/vigilant_driver.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/.gitignore` & `vigilant_kit-1.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/LICENSE` & `vigilant_kit-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.6/README.md` & `vigilant_kit-1.2.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,55 @@
 # Vigilant Kit
-Vigilant is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. With Vigilant, you can start writing complex test
-cases in a minute.
+Vigilant is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. With 
+Vigilant, you can start writing complex test cases in a minute.
 
 ## Why Vigilant?
-- **Easy to start & Fast To Write**: Vigilant provides you with methods that help you write functional tests quickly 
+* **Easy to start & Fast To Write**: Vigilant provides you with methods that help you write functional tests quickly 
 without spending time on writing boilerplate code every time you start a new project.
-- **Flexible Framework Usage**: Usage is not limited to a single testing framework; you can use Vigilant with unittest,
+* **Flexible Framework Usage**: Usage is not limited to a single testing framework; you can use Vigilant with unittest,
   pytest, or anything else.
+* **Stability**: We use Selenium WebDriver. It is a W3C Recommendation.
+   - WebDriver drives a browser natively, as a user would, either locally or on a remote machine using the Selenium server.
+   - WebDriver is designed as a simple and more concise programming interface.
+   - WebDriver is a compact object-oriented API.
+   - It drives the browser effectively.
 
 ## What it includes?
-Methods for **interacting** with WebBrowser (`click`, `scroll_to`,  etc.), **assertions** (`see`, `dont_see`, `see_text`
-, etc.) **waiters** (`wait_for_element_to_be_visible`, `wait_for_element_to_be_clickable`, etc.)
-It is already there, ready to use.
+Vigilant include methods for interacting with browser,  for asserting conditions and also methods for waiting 
+those conditions.
 
-Also, a bunch of CLI scripts, to make your life easier!
+**Interacting with WebBrowser** 
+   - `click()`
+   - `scroll_to()`
+   - `fill_form()`
+   - `move_mouse_on_element()`
+   - ...
+
+**Assertions** 
+   - `see()`
+   - `dont_see()`
+   - `see_text()`
+   - `see_in_title()`
+   - ...
+
+
+**Waiters** 
+   - `wait_for_element_to_be_visible()`
+   - `wait_for_element_to_be_clickable()`
+   - `wait_for_text_to_be_present_in_element()`
+   - `wait_for_element_to_disappear()`
+   - ...
+
+And much more! Check list of all available - [Actions](docs/actions.md)
+
+
+Also, CLI scripts included, to make your life easier!
 
 Use `vgl --help` to see all available commands.
 
-List of all available [actions](docs/actions.md).
 
 ## Extending Functionality
 If you need something that is not covered in this library, you still have access to all native `Selenium WebDriver` 
 methods. You can create your own methods or use native `WebDriver` methods and share them on one browser session.
 
 ## Install
 ```shell
```

### Comparing `vigilant_kit-1.2.6/pyproject.toml` & `vigilant_kit-1.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.2.6"
+version = "1.2.7"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vigilant_kit-1.2.6/PKG-INFO` & `vigilant_kit-1.2.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,71 @@
 Metadata-Version: 2.1
 Name: vigilant_kit
-Version: 1.2.6
+Version: 1.2.7
 Summary: Library that makes functional testing with Selenium WebDriver fast and easy. 
 Project-URL: Homepage, https://github.com/ivpel/vigilant
 Project-URL: Bug Tracker, https://github.com/ivpel/vigilant/issues
 Author-email: Pelykh Ivan <ivan.pelykh@protonmail.com>
 License-File: LICENSE
 Keywords: bdd,functional,functional-testing,pytest,selenium,tdd,testing,unittest,webdriver
 Requires-Python: >=3.7
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: selenium
 Description-Content-Type: text/markdown
 
 # Vigilant Kit
-Vigilant is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. With Vigilant, you can start writing complex test
-cases in a minute.
+Vigilant is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. With 
+Vigilant, you can start writing complex test cases in a minute.
 
 ## Why Vigilant?
-- **Easy to start & Fast To Write**: Vigilant provides you with methods that help you write functional tests quickly 
+* **Easy to start & Fast To Write**: Vigilant provides you with methods that help you write functional tests quickly 
 without spending time on writing boilerplate code every time you start a new project.
-- **Flexible Framework Usage**: Usage is not limited to a single testing framework; you can use Vigilant with unittest,
+* **Flexible Framework Usage**: Usage is not limited to a single testing framework; you can use Vigilant with unittest,
   pytest, or anything else.
+* **Stability**: We use Selenium WebDriver. It is a W3C Recommendation.
+   - WebDriver drives a browser natively, as a user would, either locally or on a remote machine using the Selenium server.
+   - WebDriver is designed as a simple and more concise programming interface.
+   - WebDriver is a compact object-oriented API.
+   - It drives the browser effectively.
 
 ## What it includes?
-Methods for **interacting** with WebBrowser (`click`, `scroll_to`,  etc.), **assertions** (`see`, `dont_see`, `see_text`
-, etc.) **waiters** (`wait_for_element_to_be_visible`, `wait_for_element_to_be_clickable`, etc.)
-It is already there, ready to use.
+Vigilant include methods for interacting with browser,  for asserting conditions and also methods for waiting 
+those conditions.
 
-Also, a bunch of CLI scripts, to make your life easier!
+**Interacting with WebBrowser** 
+   - `click()`
+   - `scroll_to()`
+   - `fill_form()`
+   - `move_mouse_on_element()`
+   - ...
+
+**Assertions** 
+   - `see()`
+   - `dont_see()`
+   - `see_text()`
+   - `see_in_title()`
+   - ...
+
+
+**Waiters** 
+   - `wait_for_element_to_be_visible()`
+   - `wait_for_element_to_be_clickable()`
+   - `wait_for_text_to_be_present_in_element()`
+   - `wait_for_element_to_disappear()`
+   - ...
+
+And much more! Check list of all available - [Actions](docs/actions.md)
+
+
+Also, CLI scripts included, to make your life easier!
 
 Use `vgl --help` to see all available commands.
 
-List of all available [actions](docs/actions.md).
 
 ## Extending Functionality
 If you need something that is not covered in this library, you still have access to all native `Selenium WebDriver` 
 methods. You can create your own methods or use native `WebDriver` methods and share them on one browser session.
 
 ## Install
 ```shell
```

