# Comparing `tmp/PySciMath-1.5.6.tar.gz` & `tmp/PySciMath-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.5.6.tar", last modified: Thu May 25 10:55:08 2023, max compression
+gzip compressed data, was "PySciMath-1.5.7.tar", last modified: Mon May 29 15:03:04 2023, max compression
```

## Comparing `PySciMath-1.5.6.tar` & `PySciMath-1.5.7.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 10:55:08.686609 PySciMath-1.5.6/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.6/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 06:30:09.000000 PySciMath-1.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2616 2023-05-25 10:55:08.684615 PySciMath-1.5.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-25 10:55:08.664669 PySciMath-1.5.6/PySciMath/
--rw-rw-rw-   0        0        0     2663 2023-05-22 12:48:50.000000 PySciMath-1.5.6/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0    21993 2023-05-25 10:41:29.000000 PySciMath-1.5.6/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0      564 2023-05-25 10:41:56.000000 PySciMath-1.5.6/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1262 2023-05-25 10:42:52.000000 PySciMath-1.5.6/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      554 2023-05-22 12:49:19.000000 PySciMath-1.5.6/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.6/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:55:08.680626 PySciMath-1.5.6/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2616 2023-05-25 10:55:08.000000 PySciMath-1.5.6/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-25 10:55:08.000000 PySciMath-1.5.6/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 10:55:08.000000 PySciMath-1.5.6/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 10:55:08.000000 PySciMath-1.5.6/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2081 2023-05-25 10:46:35.000000 PySciMath-1.5.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 10:55:08.686609 PySciMath-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-05-25 10:47:10.000000 PySciMath-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:03:04.895157 PySciMath-1.5.7/
+-rw-rw-rw-   0        0        0      523 2023-05-29 14:28:28.000000 PySciMath-1.5.7/CREDITS.md
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       58 2023-05-29 15:01:18.000000 PySciMath-1.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2681 2023-05-29 15:03:04.892165 PySciMath-1.5.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 15:03:04.870907 PySciMath-1.5.7/PySciMath/
+-rw-rw-rw-   0        0        0     2663 2023-05-22 12:48:50.000000 PySciMath-1.5.7/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0    21993 2023-05-25 10:41:29.000000 PySciMath-1.5.7/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0    11013 2023-05-29 14:58:49.000000 PySciMath-1.5.7/PySciMath/Graphs.py
+-rw-rw-rw-   0        0        0      564 2023-05-25 10:41:56.000000 PySciMath-1.5.7/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1262 2023-05-25 10:42:52.000000 PySciMath-1.5.7/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      554 2023-05-22 12:49:19.000000 PySciMath-1.5.7/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.7/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:03:04.887178 PySciMath-1.5.7/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2681 2023-05-29 15:03:03.000000 PySciMath-1.5.7/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-05-29 15:03:03.000000 PySciMath-1.5.7/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 15:03:03.000000 PySciMath-1.5.7/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-29 15:03:03.000000 PySciMath-1.5.7/PySciMath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 15:03:03.000000 PySciMath-1.5.7/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2142 2023-05-29 14:59:43.000000 PySciMath-1.5.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 15:03:04.896153 PySciMath-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-05-29 15:00:38.000000 PySciMath-1.5.7/setup.py
```

### Comparing `PySciMath-1.5.6/LICENSE.txt` & `PySciMath-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.6/PKG-INFO` & `PySciMath-1.5.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.6
+Version: 1.5.7
 Summary: PySciMath is a general-purpose Python package to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Mathematics,Science,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Package Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.6</br>
+**Version** - 1.5.7</br>
 **Description** - PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
@@ -49,14 +49,18 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
+## Credits
+
+Go to the `CREDITS.md` file to see the credits.
+
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
 I hope you liked this package. Thank you!
```

### Comparing `PySciMath-1.5.6/PySciMath/Arithmetic.py` & `PySciMath-1.5.7/PySciMath/Arithmetic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.6/PySciMath/Geometry.py` & `PySciMath-1.5.7/PySciMath/Geometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.6/PySciMath/Quadratic.py` & `PySciMath-1.5.7/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.6/PySciMath/Statistics.py` & `PySciMath-1.5.7/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.6/PySciMath/Trigonometry.py` & `PySciMath-1.5.7/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.6/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.5.7/PySciMath.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.6
+Version: 1.5.7
 Summary: PySciMath is a general-purpose Python package to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Mathematics,Science,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Package Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.6</br>
+**Version** - 1.5.7</br>
 **Description** - PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
@@ -49,14 +49,18 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
+## Credits
+
+Go to the `CREDITS.md` file to see the credits.
+
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
 I hope you liked this package. Thank you!
```

### Comparing `PySciMath-1.5.6/README.md` & `PySciMath-1.5.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Package Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.6</br>
+**Version** - 1.5.7</br>
 **Description** - PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
@@ -36,14 +36,18 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
+## Credits
+
+Go to the `CREDITS.md` file to see the credits.
+
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
 I hope you liked this package. Thank you!
```

### Comparing `PySciMath-1.5.6/setup.py` & `PySciMath-1.5.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.5.6",
+    version="1.5.7",
     description="PySciMath is a general-purpose Python package to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
     author_email="anikethchavare@outlook.com",
     keywords=["Math", "Mathematics", "Science", "Calculations"],
     url="https://github.com/Anikethc/PySciMath",
     download_url="https://pypi.org/project/PySciMath"
 )
 
+# Install Requires
+install_requires = ["matplotlib", "numpy"]
+
 # Run the Setup File
 if __name__ == "__main__":
-    setup(**setup_args)
+    setup(**setup_args, install_requires=install_requires)
```

