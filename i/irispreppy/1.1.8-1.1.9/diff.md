# Comparing `tmp/irispreppy-1.1.8.tar.gz` & `tmp/irispreppy-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irispreppy-1.1.8.tar", last modified: Wed Mar 22 18:02:56 2023, max compression
+gzip compressed data, was "irispreppy-1.1.9.tar", last modified: Wed Mar 22 18:09:01 2023, max compression
```

## Comparing `irispreppy-1.1.8.tar` & `irispreppy-1.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:02:56.089427 irispreppy-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 18:02:47.000000 irispreppy-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-22 18:02:47.000000 irispreppy-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-22 18:02:56.089427 irispreppy-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-22 18:02:47.000000 irispreppy-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:02:56.085427 irispreppy-1.1.8/irispreppy/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:02:56.085427 irispreppy-1.1.8/irispreppy/psf/
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/psf/IRIS_SG_PSFs.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/psf/IRIS_SG_deconvolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/psf/deconvolve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:02:56.085427 irispreppy-1.1.8/irispreppy/radcal/
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/radcal/iris_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/radcal/radcal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:02:56.089427 irispreppy-1.1.8/irispreppy/radcal/responses/
--rw-r--r--   0 runner    (1001) docker     (123)   394039 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_20130211.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   394068 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_20130715.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   396255 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_c_20150331.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   396488 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_c_20161022.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   396489 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_c_20191101.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   396964 2023-03-22 18:02:47.000000 irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_c_20200223.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:02:56.085427 irispreppy-1.1.8/irispreppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-22 18:02:56.000000 irispreppy-1.1.8/irispreppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-22 18:02:56.000000 irispreppy-1.1.8/irispreppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 18:02:56.000000 irispreppy-1.1.8/irispreppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 18:02:55.000000 irispreppy-1.1.8/irispreppy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-22 18:02:56.000000 irispreppy-1.1.8/irispreppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 18:02:56.000000 irispreppy-1.1.8/irispreppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 18:02:56.089427 irispreppy-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-22 18:02:47.000000 irispreppy-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:09:01.800244 irispreppy-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 18:08:49.000000 irispreppy-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-22 18:08:49.000000 irispreppy-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-22 18:09:01.800244 irispreppy-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-22 18:08:49.000000 irispreppy-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:09:01.796244 irispreppy-1.1.9/irispreppy/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:09:01.796244 irispreppy-1.1.9/irispreppy/psf/
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/psf/IRIS_SG_PSFs.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/psf/IRIS_SG_deconvolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/psf/deconvolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:09:01.800244 irispreppy-1.1.9/irispreppy/radcal/
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/radcal/iris_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17873 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/radcal/radcal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:09:01.800244 irispreppy-1.1.9/irispreppy/radcal/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)   394039 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_20130211.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   394068 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_20130715.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   396255 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_c_20150331.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   396488 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_c_20161022.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   396489 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_c_20191101.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   396964 2023-03-22 18:08:49.000000 irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_c_20200223.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:09:01.796244 irispreppy-1.1.9/irispreppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-22 18:09:01.000000 irispreppy-1.1.9/irispreppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-22 18:09:01.000000 irispreppy-1.1.9/irispreppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 18:09:01.000000 irispreppy-1.1.9/irispreppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 18:09:01.000000 irispreppy-1.1.9/irispreppy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-22 18:09:01.000000 irispreppy-1.1.9/irispreppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 18:09:01.000000 irispreppy-1.1.9/irispreppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 18:09:01.800244 irispreppy-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-22 18:08:49.000000 irispreppy-1.1.9/setup.py
```

### Comparing `irispreppy-1.1.8/LICENSE` & `irispreppy-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/PKG-INFO` & `irispreppy-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irispreppy
-Version: 1.1.8
+Version: 1.1.9
 Home-page: https://github.com/OfAaron3/irispreppy
 Author: Aaron W. Peat
 Author-email: a.peat.1@research.gla.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irispreppy-1.1.8/README.md` & `irispreppy-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/psf/IRIS_SG_PSFs.pkl` & `irispreppy-1.1.9/irispreppy/psf/IRIS_SG_PSFs.pkl`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/psf/IRIS_SG_deconvolve.py` & `irispreppy-1.1.9/irispreppy/psf/IRIS_SG_deconvolve.py`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/psf/deconvolve.py` & `irispreppy-1.1.9/irispreppy/psf/deconvolve.py`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/radcal/iris_get_response.py` & `irispreppy-1.1.9/irispreppy/radcal/iris_get_response.py`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/radcal/radcal.py` & `irispreppy-1.1.9/irispreppy/radcal/radcal.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
                 hdr0['TDP90_'+str(indices[key])]=flatdat[int(np.round(len(flatdat)*0.9))]
                 hdr0['TDP95_'+str(indices[key])]=flatdat[int(np.round(len(flatdat)*0.95))]
                 hdr0['TDP98_'+str(indices[key])]=flatdat[int(np.round(len(flatdat)*0.98))]
                 hdr0['TDP99_'+str(indices[key])]=flatdat[int(np.round(len(flatdat)*0.99))]
                 del flatdat
             else:
                 dat[key]=dc(rasfits[indices[key]].data[lamwin[key][0]:lamwin[key][1]])
