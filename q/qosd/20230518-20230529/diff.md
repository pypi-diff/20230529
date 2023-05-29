# Comparing `tmp/qosd-20230518.tar.gz` & `tmp/qosd-20230529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qosd-20230518.tar", last modified: Thu May 18 15:05:16 2023, max compression
+gzip compressed data, was "qosd-20230529.tar", last modified: Mon May 29 10:39:57 2023, max compression
```

## Comparing `qosd-20230518.tar` & `qosd-20230529.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-18 15:05:16.455188 qosd-20230518/
--rw-rw-r--   0 l         (1000) l         (1000)     1978 2023-05-18 15:05:16.455188 qosd-20230518/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)     1673 2023-05-18 14:45:10.000000 qosd-20230518/README.md
--rw-rw-r--   0 l         (1000) l         (1000)      605 2023-05-18 15:02:10.000000 qosd-20230518/pyproject.toml
--rw-rw-r--   0 l         (1000) l         (1000)       38 2023-05-18 15:05:16.455188 qosd-20230518/setup.cfg
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-18 15:05:16.455188 qosd-20230518/src/
--rw-rw-r--   0 l         (1000) l         (1000)        0 2023-05-18 08:26:03.000000 qosd-20230518/src/__init__.py
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-18 15:05:16.455188 qosd-20230518/src/qosd.egg-info/
--rw-rw-r--   0 l         (1000) l         (1000)     1978 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)      246 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/SOURCES.txt
--rw-rw-r--   0 l         (1000) l         (1000)        1 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/dependency_links.txt
--rw-rw-r--   0 l         (1000) l         (1000)       35 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/entry_points.txt
--rw-rw-r--   0 l         (1000) l         (1000)       54 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/requires.txt
--rw-rw-r--   0 l         (1000) l         (1000)       14 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/top_level.txt
--rwxrwxr-x   0 l         (1000) l         (1000)     7832 2023-05-18 15:02:21.000000 qosd-20230518/src/qosd.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 10:39:57.911336 qosd-20230529/
+-rw-rw-r--   0 l         (1000) l         (1000)     2087 2023-05-29 10:39:57.911336 qosd-20230529/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)     1782 2023-05-29 10:37:44.000000 qosd-20230529/README.md
+-rw-rw-r--   0 l         (1000) l         (1000)      605 2023-05-18 15:02:10.000000 qosd-20230529/pyproject.toml
+-rw-rw-r--   0 l         (1000) l         (1000)       38 2023-05-29 10:39:57.911336 qosd-20230529/setup.cfg
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 10:39:57.911336 qosd-20230529/src/
+-rw-rw-r--   0 l         (1000) l         (1000)        0 2023-05-18 08:26:03.000000 qosd-20230529/src/__init__.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 10:39:57.911336 qosd-20230529/src/qosd.egg-info/
+-rw-rw-r--   0 l         (1000) l         (1000)     2087 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)      246 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/SOURCES.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        1 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/dependency_links.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       35 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/entry_points.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       54 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/requires.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       14 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/top_level.txt
+-rwxrwxr-x   0 l         (1000) l         (1000)     8150 2023-05-29 10:33:05.000000 qosd-20230529/src/qosd.py
```

### Comparing `qosd-20230518/PKG-INFO` & `qosd-20230529/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qosd
-Version: 20230518
+Version: 20230529
 Summary: QOSD for python
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/qosd
 Keywords: osd,on-screen-display,tail
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
@@ -22,31 +22,31 @@
 ```
 pip install qosd
 ```
 
 # Usage
 
 ```
-usage: qosd [-h] [-i] [-m MAXLINES] [-n SESSION_NAME] [-o OPACITY] [-p {topleft,topright,bottomleft,bottomright}] [-P POSITION_OFFSET POSITION_OFFSET] [-s STYLE] [-t TIMEOUT] text [text ...]
+usage: qosd [-h] [-i] [-m MAXLINES] [-n SESSION_NAME] [-o OPACITY] [-p {topleft,topright,bottomleft,bottomright,center,centerleft,centerright}] [-P POSITION_OFFSET POSITION_OFFSET] [-s STYLE] [-t TIMEOUT] text [text ...]
 
-qosd - OSD from python - v20230516
+qosd - display text over your Xorg screen - v20230529
 
 positional arguments:
   text                  text to display, or '-' for stdin
 
 options:
   -h, --help            show this help message and exit
   -i, --no-input        set window transparent to input
   -m MAXLINES, --maxlines MAXLINES
                         default: 30
   -n SESSION_NAME, --session-name SESSION_NAME
                         start named OSD display session, killing previous OSD with same session name
   -o OPACITY, --opacity OPACITY
                         default: 1.0
-  -p {topleft,topright,bottomleft,bottomright}, --position {topleft,topright,bottomleft,bottomright}
+  -p {topleft,topright,bottomleft,bottomright,center,centerleft,centerright}, --position {topleft,topright,bottomleft,bottomright,center,centerleft,centerright}
                         text position, default=topleft
   -P POSITION_OFFSET POSITION_OFFSET, --position-offset POSITION_OFFSET POSITION_OFFSET
                         offset in pixels from position, default: 0 0
   -s STYLE, --style STYLE
                         default: 'color:"#FFFFFF";background-color:"#99000000";font-size:11pt;font-weight:bold;'
   -t TIMEOUT, --timeout TIMEOUT
                         display timeout in seconds, default: 3
```

