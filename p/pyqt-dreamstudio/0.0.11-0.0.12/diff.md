# Comparing `tmp/pyqt-dreamstudio-0.0.11.tar.gz` & `tmp/pyqt-dreamstudio-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-dreamstudio-0.0.11.tar", last modified: Mon May 29 05:19:20 2023, max compression
+gzip compressed data, was "pyqt-dreamstudio-0.0.12.tar", last modified: Mon May 29 08:48:37 2023, max compression
```

## Comparing `pyqt-dreamstudio-0.0.11.tar` & `pyqt-dreamstudio-0.0.12.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 05:19:20.351457 pyqt-dreamstudio-0.0.11/
--rw-rw-rw-   0        0        0     1086 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/LICENSE
--rw-rw-rw-   0        0        0     2544 2023-05-29 05:19:20.350460 pyqt-dreamstudio-0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0     2162 2023-05-29 05:18:57.000000 pyqt-dreamstudio-0.0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 05:19:20.319542 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/
--rw-rw-rw-   0        0        0        0 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/__init__.py
--rw-rw-rw-   0        0        0     1558 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/currentImageView.py
--rw-rw-rw-   0        0        0     1723 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/explorerWidget.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:19:20.348465 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/
--rw-rw-rw-   0        0        0        0 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/__init__.py
--rw-rw-rw-   0        0        0      712 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/history.svg
--rw-rw-rw-   0        0        0     1283 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/setting.svg
--rw-rw-rw-   0        0        0     5100 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageListWidget.py
--rw-rw-rw-   0        0        0    18245 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageSqlite.py
--rw-rw-rw-   0        0        0    11031 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageStableDiffusionPage.py
--rw-rw-rw-   0        0        0     1444 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/inputDialog.py
--rw-rw-rw-   0        0        0     3865 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/leftSideBar.py
--rw-rw-rw-   0        0        0   232520 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/logo.png
--rw-rw-rw-   0        0        0     4976 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/main.py
--rw-rw-rw-   0        0        0     3270 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/notifier.py
--rw-rw-rw-   0        0        0      699 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/rightSideBar.py
--rw-rw-rw-   0        0        0     2854 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/searchBar.py
--rw-rw-rw-   0        0        0     5918 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/svgButton.py
--rw-rw-rw-   0        0        0      765 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/svgLabel.py
--rw-rw-rw-   0        0        0     4077 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/thumbnailView.py
--rw-rw-rw-   0        0        0     4884 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/toast.py
--rw-rw-rw-   0        0        0     1899 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/viewWidget.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:19:20.342482 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/
--rw-rw-rw-   0        0        0     2544 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      895 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 05:19:20.351457 pyqt-dreamstudio-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-05-29 05:15:51.000000 pyqt-dreamstudio-0.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:48:37.703591 pyqt-dreamstudio-0.0.12/
+-rw-rw-rw-   0        0        0     1086 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/LICENSE
+-rw-rw-rw-   0        0        0     2627 2023-05-29 08:48:37.702592 pyqt-dreamstudio-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2240 2023-05-29 08:47:05.000000 pyqt-dreamstudio-0.0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 08:48:37.643953 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/
+-rw-rw-rw-   0        0        0        0 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/__init__.py
+-rw-rw-rw-   0        0        0     1558 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/currentImageView.py
+-rw-rw-rw-   0        0        0     1723 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/explorerWidget.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:48:37.700633 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/ico/
+-rw-rw-rw-   0        0        0        0 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/ico/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-29 08:47:28.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/ico/copy_light.svg
+-rw-rw-rw-   0        0        0      712 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/ico/history.svg
+-rw-rw-rw-   0        0        0      669 2023-05-29 08:47:28.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/ico/save_light.svg
+-rw-rw-rw-   0        0        0     1283 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/ico/setting.svg
+-rw-rw-rw-   0        0        0     5100 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/imageListWidget.py
+-rw-rw-rw-   0        0        0    18245 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/imageSqlite.py
+-rw-rw-rw-   0        0        0    11031 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/imageStableDiffusionPage.py
+-rw-rw-rw-   0        0        0     1444 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/inputDialog.py
+-rw-rw-rw-   0        0        0     3865 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/leftSideBar.py
+-rw-rw-rw-   0        0        0   232520 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/logo.png
+-rw-rw-rw-   0        0        0     4976 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/main.py
+-rw-rw-rw-   0        0        0     3270 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/notifier.py
+-rw-rw-rw-   0        0        0      699 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/rightSideBar.py
+-rw-rw-rw-   0        0        0     2871 2023-05-29 08:47:28.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/searchBar.py
+-rw-rw-rw-   0        0        0     5918 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/svgButton.py
+-rw-rw-rw-   0        0        0      765 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/svgLabel.py
+-rw-rw-rw-   0        0        0     4077 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/thumbnailView.py
+-rw-rw-rw-   0        0        0     4884 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/toast.py
+-rw-rw-rw-   0        0        0     1899 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/viewWidget.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:48:37.679551 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio.egg-info/
+-rw-rw-rw-   0        0        0     2627 2023-05-29 08:48:37.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      967 2023-05-29 08:48:37.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 08:48:37.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-29 08:48:37.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-29 08:48:37.000000 pyqt-dreamstudio-0.0.12/pyqt_dreamstudio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 08:48:37.703591 pyqt-dreamstudio-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      915 2023-05-29 08:48:08.000000 pyqt-dreamstudio-0.0.12/setup.py
```

### Comparing `pyqt-dreamstudio-0.0.11/LICENSE` & `pyqt-dreamstudio-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/PKG-INFO` & `pyqt-dreamstudio-0.0.12/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-dreamstudio
-Version: 0.0.11
+Version: 0.0.12
 Summary: Using DreamStudio API in Python desktop application
 Home-page: https://github.com/yjg30737/pyqt-dreamstudio.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,20 +34,25 @@
 4. python setup.py install
 5. cd pyqt_dreamstudio
 6. python main.py
 ### By pip
 1. pip install pyqt_dreamstudio
 2. 
 ```python
-from pyqt_dreamstudio.imageGeneratingToolWidget import ImageGeneratingToolWidget
+from PyQt5.QtWidgets import QApplication
+# can use PySide6 as well
+from pyqt_dreamstudio.main import ImageGeneratingToolWidget
+
 
 if __name__ == "__main__":
+    import sys
+
     app = QApplication(sys.argv)
-    w = ImageGeneratingToolWidget()
-    w.show()
+    window = ImageGeneratingToolWidget()
+    window.show()
     sys.exit(app.exec_())
 ```
 
 ## How to Use
 There is the options tab at the right side of the window. 
 
 Input your API key, choose parameters you want to set, write propmt, submit it, and you can see the result at the left side (which looks like file explorer) soon enough.