-                for ind, _ in np.ndenumerate(dat[key][0]):
+                for ind, _ in np.ndenumerate(dat[key][...,0]):
                     dat[key][ind]=np.multiply(dat[key][ind], rcfs[key])
                 hdrdict[key]=dc(rasfits[indices[key]].header)
                 hdrdict[key]['CRVAL3']=wvlns[key][lamwin[key][0]]
                 hdrdict[key]['NAXIS3']=lamwin[key][1]-lamwin[key][0]+1 #Counting "0", of course
 
 
         if key!='NUV' and key!='FUV': #Full disc
@@ -396,15 +396,15 @@
             phdu=fits.PrimaryHDU(None, header=hdr0)
             hduls=[phdu]
             for key in indices:
                 hduls.append(fits.ImageHDU(dat[key], header=hdrdict[key]))
         
         else:
             phdu=fits.PrimaryHDU(dat[list(indices.keys())[0]], header=hdrdict[list(indices.keys())[0]])
-            hduls[phdu]
+            hduls=[phdu]
             for hds in range(1, len(rasfits)):
                 hduls.append(dc(asfits[hds]))
 
         hdul=fits.HDUList(hduls)
         if save:
             hdul.writeto(rasfits.filename()[:-5]+'_rc.fits')
         else:
```

### Comparing `irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_20130211.pkl` & `irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_20130211.pkl`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_20130715.pkl` & `irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_20130715.pkl`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_c_20150331.pkl` & `irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_c_20150331.pkl`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_c_20161022.pkl` & `irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_c_20161022.pkl`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_c_20191101.pkl` & `irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_c_20191101.pkl`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy/radcal/responses/iris_sra_c_20200223.pkl` & `irispreppy-1.1.9/irispreppy/radcal/responses/iris_sra_c_20200223.pkl`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/irispreppy.egg-info/PKG-INFO` & `irispreppy-1.1.9/irispreppy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irispreppy
-Version: 1.1.8
+Version: 1.1.9
 Home-page: https://github.com/OfAaron3/irispreppy
 Author: Aaron W. Peat
 Author-email: a.peat.1@research.gla.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irispreppy-1.1.8/irispreppy.egg-info/SOURCES.txt` & `irispreppy-1.1.9/irispreppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irispreppy-1.1.8/setup.py` & `irispreppy-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 setup(name='irispreppy',
-      version="1.1.8",
+      version="1.1.9",
       url='https://github.com/OfAaron3/irispreppy',
       author='Aaron W. Peat',
       author_email='a.peat.1@research.gla.ac.uk',
       license='MIT',
       packages=['irispreppy.psf', 'irispreppy.radcal', 'irispreppy', 'irispreppy.radcal.responses'],
       install_requires=[
           'numpy',
```

