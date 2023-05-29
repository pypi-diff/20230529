# Comparing `tmp/pyvolsuggester-0.0.4.tar.gz` & `tmp/pyvolsuggester-0.0.5.tar.gz`

## Comparing `pyvolsuggester-0.0.4.tar` & `pyvolsuggester-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,20 @@
--rw-r--r--   0        0        0    16088 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/src/PyVolSuggester/Suggester.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/src/PyVolSuggester/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/License.txt
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/README.md
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0   348044 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/1.png
+-rw-r--r--   0        0        0    98739 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/10.png
+-rw-r--r--   0        0        0   360267 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/11.png
+-rw-r--r--   0        0        0    96844 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/12.png
+-rw-r--r--   0        0        0   213069 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/13.png
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/14.png
+-rw-r--r--   0        0        0   147275 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/2.png
+-rw-r--r--   0        0        0    70013 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/3.png
+-rw-r--r--   0        0        0    22104 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/4.png
+-rw-r--r--   0        0        0    17706 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/5.png
+-rw-r--r--   0        0        0   101783 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/6.png
+-rw-r--r--   0        0        0   944565 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/7.png
+-rw-r--r--   0        0        0   573913 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/8.png
+-rw-r--r--   0        0        0   105460 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/9.png
+-rw-r--r--   0        0        0    16169 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/src/PyVolSuggester/Suggester.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/src/PyVolSuggester/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/License.txt
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/README.md
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/PKG-INFO
```

### Comparing `pyvolsuggester-0.0.4/src/PyVolSuggester/Suggester.py` & `pyvolsuggester-0.0.5/src/PyVolSuggester/Suggester.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     ax[0].semilogy(times, rms[0], label='RMS Energy')
 
     ## calculating average rms
     for i in rms[0]:
         avg_rms = avg_rms + i
 
     avg_rms = avg_rms/len(times)
-    print(avg_rms)
+    # print(avg_rms)
 
     ax[0].set(title=file_name + ' - RMS Energy', xticks=[])
     ax[0].legend()
     ax[0].label_outer()
     librosa.display.specshow(librosa.amplitude_to_db(S, ref=np.max), y_axis='log', x_axis='time', ax=ax[1])
     ax[1].set(title=file_name + ' - log Power spectrogram')
     # plt.legend()
@@ -424,14 +424,19 @@
 
     if(avg_rms>0.00001):
         print("High Volume")
     else:
         print("Low Volume")
 
 
+## function defined to exit from program
+def exit_program():
+    exit()
+
+
 ## defining main function
 def main():
     global file
     print("Select Audio file : ")
     file = filedialog.askopenfilename(title="Select an Audio file", filetypes=[("Audio Files", "*.mp3"), ("All Files", "*.*")])
     if (file != ""):
         print(file)
```

### Comparing `pyvolsuggester-0.0.4/License.txt` & `pyvolsuggester-0.0.5/License.txt`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-0.0.4/README.md` & `pyvolsuggester-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-0.0.4/pyproject.toml` & `pyvolsuggester-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 name = "PyVolSuggester"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.4"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
+version = "0.0.5"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Does audio feature extraction and suggest the feasible volumne for better feeling and experience."  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is an optional longer description of your project that represents
```

### Comparing `pyvolsuggester-0.0.4/PKG-INFO` & `pyvolsuggester-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVolSuggester
-Version: 0.0.4
+Version: 0.0.5
 Summary: Does audio feature extraction and suggest the feasible volumne for better feeling and experience.
 Project-URL: Homepage, https://github.com/akash-rajak/PyVolSuggester
 Project-URL: Bug Reports, https://github.com/akash-rajak/PyVolSuggester/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Source, https://github.com/akash-rajak/PyVolSuggester
 Author-email: Akash Rajak <aakashrajak02@gmail.com>
 Maintainer-email: Akash Rajak <aakashrajak02@gmail.com>
```

