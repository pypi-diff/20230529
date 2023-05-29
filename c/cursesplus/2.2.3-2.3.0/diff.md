# Comparing `tmp/cursesplus-2.2.3.tar.gz` & `tmp/cursesplus-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.2.3.tar", last modified: Thu May 18 16:18:54 2023, max compression
+gzip compressed data, was "cursesplus-2.3.0.tar", last modified: Mon May 29 19:43:03 2023, max compression
```

## Comparing `cursesplus-2.2.3.tar` & `cursesplus-2.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:18:54.381146 cursesplus-2.2.3/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.2.3/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1712 2023-05-18 16:18:54.381146 cursesplus-2.2.3/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1109 2023-05-18 16:14:16.000000 cursesplus-2.2.3/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-18 16:18:29.000000 cursesplus-2.2.3/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-18 16:18:54.381146 cursesplus-2.2.3/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:18:54.381146 cursesplus-2.2.3/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      441 2023-05-18 15:57:38.000000 cursesplus-2.2.3/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:18:54.381146 cursesplus-2.2.3/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.2.3/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    12449 2023-05-18 16:18:20.000000 cursesplus-2.2.3/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.2.3/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.2.3/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:18:54.381146 cursesplus-2.2.3/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1712 2023-05-18 16:18:54.000000 cursesplus-2.2.3/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-18 16:18:54.000000 cursesplus-2.2.3/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-18 16:18:54.000000 cursesplus-2.2.3/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-18 16:18:54.000000 cursesplus-2.2.3/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 19:43:03.296406 cursesplus-2.3.0/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.0/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1413 2023-05-29 19:43:03.296406 cursesplus-2.3.0/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      810 2023-05-29 19:42:38.000000 cursesplus-2.3.0/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-29 19:40:43.000000 cursesplus-2.3.0/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-29 19:43:03.296406 cursesplus-2.3.0/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 19:43:03.286406 cursesplus-2.3.0/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      313 2023-05-29 19:28:28.000000 cursesplus-2.3.0/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 19:43:03.296406 cursesplus-2.3.0/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.0/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    15024 2023-05-29 19:39:12.000000 cursesplus-2.3.0/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.0/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.0/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-29 19:43:03.296406 cursesplus-2.3.0/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1413 2023-05-29 19:43:03.000000 cursesplus-2.3.0/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-29 19:43:03.000000 cursesplus-2.3.0/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-29 19:43:03.000000 cursesplus-2.3.0/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-29 19:43:03.000000 cursesplus-2.3.0/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.2.3/LICENSE` & `cursesplus-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.2.3/PKG-INFO` & `cursesplus-2.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.2.3
+Version: 2.3.0
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,33 +23,19 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Version 2.2: Progressbar
+### Version 2.3: New Input
 
--Add ProgressBarTypes enum-class
+-Rewrite cursesinput function
 
--Add ProgressBarLocation enum-class
-
--You can now have a small progress bar that does not clear the screen
-
--displaymsg() will no longer clear itself.
-
-**-WARNING! This update may break progress bars.**
-
-### Version 2.1: Files 'n' Folders
-
--Add openfolderdialog()
-
--Change colours
-
--Performance improvements for all methods
+-Remains backwards-compatible
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 
 -Rewrite colour system. load_colours() is now nonexistent.
```

### Comparing `cursesplus-2.2.3/README.md` & `cursesplus-2.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -9,33 +9,19 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Version 2.2: Progressbar
+### Version 2.3: New Input
 
--Add ProgressBarTypes enum-class
+-Rewrite cursesinput function
 
--Add ProgressBarLocation enum-class
-
--You can now have a small progress bar that does not clear the screen
-
--displaymsg() will no longer clear itself.
-
-**-WARNING! This update may break progress bars.**
-
-### Version 2.1: Files 'n' Folders
-
--Add openfolderdialog()
-
--Change colours
-
--Performance improvements for all methods
+-Remains backwards-compatible
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 
 -Rewrite colour system. load_colours() is now nonexistent.
```

### Comparing `cursesplus-2.2.3/pyproject.toml` & `cursesplus-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.2.3"
+version = "2.3.0"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.2.3/src/cursesplus/__init__.py` & `cursesplus-2.3.0/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.2.3/src/cursesplus/cp.py` & `cursesplus-2.3.0/src/cursesplus/cp.py`

 * *Files 14% similar despite different names*

```diff
@@ -102,36 +102,108 @@
     stdscr.addstr(0,0,"Message: ")
     mi = -(len(message)/2)
     
     for msgl in message:
         mi += 1
         stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl)
     stdscr.refresh()
-    
+def __retr_nbl_lst(input:list)->list:
+    return [l for l in input if str(l) != ""]  
+def __shft_lst(input:list)->list:
+    xl = [i for i in input if str(i) != ""]
+    return xl + ["" for _ in range(1000-len(xl))]
 
