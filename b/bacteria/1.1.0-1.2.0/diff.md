# Comparing `tmp/bacteria-1.1.0.tar.gz` & `tmp/bacteria-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-1.1.0.tar", last modified: Mon May 29 16:52:00 2023, max compression
+gzip compressed data, was "bacteria-1.2.0.tar", last modified: Mon May 29 16:58:43 2023, max compression
```

## Comparing `bacteria-1.1.0.tar` & `bacteria-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 16:52:00.294000 bacteria-1.1.0/
--rw-rw-rw-   0        0        0      593 2023-05-29 16:52:00.147000 bacteria-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      826 2023-04-30 14:09:49.000000 bacteria-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 16:51:59.661000 bacteria-1.1.0/bacteria/
--rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-1.1.0/bacteria/__init__.py
--rw-rw-rw-   0        0        0   146448 2023-05-29 16:50:59.000000 bacteria-1.1.0/bacteria/functions.py
-drwxrwxrwx   0        0        0        0 2023-05-29 16:52:00.080000 bacteria-1.1.0/bacteria.egg-info/
--rw-rw-rw-   0        0        0      593 2023-05-29 16:51:58.000000 bacteria-1.1.0/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-05-29 16:51:58.000000 bacteria-1.1.0/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 16:51:58.000000 bacteria-1.1.0/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-29 16:51:58.000000 bacteria-1.1.0/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 16:51:58.000000 bacteria-1.1.0/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 16:52:00.255000 bacteria-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1096 2023-05-29 16:51:21.000000 bacteria-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:58:43.818000 bacteria-1.2.0/
+-rw-rw-rw-   0        0        0      593 2023-05-29 16:58:43.745000 bacteria-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-04-30 14:09:49.000000 bacteria-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 16:58:43.248000 bacteria-1.2.0/bacteria/
+-rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-1.2.0/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   146428 2023-05-29 16:58:16.000000 bacteria-1.2.0/bacteria/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:58:43.729000 bacteria-1.2.0/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-05-29 16:58:42.000000 bacteria-1.2.0/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-05-29 16:58:42.000000 bacteria-1.2.0/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 16:58:42.000000 bacteria-1.2.0/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-29 16:58:42.000000 bacteria-1.2.0/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 16:58:42.000000 bacteria-1.2.0/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 16:58:43.785000 bacteria-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1096 2023-05-29 16:58:34.000000 bacteria-1.2.0/setup.py
```

### Comparing `bacteria-1.1.0/PKG-INFO` & `bacteria-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 1.1.0
+Version: 1.2.0
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-1.1.0/README.md` & `bacteria-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bacteria-1.1.0/bacteria/functions.py` & `bacteria-1.2.0/bacteria/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1293,24 +1293,24 @@
         out.append(ax.fill_between(times,ci[:,0],ci[:,1],color=color, alpha = .3))
         out.append(ax.set_title(column+ ' Mean', fontsize = 17))
         out.append(ax.set_xlabel('Time (min)', fontsize = 15))
         out.append(ax.set_ylabel(column, fontsize = 17))
         
         return out
 
-def column2d_mean(df,column = 'Vd-Vb',window=30,conf = .95, method = np.mean):
+def column2d_mean(df,column = 'Vd-Vb',window=30, conf = .95, method = np.mean):
     """
     Estimate the column mean for all cells using
     the 'pd.melt()' method, sorting by time at division.
 
     Parameters
     --------------
     df : DataFrame
         DataFrame with the deravtive data alongside 
-        with the time and volume or the 3D df
+        with the time and volume or the 2D df
     column : str
         column to calculate the mean
     window : int
         value to use in 'rolling.mean()'
     conf : float (optional)
         confidence interval desired for bootstrap,
         default - 0.95
@@ -1326,16 +1326,15 @@
     mean : nd.array
         1D time vector with the mean for 
         each time point
     ci : nd.array
         array(2,bins) with inferior Confidence
         Interval in the first column and the 
     """
-    df_2d_temp = pd.melt(df2d, id_vars=['Cell ID','Cell age','Area death','Time Division'], value_vars=[column]).sort_values(by=['Time Division'])
-    len_data = []
+    df_2d_temp = pd.melt(df, id_vars=['Cell ID','Cell age','Area death','Time Division'], value_vars=[column]).sort_values(by=['Time Division'])
     if column == 'Vd-Vb':
         mean = df_2d_temp.value.rolling(window).mean().dropna()
     else:
         mean = df_2d_temp[column].rolling(window).mean().dropna()
     times = df_2d_temp[df_2d_temp['Time Division'].index.isin(mean.index)]['Time Division'].values
     ci = np.zeros((len(mean),2))
```

### Comparing `bacteria-1.1.0/bacteria.egg-info/PKG-INFO` & `bacteria-1.2.0/bacteria.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 1.1.0
+Version: 1.2.0
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-1.1.0/setup.py` & `bacteria-1.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '1.1.0',      
+    version = '1.2.0',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
     url = 'https://bacteria.readthedocs.io',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

