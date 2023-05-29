# Comparing `tmp/lifx_cli-2.5.6.tar.gz` & `tmp/lifx_cli-2.5.7.tar.gz`

## Comparing `lifx_cli-2.5.6.tar` & `lifx_cli-2.5.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1617 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/increment_version.sh
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/requirements.txt
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/.hooks/pre-commit
--rwxr-xr-x   0        0        0     2898 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/src/lifx/auth.py
--rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/src/lifx/colors.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/src/lifx/effects.py
--rwxr-xr-x   0        0        0    12134 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/src/lifx/lifx.py
--rwxr-xr-x   0        0        0     3798 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/src/lifx/lights.py
--rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/src/lifx/scenes.py
--rwxr-xr-x   0        0        0     2390 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/tests/lifx_cli_test.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/tests/requirements.txt
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/LICENSE
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/README.md
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/pyproject.toml
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 lifx_cli-2.5.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1590 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/increment_version.sh
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/requirements.txt
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/.hooks/pre-commit
+-rwxr-xr-x   0        0        0     2845 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/src/lifx/auth.py
+-rwxr-xr-x   0        0        0     1904 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/src/lifx/colors.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/src/lifx/effects.py
+-rwxr-xr-x   0        0        0    12134 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/src/lifx/lifx.py
+-rwxr-xr-x   0        0        0     3772 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/src/lifx/lights.py
+-rwxr-xr-x   0        0        0     1311 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/src/lifx/scenes.py
+-rwxr-xr-x   0        0        0     2390 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/tests/lifx_cli_test.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/tests/requirements.txt
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/LICENSE
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/README.md
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/pyproject.toml
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 lifx_cli-2.5.7/PKG-INFO
```

### Comparing `lifx_cli-2.5.6/increment_version.sh` & `lifx_cli-2.5.7/increment_version.sh`

 * *Files 5% similar despite different names*

```diff
@@ -55,13 +55,12 @@
 
 if ! echo ${NEW_VERSION} | grep -q "^[0-9]*\.[0-9]*\.[0-9]*$"; then
     err 6 "New version number is in the wrong format. Must be: <MAJOR>.<MINOR>.<PATCH>"
 fi
 
 is_command gawk
 
-echo "Current Tagged Version: ${CURRENT_VERSION}"
-read -p "Are you certain that you want to increment to version ${NEW_VERSION}? y/N " ANSWER
+read -p "Are you certain that you want to increment to version: ${CURRENT_VERSION} -> ${NEW_VERSION}? y/N " ANSWER
 
 if [ "${ANSWER}" == "y" ]; then
     increment_version
 fi
```

### Comparing `lifx_cli-2.5.6/.github/workflows/pylint.yml` & `lifx_cli-2.5.7/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.6/.github/workflows/pytest.yml` & `lifx_cli-2.5.7/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.6/.github/workflows/python-publish.yml` & `lifx_cli-2.5.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.6/src/lifx/auth.py` & `lifx_cli-2.5.7/src/lifx/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,14 @@
             else:
                 break
 
         if path.exists(self.auth_file):
             config.read(self.auth_file)
 
         if not config.has_section(self.auth_file_section):
