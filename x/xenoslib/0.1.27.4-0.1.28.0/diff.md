# Comparing `tmp/xenoslib-0.1.27.4.tar.gz` & `tmp/xenoslib-0.1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.27.4.tar", last modified: Wed May 24 00:59:25 2023, max compression
+gzip compressed data, was "xenoslib-0.1.28.0.tar", last modified: Mon May 29 02:18:45 2023, max compression
```

## Comparing `xenoslib-0.1.27.4.tar` & `xenoslib-0.1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:59:25.414214 xenoslib-0.1.27.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 00:59:25.414214 xenoslib-0.1.27.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 00:59:25.414214 xenoslib-0.1.27.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:59:25.414214 xenoslib-0.1.27.4/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-24 00:59:14.000000 xenoslib-0.1.27.4/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:59:25.414214 xenoslib-0.1.27.4/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 00:59:25.000000 xenoslib-0.1.27.4/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-24 00:59:25.000000 xenoslib-0.1.27.4/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:59:25.000000 xenoslib-0.1.27.4/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 00:59:25.000000 xenoslib-0.1.27.4/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 00:59:25.000000 xenoslib-0.1.27.4/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:18:45.474703 xenoslib-0.1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-29 02:18:45.474703 xenoslib-0.1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:18:45.474703 xenoslib-0.1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:18:45.474703 xenoslib-0.1.28.0/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-29 02:18:33.000000 xenoslib-0.1.28.0/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:18:45.474703 xenoslib-0.1.28.0/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-29 02:18:45.000000 xenoslib-0.1.28.0/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 02:18:45.000000 xenoslib-0.1.28.0/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:18:45.000000 xenoslib-0.1.28.0/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 02:18:45.000000 xenoslib-0.1.28.0/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 02:18:45.000000 xenoslib-0.1.28.0/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.27.4/LICENSE` & `xenoslib-0.1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/README.md` & `xenoslib-0.1.28.0/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/setup.py` & `xenoslib-0.1.28.0/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/xenoslib/base.py` & `xenoslib-0.1.28.0/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/xenoslib/dev.py` & `xenoslib-0.1.28.0/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/xenoslib/extend.py` & `xenoslib-0.1.28.0/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/xenoslib/linux.py` & `xenoslib-0.1.28.0/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/xenoslib/mail.py` & `xenoslib-0.1.28.0/xenoslib/mail.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.imap_server = imap_server
         self.mail_addr = mail_addr
         self.mail_pwd = mail_pwd
         self.days = days
 
         self.msg_ids = deque(maxlen=999)
         if skip_current:  # mark and skip current mails
-            logger.debug("Skipping exists mails...")
+            logger.debug("Skipping existing emails...")
             mails = self.fetch_emails()
             self.msg_ids.extend(mails.keys())
         return self.fetching(interval=interval)
 
     def fetching(self, interval=30):
         """Continuously fetch emails at the specified interval."""
         logger.debug("Start checking emails...")
```

### Comparing `xenoslib-0.1.27.4/xenoslib/mock.py` & `xenoslib-0.1.28.0/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/xenoslib/onedrive.py` & `xenoslib-0.1.28.0/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/xenoslib/win_trayicon.py` & `xenoslib-0.1.28.0/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.4/xenoslib/windows.py` & `xenoslib-0.1.28.0/xenoslib/windows.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,53 +4,14 @@
 import sys
 import ctypes
 import time
 import msvcrt
 import winreg
 
 
-def refresh():
-    """refresh after update registry"""
-    HWND_BROADCAST = 0xFFFF
-    WM_SETTINGCHANGE = 0x1A
-    SMTO_ABORTIFHUNG = 0x0002
-
-    result = ctypes.c_long()
-    ctypes.windll.user32.SendMessageTimeoutW(
-        HWND_BROADCAST,
-        WM_SETTINGCHANGE,
-        0,
-        "Environment",
-        SMTO_ABORTIFHUNG,
-        5000,
-        ctypes.byref(result),
-    )
-
-
-def add_windows_path_env(new_path):
-    """add directory to Windows path environment variable"""
-    print("add dircetory to path: %s" % new_path)
-    path_key = winreg.OpenKey(
-        winreg.HKEY_LOCAL_MACHINE,
-        r"SYSTEM\CurrentControlSet\Control\Session Manager\Environment",
-        0,
-        winreg.KEY_ALL_ACCESS,
-    )
-    path_str, _ = winreg.QueryValueEx(path_key, "Path")
-    path_list = path_str.split(";")
-    if new_path in path_list:
-        print("%s exists" % new_path)
-    else:
-        print("added %s" % new_path)
-        path_list.append(new_path)
-        new_path = ";".join(path_list)
-        winreg.SetValueEx(path_key, "Path", 0, winreg.REG_EXPAND_SZ, new_path)
-    # refresh()
-
-
 class RunAsAdmin:
     """
     Usage: RunAsAdmin(main, cmd=True)
     """
 
     @staticmethod
     def is_admin():
@@ -94,7 +55,81 @@
 def timeout(seconds):
     for second in range(seconds - 1, -1, -1):
         if msvcrt.kbhit():
             break
         print(f"Waiting {second}s , press any key to continue...", end="\r")
         time.sleep(1)
     print()  # make sure the message won't be covered
+
+
+class Environment:
+    reg_path = r"SYSTEM\CurrentControlSet\Control\Session Manager\Environment"
+
+    def __init__(self):
+        pass
+
+    def refresh(self):
+        """refresh environment after updated"""
+        HWND_BROADCAST = 0xFFFF
+        WM_SETTINGCHANGE = 0x1A
+        SMTO_ABORTIFHUNG = 0x0002
+
+        result = ctypes.c_long()
+        ctypes.windll.user32.SendMessageTimeoutW(
+            HWND_BROADCAST,
+            WM_SETTINGCHANGE,
+            0,
+            "Environment",
+            SMTO_ABORTIFHUNG,
+            5000,
+            ctypes.byref(result),
+        )
+
+    def set(self, key, value):
+        print(f"Setting [{key}] to windows environment...")
+        with winreg.OpenKey(
+            winreg.HKEY_LOCAL_MACHINE, self.reg_path, 0, winreg.KEY_ALL_ACCESS
+        ) as reg_key:
+            winreg.SetValueEx(reg_key, key, 0, winreg.REG_EXPAND_SZ, value)
+            self.refresh()
+            print(f"Setted [{key}] to windows environment.")
+
+    def get(self, key):
+        with winreg.OpenKey(
+            winreg.HKEY_LOCAL_MACHINE, self.reg_path, 0, winreg.KEY_ALL_ACCESS
+        ) as reg_key:
+            value, _ = winreg.QueryValueEx(reg_key, key)
+            return value
+
+    def update(self, environs):
+        for key, value in environs.items():
+            self.set(key, value)
+            # print(key, value)
+
+
+def add_windows_path_env(new_path):
+    """Add directory to Windows path environment variable"""
+    env = Environment()
+    path_str = env.get("Path")
+    path_list = path_str.split(";")
+    if new_path in path_list:
+        print(f"{new_path} already exists in the path, skip.")
+        return False
+    else:
+        path_list.append(new_path)
+        new_path_list = ";".join(path_list)
+        try:
+            env.set("Path", new_path_list)
+            print(f"Added {new_path} to the path")
+            return True
+        except Exception as exc:
+            print(f"Failed to update the path: {str(exc)}")
+            return False
+
+
+def test():
+    add_windows_path_env("c:\\abc")
+    pause()
+
+
+if __name__ == "__main__":
+    RunAsAdmin(test, cmd=True)
```

