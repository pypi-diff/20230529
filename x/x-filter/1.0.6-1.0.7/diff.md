# Comparing `tmp/x-filter-1.0.6.tar.gz` & `tmp/x-filter-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/x-filter-1.0.6.tar", last modified: Wed Mar  8 13:13:43 2023, max compression
+gzip compressed data, was "dist/x-filter-1.0.7.tar", last modified: Mon May 29 06:35:24 2023, max compression
```

## Comparing `x-filter-1.0.6.tar` & `x-filter-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 13:13:43.000000 x-filter-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (116)       51 2023-03-08 13:13:40.000000 x-filter-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      473 2023-03-08 13:13:43.000000 x-filter-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    10542 2023-03-08 13:13:40.000000 x-filter-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       59 2023-03-08 13:13:40.000000 x-filter-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      679 2023-03-08 13:13:43.000000 x-filter-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2023-03-08 13:13:40.000000 x-filter-1.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)    70238 2023-03-08 13:13:40.000000 x-filter-1.0.6/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 13:13:43.000000 x-filter-1.0.6/x_filter/
--rw-r--r--   0 runner    (1001) docker     (116)       93 2023-03-08 13:13:40.000000 x-filter-1.0.6/x_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8371 2023-03-08 13:13:40.000000 x-filter-1.0.6/x_filter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2023-03-08 13:13:43.000000 x-filter-1.0.6/x_filter/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)    22632 2023-03-08 13:13:40.000000 x-filter-1.0.6/x_filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (116)    11566 2023-03-08 13:13:40.000000 x-filter-1.0.6/x_filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 13:13:43.000000 x-filter-1.0.6/x_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      473 2023-03-08 13:13:43.000000 x-filter-1.0.6/x_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      363 2023-03-08 13:13:43.000000 x-filter-1.0.6/x_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-08 13:13:43.000000 x-filter-1.0.6/x_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       52 2023-03-08 13:13:43.000000 x-filter-1.0.6/x_filter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      110 2023-03-08 13:13:43.000000 x-filter-1.0.6/x_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2023-03-08 13:13:43.000000 x-filter-1.0.6/x_filter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 06:35:24.000000 x-filter-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-29 06:35:17.000000 x-filter-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-05-29 06:35:24.000000 x-filter-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10740 2023-05-29 06:35:17.000000 x-filter-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-29 06:35:17.000000 x-filter-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-05-29 06:35:24.000000 x-filter-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-29 06:35:17.000000 x-filter-1.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70238 2023-05-29 06:35:17.000000 x-filter-1.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 06:35:24.000000 x-filter-1.0.7/x_filter/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-29 06:35:17.000000 x-filter-1.0.7/x_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-05-29 06:35:17.000000 x-filter-1.0.7/x_filter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-29 06:35:24.000000 x-filter-1.0.7/x_filter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24288 2023-05-29 06:35:17.000000 x-filter-1.0.7/x_filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11566 2023-05-29 06:35:17.000000 x-filter-1.0.7/x_filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 06:35:24.000000 x-filter-1.0.7/x_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-05-29 06:35:24.000000 x-filter-1.0.7/x_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-29 06:35:24.000000 x-filter-1.0.7/x_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 06:35:24.000000 x-filter-1.0.7/x_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-29 06:35:24.000000 x-filter-1.0.7/x_filter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-29 06:35:24.000000 x-filter-1.0.7/x_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-29 06:35:24.000000 x-filter-1.0.7/x_filter.egg-info/top_level.txt
```

### Comparing `x-filter-1.0.6/README.md` & `x-filter-1.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -137,21 +137,23 @@
    - **depth_evenness**: Coverage evenness (SD/MEAN)
    - **breadth**: Breadth of coverage
    - **breadth_expected**: Expected breadth of coverage
    - **breadth_expected_ratio**: Observed breadth to expected breadth ratio (scaled)
    - **n_alns**: Number of alignments
   - {prefix}**_group-abundances-agg.tsv.gz**: If a mapping file is provided, it reports:
     - **group**: Group name
-    - **mean**: Mean coverage values
-    - **std**: Standard deviation of coverage values
-    - **median**: Median coverage values
-    - **sum**: Sum of coverage values
+    - **coverage_mean**: Mean coverage values
+    - **coverage_stdev**: Standard deviation of coverage values
+    - **coverage_median**: Median coverage values
+    - **coverage_sum**: Sum of coverage values
     - **n_genes**: Number of genes in the group
     - **avg_read_length**: Average read length of the reads mapping to a gene
     - **stdev_read_length**: Standard deviation of read length of the reads mapping to a gene
+    - **avg_identity**: Average identity of the reads mapping to a gene
+    - **stdev_identity**: Standard deviation of identity of the reads mapping to a gene
   - {prefix}**_group-abundances.tsv.gz**: If a mapping file is provided, it reports:
     - **reference**: Reference name
     - **group**: Group name
     - **depth_mean**: Coverage mean
     - **depth_std**: Coverage standard deviation
     - **depth_evenness**: Coverage evenness (SD/MEAN)
     - **breadth**: Breadth of coverage
