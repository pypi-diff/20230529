# Comparing `tmp/xcodex-0.0.4.tar.gz` & `tmp/xcodex-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcodex-0.0.4.tar", last modified: Sun May 28 14:45:02 2023, max compression
+gzip compressed data, was "xcodex-0.0.5.tar", last modified: Mon May 29 19:54:47 2023, max compression
```

## Comparing `xcodex-0.0.4.tar` & `xcodex-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:02.836321 xcodex-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-28 14:44:22.000000 xcodex-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-28 14:45:02.836321 xcodex-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-28 14:44:22.000000 xcodex-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-28 14:44:22.000000 xcodex-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:45:02.836321 xcodex-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-28 14:44:22.000000 xcodex-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:02.832321 xcodex-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:02.836321 xcodex-0.0.4/src/Util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/create_dodsrc.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/create_netrc.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/download_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/download_file_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/generate_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/make_Dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/Util/var_imp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:02.836321 xcodex-0.0.4/src/xcodex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/xcodex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-05-28 14:44:22.000000 xcodex-0.0.4/src/xcodex/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:02.836321 xcodex-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 14:44:22.000000 xcodex-0.0.4/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:02.836321 xcodex-0.0.4/xcodex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-28 14:45:02.000000 xcodex-0.0.4/xcodex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-28 14:45:02.000000 xcodex-0.0.4/xcodex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:45:02.000000 xcodex-0.0.4/xcodex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-28 14:45:02.000000 xcodex-0.0.4/xcodex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-28 14:45:02.000000 xcodex-0.0.4/xcodex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-29 19:54:14.000000 xcodex-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-29 19:54:47.786617 xcodex-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-29 19:54:14.000000 xcodex-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-29 19:54:14.000000 xcodex-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:54:47.786617 xcodex-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-29 19:54:14.000000 xcodex-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.782617 xcodex-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/src/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/create_dodsrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/create_netrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/download_file_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/generate_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/make_Dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/var_imp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/src/xcodex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/xcodex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/xcodex/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 19:54:14.000000 xcodex-0.0.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/xcodex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/top_level.txt
```

### Comparing `xcodex-0.0.4/LICENSE` & `xcodex-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.4/PKG-INFO` & `xcodex-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xcodex
-Version: 0.0.4
-Summary: This package will extract daily data from netCDF4 files downloaded at GES DISC database"
+Version: 0.0.5
+Summary: This package will download and extract daily data of XCO2 from the NASA Goddard Earth Sciences (GES)
 Author: henriquefl24@git
 Author-email: Henrique Fontellas Laurito <henrique.f.laurito@unesp.br>
 Project-URL: Homepage, https://github.com/henriquefl24/xcodex
 Project-URL: Bug Tracker, https://github.com/henriquefl24/xcodex/issues
 Keywords: python,NASA,GES DISC,XCO2,daily,OCO-2,jupyter notebook,xcodex
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,41 +16,45 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![CABEÇALHO](https://i.imgur.com/Pq8uUM3.jpg)
 
+### *Please, cite this package as:*
+
+Laurito, H., La Scala, N., Rolim, G. S., 2023. Extracting XCO2-NASA Daily data with XCODEX:
+A Python package designed for data extraction and structuration. Jaboticabal, SP, BR, (...)
 
 # **Welcome to XCODEX - XCO2 Daily EXtractor**
 
 Hi there! My name is Henrique.
 
 The creation of this Python package was intended to create a simple solution for extracting daily data from XCO2 retrieved from the GES DISC platform.
 
 I will attach the links containing the GitHub profile of the researchers who helped me in the development of this package along with graphical visualization of the data and the citation of the OCO-2 project.
 
 I hope it's useful to you. **Long live science!**
 
-## *Instaling the package*
+## *Installing the package*
 
 To install the package, use the command:
 ```angular2html
 pip install xcodex
 ```
 ## *Using XCODEX*
 
 There's the possibility to download the .nc4 files directly here:
 ```angular2html
 # Setting historical serie
 
-from Util.download_data import download_file
+from xcodex.main import download_file
 
-start_date = "1st of February, 2022"
-end_date = "28th of February, 2022"
+start_date = "1st of January, 2022"
+end_date = "31st of January, 2022"
 
 # Downloading .nc4 files
 download_file(start_date, end_date) 
 ```
 __Note that ERROR 401 usually is related to unavailable data.__
 
 Once the download is completed, a ``downloaded_data`` folder will be created in your current path.
@@ -62,31 +66,30 @@
 from os.path import join
 from os import getcwd
 
 # Selecting the folder with .nc4 files
 
 arquive_folder = glob(join(getcwd(), "downloaded_data", "*.nc4")) 
 
-# Setting desired locations
+# Setting desired locations to build a time series XCO2 data
 
 locations = dict(Mauna_loa=[19.479488, -155.602829],
                  New_York=[40.712776, -74.005974],
                  Paris=[48.856613, 2.352222])
 
 from xcodex.main import xco2_extract
 
 df = xco2_extract(path=arquive_folder,
                   start=start_date,
                   end=end_date,
                   missing_data=False,
-                  **locations) # Extracting XCO2
-
-df          
+                  **locations); df # Extracting XCO2
+      
 ```
-Note1: The location used in this example was Mauna Loa. Any location can be used<br>
+Note1: The location used in this example was Mauna Loa, New York and Paris. Any location can be used<br>
 as long the format "Location[lat, lon]" is respected. The values of <br>
 latitude and longitude must be in decimal degrees.
 
 for more information, please execute the command: <br>
 
 ````angular2html
 help(xco2_extractor)
@@ -178,18 +181,13 @@
 ````
 ### *GitHub profiles*:
 
 https://github.com/GlaucoRolim (Co-author) <br>
 https://github.com/kyuenjpl/ARSET_XCO2 <br>
 https://github.com/sagarlimbu0/OCO2-OCO3
 
-### *Please, cite this package as:*
-
-Laurito, H., Rolim, G., 2023. Extracting XCO2-NASA Daily data with XCODEX:
-A Python package designed for data extraction and structuration. Jaboticabal, SP, BR, (...)
-
 ### **Data source citation**:
 
 Brad Weir, Lesley Ott and OCO-2 Science Team (2022), OCO-2 GEOS Level 3 daily,
 0.5x0.625 assimilated CO2 V10r, Greenbelt, MD, USA, Goddard Earth Sciences Data
 and Information Services Center (GES DISC), Accessed: 10/31/2022,
 doi: 10.5067/Y9M4NM9MPCGH
```

