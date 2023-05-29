# Comparing `tmp/anticor_features-0.2.0.tar.gz` & `tmp/anticor_features-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anticor_features-0.2.0.tar", last modified: Sat Mar 11 14:49:50 2023, max compression
+gzip compressed data, was "dist/anticor_features-0.2.1.tar", last modified: Mon May 29 21:11:42 2023, max compression
```

## Comparing `anticor_features-0.2.0.tar` & `anticor_features-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 14:49:50.026372 anticor_features-0.2.0/
--rw-rw-r--   0 root         (0) root         (0)      624 2022-09-16 00:05:47.000000 anticor_features-0.2.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     6966 2023-03-11 14:49:50.026372 anticor_features-0.2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5559 2023-03-02 18:03:08.000000 anticor_features-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 14:49:50.026372 anticor_features-0.2.0/anticor_features/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-20 20:56:53.000000 anticor_features-0.2.0/anticor_features/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    25842 2022-12-06 12:48:14.000000 anticor_features-0.2.0/anticor_features/anticor_features.py
--rw-rw-r--   0 root         (0) root         (0)    36434 2023-03-11 14:39:59.000000 anticor_features-0.2.0/anticor_features/anticor_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 14:49:50.026372 anticor_features-0.2.0/anticor_features.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6966 2023-03-11 14:49:49.000000 anticor_features-0.2.0/anticor_features.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      345 2023-03-11 14:49:49.000000 anticor_features-0.2.0/anticor_features.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-11 14:49:49.000000 anticor_features-0.2.0/anticor_features.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-03-11 14:49:49.000000 anticor_features-0.2.0/anticor_features.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-11 14:49:49.000000 anticor_features-0.2.0/anticor_features.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       79 2023-03-11 14:45:11.000000 anticor_features-0.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-11 14:49:50.026372 anticor_features-0.2.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1077 2023-03-11 14:35:55.000000 anticor_features-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:11:42.791967 anticor_features-0.2.1/
+-rw-rw-r--   0 root         (0) root         (0)      624 2022-09-16 00:05:47.000000 anticor_features-0.2.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     6075 2023-05-29 21:11:42.791967 anticor_features-0.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5559 2023-03-02 18:03:08.000000 anticor_features-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:11:42.763967 anticor_features-0.2.1/anticor_features/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-20 20:56:53.000000 anticor_features-0.2.1/anticor_features/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    25842 2022-12-06 12:48:14.000000 anticor_features-0.2.1/anticor_features/anticor_features.py
+-rw-rw-r--   0 root         (0) root         (0)    36434 2023-03-11 14:39:59.000000 anticor_features-0.2.1/anticor_features/anticor_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:11:42.791967 anticor_features-0.2.1/anticor_features.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6075 2023-05-29 21:11:42.000000 anticor_features-0.2.1/anticor_features.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-29 21:11:42.000000 anticor_features-0.2.1/anticor_features.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 21:11:42.000000 anticor_features-0.2.1/anticor_features.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-29 21:11:42.000000 anticor_features-0.2.1/anticor_features.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-29 21:11:42.000000 anticor_features-0.2.1/anticor_features.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       86 2023-05-29 21:09:39.000000 anticor_features-0.2.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 21:11:42.791967 anticor_features-0.2.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1077 2023-05-29 21:09:48.000000 anticor_features-0.2.1/setup.py
```

### Comparing `anticor_features-0.2.0/.gitignore` & `anticor_features-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `anticor_features-0.2.0/PKG-INFO` & `anticor_features-0.2.1/anticor_features.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 Metadata-Version: 2.1
-Name: anticor_features
-Version: 0.2.0
+Name: anticor-features
+Version: 0.2.1
 Summary: Anti-correlation based feature selection for single cell datasets
 Home-page: https://scottyler892@bitbucket.org/scottyler892/anticor_features
 Author: Scott Tyler
 Author-email: scottyler89@gmail.com
 License: UNKNOWN
-Description: # README #
-        
-        ### What is this repository for? ###
-        
-        Anti-correlated genes as a method of feature selection
-        * Unsupervised feature selection for single cell omics (or anything else!) that passes the null-dataset test
-        
-        ### How do I get set up? ###
-        
-        `python3 -m pip install anticor_features`
-        
-        You can also install using the setup.py script in the distribution like so:
-        `python3 setup.py install`
-        
-        This should take less than one minute or even seconds if dependecies were already installed.
-        
-        ### How do I run use this package? ###
-        
-        ```
-        from anticor_features.anticor_features import get_anti_cor_genes
-        
-        ## Then feed in the expression matrix, with cells in columns, genes in rows
-        ## and the feature names (all_features)
-        ## and the species code (in gProfiler format, linked below)
-        
-        anti_cor_table = get_anti_cor_genes(in_mat,
-                                            all_features,
-                                            species="hsapiens")
-        
-        ```
-        A list of the gProfiler accepted species codes is listed here: https://biit.cs.ut.ee/gprofiler/page/organism-list
-        
-        The above call yields a pandas data frame that will give you the collected summary statistics, and let you filter based on the features annotated as "selected" in that column
-        ```
-        >>> print(anti_cor_table.head())
-             gene  pre_remove_feature  pre_remove_pathway  ...       FDR  num_sig_pos_cor  selected
-        0    Xkr4               False               False  ...       NaN              NaN       NaN
-        1     Rp1               False               False  ...       NaN              NaN       NaN
-        2   Sox17               False               False  ...  0.001883           3406.0      True
-        3  Mrpl15               False                True  ...       NaN              NaN       NaN
-        4  Lypla1               False                True  ...       NaN              NaN       NaN
-        ```
-        The NaNs are produced where the gene was not assayed for anti-correlations either from pre-filtering
-        (the default is to remove genes in pathways related to mitochondria, ribosomes, and hemoglobin).
-        
-        If you want to customize which GO terms are removed, or specify specific genes to exclude, you can do that with the pre_remove_features and pre_remove_pathways arguments
-        ```
-        anti_cor_table = get_anti_cor_genes(in_mat,
-                                            all_features,
-                                            species="hsapiens",
-                                            pre_remove_features = ["ACTB","MT-COX1"])
-        
-        ```
-        
-        ## Scanpy (or anything from python where you have a matrix) ##
-        * If you're using scanpy, then you can use the same basic syntax as above. The only thing worth noting is that our downsampling function assumes that the genes are in rows, and cells are in columns, which is flipped from AnnData's formatting, that's why we use the have the transpose() functions below:
-        
-        If you follow along [Scanpy's tutorial](https://scanpy-tutorials.readthedocs.io/en/latest/pbmc3k.html), then the only thing different would be swapping out:
-        
-        ```
-        [16]: sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
-        [17]: sc.pl.highly_variable_genes(adata)
-        [18]: adata.raw = adata
-        [19]: adata = adata[:, adata.var.highly_variable]
-        ```
-        for
-        ```
-        from anticor_features.anticor_features import get_anti_cor_genes
-        
-        anti_cor_table = get_anti_cor_genes(adata.X.T,
-                                            adata.var.index.tolist(),
-                                            species="hsapiens")
-        
-        selected_table = anti_cor_table[anti_cor_table["selected"]==True]
-        print(selected_table)
-        
-        ## And you can save the anti-correlation dataframe into the adata object as well:
-        import pandas as pd
-        adata.var = pd.concat([adata.var,anti_cor_table], axis=1)
-        
-        ## And then we subset the data to only include the selected features!
-        adata.raw = adata
-        adata = adata[:, selected_table.index]
-        
-        ## Note that the downstream clusters and marker genes will be slightly different!
-        ```
-        It should take ~ 1-2 minute(s) for the feature selection depending on your internet connection, the speed of the gprofiler server (if looking up pathways like ribosomes, mitochondria, etc to remove), but will also scale a bit with the complexity of the dataset. For example, the tabula muris dataset used in the manuscript took ~ 60 minutes, in part because nearly every gene was expressed at appreciable values in a subset of the cells.
-        
-        * *An important note if you're working in a cluster environment*
-        ** Anti-correlated genes are selected out of memory - to do this, the pipeline needs a hard-disk area to work in. On a stand-alone computer it'll automatically find the system temp drive, but this might not be the behavior you want on a cluster, or if you're analyzing several datasets simultaneously because they would overwrite each other.
-        ** In those cases, you should supply the additional argument `scratch_dir=</local/path/to/dataset/directory>`. This ensures that each dataset will be analyzed properly and there won't be conflicts in terms of where files get written.
-        
-        ### Command line interface ###
-        You can also use this tool at the command line, if you have either a .tsv or an hdf5 file, with the matrix under the key "infile"
-        
-        ```
-        python3 -m anticor_features.anticor_features -i exprs.tsv -species mmusculus
-        ```
-        or something similar. This outputs the pandas table to a tsv in the same folder as the input file
-        
-        See the help section for more detailed usage of the command line interface:
-        ```
-        python3 -m anticor_features.anticor_features -h
-        ```
-        
-        ### License ###
-        This package is available via the AGPLv3 license.
-        
-        ### Who do I talk to? ###
-        
-        * Repo owner/admin: scottyler89+bitbucket@gmail.com
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+
+# README #
+
+### What is this repository for? ###
+
+Anti-correlated genes as a method of feature selection
+* Unsupervised feature selection for single cell omics (or anything else!) that passes the null-dataset test
+
+### How do I get set up? ###
+
+`python3 -m pip install anticor_features`
+
+You can also install using the setup.py script in the distribution like so:
+`python3 setup.py install`
+
+This should take less than one minute or even seconds if dependecies were already installed.
+
+### How do I run use this package? ###
+
+```
+from anticor_features.anticor_features import get_anti_cor_genes
+
+## Then feed in the expression matrix, with cells in columns, genes in rows
+## and the feature names (all_features)
+## and the species code (in gProfiler format, linked below)
+
+anti_cor_table = get_anti_cor_genes(in_mat,
+                                    all_features,
+                                    species="hsapiens")
+
+```
+A list of the gProfiler accepted species codes is listed here: https://biit.cs.ut.ee/gprofiler/page/organism-list
+
+The above call yields a pandas data frame that will give you the collected summary statistics, and let you filter based on the features annotated as "selected" in that column
+```
+>>> print(anti_cor_table.head())
+     gene  pre_remove_feature  pre_remove_pathway  ...       FDR  num_sig_pos_cor  selected
+0    Xkr4               False               False  ...       NaN              NaN       NaN
+1     Rp1               False               False  ...       NaN              NaN       NaN
+2   Sox17               False               False  ...  0.001883           3406.0      True
+3  Mrpl15               False                True  ...       NaN              NaN       NaN
+4  Lypla1               False                True  ...       NaN              NaN       NaN
+```
+The NaNs are produced where the gene was not assayed for anti-correlations either from pre-filtering
+(the default is to remove genes in pathways related to mitochondria, ribosomes, and hemoglobin).
+
+If you want to customize which GO terms are removed, or specify specific genes to exclude, you can do that with the pre_remove_features and pre_remove_pathways arguments
+```
+anti_cor_table = get_anti_cor_genes(in_mat,
+                                    all_features,
+                                    species="hsapiens",
+                                    pre_remove_features = ["ACTB","MT-COX1"])
+
+```
+
+## Scanpy (or anything from python where you have a matrix) ##
+* If you're using scanpy, then you can use the same basic syntax as above. The only thing worth noting is that our downsampling function assumes that the genes are in rows, and cells are in columns, which is flipped from AnnData's formatting, that's why we use the have the transpose() functions below:
+
+If you follow along [Scanpy's tutorial](https://scanpy-tutorials.readthedocs.io/en/latest/pbmc3k.html), then the only thing different would be swapping out:
+
+```
+[16]: sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
+[17]: sc.pl.highly_variable_genes(adata)
+[18]: adata.raw = adata
+[19]: adata = adata[:, adata.var.highly_variable]
+```
+for
+```
+from anticor_features.anticor_features import get_anti_cor_genes
+
+anti_cor_table = get_anti_cor_genes(adata.X.T,
+                                    adata.var.index.tolist(),
+                                    species="hsapiens")
+
+selected_table = anti_cor_table[anti_cor_table["selected"]==True]
+print(selected_table)
+
+## And you can save the anti-correlation dataframe into the adata object as well:
+import pandas as pd
+adata.var = pd.concat([adata.var,anti_cor_table], axis=1)
+
+## And then we subset the data to only include the selected features!
+adata.raw = adata
+adata = adata[:, selected_table.index]
+
+## Note that the downstream clusters and marker genes will be slightly different!
+```
+It should take ~ 1-2 minute(s) for the feature selection depending on your internet connection, the speed of the gprofiler server (if looking up pathways like ribosomes, mitochondria, etc to remove), but will also scale a bit with the complexity of the dataset. For example, the tabula muris dataset used in the manuscript took ~ 60 minutes, in part because nearly every gene was expressed at appreciable values in a subset of the cells.
+
+* *An important note if you're working in a cluster environment*
+** Anti-correlated genes are selected out of memory - to do this, the pipeline needs a hard-disk area to work in. On a stand-alone computer it'll automatically find the system temp drive, but this might not be the behavior you want on a cluster, or if you're analyzing several datasets simultaneously because they would overwrite each other.
+** In those cases, you should supply the additional argument `scratch_dir=</local/path/to/dataset/directory>`. This ensures that each dataset will be analyzed properly and there won't be conflicts in terms of where files get written.
+
+### Command line interface ###
+You can also use this tool at the command line, if you have either a .tsv or an hdf5 file, with the matrix under the key "infile"
+
+```
+python3 -m anticor_features.anticor_features -i exprs.tsv -species mmusculus
+```
+or something similar. This outputs the pandas table to a tsv in the same folder as the input file
+
+See the help section for more detailed usage of the command line interface:
+```
+python3 -m anticor_features.anticor_features -h
+```
+
+### License ###
+This package is available via the AGPLv3 license.
+
+### Who do I talk to? ###
+
+* Repo owner/admin: scottyler89+bitbucket@gmail.com
+
```

