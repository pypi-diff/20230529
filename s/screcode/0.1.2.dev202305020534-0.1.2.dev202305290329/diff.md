# Comparing `tmp/screcode-0.1.2.dev202305020534-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202305290329-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 119319 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    61731 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202305020534.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202305020534.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202305020534.dist-info/RECORD
-6 files, 212562 bytes uncompressed, 118415 bytes compressed:  44.3%
+-rw-r--r--  2.0 unx    61723 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202305290329.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202305290329.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202305290329.dist-info/RECORD
+6 files, 212554 bytes uncompressed, 118415 bytes compressed:  44.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202305020534.dist-info/METADATA
+Filename: screcode-0.1.2.dev202305290329.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202305020534.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202305290329.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202305020534.dist-info/RECORD
+Filename: screcode-0.1.2.dev202305290329.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -521,15 +521,15 @@
 		ax1.set_xlabel('Density',fontsize=14)
 		ax1.spines['right'].set_visible(False)
 		ax1.spines['top'].set_visible(False)
 		ax1.tick_params(left=False)
 		ax1.patch.set_alpha(0)
 		#
 		x = np.linspace(ax1.set_ylim()[0],ax1.set_ylim()[1],1000)
-		dens = scipy.stats.kde.gaussian_kde(np.log10(norm_var[norm_var>0]))(x)
+		dens = scipy.stats.gaussian_kde(np.log10(norm_var[norm_var>0]))(x)
 		peak_val = x[np.argmax(dens)]
 		rate_low_var = np.sum(norm_var[norm_var>0] < 0.90)/len(norm_var[norm_var>0])
 		applicability = 'Unknown'
 		backcolor = 'w'
 		if (rate_low_var < 0.01) and (np.abs(peak_val)<0.1):
 			applicability = 'Class A (strongly applicable)'
 			backcolor = 'lightgreen'
@@ -734,15 +734,15 @@
 		ax1.tick_params(labelbottom=True,labelleft=False,bottom=True)
 		ax1.set_xlabel('Density',fontsize=14)
 		ax1.spines['right'].set_visible(False)
 		ax1.spines['top'].set_visible(False)
 		ax1.tick_params(left=False)
 		ax1.patch.set_alpha(0)
 		x = np.linspace(ax1.set_ylim()[0],ax1.set_ylim()[1],1000)
-		dens = scipy.stats.kde.gaussian_kde(np.log10(norm_var[norm_var>0]))(x)
+		dens = scipy.stats.gaussian_kde(np.log10(norm_var[norm_var>0]))(x)
 		peak_val = x[np.argmax(dens)]
 		rate_low_var = np.sum(norm_var[norm_var>0] < 0.90)/len(norm_var[norm_var>0])
 		applicability = 'Unknown'
 		backcolor = 'w'
 		if (rate_low_var < 0.01) and (np.abs(peak_val)<0.1):
 			applicability = 'Class A (strongly applicable)'
 			backcolor = 'lightgreen'
```

## Comparing `screcode-0.1.2.dev202305020534.dist-info/METADATA` & `screcode-0.1.2.dev202305290329.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202305020534
+Version: 0.1.2.dev202305290329
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