```

### Comparing `x-filter-1.0.6/setup.cfg` & `x-filter-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `x-filter-1.0.6/setup.py` & `x-filter-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `x-filter-1.0.6/versioneer.py` & `x-filter-1.0.7/versioneer.py`

 * *Files identical despite different names*

### Comparing `x-filter-1.0.6/x_filter/__main__.py` & `x-filter-1.0.7/x_filter/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 import numpy as np
 import gc
 
 log = logging.getLogger("my_logger")
 
 
 def main():
-
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(levelname)s ::: %(asctime)s ::: %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     args = get_arguments()
@@ -186,14 +185,15 @@
             "subjectId",
             "queryId",
             "subjectStart",
             "subjectEnd",
             "slen",
             "qlen",
             "alnLength",
+            "percIdentity",
         ],
     ]
 
     results = get_coverage_stats(df, trim=args.trim)
 
     # Filter results
     logging.info(f"Filtering references")
```

### Comparing `x-filter-1.0.6/x_filter/filter.py` & `x-filter-1.0.7/x_filter/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 import os
 
 import zlib
 import struct
 
 log = logging.getLogger("my_logger")
 
-sys.setrecursionlimit(10 ** 6)
+sys.setrecursionlimit(10**6)
 
 # estimate file size of a gzip compressed file
 
+
 # From https://stackoverflow.com/a/68939759
 def estimate_uncompressed_gz_size(filename):
     # From the input file, get some data:
     # - the 32 LSB from the gzip stream
     # - 1MB sample of compressed data
     # - compressed file size
     with open(filename, "rb") as gz_in:
@@ -161,15 +162,15 @@
         fsize = os.path.getsize(aln)
 
     nalns = fsize // line_estimation(
         filename=aln, first_size=int(os.path.getsize(aln) * 0.01)
     )
     logging.info(f"Approximately {nalns:,} alignments found.")
 
-    max_rows = int((2 ** 31) - 1)
+    max_rows = int((2**31) - 1)
     # max_rows = int(5e6)
     # if the number of alignmentsis larger than the number of rows
     # that can be read by fread, we need to read it by chunks instead
 
     if nalns > max_rows:
         gc.collect()
         logging.info(
@@ -339,15 +340,14 @@
 
 def resolve_multimaps(
     df,
     scale=0.9,
     iters=10,
     threads=1,
 ):
-
     """Resolve multimaps by iteratively removing the lowest scoring reads.
 
     Args:
         df ([Frame]): A Frame containing the alignments
         scale (float, optional): Scale where to filter. Defaults to 0.9.
         iters (int, optional): Number of iterations. Defaults to 10.
         threa
@@ -452,15 +452,14 @@
     else:
         df1 = df
         return df1
     return df1
 
 
 def cov_stats(alns, refs):
-
     rle = alns.to_rle(nb_cpu=1)
     g3 = rle[refs]
     df = g3.df
     df.insert(df.shape[1], "Sum", df.Value * df.Run)
     g = df.groupby(["Start", "End"])
     mean = g.Sum.sum() / g.Run.sum()
     length = g.Sum.count()
@@ -477,15 +476,15 @@
     df.insert(df.shape[1], "depth_sd", sqrt.values)
 
     df.insert(df.shape[1], "depth_evenness", df["depth_sd"] / df["depth_mean"])
 
     return df.drop("Run Value Sum Intermediate".split(), axis=1)
 
 
-def get_stats_coverage(x, gen_data, rl, trim=False, strim_5=18, strim_3=18):
+def get_stats_coverage(x, gen_data, rl, il, trim=False, strim_5=18, strim_3=18):
     """Get coverage statistics
 
     Args:
         x (list): A list with the coverage per position
         strim_5 (int, optional): How much to trim on the 5'. Defaults to 18.
         strim_3 (int, optional): How much to trim on the 3'. Defaults to 18.
 
@@ -499,17 +498,21 @@
         long_enough = cov.shape[0] >= strim_5 + strim_3 + 10
         if long_enough:
             cov = cov[strim_5:-strim_3]
 
     if gen_data[x]["n_alns"] > 1:
         rl_mean = np.mean(rl)
         rl_std = np.std(rl, ddof=1)
+        il_mean = np.mean(il)
+        il_std = np.std(il, ddof=1)
     else:
         rl_mean = rl[0]
         rl_std = 0
+        il_mean = il[0]
+        il_std = 0
 
     cov_mean = cov.mean()
     if cov_mean > 0:
         cov_std = cov.std()
         cov_evenness = cov_std / cov_mean
         breadth = ((cov != 0).sum()) / length
         breadth_exp = 1 - np.exp(-cov_mean)
@@ -526,23 +529,25 @@
             cov_evenness,
             breadth,
             breadth_exp,
             breadth_exp_ratio,
             gen_data[x]["n_alns"],
             rl_mean,
             rl_std,
+            il_mean,
+            il_std,
         )
 
 
 def get_coverage_stats(df, trim=True):