### Comparing `xcodex-0.0.4/README.md` & `xcodex-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 ![CABEÇALHO](https://i.imgur.com/Pq8uUM3.jpg)
 
+### *Please, cite this package as:*
+
+Laurito, H., La Scala, N., Rolim, G. S., 2023. Extracting XCO2-NASA Daily data with XCODEX:
+A Python package designed for data extraction and structuration. Jaboticabal, SP, BR, (...)
 
 # **Welcome to XCODEX - XCO2 Daily EXtractor**
 
 Hi there! My name is Henrique.
 
 The creation of this Python package was intended to create a simple solution for extracting daily data from XCO2 retrieved from the GES DISC platform.
 
 I will attach the links containing the GitHub profile of the researchers who helped me in the development of this package along with graphical visualization of the data and the citation of the OCO-2 project.
 
 I hope it's useful to you. **Long live science!**
 
-## *Instaling the package*
+## *Installing the package*
 
 To install the package, use the command:
 ```angular2html
 pip install xcodex
 ```
 ## *Using XCODEX*
 
 There's the possibility to download the .nc4 files directly here:
 ```angular2html
 # Setting historical serie
 
-from Util.download_data import download_file
+from xcodex.main import download_file
 
-start_date = "1st of February, 2022"
-end_date = "28th of February, 2022"
+start_date = "1st of January, 2022"
+end_date = "31st of January, 2022"
 
 # Downloading .nc4 files
 download_file(start_date, end_date) 
 ```
 __Note that ERROR 401 usually is related to unavailable data.__
 
 Once the download is completed, a ``downloaded_data`` folder will be created in your current path.