-def cursesinput(stdscr,prompt: str):
+def cursesinput(stdscr,prompt: str,lines=1,maxlen=0) -> str:
     """
-    Get a single line input of text from curses. To be used instead of Python standard input()
+    Get input from the user. Set maxlen to 0 for no maximum
     """
-    x,y = os.get_terminal_size()
-    stdscr.erase()
-    stdscr.addstr(0, 0, f"{prompt} (hit Enter to send)")
-
-    editwin = curses.newwin(1,x-2, 2,1)
-    rectangle(stdscr, 1,0, 3, x-1)
-    stdscr.refresh()
-
-    box = Textbox(editwin)
-
-    # Let the user edit until Ctrl-G is struck.
-    box.edit()
-
-    # Get resulting contents
-    message = box.gather()
-    return message[0:-1]
+    mx,my = os.get_terminal_size()
+    extoffscr = lines > my-3
+    if extoffscr:
+        lnrectmaxy = my-2
+    else:
+        lnrectmaxy = lines+2
+    text: list[list[str]] = [[] for _ in range(lines)]
+    ln=0
+    col=0
+    xoffset = 0
+    while True:
+        filline(stdscr,0,set_colour(WHITE,BLACK))
+        stdscr.addstr(0,0,str(prompt+" (Press ctrl-D to submit)")[0:mx-2],set_colour(WHITE,BLACK))
+        rectangle(stdscr,1,0,lnrectmaxy,mx-1)
+        chi = 1
+        for chln in text:
+            chi+= 1
+            stdscr.addstr(chi,1,"".join(chln)[xoffset:xoffset+mx-3])
+            if xoffset > 0:
+                stdscr.addstr(chi,0,"<",set_colour(BLUE,WHITE))
+        stdscr.addstr(0,mx-10,f"{ln},{col}",set_colour(WHITE,BLACK))
+        stdscr.move(ln+2,col-xoffset+1)
+        
+        stdscr.refresh()
+        ch = stdscr.getch()
+        chn = curses.keyname(ch)
+        if ch == 10 or ch == 13 or ch == curses.KEY_ENTER or ch == curses.KEY_DOWN:
+            if ln == lines - 1:
+                curses.beep()
+            else:
+                ln += 1
+                col = 0
+        elif ch == curses.KEY_LEFT:
+            if col > 0:
+                col -= 1
+                if xoffset > 0:
+                    xoffset -= 1
+                    stdscr.clear()
+            else:
+                curses.beep()
+        elif ch == curses.KEY_RIGHT:
+            if col < len(__retr_nbl_lst(text[ln])):
+                col += 1
+                if col-xoffset > mx-2:
+                    xoffset += 1
+                    stdscr.clear()
+            else:
+                curses.beep()
+        elif ch == curses.KEY_BACKSPACE:
+            if col > 0:
+                del text[ln][col-1]
+                col -= 1
+                if xoffset > 0:
+                    xoffset -= 1
+                stdscr.clear()#Fix render errors
+              
+            else:
+                curses.beep()
+        elif ch == curses.KEY_UP:
+            if ln > 0:
+                ln -= 1
+                col = 0
+        else:
+            if len(chn) > 1:
+                #Special char
+                if chn == b"^D":
+                    stdscr.erase()
+                    return "\n".join(["".join(t) for t in text])
+                elif chn == b"^K":
+                    text = [[] for _ in range(lines)]#Delete
+                    ln = 0
+                    col = 0
+                    stdscr.erase()
+                else:
+                    curses.beep()
+            else:
+                #append
+                col += 1
+                text[ln].insert(col-1,chn.decode())
+                
+                if col > mx-2:
+                    xoffset += 1
+                    stdscr.clear()
+    
 
 def displayops(stdscr,options: list,title="Please choose an option") -> int:
     """Display an options menu provided by options list. ALso displays title. Returns integer value of selected item."""
     mx, my = os.get_terminal_size()
     selected = 0
     
     options = [l[0:mx-3] for l in options]
```

### Comparing `cursesplus-2.2.3/src/cursesplus/filedialog.py` & `cursesplus-2.3.0/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.2.3/src/cursesplus/messagebox.py` & `cursesplus-2.3.0/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.2.3/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.3.0/src/cursesplus.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.2.3
+Version: 2.3.0
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,33 +23,19 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Version 2.2: Progressbar
+### Version 2.3: New Input
 
--Add ProgressBarTypes enum-class
+-Rewrite cursesinput function
 
--Add ProgressBarLocation enum-class
-
--You can now have a small progress bar that does not clear the screen
-
--displaymsg() will no longer clear itself.
-
-**-WARNING! This update may break progress bars.**
-
-### Version 2.1: Files 'n' Folders
-
--Add openfolderdialog()
-
--Change colours
-
--Performance improvements for all methods
+-Remains backwards-compatible
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 
 -Rewrite colour system. load_colours() is now nonexistent.
```