```

### Comparing `pyqt-dreamstudio-0.0.11/README.md` & `pyqt-dreamstudio-0.0.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,25 @@
 4. python setup.py install
 5. cd pyqt_dreamstudio
 6. python main.py
 ### By pip
 1. pip install pyqt_dreamstudio
 2. 
 ```python
-from pyqt_dreamstudio.imageGeneratingToolWidget import ImageGeneratingToolWidget
+from PyQt5.QtWidgets import QApplication
+# can use PySide6 as well
+from pyqt_dreamstudio.main import ImageGeneratingToolWidget
+
 
 if __name__ == "__main__":
+    import sys
+
     app = QApplication(sys.argv)
-    w = ImageGeneratingToolWidget()
-    w.show()
+    window = ImageGeneratingToolWidget()
+    window.show()
     sys.exit(app.exec_())
 ```
 
 ## How to Use
 There is the options tab at the right side of the window. 
 
 Input your API key, choose parameters you want to set, write propmt, submit it, and you can see the result at the left side (which looks like file explorer) soon enough.
```

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/currentImageView.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/currentImageView.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/explorerWidget.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/explorerWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/history.svg` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/ico/history.svg`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/setting.svg` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/ico/setting.svg`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageListWidget.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/imageListWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageSqlite.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/imageSqlite.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageStableDiffusionPage.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/imageStableDiffusionPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/inputDialog.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/inputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/leftSideBar.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/leftSideBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/logo.png` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/logo.png`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/main.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/main.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/notifier.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/notifier.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/rightSideBar.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/rightSideBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/searchBar.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/searchBar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from qtpy.QtWidgets import QWidget, QLineEdit, QGridLayout, QLabel, \
     QHBoxLayout, QApplication, QSizePolicy
 from qtpy.QtCore import Signal
-from svgLabel import SvgLabel
+from pyqt_dreamstudio.svgLabel import SvgLabel
 
 
 class SearchBar(QWidget):
     searched = Signal(str)
 
     def __init__(self, parent=None):
         super().__init__(parent)
```

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/svgButton.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/svgButton.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/svgLabel.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/svgLabel.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/thumbnailView.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/thumbnailView.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/toast.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/toast.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/viewWidget.py` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio/viewWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/PKG-INFO` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-dreamstudio
-Version: 0.0.11
+Version: 0.0.12
 Summary: Using DreamStudio API in Python desktop application
 Home-page: https://github.com/yjg30737/pyqt-dreamstudio.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,20 +34,25 @@
 4. python setup.py install
 5. cd pyqt_dreamstudio
 6. python main.py
 ### By pip
 1. pip install pyqt_dreamstudio
 2. 
 ```python
-from pyqt_dreamstudio.imageGeneratingToolWidget import ImageGeneratingToolWidget
+from PyQt5.QtWidgets import QApplication
+# can use PySide6 as well
+from pyqt_dreamstudio.main import ImageGeneratingToolWidget
+
 
 if __name__ == "__main__":
+    import sys
+
     app = QApplication(sys.argv)
-    w = ImageGeneratingToolWidget()
-    w.show()
+    window = ImageGeneratingToolWidget()
+    window.show()
     sys.exit(app.exec_())
 ```
 
 ## How to Use
 There is the options tab at the right side of the window. 
 
 Input your API key, choose parameters you want to set, write propmt, submit it, and you can see the result at the left side (which looks like file explorer) soon enough.