### Comparing `qosd-20230518/README.md` & `qosd-20230529/src/qosd.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: qosd
+Version: 20230529
+Summary: QOSD for python
+Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/looran/qosd
+Keywords: osd,on-screen-display,tail
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+
 ## qosd - display text over your Xorg screen
 
 `qosd` is a command-line tool and python library can display text over your Linux desktop screen:
 * text is displayed over any window (On-Screen-Display)
 * display simple line
 * tail stdin
 * transparency and text style is configurable
@@ -11,31 +22,31 @@
 ```
 pip install qosd
 ```
 
 # Usage
 
 ```
-usage: qosd [-h] [-i] [-m MAXLINES] [-n SESSION_NAME] [-o OPACITY] [-p {topleft,topright,bottomleft,bottomright}] [-P POSITION_OFFSET POSITION_OFFSET] [-s STYLE] [-t TIMEOUT] text [text ...]
+usage: qosd [-h] [-i] [-m MAXLINES] [-n SESSION_NAME] [-o OPACITY] [-p {topleft,topright,bottomleft,bottomright,center,centerleft,centerright}] [-P POSITION_OFFSET POSITION_OFFSET] [-s STYLE] [-t TIMEOUT] text [text ...]
 
-qosd - OSD from python - v20230516
+qosd - display text over your Xorg screen - v20230529
 
 positional arguments:
   text                  text to display, or '-' for stdin
 
 options:
   -h, --help            show this help message and exit
   -i, --no-input        set window transparent to input
   -m MAXLINES, --maxlines MAXLINES
                         default: 30
   -n SESSION_NAME, --session-name SESSION_NAME
                         start named OSD display session, killing previous OSD with same session name
   -o OPACITY, --opacity OPACITY
                         default: 1.0
-  -p {topleft,topright,bottomleft,bottomright}, --position {topleft,topright,bottomleft,bottomright}
+  -p {topleft,topright,bottomleft,bottomright,center,centerleft,centerright}, --position {topleft,topright,bottomleft,bottomright,center,centerleft,centerright}
                         text position, default=topleft
   -P POSITION_OFFSET POSITION_OFFSET, --position-offset POSITION_OFFSET POSITION_OFFSET
                         offset in pixels from position, default: 0 0
   -s STYLE, --style STYLE
                         default: 'color:"#FFFFFF";background-color:"#99000000";font-size:11pt;font-weight:bold;'
   -t TIMEOUT, --timeout TIMEOUT
                         display timeout in seconds, default: 3
```

### Comparing `qosd-20230518/pyproject.toml` & `qosd-20230529/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qosd-20230518/src/qosd.egg-info/PKG-INFO` & `qosd-20230529/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: qosd
-Version: 20230518
-Summary: QOSD for python
-Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
-License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/looran/qosd
-Keywords: osd,on-screen-display,tail
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-
 ## qosd - display text over your Xorg screen
 
 `qosd` is a command-line tool and python library can display text over your Linux desktop screen:
 * text is displayed over any window (On-Screen-Display)
 * display simple line
 * tail stdin
 * transparency and text style is configurable
