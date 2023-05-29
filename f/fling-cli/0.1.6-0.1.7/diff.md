# Comparing `tmp/fling_cli-0.1.6.tar.gz` & `tmp/fling_cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_cli-0.1.6.tar", max compression
+gzip compressed data, was "fling_cli-0.1.7.tar", max compression
```

## Comparing `fling_cli-0.1.6.tar` & `fling_cli-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2163 2023-04-05 23:25:42.977524 fling_cli-0.1.6/README.md
--rw-r--r--   0        0        0      647 2023-05-21 21:48:46.490496 fling_cli-0.1.6/fling_cli/__init__.py
--rw-r--r--   0        0        0     2286 2023-05-21 21:47:47.016971 fling_cli-0.1.6/fling_cli/auth.py
--rw-r--r--   0        0        0        0 2023-04-04 19:06:55.600802 fling_cli-0.1.6/fling_cli/bin/__init__.py
--rw-r--r--   0        0        0     6306 2023-05-13 22:09:25.053951 fling_cli-0.1.6/fling_cli/bin/fling.py
--rw-r--r--   0        0        0     1492 2023-05-13 23:40:28.872299 fling_cli-0.1.6/fling_cli/certbot_fling_plugin.py
--rw-r--r--   0        0        0     3834 2023-04-08 02:13:26.640377 fling_cli-0.1.6/fling_cli/logo-hc.txt
--rw-r--r--   0        0        0      990 2023-05-21 21:48:40.064803 fling_cli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 fling_cli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2163 2023-05-29 16:33:04.320435 fling_cli-0.1.7/README.md
+-rw-r--r--   0        0        0      647 2023-05-29 18:11:00.736964 fling_cli-0.1.7/fling_cli/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-29 18:07:09.590966 fling_cli-0.1.7/fling_cli/auth.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:33:04.320851 fling_cli-0.1.7/fling_cli/bin/__init__.py
+-rw-r--r--   0        0        0     6390 2023-05-29 16:33:04.320953 fling_cli-0.1.7/fling_cli/bin/fling.py
+-rw-r--r--   0        0        0     1495 2023-05-29 16:33:04.321025 fling_cli-0.1.7/fling_cli/certbot_fling_plugin.py
+-rw-r--r--   0        0        0     3834 2023-05-29 16:33:04.321091 fling_cli-0.1.7/fling_cli/logo-hc.txt
+-rw-r--r--   0        0        0      990 2023-05-29 18:10:55.262278 fling_cli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 fling_cli-0.1.7/PKG-INFO
```

### Comparing `fling_cli-0.1.6/README.md` & `fling_cli-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.6/fling_cli/__init__.py` & `fling_cli-0.1.7/fling_cli/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 
 import keyring
 from click.exceptions import UsageError
 from fling_core import settings
 from fling_client.client import Client
```

### Comparing `fling_cli-0.1.6/fling_cli/auth.py` & `fling_cli-0.1.7/fling_cli/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import logging
 import os
 import random
 import signal
 import string
-from subprocess import call
 
 import keyring
 import uvicorn
 from fastapi import BackgroundTasks, FastAPI
 from fastapi.responses import HTMLResponse
 from starlette.responses import RedirectResponse
 from fling_core import settings
-import pathlib
+from pathlib import Path
+import webbrowser
 
 
 stored_state = None
 
 
 def make_app():
     app = FastAPI()
 
     @app.on_event("startup")
     async def login():
         global stored_state
         stored_state = ''.join(random.choice(string.ascii_letters) for i in range(20))
         authorization_url = f"{settings.api_server}/github-login?state={stored_state}"
         print("Going to GitHub authorization url in a browser window...")
-        call(f'sleep 0.1 && open "{authorization_url}"', shell=True)
+        webbrowser.open(authorization_url)
 
     @app.get("/callback")
     async def callback(state: str, token: str, username: str):
         # Die after this request finishes, no matter what
 
         if state != stored_state:
             raise Exception("State doesn't match, bad!")