-
     queries = defaultdict(int)
     gen_data = defaultdict(dict)
     al = defaultdict(list)
     rl = defaultdict(list)
+    il = defaultdict(list)
     # for a, q, b, c, d, e in tqdm.tqdm(
     #     zip(
     #         df["Chromosome"],
     #         df["Query"],
     #         df["Start"],
     #         df["End"],
     #         df["slen"],
@@ -564,39 +569,43 @@
         a = df[i, "subjectId"]
         q = df[i, "queryId"]
         b = df[i, "subjectStart"]
         c = df[i, "subjectEnd"]
         d = df[i, "slen"]
         e = df[i, "alnLength"]
         f = df[i, "qlen"]
+        g = df[i, "percIdentity"]
         b = b - 1
 
         if a in gen_data:
             gen_data[a]["cov"][b:c] += 1
             gen_data[a]["n_alns"] += 1
             al[a] += [e / 3]
             rl[a] += [f]
+            il[a] += [g]
         else:
             gen_data[a]["cov"] = np.zeros(d, dtype=int)
             gen_data[a]["cov"][b:c] += 1
             gen_data[a]["n_alns"] = 0
             gen_data[a]["n_alns"] += 1
             al[a] += [e / 3]
             rl[a] += [f]
+            il[a] += [g]
     logging.info(
         f"References will be dynamically trimmed at 5'/3'-ends (half of the avg. aln length)"
     )
     stats = [
         get_stats_coverage(
             chrom,
             gen_data=gen_data,
             strim_5=int(np.mean(al[chrom]) / 2),
             strim_3=int(np.mean(al[chrom]) / 2),
             trim=trim,
             rl=rl[chrom],
+            il=il[chrom],
         )
         for chrom in tqdm.tqdm(
             gen_data,
             total=len(gen_data.keys()),
             leave=False,
             ncols=100,
             desc=f"References processed",
@@ -614,14 +623,16 @@
         "depth_evenness",
         "breadth",
         "breadth_expected",
         "breadth_expected_ratio",
         "n_alns",
         "avg_read_length",
         "stdev_read_length",
+        "avg_identity",
+        "stdev_identity",
     ]
     return stats
 
 
 def aggregate_gene_abundances(mapping_file, gene_abundances, threads=1):
     dt.options.progress.clear_on_success = True
     dt.options.nthreads = threads
@@ -678,18 +689,63 @@
             "stdev_read_length",
             axis=1,
             drop_level=True,
         )
         mappings_agg_sl = mappings_agg_sl.reset_index("group")
         mappings_agg_sl.rename({"mean": "stdev_read_length"}, axis=1, inplace=True)
 
+        # Get average identities
+        mappings_agg_ai = mappings.groupby("group").agg(
+            {
+                "avg_identity": ["mean"],
+            }
+        )
+        mappings_agg_ai = mappings_agg_ai.xs(
+            "avg_identity",
+            axis=1,
+            drop_level=True,
+        )
+        mappings_agg_ai = mappings_agg_ai.reset_index("group")
+        mappings_agg_ai.rename({"mean": "avg_identity"}, axis=1, inplace=True)
+
+        mappings_agg_si = mappings.groupby("group").agg(
+            {
+                "stdev_identity": ["mean"],
+            }
+        )
+        mappings_agg_si = mappings_agg_si.xs(
+            "stdev_identity",
+            axis=1,
+            drop_level=True,
+        )
+        mappings_agg_si = mappings_agg_si.reset_index("group")
+        mappings_agg_si.rename({"mean": "stdev_identity"}, axis=1, inplace=True)
+
         mappings_agg = reduce(
             lambda left, right: pd.merge(left, right, on=["group"], how="inner"),
-            [mappings_agg_dm, mappings_agg_al, mappings_agg_sl],
-        )
+            [
+                mappings_agg_dm,
+                mappings_agg_al,
+                mappings_agg_sl,
+                mappings_agg_ai,
+                mappings_agg_si,
+            ],
+        )
+        mappings_agg.columns = [
+            "group",
+            "coverage_mean",
+            "coverage_stdev",
+            "coverage_median",
+            "coverage_sum",
+            "n_genes",
+            "avg_read_length",
+            "stdev_read_length",
+            "avg_identity",
+            "stdev_identity",
+        ]
         return mappings, mappings_agg
 
 
 def convert_to_anvio(df, annotation_source):
     # gene_id	enzyme_accession	source	coverage	detection
     # Select and rename columns from pandas dataframe
     df = df.copy()
```

### Comparing `x-filter-1.0.6/x_filter/utils.py` & `x-filter-1.0.7/x_filter/utils.py`

 * *Files identical despite different names*