-            config = configparser.RawConfigParser()
             config.add_section(self.auth_file_section)
             config.set(self.auth_file_section, self.auth_file_key, api_key)
 
             with open(self.auth_file, 'a+', encoding='UTF-8') as file:
                 config.write(file)
         else:
             overwrite = input('You already have an API key saved in ~/.keys. '
@@ -61,24 +60,23 @@
         if response.status_code != 200:
             print("Received an unexpected response from LIFX. Please try again.")
             return False
         return True
 
     def auth(self) -> dict:
         """Returns the headers required to authenticate to the LIFX API."""
-
         try:
             if environ.get(self.auth_env_var):
                 token = getenv(self.auth_env_var)
             else:
                 config = configparser.ConfigParser()
                 config.read(self.auth_file)
 
                 token = config[self.auth_file_section][self.auth_file_key]
         except KeyError:
             print("Must configure an API token first.")
             self.configure()
 
         headers = {
-            'Authorization': f'Bearer {token}',
+            "Authorization": f"Bearer {token}",
         }
         return headers
```

### Comparing `lifx_cli-2.5.6/src/lifx/colors.py` & `lifx_cli-2.5.7/src/lifx/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python3
 """Learn about how the CLI accepts color encoding."""
-import json
 import sys
-
 from requests import get
 from tabulate import tabulate
 from src.lifx.auth import Auth
 
 API = 'https://api.lifx.com/v1'
 
 COLOR_TABLE = [['[name]', 'white, red, orange, yellow, cyan, green, blue, purple, or pink',
@@ -35,15 +33,15 @@
         """Validate the provided color with the LIFX API."""
 
         url = f'{API}/color?string={color}'
         response = get(url, headers=self.auth_headers, timeout=5)
         if response.status_code != 200:
             print(f"HTTP request failed. Status code: {response.status_code}")
             sys.exit(10)
-        response = json.loads(response.content)
+        response = response.json()
 
         hue = response['hue'] or 'None'
         saturation = response['saturation'] or 'None'
         brightness = response['brightness'] or 'None'
         kelvin = response['kelvin'] or 'None'
 
         validated_colors = [[hue, saturation, brightness, kelvin]]
```

### Comparing `lifx_cli-2.5.6/src/lifx/effects.py` & `lifx_cli-2.5.7/src/lifx/effects.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.6/src/lifx/lifx.py` & `lifx_cli-2.5.7/src/lifx/lifx.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ██      ██ ███████ ██   ██      ██████ ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ██      ██ █████     ███       ██      ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ███████ ██ ██      ██   ██      ██████ ███████ ██
 
 """
-VERSION = "2.5.6"
+VERSION = "2.5.7"
 
 
 def get_version():
     """Print the version and exit."""
     print(f"Version: {VERSION}")
     sys.exit(0)
```

### Comparing `lifx_cli-2.5.6/src/lifx/lights.py` & `lifx_cli-2.5.7/src/lifx/lights.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 #!/usr/bin/env python3
 """Control LIFX lights."""
 import sys
-import json
 from requests import get, post, put
 from tabulate import tabulate
 from src.lifx.auth import Auth
 
 API = 'https://api.lifx.com/v1'
 
 
 class Lights:
     """Control LIFX lights."""
-
     def __init__(self):
         self.auth = Auth()
         self.auth_headers = self.auth.auth()
 
     def get(self):
         """Print a list of all LIFX devices on this account."""
         url = f'{API}/lights/all'
         response = get(url, headers=self.auth_headers, timeout=5)
 
         if response.status_code != 200:
             print(f"HTTP request failed. Status code: {response.status_code}")
             sys.exit(30)
 
-        response = json.loads(response.content)
+        response = response.json()
 
         lights = []
         switches = []
 
         for _, value in enumerate(response):
             device = value["label"]
             device_id = value["id"]
```

### Comparing `lifx_cli-2.5.6/src/lifx/scenes.py` & `lifx_cli-2.5.7/src/lifx/scenes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 #!/usr/bin/env python3
 """List and control LIFX scenes."""
 import sys
-import json
 from requests import get, put
 from tabulate import tabulate
 from src.lifx.auth import Auth
 
 API = 'https://api.lifx.com/v1'
 
 
 class Scenes:
     """List and control LIFX scenes."""
-
     def __init__(self):
         self.auth = Auth()
         self.auth_headers = self.auth.auth()
 
     def get(self):
         """Print a list of all scenes on this account."""
         url = f'{API}/scenes'
         response = get(url, headers=self.auth_headers, timeout=5)
 
         if response.status_code != 200:
             print(f"HTTP request failed. Status code: {response.status_code}")
             sys.exit(40)
 
-        response = json.loads(response.content)
+        response = response.json()
 
         scenes = []
 
         for _, value in enumerate(response):
             scenes += [[value["name"], value["uuid"]]]
 
         scenes.sort()
```

### Comparing `lifx_cli-2.5.6/tests/lifx_cli_test.py` & `lifx_cli-2.5.7/tests/lifx_cli_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import src.lifx.lifx
 from src.lifx.auth import Auth
 from src.lifx.colors import Colors
 from src.lifx.effects import Effects
 from src.lifx.lights import Lights
 from src.lifx.scenes import Scenes
 
-VERSION = "2.5.6"
+VERSION = "2.5.7"
 TEST_HELP = "Control LIFX devices via the CLI!"
 TEST_GROUP = "68931117c352834e0a8f70aebcbcdae1"
 TEST_COLORS = ["purple", "green"]
 TEST_CYCLES = 4
 TEST_LIGHT = "d073d568d053"
 TEST_SCENE = "9371a59c-6ee7-4ced-a3d3-b25d9fc08aad"
```

### Comparing `lifx_cli-2.5.6/.gitignore` & `lifx_cli-2.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.6/LICENSE` & `lifx_cli-2.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.6/README.md` & `lifx_cli-2.5.7/README.md`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.6/pyproject.toml` & `lifx_cli-2.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifx-cli"
-version = "2.5.6"
+version = "2.5.7"
 authors = [{name="Wes Henderson", email="info@necrux.com"}]
 description = "The Unofficial LIFX CLI"
 readme = "README.md"
 requires-python = ">=3.5"
 dependencies = [
   'requests',
   'tabulate',
```

### Comparing `lifx_cli-2.5.6/PKG-INFO` & `lifx_cli-2.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifx-cli
-Version: 2.5.6
+Version: 2.5.7
 Summary: The Unofficial LIFX CLI
 Project-URL: Homepage, https://github.com/necrux/lifx-cli
 Project-URL: Bug Tracker, https://github.com/necrux/lifx-cli/issues
 Author-email: Wes Henderson <info@necrux.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

