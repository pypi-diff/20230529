# Comparing `tmp/fossiler-0.0.2.tar.gz` & `tmp/fossiler-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fossiler-0.0.2.tar", last modified: Mon May 29 05:43:21 2023, max compression
+gzip compressed data, was "dist/fossiler-0.0.3.tar", last modified: Mon May 29 19:44:35 2023, max compression
```

## Comparing `fossiler-0.0.2.tar` & `fossiler-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-29 05:43:21.283350 fossiler-0.0.2/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35149 2023-05-11 08:47:25.000000 fossiler-0.0.2/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    84885 2023-05-29 05:43:21.284369 fossiler-0.0.2/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    77524 2023-05-23 12:58:34.000000 fossiler-0.0.2/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)     2358 2023-05-29 05:33:19.000000 fossiler-0.0.2/command.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-29 05:43:21.277368 fossiler-0.0.2/fossiler/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    96197 2023-05-29 05:37:53.000000 fossiler-0.0.2/fossiler/fossils.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-29 05:43:21.283350 fossiler-0.0.2/fossiler.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    84885 2023-05-29 05:43:21.000000 fossiler-0.0.2/fossiler.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      261 2023-05-29 05:43:21.000000 fossiler-0.0.2/fossiler.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-29 05:43:21.000000 fossiler-0.0.2/fossiler.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       60 2023-05-29 05:43:21.000000 fossiler-0.0.2/fossiler.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       56 2023-05-29 05:43:21.000000 fossiler-0.0.2/fossiler.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       17 2023-05-29 05:43:21.000000 fossiler-0.0.2/fossiler.egg-info/top_level.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-29 05:43:21.285350 fossiler-0.0.2/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)      801 2023-05-29 05:42:57.000000 fossiler-0.0.2/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-29 19:44:35.946243 fossiler-0.0.3/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35149 2023-05-11 08:47:25.000000 fossiler-0.0.3/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    84885 2023-05-29 19:44:35.946243 fossiler-0.0.3/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    77524 2023-05-29 05:45:31.000000 fossiler-0.0.3/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     2688 2023-05-29 12:30:23.000000 fossiler-0.0.3/command.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-29 19:44:35.930618 fossiler-0.0.3/fossiler/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   142091 2023-05-29 16:45:01.000000 fossiler-0.0.3/fossiler/fossils.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-29 19:44:35.946243 fossiler-0.0.3/fossiler.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    84885 2023-05-29 19:44:35.000000 fossiler-0.0.3/fossiler.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      261 2023-05-29 19:44:35.000000 fossiler-0.0.3/fossiler.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-29 19:44:35.000000 fossiler-0.0.3/fossiler.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       60 2023-05-29 19:44:35.000000 fossiler-0.0.3/fossiler.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       56 2023-05-29 19:44:35.000000 fossiler-0.0.3/fossiler.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       17 2023-05-29 19:44:35.000000 fossiler-0.0.3/fossiler.egg-info/top_level.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-29 19:44:35.946243 fossiler-0.0.3/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      801 2023-05-29 19:03:04.000000 fossiler-0.0.3/setup.py
```

### Comparing `fossiler-0.0.2/LICENSE` & `fossiler-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fossiler-0.0.2/PKG-INFO` & `fossiler-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fossiler
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package and CLI for finding available fossils
 Home-page: http://github.com/heche-psb/fossiler
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description: <div align="center">
         
-        # `fossiler v0.0.1` : a suite tool of fossils finding
+        # `fossiler v0.0.2` : a suite tool of fossils finding
         **Hengchi Chen**
         
         [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/people/heche)**, VIB-UGent Center for Plant Systems Biology**
         
         [**Upper Limits**](#Upper-Limits) |
         [**Fossil Justifications**](#Fossil-Justifications) |
         [**References**](#References)
```

### Comparing `fossiler-0.0.2/README.md` & `fossiler-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
 
-# `fossiler v0.0.1` : a suite tool of fossils finding
+# `fossiler v0.0.2` : a suite tool of fossils finding
 **Hengchi Chen**
 
 [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/people/heche)**, VIB-UGent Center for Plant Systems Biology**
 
 [**Upper Limits**](#Upper-Limits) |
 [**Fossil Justifications**](#Fossil-Justifications) |
 [**References**](#References)
```

### Comparing `fossiler-0.0.2/command.py` & `fossiler-0.0.3/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,30 +30,33 @@
 
 # Find fossils
 @cli.command(context_settings={'help_option_names': ['-h', '--help']})
 @click.option('--outdir', '-o', default='fossiler_find', show_default=True, help='output directory')
 @click.option('--clades', '-c', default=None, show_default=True, help='clade names')
 @click.option('--rocks', '-r', default=None, type = int, show_default=True, help='rock IDs')
 @click.option('--tree', '-t', default=None, show_default=True, help='tree file in newick')
+@click.option('--sp2tree', '-s2p', default=None, show_default=True, help='species to date and get starting tree')
+@click.option('--number', '-n', default=19, show_default=True, help='number of species in the starting tree')
 @click.option('--getaxonomy', '-gt', default=None, show_default=True, help='get taxonomy of a given species name')
 @click.option('--mcmctreeformat', '-mf', is_flag=True, help='get mcmctree format output')
 @click.option('--wholetree', '-wt', is_flag=True, help='use the whole angiosperm tree infomation')
 @click.option('--setconserved', '-sc', is_flag=True, help='adopt the same maximum constraint as (Morris et al., 2018)')
 def find(**kwargs):
     """
     Find available fossils
     """
     _find(**kwargs)
 
-def _find(tree,outdir,clades,rocks,getaxonomy,mcmctreeformat,wholetree,setconserved):
-    from fossiler.fossils import rawfossils,cooccurancerecords,gettreewithfossil,standalonetaxonomy
+def _find(tree,outdir,clades,rocks,getaxonomy,mcmctreeformat,wholetree,setconserved,sp2tree,number):
+    from fossiler.fossils import rawfossils,cooccurancerecords,gettreewithfossil,standalonetaxonomy,getproperstartingtree
     if clades != None: rawfossils(clades)
     if rocks !=None: cooccurancerecords(rocks)
     if tree != None: gettreewithfossil(tree,formatt=mcmctreeformat,wholetree=wholetree,Yang=setconserved)
     if getaxonomy!= None: standalonetaxonomy(getaxonomy)
+    if sp2tree != None: getproperstartingtree(sp2tree,number,outdir)
 
 
 if __name__ == '__main__':
     start = timer()
     cli()
     end = timer()
     logging.info("Total run time: {}s".format(int(end-start)))
```

### Comparing `fossiler-0.0.2/fossiler.egg-info/PKG-INFO` & `fossiler-0.0.3/fossiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fossiler
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package and CLI for finding available fossils
 Home-page: http://github.com/heche-psb/fossiler
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description: <div align="center">
         
-        # `fossiler v0.0.1` : a suite tool of fossils finding
+        # `fossiler v0.0.2` : a suite tool of fossils finding
         **Hengchi Chen**
         
         [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/people/heche)**, VIB-UGent Center for Plant Systems Biology**
         
         [**Upper Limits**](#Upper-Limits) |
         [**Fossil Justifications**](#Fossil-Justifications) |
         [**References**](#References)
```

### Comparing `fossiler-0.0.2/setup.py` & `fossiler-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='fossiler',
-    version='0.0.2',
+    version='0.0.3',
     packages=['fossiler'],
     url='http://github.com/heche-psb/fossiler',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='Python package and CLI for finding available fossils',
     long_description=long_description,
```