### Comparing `anticor_features-0.2.0/README.md` & `anticor_features-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `anticor_features-0.2.0/anticor_features/anticor_features.py` & `anticor_features-0.2.1/anticor_features/anticor_features.py`

 * *Files identical despite different names*

### Comparing `anticor_features-0.2.0/anticor_features/anticor_stats.py` & `anticor_features-0.2.1/anticor_features/anticor_stats.py`

 * *Files identical despite different names*

### Comparing `anticor_features-0.2.0/anticor_features.egg-info/PKG-INFO` & `anticor_features-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 Metadata-Version: 2.1
-Name: anticor-features
-Version: 0.2.0
+Name: anticor_features
+Version: 0.2.1
 Summary: Anti-correlation based feature selection for single cell datasets
 Home-page: https://scottyler892@bitbucket.org/scottyler892/anticor_features
 Author: Scott Tyler
 Author-email: scottyler89@gmail.com
 License: UNKNOWN
-Description: # README #
-        
-        ### What is this repository for? ###
-        
-        Anti-correlated genes as a method of feature selection
-        * Unsupervised feature selection for single cell omics (or anything else!) that passes the null-dataset test
-        
-        ### How do I get set up? ###
-        
-        `python3 -m pip install anticor_features`
-        
-        You can also install using the setup.py script in the distribution like so:
-        `python3 setup.py install`
-        
-        This should take less than one minute or even seconds if dependecies were already installed.
-        
-        ### How do I run use this package? ###
-        
-        ```
-        from anticor_features.anticor_features import get_anti_cor_genes
-        
-        ## Then feed in the expression matrix, with cells in columns, genes in rows
-        ## and the feature names (all_features)
-        ## and the species code (in gProfiler format, linked below)
-        
-        anti_cor_table = get_anti_cor_genes(in_mat,
-                                            all_features,
-                                            species="hsapiens")
-        
-        ```
-        A list of the gProfiler accepted species codes is listed here: https://biit.cs.ut.ee/gprofiler/page/organism-list
-        
-        The above call yields a pandas data frame that will give you the collected summary statistics, and let you filter based on the features annotated as "selected" in that column
-        ```
-        >>> print(anti_cor_table.head())
-             gene  pre_remove_feature  pre_remove_pathway  ...       FDR  num_sig_pos_cor  selected
-        0    Xkr4               False               False  ...       NaN              NaN       NaN
-        1     Rp1               False               False  ...       NaN              NaN       NaN
-        2   Sox17               False               False  ...  0.001883           3406.0      True
-        3  Mrpl15               False                True  ...       NaN              NaN       NaN
-        4  Lypla1               False                True  ...       NaN              NaN       NaN
-        ```
-        The NaNs are produced where the gene was not assayed for anti-correlations either from pre-filtering
-        (the default is to remove genes in pathways related to mitochondria, ribosomes, and hemoglobin).
-        
-        If you want to customize which GO terms are removed, or specify specific genes to exclude, you can do that with the pre_remove_features and pre_remove_pathways arguments
-        ```
-        anti_cor_table = get_anti_cor_genes(in_mat,
-                                            all_features,
-                                            species="hsapiens",
-                                            pre_remove_features = ["ACTB","MT-COX1"])
-        
-        ```
-        
-        ## Scanpy (or anything from python where you have a matrix) ##
-        * If you're using scanpy, then you can use the same basic syntax as above. The only thing worth noting is that our downsampling function assumes that the genes are in rows, and cells are in columns, which is flipped from AnnData's formatting, that's why we use the have the transpose() functions below:
-        
-        If you follow along [Scanpy's tutorial](https://scanpy-tutorials.readthedocs.io/en/latest/pbmc3k.html), then the only thing different would be swapping out:
-        
-        ```
-        [16]: sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
-        [17]: sc.pl.highly_variable_genes(adata)
-        [18]: adata.raw = adata
-        [19]: adata = adata[:, adata.var.highly_variable]
-        ```
-        for
-        ```
-        from anticor_features.anticor_features import get_anti_cor_genes
-        
-        anti_cor_table = get_anti_cor_genes(adata.X.T,
-                                            adata.var.index.tolist(),
-                                            species="hsapiens")
-        
-        selected_table = anti_cor_table[anti_cor_table["selected"]==True]
-        print(selected_table)
-        
-        ## And you can save the anti-correlation dataframe into the adata object as well:
-        import pandas as pd
-        adata.var = pd.concat([adata.var,anti_cor_table], axis=1)
-        
-        ## And then we subset the data to only include the selected features!
-        adata.raw = adata
-        adata = adata[:, selected_table.index]
-        
-        ## Note that the downstream clusters and marker genes will be slightly different!
-        ```
-        It should take ~ 1-2 minute(s) for the feature selection depending on your internet connection, the speed of the gprofiler server (if looking up pathways like ribosomes, mitochondria, etc to remove), but will also scale a bit with the complexity of the dataset. For example, the tabula muris dataset used in the manuscript took ~ 60 minutes, in part because nearly every gene was expressed at appreciable values in a subset of the cells.
-        
-        * *An important note if you're working in a cluster environment*
-        ** Anti-correlated genes are selected out of memory - to do this, the pipeline needs a hard-disk area to work in. On a stand-alone computer it'll automatically find the system temp drive, but this might not be the behavior you want on a cluster, or if you're analyzing several datasets simultaneously because they would overwrite each other.
-        ** In those cases, you should supply the additional argument `scratch_dir=</local/path/to/dataset/directory>`. This ensures that each dataset will be analyzed properly and there won't be conflicts in terms of where files get written.
-        
-        ### Command line interface ###
-        You can also use this tool at the command line, if you have either a .tsv or an hdf5 file, with the matrix under the key "infile"
-        
-        ```
-        python3 -m anticor_features.anticor_features -i exprs.tsv -species mmusculus
-        ```
-        or something similar. This outputs the pandas table to a tsv in the same folder as the input file
-        
-        See the help section for more detailed usage of the command line interface:
-        ```
-        python3 -m anticor_features.anticor_features -h
-        ```
-        
-        ### License ###
-        This package is available via the AGPLv3 license.
-        
-        ### Who do I talk to? ###
-        
-        * Repo owner/admin: scottyler89+bitbucket@gmail.com
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+
+# README #
+
+### What is this repository for? ###
+
+Anti-correlated genes as a method of feature selection
+* Unsupervised feature selection for single cell omics (or anything else!) that passes the null-dataset test
+
+### How do I get set up? ###
+
+`python3 -m pip install anticor_features`
+
+You can also install using the setup.py script in the distribution like so:
+`python3 setup.py install`
+
+This should take less than one minute or even seconds if dependecies were already installed.
+
+### How do I run use this package? ###
+
+```
+from anticor_features.anticor_features import get_anti_cor_genes
+
+## Then feed in the expression matrix, with cells in columns, genes in rows
+## and the feature names (all_features)
+## and the species code (in gProfiler format, linked below)
+
+anti_cor_table = get_anti_cor_genes(in_mat,
+                                    all_features,
+                                    species="hsapiens")
+
+```
+A list of the gProfiler accepted species codes is listed here: https://biit.cs.ut.ee/gprofiler/page/organism-list
+
+The above call yields a pandas data frame that will give you the collected summary statistics, and let you filter based on the features annotated as "selected" in that column
+```
+>>> print(anti_cor_table.head())
+     gene  pre_remove_feature  pre_remove_pathway  ...       FDR  num_sig_pos_cor  selected
+0    Xkr4               False               False  ...       NaN              NaN       NaN
+1     Rp1               False               False  ...       NaN              NaN       NaN
+2   Sox17               False               False  ...  0.001883           3406.0      True
+3  Mrpl15               False                True  ...       NaN              NaN       NaN
+4  Lypla1               False                True  ...       NaN              NaN       NaN
+```
+The NaNs are produced where the gene was not assayed for anti-correlations either from pre-filtering
+(the default is to remove genes in pathways related to mitochondria, ribosomes, and hemoglobin).
+
+If you want to customize which GO terms are removed, or specify specific genes to exclude, you can do that with the pre_remove_features and pre_remove_pathways arguments
+```
+anti_cor_table = get_anti_cor_genes(in_mat,
+                                    all_features,
+                                    species="hsapiens",
+                                    pre_remove_features = ["ACTB","MT-COX1"])
+
+```
+
+## Scanpy (or anything from python where you have a matrix) ##
+* If you're using scanpy, then you can use the same basic syntax as above. The only thing worth noting is that our downsampling function assumes that the genes are in rows, and cells are in columns, which is flipped from AnnData's formatting, that's why we use the have the transpose() functions below:
+
+If you follow along [Scanpy's tutorial](https://scanpy-tutorials.readthedocs.io/en/latest/pbmc3k.html), then the only thing different would be swapping out:
+
+```
+[16]: sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
+[17]: sc.pl.highly_variable_genes(adata)
+[18]: adata.raw = adata
+[19]: adata = adata[:, adata.var.highly_variable]
+```
+for
+```
+from anticor_features.anticor_features import get_anti_cor_genes
+
+anti_cor_table = get_anti_cor_genes(adata.X.T,
+                                    adata.var.index.tolist(),
+                                    species="hsapiens")
+
+selected_table = anti_cor_table[anti_cor_table["selected"]==True]
+print(selected_table)
+
+## And you can save the anti-correlation dataframe into the adata object as well:
+import pandas as pd
+adata.var = pd.concat([adata.var,anti_cor_table], axis=1)
+
+## And then we subset the data to only include the selected features!
+adata.raw = adata
+adata = adata[:, selected_table.index]
+
+## Note that the downstream clusters and marker genes will be slightly different!
+```
+It should take ~ 1-2 minute(s) for the feature selection depending on your internet connection, the speed of the gprofiler server (if looking up pathways like ribosomes, mitochondria, etc to remove), but will also scale a bit with the complexity of the dataset. For example, the tabula muris dataset used in the manuscript took ~ 60 minutes, in part because nearly every gene was expressed at appreciable values in a subset of the cells.
+
+* *An important note if you're working in a cluster environment*
+** Anti-correlated genes are selected out of memory - to do this, the pipeline needs a hard-disk area to work in. On a stand-alone computer it'll automatically find the system temp drive, but this might not be the behavior you want on a cluster, or if you're analyzing several datasets simultaneously because they would overwrite each other.
+** In those cases, you should supply the additional argument `scratch_dir=</local/path/to/dataset/directory>`. This ensures that each dataset will be analyzed properly and there won't be conflicts in terms of where files get written.
+
+### Command line interface ###
+You can also use this tool at the command line, if you have either a .tsv or an hdf5 file, with the matrix under the key "infile"
+
+```
+python3 -m anticor_features.anticor_features -i exprs.tsv -species mmusculus
+```
+or something similar. This outputs the pandas table to a tsv in the same folder as the input file
+
+See the help section for more detailed usage of the command line interface:
+```
+python3 -m anticor_features.anticor_features -h
+```
+
+### License ###
+This package is available via the AGPLv3 license.
+
+### Who do I talk to? ###
+
+* Repo owner/admin: scottyler89+bitbucket@gmail.com
+
```

### Comparing `anticor_features-0.2.0/setup.py` & `anticor_features-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     install_requires = fh.read()
 
 #script_list = ["anticor_features/anticor_features.py", "anticor_features/anticor_stats.py"]
 script_list=[]
 
 setuptools.setup(
      name='anticor_features',  
-     version='0.2.0',
+     version='0.2.1',
      author="Scott Tyler",
      author_email="scottyler89@gmail.com",
      description="Anti-correlation based feature selection for single cell datasets",
      long_description_content_type="text/markdown",
      long_description=long_description,
      install_requires = install_requires,
      url="https://scottyler892@bitbucket.org/scottyler892/anticor_features",
```

