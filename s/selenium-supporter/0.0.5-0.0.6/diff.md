# Comparing `tmp/selenium-supporter-0.0.5.tar.gz` & `tmp/selenium-supporter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-supporter-0.0.5.tar", last modified: Sun May 28 01:51:12 2023, max compression
+gzip compressed data, was "selenium-supporter-0.0.6.tar", last modified: Mon May 29 15:45:38 2023, max compression
```

## Comparing `selenium-supporter-0.0.5.tar` & `selenium-supporter-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 01:51:12.756601 selenium-supporter-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1939 2023-05-28 01:51:12.755601 selenium-supporter-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1675 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 01:51:12.753601 selenium-supporter-0.0.5/selenium_supporter/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/selenium_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9181 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/selenium_supporter/drivers.py
--rw-r--r--   0 root         (0) root         (0)     9302 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/selenium_supporter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 01:51:12.755601 selenium-supporter-0.0.5/selenium_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1939 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 01:51:12.756601 selenium-supporter-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:45:38.303728 selenium-supporter-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-29 15:45:38.302728 selenium-supporter-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-05-29 15:45:37.000000 selenium-supporter-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:45:38.301728 selenium-supporter-0.0.6/selenium_supporter/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-29 15:45:37.000000 selenium-supporter-0.0.6/selenium_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9181 2023-05-29 15:45:37.000000 selenium-supporter-0.0.6/selenium_supporter/drivers.py
+-rw-r--r--   0 root         (0) root         (0)     9725 2023-05-29 15:45:37.000000 selenium-supporter-0.0.6/selenium_supporter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:45:38.302728 selenium-supporter-0.0.6/selenium_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-29 15:45:38.000000 selenium-supporter-0.0.6/selenium_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-29 15:45:38.000000 selenium-supporter-0.0.6/selenium_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 15:45:38.000000 selenium-supporter-0.0.6/selenium_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 15:45:38.000000 selenium-supporter-0.0.6/selenium_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-29 15:45:38.000000 selenium-supporter-0.0.6/selenium_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-29 15:45:38.000000 selenium-supporter-0.0.6/selenium_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 15:45:38.303728 selenium-supporter-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-05-29 15:45:37.000000 selenium-supporter-0.0.6/setup.py
```

### Comparing `selenium-supporter-0.0.5/PKG-INFO` & `selenium-supporter-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-supporter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Selenium supporter
 Home-page: https://github.com/automatethem/selenium-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `selenium-supporter-0.0.5/README.md` & `selenium-supporter-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `selenium-supporter-0.0.5/selenium_supporter/drivers.py` & `selenium-supporter-0.0.6/selenium_supporter/drivers.py`

 * *Files identical despite different names*

### Comparing `selenium-supporter-0.0.5/selenium_supporter/utils.py` & `selenium-supporter-0.0.6/selenium_supporter/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,27 +22,32 @@
 import time
 import sys
 from python_supporter import logging
 import getpass
 import traceback
 
 def get_chrome_web_browser_path():
-    #windows 7
-    path1 = "C:\Program Files\Google\Chrome\Application\\chrome.exe"
-    path2 = "C:\\Program Files (x86)\\Google\\Chrome\\Application\\chrome.exe"
-    #windows 10
-    home = str(Path.home())
-    #print(home) #C:\Users\hello
-    path3 = home + "\\AppData\\Local\\Google\\Chrome\Application\\chrome.exe"
-    if os.path.exists(path1):
-        return path1
-    elif os.path.exists(path2):
-        return path2
-    elif os.path.exists(path3):
-        return path3
+    if platform.system() == 'Darwin': #맥
+        return "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome"
+    elif platform.system() == 'Windows': #윈도우
+        #windows 7
+        path1 = "C:\Program Files\Google\Chrome\Application\\chrome.exe"
+        path2 = "C:\\Program Files (x86)\\Google\\Chrome\\Application\\chrome.exe"
+        #windows 10
+        home = str(Path.home())
+        #print(home) #C:\Users\hello
+        path3 = home + "\\AppData\\Local\\Google\\Chrome\Application\\chrome.exe"
+        if os.path.exists(path1):
+            return path1
+        elif os.path.exists(path2):
+            return path2
+        elif os.path.exists(path3):
+            return path3
+    elif platform.system() == 'Linux': #리눅스 (구글 콜랩)
+        return ""
 
 def kill_all_chrome_web_browser_processes():
     if platform.system() == 'Darwin': #맥
         pass
     elif platform.system() == 'Windows': #윈도우
         #https://stackoverflow.com/questions/57792469/kill-certain-chrome-process-in-python-not-all
         subprocess.call("TASKKILL /f /IM CHROME.EXE")