@@ -42,31 +46,30 @@
 from os.path import join
 from os import getcwd
 
 # Selecting the folder with .nc4 files
 
 arquive_folder = glob(join(getcwd(), "downloaded_data", "*.nc4")) 
 
-# Setting desired locations
+# Setting desired locations to build a time series XCO2 data
 
 locations = dict(Mauna_loa=[19.479488, -155.602829],
                  New_York=[40.712776, -74.005974],
                  Paris=[48.856613, 2.352222])
 
 from xcodex.main import xco2_extract
 
 df = xco2_extract(path=arquive_folder,
                   start=start_date,
                   end=end_date,
                   missing_data=False,
-                  **locations) # Extracting XCO2
-
-df          
+                  **locations); df # Extracting XCO2
+      
 ```
-Note1: The location used in this example was Mauna Loa. Any location can be used<br>
+Note1: The location used in this example was Mauna Loa, New York and Paris. Any location can be used<br>
 as long the format "Location[lat, lon]" is respected. The values of <br>
 latitude and longitude must be in decimal degrees.
 
 for more information, please execute the command: <br>
 
 ````angular2html
 help(xco2_extractor)
@@ -158,18 +161,13 @@
 ````
 ### *GitHub profiles*:
 
 https://github.com/GlaucoRolim (Co-author) <br>
 https://github.com/kyuenjpl/ARSET_XCO2 <br>
 https://github.com/sagarlimbu0/OCO2-OCO3
 
-### *Please, cite this package as:*
-
-Laurito, H., Rolim, G., 2023. Extracting XCO2-NASA Daily data with XCODEX:
-A Python package designed for data extraction and structuration. Jaboticabal, SP, BR, (...)
-
 ### **Data source citation**:
 
 Brad Weir, Lesley Ott and OCO-2 Science Team (2022), OCO-2 GEOS Level 3 daily,
 0.5x0.625 assimilated CO2 V10r, Greenbelt, MD, USA, Goddard Earth Sciences Data
 and Information Services Center (GES DISC), Accessed: 10/31/2022,
 doi: 10.5067/Y9M4NM9MPCGH
```

### Comparing `xcodex-0.0.4/pyproject.toml` & `xcodex-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 	"requests~=2.31.0",
 	"setuptools==67.8.0",
 	"jupyter==1.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xcodex"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   {name="Henrique Fontellas Laurito", email="henrique.f.laurito@unesp.br" }
 ]
-description = """This package will extract daily data from netCDF4 files downloaded at GES DISC database"
+description = """This package will download and extract daily data of XCO2 from the NASA Goddard Earth Sciences (GES)
+                 Data and Information Services Center (DISC)"
 
               Source citation: Brad Weir, Lesley Ott and OCO-2 Science Team (2022), OCO-2 GEOS Level 3 daily,
               0.5x0.625 assimilated CO2 V10r, Greenbelt, MD, USA, Goddard Earth Sciences Data
               and Information Services Center (GES DISC), Accessed: 10/31/2022,
               doi: 10.5067/Y9M4NM9MPCGH"""
 
 readme = "README.md"
```

### Comparing `xcodex-0.0.4/setup.py` & `xcodex-0.0.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from setuptools import setup
 
-VERSION = "0.0.4"
-DESCRIPTION = """This package will extract daily data from netCDF4 files downloaded at GES DISC database"
+VERSION = "0.0.5"
+DESCRIPTION = """This package will download and extract daily data of XCO2 from the NASA Goddard Earth Sciences (GES) 
+                 Data and Information Services Center (DISC)"
               Source citation: Brad Weir, Lesley Ott and OCO-2 Science Team (2022), OCO-2 GEOS Level 3 daily,
               0.5x0.625 assimilated CO2 V10r, Greenbelt, MD, USA, Goddard Earth Sciences Data
               and Information Services Center (GES DISC), Accessed: 10/31/2022,
               doi: 10.5067/Y9M4NM9MPCGH"""
 
 # Setting up