@@ -22,31 +11,31 @@
 ```
 pip install qosd
 ```
 
 # Usage
 
 ```
-usage: qosd [-h] [-i] [-m MAXLINES] [-n SESSION_NAME] [-o OPACITY] [-p {topleft,topright,bottomleft,bottomright}] [-P POSITION_OFFSET POSITION_OFFSET] [-s STYLE] [-t TIMEOUT] text [text ...]
+usage: qosd [-h] [-i] [-m MAXLINES] [-n SESSION_NAME] [-o OPACITY] [-p {topleft,topright,bottomleft,bottomright,center,centerleft,centerright}] [-P POSITION_OFFSET POSITION_OFFSET] [-s STYLE] [-t TIMEOUT] text [text ...]
 
-qosd - OSD from python - v20230516
+qosd - display text over your Xorg screen - v20230529
 
 positional arguments:
   text                  text to display, or '-' for stdin
 
 options:
   -h, --help            show this help message and exit
   -i, --no-input        set window transparent to input
   -m MAXLINES, --maxlines MAXLINES
                         default: 30
   -n SESSION_NAME, --session-name SESSION_NAME
                         start named OSD display session, killing previous OSD with same session name
   -o OPACITY, --opacity OPACITY
                         default: 1.0
-  -p {topleft,topright,bottomleft,bottomright}, --position {topleft,topright,bottomleft,bottomright}
+  -p {topleft,topright,bottomleft,bottomright,center,centerleft,centerright}, --position {topleft,topright,bottomleft,bottomright,center,centerleft,centerright}
                         text position, default=topleft
   -P POSITION_OFFSET POSITION_OFFSET, --position-offset POSITION_OFFSET POSITION_OFFSET
                         offset in pixels from position, default: 0 0
   -s STYLE, --style STYLE
                         default: 'color:"#FFFFFF";background-color:"#99000000";font-size:11pt;font-weight:bold;'
   -t TIMEOUT, --timeout TIMEOUT
                         display timeout in seconds, default: 3
```

### Comparing `qosd-20230518/src/qosd.py` & `qosd-20230529/src/qosd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-VERSION = "20230518"
+VERSION = "20230529"
 DESCRIPTION = "display text over your Xorg screen"
 EXAMPLES = """examples:
 $ qosd hello
 $ tail -f /var/log/{messages,auth.log} | qosd -
 """
 
 from pathlib import Path
@@ -31,14 +31,15 @@
         self.offset = offset
         self.setAttribute(QtCore.Qt.WA_TranslucentBackground, True)
         self.setStyleSheet(style)
         self.setWindowOpacity(opacity)
 
         self.layout = QtWidgets.QHBoxLayout()
         self.label = QtWidgets.QLabel(self)
+        #self.label.setWordWrap(True) # word wrap breaks label heightForWidth()
         self.layout.addWidget(self.label)
         self.setLayout(self.layout)
 
         self.installEventFilter(self)
         self.resize(0, 0)
 
     def eventFilter(self, obj, event):
@@ -50,25 +51,35 @@
             elif event.type() == QtGui.QHoverEvent.Type.HoverLeave:
                 self.qosd.hide_to_start()
         elif type(event) == QtGui.QMouseEvent:
             if event.type() == QtGui.QMouseEvent.Type.MouseButtonPress:
                 self.qosd.hide_or_exit()
         return True
 
-    def updatePosition(self):
+    def updateGeometry(self):
         sdim = self.screen().geometry()
+        ox, oy = self.offset[0], self.offset[1]
+        w = min(self.label.width(), sdim.width() - ox)
+        h = min(self.label.heightForWidth(w), sdim.height() - oy)
         if self.position == "topleft":
-            coord = (self.offset[0], self.offset[1])
+            x, y = ox, oy
         elif self.position == "topright":
