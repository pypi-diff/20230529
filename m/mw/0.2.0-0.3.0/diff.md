# Comparing `tmp/mw-0.2.0.tar.gz` & `tmp/mw-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mw-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mw-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mw-0.2.0.tar` & `mw-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1319 2023-05-27 06:35:15.007786 mw-0.2.0/README.md
--rw-r--r--   0        0        0     6176 2023-05-27 06:35:15.007786 mw-0.2.0/data/share/man/man1/mw.1
--rw-r--r--   0        0        0      117 2023-05-27 06:35:15.007786 mw-0.2.0/mw/__init__.py
--rw-r--r--   0        0        0      772 2023-05-27 06:35:15.007786 mw-0.2.0/mw/__main__.py
--rw-r--r--   0        0        0     1819 2023-05-27 06:35:15.007786 mw-0.2.0/mw/app.py
--rw-r--r--   0        0        0     8735 2023-05-27 06:35:15.007786 mw-0.2.0/mw/command_handler.py
--rw-r--r--   0        0        0     3775 2023-05-27 06:35:15.007786 mw-0.2.0/mw/display.py
--rw-r--r--   0        0        0     5467 2023-05-27 06:35:15.007786 mw-0.2.0/mw/stack.py
--rw-r--r--   0        0        0       74 2023-05-27 06:35:15.007786 mw-0.2.0/mw/types.py
--rw-r--r--   0        0        0     1688 2023-05-27 06:35:15.007786 mw-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 mw-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1319 2023-05-29 18:38:57.143523 mw-0.3.0/README.md
+-rw-r--r--   0        0        0     6506 2023-05-29 18:38:57.143523 mw-0.3.0/data/share/man/man1/mw.1
+-rw-r--r--   0        0        0      117 2023-05-29 18:38:57.143523 mw-0.3.0/mw/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-29 18:38:57.143523 mw-0.3.0/mw/__main__.py
+-rw-r--r--   0        0        0     2303 2023-05-29 18:38:57.143523 mw-0.3.0/mw/app.py
+-rw-r--r--   0        0        0    12177 2023-05-29 18:38:57.143523 mw-0.3.0/mw/commands.py
+-rw-r--r--   0        0        0     3775 2023-05-29 18:38:57.143523 mw-0.3.0/mw/display.py
+-rw-r--r--   0        0        0     5473 2023-05-29 18:38:57.143523 mw-0.3.0/mw/stack.py
+-rw-r--r--   0        0        0       74 2023-05-29 18:38:57.143523 mw-0.3.0/mw/types.py
+-rw-r--r--   0        0        0     1716 2023-05-29 18:38:57.143523 mw-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 mw-0.3.0/PKG-INFO
```

### Comparing `mw-0.2.0/README.md` & `mw-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mw-0.2.0/data/share/man/man1/mw.1` & `mw-0.3.0/data/share/man/man1/mw.1`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH mw 1 "2023-05-23" "Jamie Hardt" "User Manuals"
+.TH mw 1 "2023-05-29" "Jamie Hardt" "User Manuals"
 .SH NAME 
 mw \- audio sample editor
 .SH SYNOPSIS
 .SY mw
 .RI "[\-e " COMMAND "]"
 .RI "[" "FILE ..." "]"
 .SH DESCRIPTION
@@ -52,26 +52,61 @@
 Execute 
 .I COMMAND
 after loading 
 .IR FILE "s."
 Can be used multiple times to run multiple commands.
 .IP "\-h, \-\-help"
 Print brief help.
-.SH COMMANDS
+.SH COMMANDS AND ACTIONS
+
 The command prompt in 
 .B mw
-accepts lines of commands which begin with a command
-.I keyword
-followed by zero or more arguments.
+accepts lines of commands of a form similar to 
+.BR sed "."
+.RS 4
+.PP 
+[start][,end][action][arguments]
+.RS -4
+.PP
+The 
+.I start 
+and 
+.I end 
+are
+used to set the beginning and ending times for an action to act upon. When a 
+.I start 
+or 
+.I end 
+are read from the command line, they set the in and out edit points on the active
+sound, which will then be used by a following action. Some actions take additional
+arguments which follow the action, separated by spaces. Double-quotes can be used
+for arguments that contain spaces.
+When 
+.I start
+is omitted from a command, the sound in-point is used, and if it is not set,
+the beginning of the sound is used. When 
+.I end
+is omitted from a command, the sound out-point is used, and if it is not set,
+the end of the sound is used.
+.SS EXAMPLES
+.IP 0,100bloop
+Bloop the first 100 milliseconds of the sound.
+.IP 100,-100 crop
+Crop the first and last 100 milliseconds off the sound.
+.IP 0,-1 
+Set the selection in- and out- points to the beginning and end of the sound.
+.IP ,2500
+Set the selection out-point to 2500 miliseconds, do not change the in-point.
 .P
 .BR mw 's
 command prompt supports GNU 
 .BR readline (3)
 for line editing and auto-completion; all of the commands listed here will autocomplete
 with the <Tab> key.
+.SS ACTION LIST
 .IP help
 Prints a list of all command keywords 
 .B mw
 recognizes, along with a brief description. Keywords that accept arguments
 are followed by their arguments in 
 .IR [brackets] .
 .IP license
@@ -82,33 +117,14 @@
 Prints a text graphic of the sound presently at the top of the editor stack. This
 include a waveform bargraph of the sound's amplitiude with respect to time, as well
 as a text representation of the current cursor, in- and out-points.
 .IP stack
 Prints a text graphic of every sound in the editor stack, from top to bottom, 
 and prints out the length of the current editing session, being the length of
 the longest sound in the stack.
-.IP "cmills [pos]"
-Sets or updates the cursor position to 
-.I pos
-milliseconds from the beginning of the sound, or, if 
-.I pos
-is preceded by a plus or minus symbol, will position the cursor relative to it's
-current position. Without an argument, positions the cursor at the beginning of the
-sound.
-.IP "cend [pos]"
-Positions the cursor relative to the end of the sound. Without an argument, 
-positions the cursor at the end of the sound.
-.IP "i [pos]"
-Sets the selection in-point for the sound, either at the current cursor position or
-at the time given by 
-.IR pos .
-.IP "o [pos]"
-Sets the selection out-point for the sound, either at the current cursor position or
-at the time given by 
-.IR pos .
 .IP "ci"
 Clears the selection in-point.
 .IP "co"
 Clears the selection out-point.
 .IP "setw [width]"
 Sets the current display width: the number of columns
 .B mw
```