```

### Comparing `xcodex-0.0.4/src/Util/check.py` & `xcodex-0.0.5/src/Util/check.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.4/src/Util/download.py` & `xcodex-0.0.5/src/Util/download.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.4/src/Util/download_file_progress.py` & `xcodex-0.0.5/src/Util/download_file_progress.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.4/src/Util/generate_links.py` & `xcodex-0.0.5/src/Util/generate_links.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.4/src/Util/make_Dataframe.py` & `xcodex-0.0.5/src/Util/make_Dataframe.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 
     """
 
     dataframe = DataFrame()
 
     # Assigning List Values to the Dataframe
 
-    dataframe['city'] = city
+    dataframe['location'] = city
     dataframe['jd'] = jd
     dataframe['day'] = day
     dataframe['month'] = month
     dataframe['year'] = year
     dataframe['lat'] = lat
     dataframe['lon'] = lon
     dataframe['lat_index'] = lat_index
     dataframe['lon_index'] = lon_index
-    dataframe['xco2'] = XCO2_values
-    dataframe['xco2_prec'] = XCO2PREC_values
+    dataframe['XCO2'] = XCO2_values
+    dataframe['XCO2_prec'] = XCO2PREC_values
 
     # Organizing the dataframe
 
-    dataframe.sort_values(by=['city', 'year'], inplace=True)
+    dataframe.sort_values(by=['location', 'year'], inplace=True)
     dataframe.reset_index(inplace=True, drop=True)
 
     return dataframe
```

### Comparing `xcodex-0.0.4/src/Util/missing.py` & `xcodex-0.0.5/src/Util/missing.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.4/src/Util/var_imp.py` & `xcodex-0.0.5/src/Util/var_imp.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.4/src/xcodex/main.py` & `xcodex-0.0.5/src/xcodex/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -164,12 +164,30 @@
                                lon_index, XCO2_values, XCO2PREC_values)
 
     if missing_data:
         new_subset(dataframe)
 
     # Padronizing values to float
 
-    dataframe.set_index('city', inplace=True, drop=True)
+    dataframe.set_index('location', inplace=True, drop=True)
     dataframe = dataframe.astype(float)
     dataframe.reset_index(inplace=True, drop=False)
 
     return dataframe
+
+
+def download_file(start: str, end: str) -> None:
+    """
+    This method will effectively download .nc4 files from NASA
+    Args:
+        start: start date (i.e.: "1st of January, 2015")
+        end: amount of days (i.e.: 365 days)
+
+    Returns: None
+    """
+    from Util.date import calendar_days
+    from Util.generate_links import generate_links
+    from Util.download import download
+
+    date_list = calendar_days(start, end)
+    links = generate_links(date_list)
+    download(links)
```

### Comparing `xcodex-0.0.4/xcodex.egg-info/PKG-INFO` & `xcodex-0.0.5/xcodex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xcodex
-Version: 0.0.4
-Summary: This package will extract daily data from netCDF4 files downloaded at GES DISC database"
+Version: 0.0.5
+Summary: This package will download and extract daily data of XCO2 from the NASA Goddard Earth Sciences (GES)
 Author: henriquefl24@git
 Author-email: Henrique Fontellas Laurito <henrique.f.laurito@unesp.br>
 Project-URL: Homepage, https://github.com/henriquefl24/xcodex
 Project-URL: Bug Tracker, https://github.com/henriquefl24/xcodex/issues
 Keywords: python,NASA,GES DISC,XCO2,daily,OCO-2,jupyter notebook,xcodex
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,41 +16,45 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![CABEÇALHO](https://i.imgur.com/Pq8uUM3.jpg)
 
+### *Please, cite this package as:*
+
+Laurito, H., La Scala, N., Rolim, G. S., 2023. Extracting XCO2-NASA Daily data with XCODEX:
+A Python package designed for data extraction and structuration. Jaboticabal, SP, BR, (...)
 
 # **Welcome to XCODEX - XCO2 Daily EXtractor**
 
 Hi there! My name is Henrique.
 
 The creation of this Python package was intended to create a simple solution for extracting daily data from XCO2 retrieved from the GES DISC platform.
 
 I will attach the links containing the GitHub profile of the researchers who helped me in the development of this package along with graphical visualization of the data and the citation of the OCO-2 project.
 
 I hope it's useful to you. **Long live science!**
 
-## *Instaling the package*
+## *Installing the package*
 
 To install the package, use the command:
 ```angular2html
 pip install xcodex
 ```
 ## *Using XCODEX*
 
 There's the possibility to download the .nc4 files directly here:
 ```angular2html
 # Setting historical serie
 
-from Util.download_data import download_file
+from xcodex.main import download_file
 
-start_date = "1st of February, 2022"
-end_date = "28th of February, 2022"
+start_date = "1st of January, 2022"
+end_date = "31st of January, 2022"
 
 # Downloading .nc4 files
 download_file(start_date, end_date) 
 ```
 __Note that ERROR 401 usually is related to unavailable data.__
 
 Once the download is completed, a ``downloaded_data`` folder will be created in your current path.
@@ -62,31 +66,30 @@
 from os.path import join
 from os import getcwd
 
 # Selecting the folder with .nc4 files
 
 arquive_folder = glob(join(getcwd(), "downloaded_data", "*.nc4")) 
 
-# Setting desired locations
+# Setting desired locations to build a time series XCO2 data
 
 locations = dict(Mauna_loa=[19.479488, -155.602829],
                  New_York=[40.712776, -74.005974],
                  Paris=[48.856613, 2.352222])
 
 from xcodex.main import xco2_extract
 
 df = xco2_extract(path=arquive_folder,
                   start=start_date,
                   end=end_date,
                   missing_data=False,
-                  **locations) # Extracting XCO2
-
-df          
+                  **locations); df # Extracting XCO2
+      
 ```
-Note1: The location used in this example was Mauna Loa. Any location can be used<br>
+Note1: The location used in this example was Mauna Loa, New York and Paris. Any location can be used<br>
 as long the format "Location[lat, lon]" is respected. The values of <br>
 latitude and longitude must be in decimal degrees.
 
 for more information, please execute the command: <br>
 
 ````angular2html
 help(xco2_extractor)
@@ -178,18 +181,13 @@
 ````
 ### *GitHub profiles*:
 
 https://github.com/GlaucoRolim (Co-author) <br>
 https://github.com/kyuenjpl/ARSET_XCO2 <br>
 https://github.com/sagarlimbu0/OCO2-OCO3
 
-### *Please, cite this package as:*
-
-Laurito, H., Rolim, G., 2023. Extracting XCO2-NASA Daily data with XCODEX:
-A Python package designed for data extraction and structuration. Jaboticabal, SP, BR, (...)
-
 ### **Data source citation**:
 
 Brad Weir, Lesley Ott and OCO-2 Science Team (2022), OCO-2 GEOS Level 3 daily,
 0.5x0.625 assimilated CO2 V10r, Greenbelt, MD, USA, Goddard Earth Sciences Data
 and Information Services Center (GES DISC), Accessed: 10/31/2022,
 doi: 10.5067/Y9M4NM9MPCGH
```