-            coord = ((sdim.right()-self.width())-self.offset[0], self.offset[1])
+            x, y = sdim.width() - (w + ox), oy
         elif self.position == "bottomleft":
-            coord = (self.offset[0], (sdim.bottom()-self.height())+self.offset[1])
+            x, y = ox, sdim.height() - (h + oy)
         elif self.position == "bottomright":
-            coord = ((sdim.right()-self.width())-self.offset[0], (sdim.bottom()-self.height())-self.offset[1])
-        self.move(coord[0], coord[1])
+            x, y = sdim.width() - (w + ox), sdim.height() - (h + oy)
+        elif self.position == "center":
+            x, y = (sdim.width() / 2 - w / 2) + ox, (sdim.height() / 2 - h / 2) + oy
+        elif self.position == "centerleft":
+            x, y = ox, (sdim.height() / 2 - h / 2) + oy
+        elif self.position == "centerright":
+            x, y = sdim.width() - (w + ox), (sdim.height() / 2 - h / 2) + oy
+        self.move(x, y)
+        self.resize(w, h)
 
 class Qosd(object):
     TIMEOUT = 3
     MAXLINES = 30
 
     def __init__(self, style, opacity, timeout=TIMEOUT, maxlines=MAXLINES, position=Qosd_win.POSITION, offset=(0,0), no_input=False):
         self.maxlines = maxlines
@@ -94,28 +105,23 @@
         else:
             self.text_log = text
         lines = self.text_log.split('\n')
         if len(lines) > self.maxlines:
             self.text_log = '\n'.join(lines[-self.maxlines:])
         self.win.label.setText(self.text_log.strip())
         self.win.label.adjustSize()
-        self.win.resize(self.win.label.width(), self.win.label.heightForWidth(self.win.label.width()))
-        self.win.updatePosition()
+        self.win.updateGeometry()
 
     def text_stdin(self):
         flags = fcntl.fcntl(sys.stdin, fcntl.F_GETFL)
         fcntl.fcntl(sys.stdin, fcntl.F_SETFL, flags | os.O_NONBLOCK)
         self.stdin = QtCore.QSocketNotifier(sys.stdin.fileno(), QtCore.QSocketNotifier.Read, self.win)
         self.stdin.activated.connect(self._cb_read_stdin)
         self.stdin.setEnabled(True)
 
-    def history(self, signum, stack):
-        self.win.close()
-        self.app.exit()
-
     def run(self):
         self.app.exec()
 
     def exit(self):
         self.win.close()
         self.app.exit()
 
@@ -180,15 +186,15 @@
 
 def main():
     parser = argparse.ArgumentParser(description="qosd - "+DESCRIPTION+" - v"+VERSION, epilog=EXAMPLES, formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('-i', '--no-input', action='store_true', help='set window transparent to input')
     parser.add_argument('-m', '--maxlines', type=int, default=Qosd.MAXLINES, help='default: %s' % Qosd.MAXLINES)
     parser.add_argument('-n', '--session-name', help='start named OSD display session, killing previous OSD with same session name')
     parser.add_argument('-o', '--opacity', type=float, default=Qosd_win.OPACITY, help='default: %s' % Qosd_win.OPACITY)
-    parser.add_argument('-p', '--position', default=Qosd_win.POSITION, choices=["topleft", "topright", "bottomleft", "bottomright"], help='text position, default=%s' % Qosd_win.POSITION)
+    parser.add_argument('-p', '--position', default=Qosd_win.POSITION, choices=["topleft", "topright", "bottomleft", "bottomright", "center", "centerleft", "centerright"], help='text position, default=%s' % Qosd_win.POSITION)
     parser.add_argument('-P', '--position-offset', type=int, nargs=2, default=(0,0), help='offset in pixels from position, default: 0 0')
     parser.add_argument('-s', '--style', default=Qosd_win.STYLE, help='default: \'%s\'' % Qosd_win.STYLE)
     parser.add_argument('-t', '--timeout', type=float, default=Qosd.TIMEOUT, help='display timeout in seconds, default: %s' % Qosd.TIMEOUT)
     parser.add_argument('text', nargs="+", help='text to display, or \'-\' for stdin')
 
     args = parser.parse_args()
```

