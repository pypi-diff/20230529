# Comparing `tmp/type3detect-0.0.1.tar.gz` & `tmp/type3detect-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "type3detect-0.0.1.tar", last modified: Sat Oct 22 17:13:48 2022, max compression
+gzip compressed data, was "type3detect-0.0.2.tar", last modified: Mon May 29 13:18:57 2023, max compression
```

## Comparing `type3detect-0.0.1.tar` & `type3detect-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-10-22 17:13:48.855477 type3detect-0.0.1/
--rw-rw-rw-   0        0        0     2622 2022-10-22 17:13:48.854473 type3detect-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-10-22 17:13:48.855477 type3detect-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1968 2022-10-22 16:04:34.000000 type3detect-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-22 17:13:48.844218 type3detect-0.0.1/type3detect/
--rw-rw-rw-   0        0        0     3049 2022-10-22 15:38:05.000000 type3detect-0.0.1/type3detect/ACBone.py
--rw-rw-rw-   0        0        0       88 2022-10-22 16:23:08.000000 type3detect-0.0.1/type3detect/__init__.py
--rw-rw-rw-   0        0        0     5905 2022-10-22 17:12:07.000000 type3detect-0.0.1/type3detect/detectRadioburst.py
--rw-rw-rw-   0        0        0     1940 2022-04-30 12:20:33.000000 type3detect-0.0.1/type3detect/radioTools.py
-drwxrwxrwx   0        0        0        0 2022-10-22 17:13:48.853215 type3detect-0.0.1/type3detect.egg-info/
--rw-rw-rw-   0        0        0     2622 2022-10-22 17:13:48.000000 type3detect-0.0.1/type3detect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2022-10-22 17:13:48.000000 type3detect-0.0.1/type3detect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-22 17:13:48.000000 type3detect-0.0.1/type3detect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-10-22 17:13:48.000000 type3detect-0.0.1/type3detect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-10-22 17:13:48.000000 type3detect-0.0.1/type3detect.egg-info/top_level.txt
+drwxr-xr-x   0 peijinzh (504179704) ATKK\hyad-all (984178727)        0 2023-05-29 13:18:57.714900 type3detect-0.0.2/
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     3853 2023-05-29 13:18:57.714232 type3detect-0.0.2/PKG-INFO
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       38 2023-05-29 13:18:57.715046 type3detect-0.0.2/setup.cfg
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     1930 2023-05-29 13:16:38.000000 type3detect-0.0.2/setup.py
+drwxr-xr-x   0 peijinzh (504179704) ATKK\hyad-all (984178727)        0 2023-05-29 13:18:57.708742 type3detect-0.0.2/type3detect/
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     2975 2023-05-29 13:02:56.000000 type3detect-0.0.2/type3detect/ACBone.py
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       87 2023-05-29 13:02:56.000000 type3detect-0.0.2/type3detect/__init__.py
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     5905 2023-05-29 13:02:56.000000 type3detect-0.0.2/type3detect/detectRadioburst.py
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     1940 2023-05-29 13:02:56.000000 type3detect-0.0.2/type3detect/radioTools.py
+drwxr-xr-x   0 peijinzh (504179704) ATKK\hyad-all (984178727)        0 2023-05-29 13:18:57.713221 type3detect-0.0.2/type3detect.egg-info/
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     3853 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/PKG-INFO
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)      286 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/SOURCES.txt
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)        1 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/dependency_links.txt
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       42 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/requires.txt
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       12 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/top_level.txt
```

### Comparing `type3detect-0.0.1/setup.py` & `type3detect-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-#from distutils.core import setup
-import setuptools
-from setuptools import setup
-from os import path
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory,'../..','README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-  name = 'type3detect',         # How you named your package folder 
-  packages = setuptools.find_packages(),#['lofarSun','lofarSun.IM','lofarSun.BF','lofarSun.BF.GUI'],   # Chose the same as "name"
-  include_package_data=True,
-  version = '0.0.1',      # Start with a small number and increase it with every change you make
-  license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'tools to process the lofar solar data',   # Give a short description about your library
-  author = 'Peijin',                   # Type in your name
-  author_email = 'pjer1316@gmail.com',      # Type in your E-Mail
-  url = 'https://github.com/peijin94/type3detect',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/peijin94/type3detect/archive/refs/heads/master.zip',    
-  keywords = ['LOFAR', 'Solar', 'radio'],   # Keywords that define your package best
-  install_requires=[            # I get to this in a second
-          'matplotlib',
-          'sunpy',
-          'astropy',
-          'h5py',
-          'scipy',
-          'numpy'
-      ],
-  classifiers=[
-    'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-    'Intended Audience :: Developers',     # Define that your audience are developers
-    'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: MIT License',   # Again, pick a license,
-    'Programming Language :: Python :: 3.8',
-  ],
-  long_description=long_description,
-  long_description_content_type='text/markdown'
-)
+#from distutils.core import setup
+import setuptools
+from setuptools import setup
+from os import path
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory,'../..','README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+  name = 'type3detect',         # How you named your package folder 
+  packages = setuptools.find_packages(),#['lofarSun','lofarSun.IM','lofarSun.BF','lofarSun.BF.GUI'],   # Chose the same as "name"
+  include_package_data=True,
+  version = '0.0.2',      # Start with a small number and increase it with every change you make
+  license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
+  description = 'tools to process the lofar solar data',   # Give a short description about your library
+  author = 'Peijin',                   # Type in your name
+  author_email = 'pjer1316@gmail.com',      # Type in your E-Mail
+  url = 'https://github.com/peijin94/type3detect',   # Provide either the link to your github or to your website
+  download_url = 'https://github.com/peijin94/type3detect/archive/refs/heads/master.zip',    
+  keywords = ['LOFAR', 'Solar', 'radio'],   # Keywords that define your package best
+  install_requires=[            # I get to this in a second
+          'matplotlib',
+          'sunpy',
+          'astropy',
+          'h5py',
+          'scipy',
+          'numpy'
+      ],
+  classifiers=[
+    'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+    'Intended Audience :: Developers',     # Define that your audience are developers
+    'Topic :: Software Development :: Build Tools',
+    'License :: OSI Approved :: MIT License',   # Again, pick a license,
+    'Programming Language :: Python :: 3.9',
+  ],
+  long_description=long_description,
+  long_description_content_type='text/markdown'
+)
```

### Comparing `type3detect-0.0.1/type3detect/ACBone.py` & `type3detect-0.0.2/type3detect/ACBone.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import numpy as np
-import numpy.linalg as LA
-from scipy.interpolate import interp2d
-from scipy.ndimage.filters import gaussian_filter
-import numpy.linalg as LA
-
-def PJcurvature(x,y):
-    """
-    input  : the coordinate of the three point
-    output : the curvature and norm direction
-    refer to https://github.com/peijin94/PJCurvature for detail
-    """
-    t_a = LA.norm([x[1]-x[0],y[1]-y[0]])
-    t_b = LA.norm([x[2]-x[1],y[2]-y[1]])
-
-    M = np.array([
-        [1, -t_a, t_a**2],
-        [1, 0,    0     ],
-        [1,  t_b, t_b**2]])
-
-    a = np.matmul(LA.pinv(M),x)
-    b = np.matmul(LA.pinv(M),y)
-
-    kappa = 2*(a[2]*b[1]-b[2]*a[1])/(a[1]**2.+b[1]**2.)**(1.5)
-    return kappa, [b[1],-a[1]]/np.sqrt(a[1]**2.+b[1]**2.)
-
-
-def ACBone(img,x,y,x0,y0,n_iter = 200,d_step=0.2,alpha=25,beta=6000,y_gap=90.,blur_sigma=2.5):
-        yy = np.linspace((y0[0]),(y0[1]), int(abs(y0[1]-y0[0])/y_gap))
-        xx = np.linspace((x0[0]),(x0[1]), len(yy))# +  np.random.normal(0, 0.1, len(yy))
-
-        blurred = gaussian_filter(img, sigma=blur_sigma)
-
-        Grad_x = interp2d(x, y, np.gradient(img,axis=1)/(np.max(np.gradient(img,axis=1))), kind='quintic')
-        Grad_y = interp2d(x, y, np.gradient(img,axis=0)/(np.max(np.gradient(img,axis=0))), kind='quintic')
-
-
-        Grad_x_blur = interp2d(x, y, np.gradient(blurred,axis=1)/(np.max(np.gradient(blurred,axis=1))), kind='quintic')
-        Grad_y_blur = interp2d(x, y, np.gradient(blurred,axis=0)/(np.max(np.gradient(blurred,axis=0))), kind='quintic')
-
-        xx_new = xx
-        yy_new = yy
-
-        idx_img=0
-        for step in range(n_iter):
-            kappa_arr = np.zeros(len(xx))
-            norm_arr  = np.zeros([len(xx),2])
-            for idx,val in enumerate(xx[1:-1]):
-                ytmp = yy_new[idx:idx+3]
-                xtmp = xx_new[idx:idx+3]
-                kappa,norm_l = PJcurvature(xtmp,ytmp)
-                kappa_arr[idx+1] = kappa
-                norm_arr[idx+1,:] = norm_l
-
-
-            f_x = beta* kappa_arr*norm_arr[:,0]
-            f_x[-1] = -f_x[-2]
-            f_x[0] = -f_x[1]
-            if step>n_iter/3.5 :
-                xx_new = xx_new+ d_step* (alpha * np.array([Grad_x(xx_new[i],yy_new[i])
-                            for i in np.arange(len(xx_new))])[:,0] + f_x)
-            else:
-                xx_new = xx_new+ d_step* (alpha * np.array([Grad_x_blur(xx_new[i],yy_new[i])
-                            for i in np.arange(len(xx_new))])[:,0] + f_x)
-
-            #print(alpha * np.array([Grad_x_blur(xx_new[i],yy_new[i])
-            #                for i in np.arange(len(xx_new))])[:,0])
-            #yy_new = yy_new+ d_step/1000* (alpha * np.array([Grad_y(xx_new[i],yy_new[i])
-            #                                            for i in np.arange(len(xx_new))])[:,0])
-
-        img_xy = interp2d(x, y, img, kind='quintic')
-        flux = np.array([img_xy(xx_new[i],yy_new[i])
-                            for i in np.arange(len(xx_new))])[:,0]
-
+import numpy as np
+import numpy.linalg as LA
+from scipy.interpolate import interp2d
+from scipy.ndimage.filters import gaussian_filter
+import numpy.linalg as LA
+
+def PJcurvature(x,y):
+    """
+    input  : the coordinate of the three point
+    output : the curvature and norm direction
+    refer to https://github.com/peijin94/PJCurvature for detail
+    """
+    t_a = LA.norm([x[1]-x[0],y[1]-y[0]])
+    t_b = LA.norm([x[2]-x[1],y[2]-y[1]])
+
+    M = np.array([
+        [1, -t_a, t_a**2],
+        [1, 0,    0     ],
+        [1,  t_b, t_b**2]])
+
+    a = np.matmul(LA.pinv(M),x)
+    b = np.matmul(LA.pinv(M),y)
+
+    kappa = 2*(a[2]*b[1]-b[2]*a[1])/(a[1]**2.+b[1]**2.)**(1.5)
+    return kappa, [b[1],-a[1]]/np.sqrt(a[1]**2.+b[1]**2.)
+
+
+def ACBone(img,x,y,x0,y0,n_iter = 200,d_step=0.2,alpha=25,beta=6000,y_gap=90.,blur_sigma=2.5):
+        yy = np.linspace((y0[0]),(y0[1]), int(abs(y0[1]-y0[0])/y_gap))
+        xx = np.linspace((x0[0]),(x0[1]), len(yy))# +  np.random.normal(0, 0.1, len(yy))
+
+        blurred = gaussian_filter(img, sigma=blur_sigma)
+
+        Grad_x = interp2d(x, y, np.gradient(img,axis=1)/(np.max(np.gradient(img,axis=1))), kind='quintic')
+        Grad_y = interp2d(x, y, np.gradient(img,axis=0)/(np.max(np.gradient(img,axis=0))), kind='quintic')
+
+
+        Grad_x_blur = interp2d(x, y, np.gradient(blurred,axis=1)/(np.max(np.gradient(blurred,axis=1))), kind='quintic')
+        Grad_y_blur = interp2d(x, y, np.gradient(blurred,axis=0)/(np.max(np.gradient(blurred,axis=0))), kind='quintic')
+
+        xx_new = xx
+        yy_new = yy
+
+        idx_img=0
+        for step in range(n_iter):
+            kappa_arr = np.zeros(len(xx))
+            norm_arr  = np.zeros([len(xx),2])
+            for idx,val in enumerate(xx[1:-1]):
+                ytmp = yy_new[idx:idx+3]
+                xtmp = xx_new[idx:idx+3]
+                kappa,norm_l = PJcurvature(xtmp,ytmp)
+                kappa_arr[idx+1] = kappa
+                norm_arr[idx+1,:] = norm_l
+
+
+            f_x = beta* kappa_arr*norm_arr[:,0]
+            f_x[-1] = -f_x[-2]
+            f_x[0] = -f_x[1]
+            if step>n_iter/3.5 :
+                xx_new = xx_new+ d_step* (alpha * np.array([Grad_x(xx_new[i],yy_new[i])
+                            for i in np.arange(len(xx_new))])[:,0] + f_x)
+            else:
+                xx_new = xx_new+ d_step* (alpha * np.array([Grad_x_blur(xx_new[i],yy_new[i])
+                            for i in np.arange(len(xx_new))])[:,0] + f_x)
+
+            #print(alpha * np.array([Grad_x_blur(xx_new[i],yy_new[i])
+            #                for i in np.arange(len(xx_new))])[:,0])
+            #yy_new = yy_new+ d_step/1000* (alpha * np.array([Grad_y(xx_new[i],yy_new[i])
+            #                                            for i in np.arange(len(xx_new))])[:,0])
+
+        img_xy = interp2d(x, y, img, kind='quintic')
+        flux = np.array([img_xy(xx_new[i],yy_new[i])
+                            for i in np.arange(len(xx_new))])[:,0]
+
         return xx_new,yy_new,flux
```

### Comparing `type3detect-0.0.1/type3detect/detectRadioburst.py` & `type3detect-0.0.2/type3detect/detectRadioburst.py`

 * *Files identical despite different names*

### Comparing `type3detect-0.0.1/type3detect/radioTools.py` & `type3detect-0.0.2/type3detect/radioTools.py`

 * *Files identical despite different names*