```

### Comparing `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/SOURCES.txt` & `pyqt-dreamstudio-0.0.12/pyqt_dreamstudio.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -21,9 +21,11 @@
 pyqt_dreamstudio/viewWidget.py
 pyqt_dreamstudio.egg-info/PKG-INFO
 pyqt_dreamstudio.egg-info/SOURCES.txt
 pyqt_dreamstudio.egg-info/dependency_links.txt
 pyqt_dreamstudio.egg-info/requires.txt
 pyqt_dreamstudio.egg-info/top_level.txt
 pyqt_dreamstudio/ico/__init__.py
+pyqt_dreamstudio/ico/copy_light.svg
 pyqt_dreamstudio/ico/history.svg
+pyqt_dreamstudio/ico/save_light.svg
 pyqt_dreamstudio/ico/setting.svg
```

### Comparing `pyqt-dreamstudio-0.0.11/setup.py` & `pyqt-dreamstudio-0.0.12/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='pyqt-dreamstudio',
-    version='0.0.11',
+    version='0.0.12',
     author='Jung Gyu Yoon',
     author_email='yjg30737@gmail.com',
     license='MIT',
     packages=find_packages(),
-    package_data={'pyqt_dreamstudio': ['logo.png'], 'pyqt_dreamstudio.ico': ['history.svg', 'setting.svg']},
+    package_data={'pyqt_dreamstudio': ['logo.png'], 'pyqt_dreamstudio.ico': ['history.svg', 'setting.svg', 'copy_light.svg', 'save_light.svg']},
     description='Using DreamStudio API in Python desktop application',
     url='https://github.com/yjg30737/pyqt-dreamstudio.git',
     long_description_content_type='text/markdown',
     long_description=long_description,
     install_requires=[
         'PyQt5>=5.14',
         'PySide6',
```