@@ -63,48 +68,32 @@
     user_data_dir_option = ""
     if user_data_dir:
         user_data_dir_option = f"--user-data-dir={user_data_dir}"
     #https://www.chromium.org/developers/design-documents/network-stack/socks-proxy/
     proxy_server_option = ""
     if proxy_server:
         proxy_server_option = f"--proxy-server={proxy_server}"
-    subprocess.Popen(f'{chrome_web_browser_path} {user_data_dir_option} {proxy_server_option}  --disk-cache-dir=null --disk-cache-size=0') 
+    #subprocess.Popen(f'{chrome_web_browser_path} {user_data_dir_option} {proxy_server_option}  --disk-cache-dir=null --disk-cache-size=0') 
+    subprocess.Popen([chrome_web_browser_path, f"{user_data_dir_option} {proxy_server_option}  --disk-cache-dir=null --disk-cache-size=0"]) 
 
 def open_chrome_web_browser_with_remote_debugging_mode(remote_debugging_port, remote_debugging_address, user_data_dir=None, proxy_server=None, headless=False):
     chrome_web_browser_path = get_chrome_web_browser_path()
     #https://not-to-be-reset.tistory.com/454
     user_data_dir_option = ""
     if user_data_dir:
         user_data_dir_option = f"--user-data-dir={user_data_dir}"
     #https://www.chromium.org/developers/design-documents/network-stack/socks-proxy/
     proxy_server_option = ""
     if proxy_server:
         proxy_server_option = f"--proxy-server={proxy_server}"
     headless_option = ""
     if headless:
         headless_option = f"--headless={headless}"
-    subprocess.Popen(f'{chrome_web_browser_path} --remote-debugging-port={remote_debugging_port} --remote-debugging-address={remote_debugging_address} {user_data_dir_option} {proxy_server_option} {headless_option} --disk-cache-dir=null --disk-cache-size=0') 
-    
-'''    
-def check_port_open(ip, port):
-    tcp_sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    tcp_result = tcp_sock.connect_ex((ip, port))
-    tcp_sock.close()
-    #print(tcp_result)
-
-    if tcp_result == 0:
-        return True
-    else:
-        return False
-'''
-    
-    
-    
-
-    
+    subprocess.Popen([chrome_web_browser_path, f'--remote-debugging-port={remote_debugging_port} --remote-debugging-address={remote_debugging_address} {user_data_dir_option} {proxy_server_option} {headless_option} --disk-cache-dir=null --disk-cache-size=0']) 
+    #subprocess.Popen(f'{chrome_web_browser_path} --remote-debugging-port={remote_debugging_port} --remote-debugging-address={remote_debugging_address} {user_data_dir_option} {proxy_server_option} {headless_option} --disk-cache-dir=null --disk-cache-size=0') #윈도우 ok 
 
 def save_partial_screenshot(element, image_file):
     #'''
     png = element.screenshot_as_png
     with open(image_file, "wb") as f:
         f.write(png)
     #'''
```

### Comparing `selenium-supporter-0.0.5/selenium_supporter.egg-info/PKG-INFO` & `selenium-supporter-0.0.6/selenium_supporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-supporter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Selenium supporter
 Home-page: https://github.com/automatethem/selenium-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `selenium-supporter-0.0.5/setup.py` & `selenium-supporter-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='selenium-supporter',
-	version='0.0.5',
+	version='0.0.6',
 	description='Selenium supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/selenium-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

