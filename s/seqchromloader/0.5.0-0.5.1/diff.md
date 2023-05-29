# Comparing `tmp/seqchromloader-0.5.0.tar.gz` & `tmp/seqchromloader-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.5.0.tar", last modified: Mon May 29 19:06:59 2023, max compression
+gzip compressed data, was "seqchromloader-0.5.1.tar", last modified: Mon May 29 21:13:35 2023, max compression
```

## Comparing `seqchromloader-0.5.0.tar` & `seqchromloader-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 19:06:59.043941 seqchromloader-0.5.0/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-05-29 19:06:59.043643 seqchromloader-0.5.0/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.5.0/README.md
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 19:06:59.038916 seqchromloader-0.5.0/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      280 2023-05-29 18:55:42.000000 seqchromloader-0.5.0/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12427 2023-04-12 19:57:21.000000 seqchromloader-0.5.0/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     9899 2023-05-29 18:44:55.000000 seqchromloader-0.5.0/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     6248 2023-04-12 20:33:18.000000 seqchromloader-0.5.0/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 19:06:59.043132 seqchromloader-0.5.0/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-05-29 19:06:58.000000 seqchromloader-0.5.0/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      308 2023-05-29 19:06:59.000000 seqchromloader-0.5.0/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-05-29 19:06:58.000000 seqchromloader-0.5.0/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-05-29 19:06:58.000000 seqchromloader-0.5.0/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-05-29 19:06:58.000000 seqchromloader-0.5.0/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-05-29 19:06:59.044023 seqchromloader-0.5.0/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-05-29 18:56:49.000000 seqchromloader-0.5.0/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 21:13:35.871455 seqchromloader-0.5.1/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-05-29 21:13:35.871112 seqchromloader-0.5.1/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.5.1/README.md
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 21:13:35.866532 seqchromloader-0.5.1/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      280 2023-05-29 18:55:42.000000 seqchromloader-0.5.1/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12427 2023-04-12 19:57:21.000000 seqchromloader-0.5.1/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     9899 2023-05-29 19:56:30.000000 seqchromloader-0.5.1/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     6666 2023-05-29 21:12:24.000000 seqchromloader-0.5.1/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 21:13:35.870646 seqchromloader-0.5.1/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      308 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-05-29 21:13:35.871541 seqchromloader-0.5.1/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-05-29 21:13:04.000000 seqchromloader-0.5.1/setup.py
```

### Comparing `seqchromloader-0.5.0/PKG-INFO` & `seqchromloader-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.5.0
+Version: 0.5.1
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.5.0/README.md` & `seqchromloader-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.5.0/seqchromloader/loader.py` & `seqchromloader-0.5.1/seqchromloader/loader.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.5.0/seqchromloader/utils.py` & `seqchromloader-0.5.1/seqchromloader/utils.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.5.0/seqchromloader/writer.py` & `seqchromloader-0.5.1/seqchromloader/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     
 def dump_data_webdataset(coords, genome_fasta, bigwig_filelist,
                         target_bam=None, 
                         outdir="dataset/", outprefix="seqchrom", 
                         compress=True, 
                         numProcessors=1,
                         transforms=None,
+                        braceexpand=True,
                         DALI=False):
     """
     Given coordinates dataframe, extract the sequence and chromatin signal, save in webdataset format
 
     :param coords: pandas DataFrame containing genomic coordinates with columns **[chrom, start, end, label]**
     :type coords: pandas DataFrame
     :param genome_fasta: Genome fasta file.
@@ -71,14 +72,16 @@
     :type outdir: str
     :param outprefix: prefix of output files
     :type outprefix: str
     :param compress: whether to compress the output files
     :type compress: boolean
     :param numProcessors: number of processors
     :type numProcessors: int
+    :param braceexpand: if use brace to simplify the wds file list into a string
+    :param braceexpand: boolean
     :param DALI: Set to True if you want to use the dataset for NVIDIA DALI, it would save all arrays in bytes, which results in losing the array shape info
     :param DALI: boolean
     """
 
     # split coordinates and assign chunks to workers
     num_chunks = math.ceil(len(coords) / 7000)
     chunks = np.array_split(coords, num_chunks)
@@ -99,16 +102,21 @@
     while num_chunks > 0:
        num_chunks = int(num_chunks/10)
        count_of_digits += 1
 
     pool = Pool(numProcessors)
     res = pool.starmap_async(dump_data_worker_freeze, zip(chunks, [outprefix + "_" + format(i, f'0{count_of_digits}d') for i in range(num_chunks)]))
     files = res.get()
-
-    return files
+    
+    if braceexpand:
+        begin = f'0{count_of_digits}d'.format(0)
+        end = f'0{count_of_digits}d'.format(range(num_chunks)[-1])
+        return f"outprefix_{{{begin}...{end}}}.tar.gz" if compress else f"outprefix_{{{begin}...{end}}}.tar"
+    else:
+        return files
 
 def dump_data_webdataset_worker(coords, 
                                 outprefix, 
                                 fasta, 
                                 bigwig_files,
                                 target_bam=None, 
                                 outdir="dataset/",
```

### Comparing `seqchromloader-0.5.0/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.5.1/seqchromloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.5.0
+Version: 0.5.1
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.5.0/setup.py` & `seqchromloader-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.5.0",
+    version="0.5.1",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
```