-        print(f"Saving token for `{username}` to keyring.")
-        os.makedirs(pathlib.Path(pathlib.Path.home(), ".flingdev"), exist_ok=True)
-        with open(pathlib.Path(pathlib.Path.home(), ".flingdev", "flinguser.txt"), "w") as userfile:
+        os.makedirs(Path(Path.home(), ".flingdev"), exist_ok=True)
+        with open(Path(Path.home(), ".flingdev", "flinguser.txt"), "w+") as userfile:
+            userfile.write(username)
+        os.makedirs(Path("/Users", "Shared", ".loophost"), exist_ok=True)
+        with open(Path("/Users", "Shared", ".loophost", "flinguser.txt"), "w+") as userfile:
             userfile.write(username)
+        print(f"Saving token for `{username}` to keyring.")
         keyring.set_password("fling-github-token", username, token)
-        # default_password = keyring.get_password("fling-github-token", "system-default")
-        # if not default_password:
-        #     print(f"No default account, Saving token for `{username}` as default.")
         keyring.set_password("fling-github-token", "system-default", token)
         return RedirectResponse('http://localhost:5817', status_code=302)
 
     @app.get("/")
     def app_index(background_tasks: BackgroundTasks):
         background_tasks.add_task(signal.raise_signal, signal.SIGINT)
         return HTMLResponse(
@@ -56,14 +56,14 @@
 
 
 def gh_authenticate():
     temp_port = int(settings.local_cli_port)
     app = make_app()
     try:
         uvicorn.run(
-            app, host="0.0.0.0", port=temp_port, log_level=logging.CRITICAL)
+            app, host="0.0.0.0", port=temp_port, log_level=logging.DEBUG)  # log_level=logging.CRITICAL)
     finally:
         print("Ok.")
 
 
 if __name__ == "__main__":
     gh_authenticate()
```

### Comparing `fling_cli-0.1.6/fling_cli/bin/fling.py` & `fling_cli-0.1.7/fling_cli/bin/fling.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import hashlib
 from pathlib import Path
 import pathlib
 from fling_cli.auth import gh_authenticate
 from fling_cli import get_fling_client
 import rich_click as click
+import platform
 from click.exceptions import UsageError
 from rich import print, print_json
 from rich.tree import Tree
 from cookiecutter.main import cookiecutter
 from fling_client.api.names import generate_names_namer_get
 from fling_client.api.data import (
     add_data_fling_id_add_post,
@@ -48,17 +49,18 @@
 
 @click.group()
 @click.pass_context
 @click.option("-v", "--verbose", is_flag=True, default=False)
 def fling(ctx, verbose):
     ctx.ensure_object(dict)
     ctx.obj["verbose"] = verbose
-    logo_path = pathlib.Path(__file__).parent.parent / "logo-hc.txt"
-    with open(logo_path, "r") as logo:
-        print(f"[green]{logo.read()}[/green]", end="")
+    if not platform.system().lower().startswith('win'):
+        logo_path = pathlib.Path(__file__).parent.parent / "logo-hc.txt"
+        with open(logo_path, "r") as logo:
+            print(f"[green]{logo.read()}[/green]", end="")
     print()
 
 
 @fling.command(help="Authenticate with GitHub")
 @click.pass_context
 def auth(ctx):
     gh_authenticate()
```

### Comparing `fling_cli-0.1.6/fling_cli/certbot_fling_plugin.py` & `fling_cli-0.1.7/fling_cli/certbot_fling_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     del_txt_record_txt_record_delete,
 )
 
 
 class Authenticator(dns_common.DNSAuthenticator):
     """DNS Authenticator for Loophost
 
-    This Authenticator uses the Fling API to fulfill a dns-01 challenge on a *.fling.dev domain.
+    This Authenticator uses the Fling API to fulfill a dns-01 challenge on a *.loophost.dev domain.
     """
 
     description = "Obtain certificates for a loophost account"
     ttl = 60
     fling_client = None
 
     def more_info(self) -> str:
```

### Comparing `fling_cli-0.1.6/fling_cli/logo-hc.txt` & `fling_cli-0.1.7/fling_cli/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.6/pyproject.toml` & `fling_cli-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fling-cli"
-version = "0.1.6"
+version = "0.1.7"
 description = "Side Project Management from the command line"
 authors = ["Joshua McKenty <jmckenty@gmail.com>", "Anouk Ruhaak <anoukruhaak@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fling_cli"}]
 
 [tool.poetry.dependencies]
 click = "*"
```

### Comparing `fling_cli-0.1.6/PKG-INFO` & `fling_cli-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: Side Project Management from the command line
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