### Comparing `mw-0.2.0/mw/__main__.py` & `mw-0.3.0/mw/__main__.py`

 * *Files identical despite different names*

### Comparing `mw-0.2.0/mw/display.py` & `mw-0.3.0/mw/display.py`

 * *Files identical despite different names*

### Comparing `mw-0.2.0/mw/stack.py` & `mw-0.3.0/mw/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         self.segment = cast(AudioSegment, self.segment[start:end])
         self.in_point = None
         self.out_point = None
         self.cursor = Milliseconds(0)
         self.view_start = Milliseconds(0)
         self.view_end = Milliseconds(len(self.segment))
 
-    def crop_to_selection(self):
-        self.crop(self.in_point or Milliseconds(0), 
-                  self.out_point or Milliseconds(len(self.segment)))
+    # def crop_to_selection(self):
+    #     self.crop(self.in_point or Milliseconds(0), 
+    #               self.out_point or Milliseconds(len(self.segment)))
 
     def insert_silence(self, duration: Milliseconds, at: Milliseconds):
         assert at < len(self.segment), "Insertion point past end of sound"
         a = self.segment[0:at]
         b = self.segment[at:]
         silence = AudioSegment.silent(duration=duration)
         self.segment = a + silence + b
```

### Comparing `mw-0.2.0/pyproject.toml` & `mw-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "Programming Language :: Python :: 3.8",  
     "Programming Language :: Python :: 3.9",    
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
   "numpy ~= 1.24.3",
+  "parsimonious ~= 0.10.0",
   "pydub ~= 0.25.1",
   "apeek ~= 0.1.0",
   "gnureadline ~= 8.1.2"
 ]
 keywords = [
     'waveform', 
     'metadata',
```

### Comparing `mw-0.2.0/PKG-INFO` & `mw-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mw
-Version: 0.2.0
+Version: 0.3.0
 Summary: mw is an audio sample editor for the terminal.
 Keywords: waveform,metadata,audio,console
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -12,14 +12,15 @@
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy ~= 1.24.3
+Requires-Dist: parsimonious ~= 0.10.0
 Requires-Dist: pydub ~= 0.25.1
 Requires-Dist: apeek ~= 0.1.0
 Requires-Dist: gnureadline ~= 8.1.2
 Requires-Dist: sphinx >= 5.3.0 ; extra == "doc"
 Requires-Dist: sphinx_rtd_theme >= 1.1.1 ; extra == "doc"
 Project-URL: Home, https://github.com/iluvcapra/mw
 Project-URL: Issues, https://github.com/iluvcapra/mw/issues
```

