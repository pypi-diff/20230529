# Comparing `tmp/loophost-0.2.9.tar.gz` & `tmp/loophost-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loophost-0.2.9.tar", max compression
+gzip compressed data, was "loophost-0.3.0.tar", max compression
```

## Comparing `loophost-0.2.9.tar` & `loophost-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,32 @@
--rw-r--r--   0        0        0       68 2023-05-22 20:54:45.002992 loophost-0.2.9/README.md
--rw-r--r--   0        0        0        5 2023-05-24 00:22:51.371190 loophost-0.2.9/VERSION
--rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 loophost-0.2.9/build.py
--rw-r--r--   0        0        0      669 2023-05-24 00:22:54.638480 loophost-0.2.9/loophost/__init__.py
--rw-r--r--   0        0        0     3762 2023-05-23 22:36:10.606608 loophost-0.2.9/loophost/flingroute.py
--rw-r--r--   0        0        0     1281 2023-05-23 04:59:46.905055 loophost-0.2.9/loophost/launchd_plist.py
--rwxr-xr-x   0        0        0  8045858 2023-05-23 06:12:56.942402 loophost-0.2.9/loophost/loopproxy
--rw-r--r--   0        0        0      904 2023-05-22 21:02:29.003769 loophost-0.2.9/loophost/plist/hub.plist.template
--rw-r--r--   0        0        0      771 2023-05-22 20:59:18.324250 loophost-0.2.9/loophost/plist/loophost.plist.template
--rw-r--r--   0        0        0     1150 2023-05-23 00:41:15.244678 loophost-0.2.9/loophost/plist/ssh.plist.template
--rw-r--r--   0        0        0     3611 2023-05-24 00:22:29.800259 loophost-0.2.9/loophost/postinstall.py
--rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 loophost-0.2.9/loophost/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 loophost-0.2.9/loophost/static/fling-logo-light.png
--rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 loophost-0.2.9/loophost/static/logo-hc.txt
--rw-r--r--   0        0        0    34153 2023-05-21 23:31:29.960428 loophost-0.2.9/loophost/static/logo-square.png
--rw-r--r--   0        0        0      828 2023-05-23 21:16:55.287812 loophost-0.2.9/loophost/templates/admin.html
--rw-r--r--   0        0        0     1606 2023-05-23 21:15:55.482064 loophost-0.2.9/loophost/templates/base.html
--rw-r--r--   0        0        0     1257 2023-05-23 21:14:15.086302 loophost-0.2.9/loophost/templates/local.html
--rw-r--r--   0        0        0     1474 2023-05-23 21:13:30.120822 loophost-0.2.9/loophost/templates/partials/apptable.html
--rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 loophost-0.2.9/loophost/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1604 2023-05-23 04:10:54.125164 loophost-0.2.9/loophost/uninstall.py
--rw-r--r--   0        0        0     1187 2023-05-24 00:22:48.491310 loophost-0.2.9/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 loophost-0.2.9/setup.py
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 loophost-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-05-29 17:20:30.603117 loophost-0.3.0/README.md
+-rw-r--r--   0        0        0        5 2023-05-29 17:28:43.194303 loophost-0.3.0/VERSION
+-rw-r--r--   0        0        0      670 2023-05-29 17:20:30.603221 loophost-0.3.0/build.py
+-rw-r--r--   0        0        0      930 2023-05-29 17:30:53.038781 loophost-0.3.0/loophost/__init__.py
+-rw-r--r--   0        0        0     4176 2023-05-29 17:20:30.603408 loophost-0.3.0/loophost/flingroute.py
+-rw-r--r--   0        0        0     3452 2023-05-29 17:20:30.603479 loophost-0.3.0/loophost/installer.py
+-rw-r--r--   0        0        0     1353 2023-05-29 17:20:30.603534 loophost-0.3.0/loophost/launchd_plist.py
+-rwxr-xr-x   0        0        0  8293472 2023-05-29 17:31:09.791237 loophost-0.3.0/loophost/loopproxy
+-rw-r--r--   0        0        0  8751616 2023-05-29 17:20:30.671610 loophost-0.3.0/loophost/loopproxy.exe
+-rw-r--r--   0        0        0      783 2023-05-29 17:20:30.671883 loophost-0.3.0/loophost/plist/hub.plist.template
+-rw-r--r--   0        0        0      771 2023-05-29 17:20:30.671967 loophost-0.3.0/loophost/plist/loophost.plist.template
+-rw-r--r--   0        0        0     1150 2023-05-29 17:20:30.672026 loophost-0.3.0/loophost/plist/ssh.plist.template
+-rw-r--r--   0        0        0      100 2023-05-29 17:20:30.672086 loophost-0.3.0/loophost/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-05-29 17:20:30.672552 loophost-0.3.0/loophost/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-05-29 17:20:30.673511 loophost-0.3.0/loophost/static/fling-logo-light.png
+-rw-r--r--   0        0        0     6393 2023-05-29 17:20:30.673568 loophost-0.3.0/loophost/static/github-mark.png
+-rw-r--r--   0        0        0     3834 2023-05-29 17:20:30.673629 loophost-0.3.0/loophost/static/logo-hc.txt
+-rw-r--r--   0        0        0    34153 2023-05-29 17:20:30.673803 loophost-0.3.0/loophost/static/logo-square.png
+-rw-r--r--   0        0        0      457 2023-05-29 17:20:30.673856 loophost-0.3.0/loophost/step_two.py
+-rw-r--r--   0        0        0      828 2023-05-29 17:20:30.673946 loophost-0.3.0/loophost/templates/admin.html
+-rw-r--r--   0        0        0     1657 2023-05-29 17:20:30.674006 loophost-0.3.0/loophost/templates/base.html
+-rw-r--r--   0        0        0     2921 2023-05-29 17:20:30.674069 loophost-0.3.0/loophost/templates/local.html
+-rw-r--r--   0        0        0     1478 2023-05-29 17:20:30.674160 loophost-0.3.0/loophost/templates/partials/apptable.html
+-rw-r--r--   0        0        0      289 2023-05-29 17:20:30.674219 loophost-0.3.0/loophost/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1656 2023-05-29 17:20:30.674299 loophost-0.3.0/loophost/uninstall.py
+-rw-r--r--   0        0        0      230 2023-05-29 17:20:30.674478 loophost-0.3.0/loophost/win/build.txt
+-rw-r--r--   0        0        0     2431 2023-05-29 17:20:30.674551 loophost-0.3.0/loophost/win_hub.py
+-rw-r--r--   0        0        0      828 2023-05-29 17:20:30.674606 loophost-0.3.0/loophost/win_hub.spec
+-rw-r--r--   0        0        0     2586 2023-05-29 17:20:30.674668 loophost-0.3.0/loophost/win_lp.py
+-rw-r--r--   0        0        0     1257 2023-05-29 17:32:28.000751 loophost-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-29 17:20:30.675256 loophost-0.3.0/setup.py
+-rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 loophost-0.3.0/PKG-INFO
```

### Comparing `loophost-0.2.9/build.py` & `loophost-0.3.0/build.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def build(setup_kwargs: Dict[str, Any]) -> None:
     print("Inside the Build method")
     setup_kwargs.update(
         {
             "zip_safe": False,
-            "build_golang": {"root": "github.com/10in30/loophost"},
+            "build_golang": {"root": "github.com/delving-co/loophost"},
             "ext_modules": [
                 Extension(
                     "loophost",
                     ["loophost/main.go"],
                     ["loophost/reverseproxy"],
                     py_limited_api=True,
                     define_macros=[("Py_LIMITED_API", None)],
```

### Comparing `loophost-0.2.9/loophost/flingroute.py` & `loophost-0.3.0/loophost/flingroute.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Loophost administration web app.
 This runs as a launchd-dispatched python web app.
 It displays a web-based administration screen.
-Must be run with a CWD of the .flingdev folder in the user's home directory.
+Must be run with a CWD of the .loophost folder.
 """
 
 import os
 import json
 import pathlib
 from fling.start import start
 from flask import Flask, request, render_template, redirect
 from flask_bootstrap import Bootstrap5
 from flask_caching import Cache
 from loophost.launchd_plist import register_tunnel, unregister_tunnel, generate_keys
 from loophost import HUBDIR, __version__, DATA_FILE_PATH
 from lastversion import has_update
 from fling_cli import get_fling_client
 from fling_client.api.loophost import expose_app_expose_app_put
+from flask_wtf.csrf import CSRFProtect
 
 
-config = json.loads(pathlib.Path.read_text(DATA_FILE_PATH))
+config = json.loads(pathlib.Path.read_text(DATA_FILE_PATH()))
 
 
 admin = Flask(__name__)
+admin.config["SECRET_KEY"] = config.get('SECRET_KEY', 'foobar')
+csrf = CSRFProtect(admin)
 bootstrap = Bootstrap5(admin)
 cache = Cache(config={"CACHE_TYPE": "SimpleCache"})
 cache.init_app(admin)
 admin.register_blueprint(start, url_prefix="/start")  # unused but I need the templates
 
 
 @cache.cached(timeout=3600)
@@ -34,74 +37,79 @@
 
 
 @admin.context_processor
 def inject_globals():
     return dict(NEW_VERSION=latest_version())
 
 
-@admin.route("/unbind")
-def unbind():
-    project = request.args.get("project")
-    if project and project in config["apps"]:
-        del config["apps"][project]
-        with open(DATA_FILE_PATH, "w+") as appjson:
-            appjson.write(json.dumps(config))
-    return redirect("/")
-
-
-@admin.route("/share")
-def share():
-    project = request.args.get("project")
-    target = pathlib.Path(
-        pathlib.Path.home(),
-        "Library",
-        "LaunchAgents",
-        f"dev.fling.hub.ssh.{project}.plist",
-    )
-
+def setup_tunnel_keys(project):
     if not os.path.exists("tunnelkey.pub"):
         # TODO(JMC): Don't do this so often
         fling_client = get_fling_client(require_auth=True)
         pub, priv = generate_keys()
         with open("tunnelkey.pub", "w+") as pubfile:
             pubfile.write(pub)
         with open("tunnelkey", "w+") as privfile:
             privfile.write(priv)
         os.chmod("tunnelkey", 0o600)
         expose_app_expose_app_put.sync(
             client=fling_client, app_name=project, ssh_public_key=pub
         )
 
+
+def unbind(project):
+    del config["apps"][project]
+    with open(DATA_FILE_PATH(), "w+") as appjson:
+        appjson.write(json.dumps(config))
+    return
+
+
+def share(project):
+    target = pathlib.Path(
+        pathlib.Path.home(),
+        "Library",
+        "LaunchAgents",
+        f"dev.fling.hub.ssh.{project}.plist",
+    )
+
     if project and project in config.get("share", {}):
         del config["share"][project]
         unregister_tunnel(target)
     elif project:
+        setup_tunnel_keys(project)
         if not config.get("share"):
             config["share"] = {}
         config["share"][project] = "public"
         register_tunnel(
             project, pathlib.Path(HUBDIR, "plist", "ssh.plist.template"), target
         )
-    with open(DATA_FILE_PATH, "w+") as appjson:
+    with open(DATA_FILE_PATH(), "w+") as appjson:
         appjson.write(json.dumps(config))
-    return redirect("/")
+    return redirect(f"/config/{project}")
 
 
 @admin.route("/config/<project>", methods=["GET", "POST"])
 def config_page(project):
-    if request.form.get("application_port"):
+    if project and project in config["apps"]:
+        print(f"Updating config for {project} with action {request.form.get('action')}")
+        if request.form.get("action") == "unbind":
+            unbind(project)
+            return redirect("/")
+        elif request.form.get("action") == "share":
+            share(project)
+    if request.form.get("application_port") and not request.form.get("action"):
         config["apps"][project] = request.form.get("application_port")
-        with open(DATA_FILE_PATH, "w+") as appjson:
+        with open(DATA_FILE_PATH(), "w+") as appjson:
             appjson.write(json.dumps(config))
 
     return render_template(
         "local.html",
         config=config,
         apps=config["apps"],
-        share=config.get("share"),
+        share=config.get("share", {}),
         project=project,
     )
 
 
 @admin.route("/", defaults={"path": ""}, methods=["GET", "POST"])
 @admin.route("/<path:path>", methods=["GET", "POST"])
 def admin_page(path):
@@ -115,8 +123,10 @@
             fqdn=".".join(fqdn),
         )
     project = fqdn.pop(0)
     return redirect(f"https://{config['fqdn']}/config/{project}")
 
 
 if __name__ == "__main__":
-    admin.run(host=f"unix://{os.getcwd()}/loophost.soc")
+    # admin.run(host=f"unix://{os.getcwd()}/loophost.soc")
+    admin.run(host=f"0.0.0.0", port=5816)
+
```

### Comparing `loophost-0.2.9/loophost/launchd_plist.py` & `loophost-0.3.0/loophost/launchd_plist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from io import StringIO
 import pathlib
 import shutil
-from loophost import LOOPHOST_DOMAIN, TUNNEL_DOMAIN, TARGET_DIR, PYEX, HUBDIR, USERNAME
+from loophost import LOOPHOST_DOMAIN, TUNNEL_DOMAIN, PYEX, HUBDIR, GET_FLINGUSER_NAME, GET_LOOPHOST_DIR
 from string import Template
 from subprocess import run
 import paramiko
 
 
 def generate_keys():
     key = paramiko.RSAKey.generate(2048)
     privateString = StringIO()
     key.write_private_key(privateString)
     return f"{key.get_name()} {key.get_base64()}", privateString.getvalue()
 
 
 def register_tunnel(project, template_path, target_path):
+    TARGET_DIR = GET_LOOPHOST_DIR()
     shutil.copy2(template_path, TARGET_DIR)
 
     d = {"CWD": TARGET_DIR,
-         "USERNAME": USERNAME,
+         "USERNAME": GET_FLINGUSER_NAME(),
          "PYEX": PYEX,
          "HUBDIR": HUBDIR,
          "LOOPHOST_DOMAIN": LOOPHOST_DOMAIN,
          "TUNNEL_DOMAIN": TUNNEL_DOMAIN,
          "LOCAL_USER": pathlib.Path('localuser.txt').read_text().strip(),
          "PROJECT": project}
 
@@ -33,9 +34,9 @@
             o.write(result)
 
     run(["launchctl", "unload", target_path], cwd=TARGET_DIR)
     run(["launchctl", "load", target_path], cwd=TARGET_DIR)
 
 
 def unregister_tunnel(target_path):
-    run(["launchctl", "unload", target_path], cwd=TARGET_DIR)
+    run(["launchctl", "unload", target_path], cwd=GET_LOOPHOST_DIR())
     shutil.rmtree(target_path, ignore_errors=True)
```

### Comparing `loophost-0.2.9/loophost/plist/hub.plist.template` & `loophost-0.3.0/loophost/plist/hub.plist.template`

 * *Files 13% similar despite different names*

#### Comparing `loophost-0.2.9/loophost/plist/hub.plist.template` & `loophost-0.3.0/loophost/plist/hub.plist.template`

```diff
@@ -5,20 +5,16 @@
 <plist version="1.0">
   <dict>
     <key>Label</key>
     <string>dev.fling.hub</string>
     <key>ProgramArguments</key>
     <array>
       <string>${HUBDIR}/loopproxy</string>
-    </array>
-    <key>EnvironmentVariables</key>
-    <dict>
-      <key>LOOPHOST_DATA_PATH</key>
       <string>${CWD}</string>
-    </dict>
+    </array>
     <key>RunAtLoad</key>
     <true/>
     <key>KeepAlive</key>
     <true/>
     <key>WorkingDirectory</key>
     <string>${CWD}</string>
     <key>StandardInPath</key>
```

### Comparing `loophost-0.2.9/loophost/plist/loophost.plist.template` & `loophost-0.3.0/loophost/plist/loophost.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.9/loophost/plist/ssh.plist.template` & `loophost-0.3.0/loophost/plist/ssh.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-0.2.9/loophost/postinstall.py` & `loophost-0.3.0/loophost/installer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,66 @@
+import getpass
 import json
 import os
+import platform
 import sys
 import pathlib
 import subprocess
 from subprocess import run
+import webbrowser
 from certbot.main import main as certmain
 from fling_cli.auth import gh_authenticate
+
 from loophost.launchd_plist import register_tunnel
 from loophost import (
     LOOPHOST_DOMAIN,
     TUNNEL_DOMAIN,
-    TARGET_DIR,
     HUBDIR,
-    USERNAME,
+    GET_LOOPHOST_DIR,
+    GET_FLINGUSER_NAME,
     DATA_FILE_PATH,
 )
 
 
 def post_install_one():
-    global USERNAME
     print("Installing LoopHost...")
-    os.makedirs(pathlib.Path(TARGET_DIR), exist_ok=True)
-    os.chdir(TARGET_DIR)
-    with open("localuser.txt", "w+") as userfile:
-        userfile.write(os.getenv("USER"))
+    localuser_file = pathlib.Path(GET_LOOPHOST_DIR(), "localuser.txt")
+    with open(localuser_file, "w+") as userfile:
+        userfile.write(getpass.getuser())
     authenticate_with_fling()
-    with open(pathlib.Path(TARGET_DIR, "flinguser.txt"), "r") as userfile:
-        USERNAME = userfile.read()
-    issue_certs()
+    if not platform.system().lower().startswith('win'):
+        issue_certs()
     create_update_loophost_json()
     register_tunnel(
         "flinghub",
         pathlib.Path(HUBDIR, "plist", "loophost.plist.template"),
         pathlib.Path(
             pathlib.Path.home(), "Library/LaunchAgents/dev.fling.hub.local.plist"
         ),
     )
 
-    restart_as_sudo()
+    step_two_as_root()
 
 
 def post_install_two():
+    if platform.system().lower().startswith('win'):
+        issue_certs()
     setup_launchd_scripts()
 
 
 def authenticate_with_fling():
-    global USERNAME
-    if not os.path.exists(pathlib.Path(TARGET_DIR, "flinguser.txt")):
+    if not GET_FLINGUSER_NAME():
         gh_authenticate()
-    if not os.path.exists(pathlib.Path(TARGET_DIR, "flinguser.txt")):
+    if not GET_FLINGUSER_NAME():
         raise Exception("Github authentication failed, can't continue install.")
-    with open(pathlib.Path(TARGET_DIR, "flinguser.txt"), "r") as userfile:
-        USERNAME = userfile.read()
+
 
 
 def issue_certs():
-    global USERNAME, TARGET_DIR
+    USERNAME = GET_FLINGUSER_NAME()
     print("Generating SSL certificates (this may take a minute)...")
     cmd = [
             "certonly",
             "--config-dir", "./",
             "--work-dir", "./",
             "--logs-dir", "./",
             "--non-interactive",
@@ -68,63 +69,60 @@
             f"-m webmaster@{LOOPHOST_DOMAIN}",
             "--authenticator=fling_authenticator",
             f'-d *.{USERNAME}.{LOOPHOST_DOMAIN}',
             f'-d *.{USERNAME}.{TUNNEL_DOMAIN}',
             f'-d {USERNAME}.{LOOPHOST_DOMAIN}',
             "--fling_authenticator-propagation-seconds=15",
         ]
-    # print(cmd)
+    
     certmain(cmd)
 
 
 def create_update_loophost_json():
+    USERNAME = GET_FLINGUSER_NAME()
     data = None
-    if os.path.exists(DATA_FILE_PATH):
-        with open(DATA_FILE_PATH, "r") as datafile:
+    if os.path.exists(DATA_FILE_PATH()):
+        with open(DATA_FILE_PATH(), "r") as datafile:
             data = json.loads(datafile.read())
     else:
         data = {"apps": {}, "share": {}}
     data.update(
         {
             "fqdn": f"{USERNAME}.{LOOPHOST_DOMAIN}",
             "tunnel": f"{USERNAME}.{TUNNEL_DOMAIN}",
         }
     )
-    with open(DATA_FILE_PATH, "w") as datafile:
+    with open(DATA_FILE_PATH(), "w") as datafile:
         datafile.write(json.dumps(data))
     return data
 
 
 def setup_launchd_scripts():
     register_tunnel(
         "flinghub",
         pathlib.Path(HUBDIR, "plist", "hub.plist.template"),
         "/Library/LaunchDaemons/dev.fling.hub.plist",
     )
     print("All done.")
 
 
-def restart_as_sudo():
-    global USERNAME
+def step_two_as_root():
     print(
-        """Switching to root user to install web services on ports 443 and 80\n\r
+        """Switching to root/admin user to install web services on ports 443 and 80\n\r
         (you will be prompted for your password)"""
     )
+    cmd = "sudo python3 -m loophost.step_two"
+    if platform.system().lower().startswith('win'):
+        cmd = "python3 -m loophost.step_two"
     run(
-        "sudo python3 -m loophost.postinstall",
+        cmd,
         shell=True,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        stdin=subprocess.PIPE,
-        cwd=TARGET_DIR,
+        # stdout=subprocess.PIPE,
+        # stderr=subprocess.PIPE,
+        # stdin=subprocess.PIPE,
+        cwd=GET_LOOPHOST_DIR(),
+        check=True
     )
     print("All finished.")
-    run(f"""/usr/bin/open "https://{USERNAME}.{LOOPHOST_DOMAIN}" """, shell=True)
+    webbrowser.open(f"https://{GET_FLINGUSER_NAME()}.{LOOPHOST_DOMAIN}")
     sys.exit()
 
-
-if __name__ == "__main__":
-    # TODO: Make this impotent and reentrant safe
-    if os.geteuid() == 0:
-        post_install_two()
-    else:
-        post_install_one()
```

### Comparing `loophost-0.2.9/loophost/static/fling-logo-dark.png` & `loophost-0.3.0/loophost/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.9/loophost/static/fling-logo-light.png` & `loophost-0.3.0/loophost/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.9/loophost/static/logo-hc.txt` & `loophost-0.3.0/loophost/static/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `loophost-0.2.9/loophost/static/logo-square.png` & `loophost-0.3.0/loophost/static/logo-square.png`

 * *Files identical despite different names*

### Comparing `loophost-0.2.9/loophost/templates/admin.html` & `loophost-0.3.0/loophost/templates/admin.html`

 * *Files identical despite different names*

### Comparing `loophost-0.2.9/loophost/templates/base.html` & `loophost-0.3.0/loophost/templates/base.html`

 * *Files 18% similar despite different names*

```diff
@@ -43,17 +43,17 @@
   </script>
 <footer class="footer mt-auto py-3 bg-light">
   <div class="container">
   <div class="row justify-content-between">
     <div class="col col-12 col-lg-3 text-end">
         <a href="/">Home</a>
         <a href="https://readthedocs.org/loophost">Docs</a>
-        <a href="https://github.com/delving-co/loophost">Open Source</a>
+        <a href="https://github.com/delving-co/loophost"><img src="/static/github-mark.png" style="max-width: 32px;"></a>
     </div>
-    <div class="col col-12 col-lg-3 text-end">
+    <div class="col col-12 col-lg-4 text-start">
         <span class="text-muted">Another fun project from <a href="https://github.com/delving-co">delving</a>.</span>
     </div>
   </div>
 </footer>
 {% endblock %}
 </div>
 </body>
```

#### html2text {}

```diff
@@ -3,11 +3,11 @@
  {% endblock %} {% block body %}
 {% include "partials/upgrade.html" %}
 {% block headline %} {% endblock %}
 [/static/logo-square.png]
 {% block content %} {{ super() }} {% endblock %} {% block scripts %} {{ super()
 }}
 
-Home Docs Open_Source
+Home Docs [/static/github-mark.png]
 Another fun project from delving.
  {% endblock %}
 {% endblock %}
```

### Comparing `loophost-0.2.9/loophost/uninstall.py` & `loophost-0.3.0/loophost/uninstall.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import os
 from pathlib import Path
 import shutil
 from subprocess import run
 import subprocess
 import sys
-from loophost import TARGET_DIR, USERNAME
+from loophost import GET_LOOPHOST_DIR, GET_FLINGUSER_NAME
 
 
 def uninstall_one():
     if not os.path.exists(Path("localuser.txt")):
         print("Seems to have already been uninstalled")
         exit(0)
     LOCAL_USER = Path("localuser.txt").read_text().strip()
     for service in Path("/Users", LOCAL_USER, "Library", "LaunchAgents").glob(
         "dev.fling.hub*"
     ):
-        run(["launchctl", "unload", service], cwd=TARGET_DIR)
+        run(["launchctl", "unload", service], cwd=GET_LOOPHOST_DIR())
         os.unlink(service)
     os.chdir(Path("/Users", LOCAL_USER))
     restart_as_sudo()
 
 
 def uninstall_two():
     for service in Path("/Library", "LaunchDaemons").glob("dev.fling.hub*"):
-        run(["launchctl", "unload", service], cwd=TARGET_DIR)
+        run(["launchctl", "unload", service], cwd=GET_LOOPHOST_DIR())
         os.unlink(service)
-    shutil.rmtree(TARGET_DIR)
-    os.makedirs(TARGET_DIR, exist_ok=True)
-    with open(Path(TARGET_DIR, "flinguser.txt"), "w+") as userfile:
-        userfile.write(USERNAME)
+    # shutil.rmtree(TARGET_DIR)
+    # os.makedirs(TARGET_DIR, exist_ok=True)
+    # with open(Path(TARGET_DIR, "flinguser.txt"), "w+") as userfile:
+    #     userfile.write(GET_FLINGUSER_NAME())
 
 
 def restart_as_sudo():
     print(
         """Switching to root user to uninstall web services \n\n
         (you will be prompted for your password)"""
     )
```

### Comparing `loophost-0.2.9/pyproject.toml` & `loophost-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel", "setuptools-cpp", "setuptools-golang"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "loophost"
-version = "0.2.9"
+version = "0.3.0"
 description = "Loophost: for a better local dev"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 include = [{ path = "VERSION" }, 
             { path = "README.md" }, 
             { path = "setup.py" }, 
             { path = "build.py" }, 
             { path = "loophost/templates" }, 
             { path = "loophost/static" }, 
             { path = "loophost/loopproxy"}, 
+            { path = "loophost/loopproxy.exe"}, 
             { path = "loophost/plist/*.plist.template"}] 
 packages = [
     { include = "loophost", format = ["wheel"] },
 ]
 build = "build.py"
 
 [tool.poetry.urls]
@@ -37,7 +38,8 @@
 python = "^3.9"
 fling-start = "^0.1.14"
 fling-cli = "^0.1.5"
 certbot = "^2.6.0"
 flask = "^2.3.2"
 lastversion = "^2.4.15"
 paramiko = "^3.1.0"
+flask-wtf = "^1.1.1"
```

### Comparing `loophost-0.2.9/PKG-INFO` & `loophost-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: loophost
-Version: 0.2.9
+Version: 0.3.0
 Summary: Loophost: for a better local dev
 License: Apache-2.0
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certbot (>=2.6.0,<3.0.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: flask-wtf (>=1.1.1,<2.0.0)
 Requires-Dist: fling-cli (>=0.1.5,<0.2.0)
 Requires-Dist: fling-start (>=0.1.14,<0.2.0)
 Requires-Dist: lastversion (>=2.4.15,<3.0.0)
 Requires-Dist: paramiko (>=3.1.0,<4.0.0)
 Project-URL: documentation, https://readthedocs.org/loophost
 Project-URL: homepage, https://loophost.dev
 Project-URL: repository, https://github.com/delving-co/loophost.git
```

