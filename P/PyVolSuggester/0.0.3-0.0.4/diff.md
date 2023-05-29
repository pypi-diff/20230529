# Comparing `tmp/pyvolsuggester-0.0.3.tar.gz` & `tmp/pyvolsuggester-0.0.4.tar.gz`

## Comparing `pyvolsuggester-0.0.3.tar` & `pyvolsuggester-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    16086 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.3/src/PyVolSuggester/Suggester.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.3/src/PyVolSuggester/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.3/License.txt
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.3/README.md
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    16088 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/src/PyVolSuggester/Suggester.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/src/PyVolSuggester/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/License.txt
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/README.md
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/PKG-INFO
```

### Comparing `pyvolsuggester-0.0.3/src/PyVolSuggester/Suggester.py` & `pyvolsuggester-0.0.4/src/PyVolSuggester/Suggester.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         __import__(module)
     except ImportError:
         subprocess.check_call(["pip", "install", module])
 
 
 ## importing necessary library
 from tkinter import filedialog, Tk
-from playsound import playsound
+# from playsound import playsound
 import pyaudio
 import time
 from pynput import keyboard
 from pydub import AudioSegment
 import wave
 import os
 import numpy as np
@@ -49,16 +49,16 @@
 
     dir_name = os.path.dirname(file)
     base_file_name = Path(file).stem
     wav_file = dir_name + "/" + base_file_name + "_wav" + ".wav"
     print("\nConverted .mp3 to .wav file and saved to same location from where .mp3 file selected...")
     print("Created : " + base_file_name + "_wav" + ".wav")
     # print(wav_file)
-    # subprocess.call(['C:/Users/MAQ/Path_programs/ffmpeg.exe', '-i', file, wav_file])
-    subprocess.call(['C:/Users/aakas/PATH_Programs/ffmpeg-master-latest-win64-gpl/bin/ffmpeg.exe', '-i', file, wav_file])
+    subprocess.call(['C:/Users/MAQ/Path_programs/ffmpeg.exe', '-i', file, wav_file])
+    # subprocess.call(['C:/Users/aakas/PATH_Programs/ffmpeg-master-latest-win64-gpl/bin/ffmpeg.exe', '-i', file, wav_file])
 
     ## creating folder for saving output plot
     new_dir = pathlib.Path(dir_name, base_file_name + " - Plot")
     new_dir.mkdir(parents=True, exist_ok=True)
     plot_path = os.path.dirname(file)
     # print(plot_path)
```

### Comparing `pyvolsuggester-0.0.3/License.txt` & `pyvolsuggester-0.0.4/License.txt`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-0.0.3/README.md` & `pyvolsuggester-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-0.0.3/pyproject.toml` & `pyvolsuggester-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 name = "PyVolSuggester"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.3"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
+version = "0.0.4"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Does audio feature extraction and suggest the feasible volumne for better feeling and experience."  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is an optional longer description of your project that represents
```

### Comparing `pyvolsuggester-0.0.3/PKG-INFO` & `pyvolsuggester-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVolSuggester
-Version: 0.0.3
+Version: 0.0.4
 Summary: Does audio feature extraction and suggest the feasible volumne for better feeling and experience.
 Project-URL: Homepage, https://github.com/akash-rajak/PyVolSuggester
 Project-URL: Bug Reports, https://github.com/akash-rajak/PyVolSuggester/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Source, https://github.com/akash-rajak/PyVolSuggester
 Author-email: Akash Rajak <aakashrajak02@gmail.com>
 Maintainer-email: Akash Rajak <aakashrajak02@gmail.com>
```

