# Comparing `tmp/fetch_features-0.2.2.tar.gz` & `tmp/fetch_features-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetch_features-0.2.2.tar", last modified: Fri May 26 22:13:33 2023, max compression
+gzip compressed data, was "fetch_features-0.2.3.tar", last modified: Sun May 28 23:59:38 2023, max compression
```

## Comparing `fetch_features-0.2.2.tar` & `fetch_features-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.875060 fetch_features-0.2.2/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-04-07 00:12:37.000000 fetch_features-0.2.2/LICENSE.md
--rw-r--r--   0 msp        (501) staff       (20)     3235 2023-05-26 22:13:33.874471 fetch_features-0.2.2/PKG-INFO
--rwxr-xr-x   0 msp        (501) staff       (20)     2509 2023-05-26 22:10:06.000000 fetch_features-0.2.2/README.md
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.859080 fetch_features-0.2.2/images/
--rw-r--r--   0 msp        (501) staff       (20)   340268 2023-04-30 01:32:33.000000 fetch_features-0.2.2/images/fetch_features_gui.png
--rw-r--r--   0 msp        (501) staff       (20)     1156 2023-05-26 21:25:14.000000 fetch_features-0.2.2/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-05-26 22:13:33.875201 fetch_features-0.2.2/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.855887 fetch_features-0.2.2/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.867561 fetch_features-0.2.2/src/fetch_features.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     3235 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      466 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       57 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)      159 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        8 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/top_level.txt
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.873347 fetch_features-0.2.2/src/fetcher/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-05-04 15:38:40.000000 fetch_features-0.2.2/src/fetcher/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)     1239 2023-05-13 22:48:30.000000 fetch_features-0.2.2/src/fetcher/__main__.py
--rwx------   0 msp        (501) staff       (20)    16395 2023-05-13 22:49:16.000000 fetch_features-0.2.2/src/fetcher/access_genbank.py
--rwx------   0 msp        (501) staff       (20)    33243 2023-05-04 16:18:08.000000 fetch_features-0.2.2/src/fetcher/database.py
--rw-r--r--   0 msp        (501) staff       (20)    17348 2023-05-13 22:50:35.000000 fetch_features-0.2.2/src/fetcher/gui.py
--rw-r--r--   0 msp        (501) staff       (20)    10405 2023-05-26 21:57:12.000000 fetch_features-0.2.2/src/fetcher/user_input.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.408218 fetch_features-0.2.3/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-04-07 00:12:37.000000 fetch_features-0.2.3/LICENSE.md
+-rw-r--r--   0 msp        (501) staff       (20)     3259 2023-05-28 23:59:38.407515 fetch_features-0.2.3/PKG-INFO
+-rwxr-xr-x   0 msp        (501) staff       (20)     2533 2023-05-28 22:29:31.000000 fetch_features-0.2.3/README.md
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.382464 fetch_features-0.2.3/images/
+-rw-r--r--   0 msp        (501) staff       (20)   340268 2023-04-30 01:32:33.000000 fetch_features-0.2.3/images/fetch_features_gui.png
+-rw-r--r--   0 msp        (501) staff       (20)     1137 2023-05-28 23:34:25.000000 fetch_features-0.2.3/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-05-28 23:59:38.408374 fetch_features-0.2.3/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.377710 fetch_features-0.2.3/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.390154 fetch_features-0.2.3/src/fetch_features.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     3259 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)      466 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       57 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)      146 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        8 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.405568 fetch_features-0.2.3/src/fetcher/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-05-04 15:38:40.000000 fetch_features-0.2.3/src/fetcher/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)     1239 2023-05-13 22:48:30.000000 fetch_features-0.2.3/src/fetcher/__main__.py
+-rwx------   0 msp        (501) staff       (20)    16594 2023-05-28 22:51:12.000000 fetch_features-0.2.3/src/fetcher/access_genbank.py
+-rwx------   0 msp        (501) staff       (20)    32983 2023-05-28 18:16:08.000000 fetch_features-0.2.3/src/fetcher/database.py
+-rw-r--r--   0 msp        (501) staff       (20)    17348 2023-05-13 22:50:35.000000 fetch_features-0.2.3/src/fetcher/gui.py
+-rw-r--r--   0 msp        (501) staff       (20)    10405 2023-05-26 21:57:12.000000 fetch_features-0.2.3/src/fetcher/user_input.py
```

### Comparing `fetch_features-0.2.2/LICENSE.md` & `fetch_features-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.2/PKG-INFO` & `fetch_features-0.2.3/src/fetch_features.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fetch_features
-Version: 0.2.2
+Name: fetch-features
+Version: 0.2.3
 Summary: Fetch features from a list of accession or BioSample numbers.
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/fetch_features
 Keywords: unique identifier,accession number,BioSample number,GenBank,sequence features
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -90,12 +90,10 @@
 
 3. If you prefer the GUI version.
 
 ```bash
 fetch_features --gui
 ```
 
-<p align="center">
-  <picture>
-    <img src="./images/fetch_features_gui.png">
-  </picture>
+<p align='center'>
+  <img src=https://github.com/ivanmugu/fetch_features/blob/main/images/fetch_features_gui.png />
 </p>
```

### Comparing `fetch_features-0.2.2/README.md` & `fetch_features-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -73,12 +73,10 @@
 
 3. If you prefer the GUI version.
 
 ```bash
 fetch_features --gui
 ```
 
-<p align="center">
-  <picture>
-    <img src="./images/fetch_features_gui.png">
-  </picture>
+<p align='center'>
+  <img src=https://github.com/ivanmugu/fetch_features/blob/main/images/fetch_features_gui.png />
 </p>
```

### Comparing `fetch_features-0.2.2/images/fetch_features_gui.png` & `fetch_features-0.2.3/images/fetch_features_gui.png`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.2/pyproject.toml` & `fetch_features-0.2.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fetch_features"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Fetch features from a list of accession or BioSample numbers."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
@@ -29,15 +29,14 @@
     "darkdetect==0.8.0",
     "numpy==1.24.3",
     "pandas==2.0.1",
     "python-dateutil==2.8.2",
     "pytz==2023.3",
     "six==1.16.0",
     "tzdata==2023.3",
-    "toml==0.10.2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ivanmugu/fetch_features"
 
 [project.scripts]
 fetch_features = "fetcher.__main__:main"
```

### Comparing `fetch_features-0.2.2/src/fetch_features.egg-info/PKG-INFO` & `fetch_features-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fetch-features
-Version: 0.2.2
+Name: fetch_features
+Version: 0.2.3
 Summary: Fetch features from a list of accession or BioSample numbers.
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/fetch_features
 Keywords: unique identifier,accession number,BioSample number,GenBank,sequence features
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -90,12 +90,10 @@
 
 3. If you prefer the GUI version.
 
 ```bash
 fetch_features --gui
 ```
 
-<p align="center">
-  <picture>
-    <img src="./images/fetch_features_gui.png">
-  </picture>
+<p align='center'>
+  <img src=https://github.com/ivanmugu/fetch_features/blob/main/images/fetch_features_gui.png />
 </p>
```

### Comparing `fetch_features-0.2.2/src/fetcher/__main__.py` & `fetch_features-0.2.3/src/fetcher/__main__.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.2/src/fetcher/access_genbank.py` & `fetch_features-0.2.3/src/fetcher/access_genbank.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,16 +319,16 @@
 
     # results' field names for the csv table.
     fields = [
         "set_batch", "description", "accession", "size",
         "molecule", "mod_date", "topology", "mol_type", "organism",
         "strain", "isolation_source", "host", "plasmid", "country",
         "lat_lon", "collection_date", "note", "serovar", "collected_by",
-        "genotype", "BioProject", "BioSample", "Assem_Method",
-        "Gen_Coverage", "Seq_Technol", "Gen_Represent", "Exp_Final_Ver"]
+        "genotype", "bioproject", "biosample", "assem_method",
+        "gen_coverage", "seq_technol", "gen_represent", "exp_final_ver"]
     # references' field names for the csv table.
     ref_fields = [
         "accession", "reference_num", "location", "authors", "title",
         "journal", "medline_id", "pubmed_id", "comment"
     ]
     # Create DictWriter for results.
     results_writer = csv.DictWriter(results, fields)
@@ -336,36 +336,43 @@
     # Write headers into csv files.
     results_writer.writeheader()
     ref_results_writer.writeheader()
 
     # If user requested features from list of accession numbers use the
     # `fetch_from_accession` function.
     if type_list == 'accession' and (not access_biosample_from_accession):
-        # Formating list of accession numbers in batches
-        submission_list = database.make_uid_batch_list(list_accessions)
+        # Formating list of accession numbers in batches. Don't make batches
+        # greater than 500.
+        submission_list = database.make_uid_batch_list(
+            uid_list=list_accessions, batch_size=200
+        )
         # Fetching features
         print("\nFetching features\n")
         fetch_from_accession(
             results_file=results,
             results_fields=fields,
             ref_results_file=ref_results,
             ref_results_fields=ref_fields,
             submission_list=submission_list,
         )
 
     # If user requested to access the BioSample numbers linked to accession
     # numbers, use the `get_biosample_numbers` function to retrieve the linked
     # BioSample numbers. Then use the `fetch_from_biosample` function.
     if type_list == 'accession' and access_biosample_from_accession:
-        # Formating list of accession numbers in batches
-        submission_list = database.make_uid_batch_list(list_accessions)
+        # Formating list of accession numbers in batches. Don't make batches
+        # greater than 500.
+        submission_list = database.make_uid_batch_list(
+            uid_list=list_accessions, batch_size=200
+        )
         # Getting BioSample numbers
         print("Retrieving BioSample numbers from list of accession numbers")
         list_biosamples = database.get_biosample_numbers(
-            submission_list, email_address)
+            submission_list, email_address
+        )
         # Fetching features
         print("\nFetching features\n")
         fetch_from_biosample(
             results_file=results,
             results_fields=fields,
             ref_results_file=ref_results,
             ref_results_fields=ref_fields,
```

### Comparing `fetch_features-0.2.2/src/fetcher/database.py` & `fetch_features-0.2.3/src/fetcher/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -239,14 +239,57 @@
                 if 'BioSample' in list_dbxrefs:
                     biosample_numbers.append(list_dbxrefs[1])
                     break
 
     return biosample_numbers
 
 
+class Info:
+    """"Class to store data retrieved from the nuccore database."""
+
+    def __init__(
+        self, set_batch='missing', description='missing', accession='missing',
+        size='missing', mod_date='missing', molecule='missing',
+        topology='missing', mol_type='missing', organism='missing',
+        strain='missing', isolation_source='missing', host='missing',
+        plasmid='missing', country='missing', lat_lon='missing',
+        collection_date='missing', note='missing', serovar='missing',
+        collected_by='missing', genotype='missing', bioproject='missing',
+        biosample='missing', assem_method='missing', gen_coverage='missing',
+        seq_technol='missing', gen_represent='missing', exp_final_ver='missing'
+    ):
+        self.set_batch = set_batch
+        self.description = description
+        self.accession = accession
+        self.size = size
+        self.molecule = molecule
+        self.mod_date = mod_date
+        self.topology = topology
+        self.mol_type = mol_type
+        self.organism = organism
+        self.strain = strain
+        self.isolation_source = isolation_source
+        self.host = host
+        self.plasmid = plasmid
+        self.country = country
+        self.lat_lon = lat_lon
+        self.collection_date = collection_date
+        self.note = note
+        self.serovar = serovar
+        self.collected_by = collected_by
+        self.genotype = genotype
+        self.bioproject = bioproject
+        self.biosample = biosample
+        self.assem_method = assem_method
+        self.gen_coverage = gen_coverage
+        self.seq_technol = seq_technol
+        self.gen_represent = gen_represent
+        self.exp_final_ver = exp_final_ver
+
+
 def parser(fetch_handle: IO, set_number: int) -> tuple:
     """Parse information fetched from nuccore NCBI.
 
     Parameters
     ----------
     fetch_handle : IO Entre.efetch object
         Pointer to a network connection that will allow to download and parse
@@ -261,309 +304,255 @@
         List of dictionaries. Every dictionary corresponds to features of one
         accession number.
     ref_records: list
         List of dictionaries. Every dictionary carries information of the
         references of an accession number. One accession number can have one or
         more references. Therefore, this list may be longer than `records`.
     """
-    # Create a list to save records in dictionaries.
+    # Create a list to save Info classes with records.
     records = []
     # Create a list to save the references related to each accession number.
     ref_records = []
 
     # Parse the fetched information.
     for seq_record in SeqIO.parse(fetch_handle, "gb"):
-        # Dictionary to store fetched information.
-        info = {}
+        # Initiate an Info class to store collected data.
+        info = Info()
         # Keep track of the set_number (or batch) analyzed.
-        info['set_batch'] = set_number
+        info.set_batch = set_number
         # Extract `description`.
-        info['description'] = seq_record.description
+        info.description = seq_record.description
         # Extract sequence id, i.e. `accession` number.
-        info['accession'] = seq_record.id
+        info.accession = seq_record.id
         # Extract `size` from `.seq`.
         # `.seq` is an object with the sequence itself.
-        info['size'] = len(seq_record.seq)
+        info.size = len(seq_record.seq)
 
         #######################################################################
         # '.annotations' is a dictionary of aditional information about the
         # sequence as last modification date, topology, sequence_version,
         # organims, references, etc.
         #######################################################################
         # Extract `date` and give format.
         if 'date' in seq_record.annotations:
             mod_date = seq_record.annotations['date']
             mod_date = datetime.strptime(mod_date, '%d-%b-%Y')
             mod_date = datetime.strftime(mod_date, "%Y-%m-%d")
-            info['mod_date'] = mod_date
-        else:
-            info['mod_date'] = 'missing'
+            info.mod_date = mod_date
         # Extract `topology`.
         if "topology" in seq_record.annotations:
-            info['topology'] = seq_record.annotations["topology"]
-        else:
-            info['topology'] = "missing"
+            info.topology = seq_record.annotations["topology"]
 
         # Check whether it is `chromosome` or `plasmid`. The 3,000,000 length
-        # used in `size` is an arbitrary number that considers chormosomes of
+        # used in `size` is an arbitrary number that considers chromosomes of
         # that length.
         # Check if label `chromosome` is in the `description`.
-        if 'chromosome' in info['description']:
-            info['molecule'] = 'chromosome'
+        if 'chromosome' in info.description:
+            info.molecule = 'chromosome'
         # If not, consider a chromosome the at least 3,000,000 in legth.
-        elif info['size'] >= 3_000_000 and info['topology'] == 'circular':
-            info['molecule'] = 'chromosome'
-        # If it is not a chromosome, the check if it is a `plasmid`.
-        elif 'plasmid' in info['description']:
-            info['molecule'] = 'plasmid'
-        else:
-            info['molecule'] = 'missing'
+        elif info.size >= 3_000_000 and info.topology == 'circular':
+            info.molecule = 'chromosome'
+        # If it is not a chromosome, then check if it is a `plasmid`.
+        elif 'plasmid' in info.description:
+            info.molecule = 'plasmid'
 
-        # '.features' is a list of SeqFeatures objects with more structured
+        # `.features` is a list of SeqFeatures objects with more structured
         # information about the features on a sequence.
-        feature = seq_record.features
-
-        # Loop over list feature.
-        for index in feature:
-            # '.type' is only a description of the type of feature
-            # that could be source, CDS, gene, etc.
-            # In source we can find organism, strain, host, country, etc.
-            if index.type == "source":
-                # Create a dictionary of the qualifiers from source.
-                dictionary = dict(index.qualifiers)
-                # '.get' gives a list
-                # Extract molecule type (`mol_type`).
-                if "mol_type" in dictionary:
-                    info['mol_type'] = dictionary.get("mol_type")[0]
-                else:
-                    info['mol_type'] = 'missing'
-                # Extract `organism`.
-                if 'organism' in dictionary:
-                    info['organism'] = dictionary.get('organism')[0]
-                else:
-                    info['organism'] = 'missing'
-                # Extract `strain`.
-                if 'strain' in dictionary:
-                    info['strain'] = dictionary.get('strain')[0]
-                else:
-                    info['strain'] = 'missing'
-                # Extract `isolation_source`.
-                if 'isolation_source' in dictionary:
-                    info['isolation_source'] =\
-                        dictionary.get('isolation_source')[0]
-                else:
-                    info['isolation_source'] = 'missing'
-                # Extract `host`.
-                if 'host' in dictionary:
-                    info['host'] = dictionary.get('host')[0]
-                else:
-                    info['host'] = 'missing'
-                # Extract `plasmid`.
-                if 'plasmid' in dictionary:
-                    info['plasmid'] = dictionary.get('plasmid')[0]
-                else:
-                    info['plasmid'] = 'missing'
-                # Extract `country`.
-                if 'country' in dictionary:
-                    info['country'] = dictionary.get('country')[0]
-                else:
-                    info['country'] = 'missing'
-                # Extract `coordinates`.
-                if "lat_lon" in dictionary:
-                    info['lat_lon'] = dictionary.get("lat_lon")[0]
-                else:
-                    info['lat_lon'] = 'missing'
-                # Extract `collection_date`.
-                if "collection_date" in dictionary:
-                    info['collection_date'] =\
-                        dictionary.get("collection_date")[0]
-                else:
-                    info['collection_date'] = 'missing'
-                # Extract `note`.
-                if "note" in dictionary:
-                    info['note'] = dictionary.get("note")[0]
-                else:
-                    info['note'] = 'missing'
-                # Extract `serovar`.
-                if "serovar" in dictionary:
-                    info['serovar'] = dictionary.get("serovar")[0]
-                else:
-                    info['serovar'] = 'missing'
-                # Extract `collected_by`.
-                if "collected_by" in dictionary:
-                    info['collected_by'] = dictionary.get("collected_by")[0]
-                else:
-                    info['collected_by'] = 'missing'
-                # Extract `genotype`.
-                if "genotype" in dictionary:
-                    info['genotype'] = dictionary.get("genotype")[0]
-                else:
-                    info['genotype'] = 'missing'
-
+        # Loop over list of features to find the type source.
+        for feature in seq_record.features:
+            # `.type` is only a description of the type of feature that could
+            # be source, CDS, gene, etc. The feature that we need is `source`.
+            # In type `source` we can find organism, strain, host, country, etc.
+            if feature.type == "source":
+                # `qualifiers` is a Python dictionary of additional information
+                # about the feature.
+                source = feature.qualifiers
                 break
-
-        # '.dbxrefs' is a list populated from any PROJECT or DBLINK
-        # Check if .dbxrefs has any information.
-        if len(seq_record.dbxrefs) == 0:
-            info['BioProject'] = 'missing'
-            info['BioSample'] = 'missing'
-
-        # Convert the list dbxrefs into dictionary.
-        dictionary_dbxrefs = {}
-        for i in range(len(seq_record.dbxrefs)):
-            s = seq_record.dbxrefs[i].split(":")
-            dictionary_dbxrefs[s[0]] = s[1]
-
-        # Extract `BioProject` and `BioSample`.
-        if "BioProject" in dictionary_dbxrefs:
-            info['BioProject'] = dictionary_dbxrefs.get("BioProject")
-        else:
-            info['BioProject'] = 'missing'
-        if "BioSample" in dictionary_dbxrefs:
-            info['BioSample'] = dictionary_dbxrefs.get("BioSample")
-        else:
-            info['BioSample'] = 'missing'
+        # Extract all the info from the type `source`.
+        # `source` is a dictionary where the key-values are lists. Therefore,
+        # the `.get` method retrieves a list.
+        # Extract molecule type (`mol_type`).
+        if "mol_type" in source:
+            info.mol_type = source.get("mol_type")[0]
+        # Extract `organism`.
+        if 'organism' in source:
+            info.organism = source.get('organism')[0]
+        # Extract `strain`.
+        if 'strain' in source:
+            info.strain = source.get('strain')[0]
+        # Extract `isolation_source`.
+        if 'isolation_source' in source:
+            info.isolation_source = source.get('isolation_source')[0]
+        # Extract `host`.
+        if 'host' in source:
+            info.host = source.get('host')[0]
+        # Extract `plasmid`.
+        if 'plasmid' in source:
+            info.plasmid = source.get('plasmid')[0]
+        # Extract `country`.
+        if 'country' in source:
+            info.country = source.get('country')[0]
+        # Extract `coordinates`.
+        if "lat_lon" in source:
+            info.lat_lon = source.get("lat_lon")[0]
+        # Extract `collection_date`.
+        if "collection_date" in source:
+            info.collection_date = source.get("collection_date")[0]
+        # Extract `note`.
+        if "note" in source:
+            info.note = source.get("note")[0]
+        # Extract `serovar`.
+        if "serovar" in source:
+            info.serovar = source.get("serovar")[0]
+        # Extract `collected_by`.
+        if "collected_by" in source:
+            info.collected_by = source.get("collected_by")[0]
+        # Extract `genotype`.
+        if "genotype" in source:
+            info.genotype = source.get("genotype")[0]
+
+        # `.dbxrefs` is a list populated from any PROJECT or DBLINK.
+        # If `.dbxrefs` has information, extract `BioProject` and `BioSample`.
+        if len(seq_record.dbxrefs) != 0:
+            for dbxref in seq_record.dbxrefs:
+                # Extract `BioProject` and `BioSample`.
+                if "BioProject" in dbxref:
+                    info.bioproject = dbxref.split(':')[1]
+                if "BioSample" in dbxref:
+                    info.biosample = dbxref.split(':')[1]
 
         # #####################################################################
         # Mine `structured_comment`
         # #####################################################################
         # Sometimes the data needed is organized in `Genome-Assembly-Data` or
         # in `Assembly-Data`. Check if the sequence has `structured_comment`
         # and `Genome-Assembly-Data`.
         if "structured_comment" in seq_record.annotations and (
             "Genome-Assembly-Data" in (
                 seq_record.annotations["structured_comment"])):
             # Extract `Assembly Method`.
             if ("Assembly Method" in (
                 seq_record.annotations["structured_comment"]
                                       ["Genome-Assembly-Data"])):
-                info['Assem_Method'] = (
+                info.assem_method = (
                     seq_record.annotations["structured_comment"]
                                           ["Genome-Assembly-Data"]
                                           ["Assembly Method"])
-            else:
-                info['Assem_Method'] = "missing"
             # Extract `Genome Representation`.
             if "Genome Representation" in (
                 seq_record.annotations["structured_comment"]
                                       ["Genome-Assembly-Data"]):
-                info['Gen_Represent'] = (
+                info.gen_represent = (
                     seq_record.annotations["structured_comment"]
                                           ["Genome-Assembly-Data"]
                                           ["Genome Representation"])
-            else:
-                info['Gen_Represent'] = "missing"
             # Extract `Expected Final Version`.
             if "Expected Final Version" in (
                 seq_record.annotations["structured_comment"]
                                       ["Genome-Assembly-Data"]
             ):
-                info['Exp_Final_Ver'] = (
+                info.exp_final_ver = (
                     seq_record.annotations["structured_comment"]
                                           ["Genome-Assembly-Data"]
                                           ["Expected Final Version"]
                 )
-            else:
-                info['Exp_Final_Ver'] = "missing"
             # Extract `Genome Coverage`.
             if "Genome Coverage" in (
                 seq_record.annotations["structured_comment"]
                                       ["Genome-Assembly-Data"]):
-                info['Gen_Coverage'] = (
+                info.gen_coverage = (
                     seq_record.annotations["structured_comment"]
                                           ["Genome-Assembly-Data"]
                                           ["Genome Coverage"])
-            else:
-                info['Gen_Coverage'] = "missing"
-            # Exteract `Sequencing Technology`.
+            # Extract `Sequencing Technology`.
             if "Sequencing Technology" in (
                 seq_record.annotations["structured_comment"]
                                       ["Genome-Assembly-Data"]):
-                info['Seq_Technol'] = (
+                info.seq_technol = (
                     seq_record.annotations["structured_comment"]
                                           ["Genome-Assembly-Data"]
                                           ["Sequencing Technology"])
-            else:
-                info['Seq_Technol'] = "missing"
         # Check if the sequence has `structured_comment` and `Assembly-Data`.
         elif "structured_comment" in seq_record.annotations and (
             "Assembly-Data" in (
                 seq_record.annotations["structured_comment"])):
             # Extract `Assembly Method`.
             if "Assembly Method" in (
                 seq_record.annotations["structured_comment"]
                                       ["Assembly-Data"]):
-                info['Assem_Method'] = (
+                info.assem_method = (
                     seq_record.annotations["structured_comment"]
                                           ["Assembly-Data"]
                                           ["Assembly Method"])
-            else:
-                info['Assem_Method'] = "missing"
             # Extract `Genome Representation`.
             if "Genome Representation" in (
                 seq_record.annotations["structured_comment"]
                                       ["Genome-Assembly-Data"]):
-                info['Gen_Represent'] = (
+                info.gen_represent = (
                     seq_record.annotations["structured_comment"]
                                           ["Genome-Assembly-Data"]
                                           ["Genome Representation"])
-            else:
-                info['Gen_Represent'] = "missing"
             # Extract `Expected Final Version`.
             if "Expected Final Version" in (
                 seq_record.annotations["structured_comment"]
                                       ["Genome-Assembly-Data"]
             ):
-                info['Exp_Final_Ver'] = (
+                info.exp_final_ver = (
                     seq_record.annotations["structured_comment"]
                                           ["Genome-Assembly-Data"]
                                           ["Expected Final Version"]
                 )
-            else:
-                info['Exp_Final_Ver'] = "missing"
             # Extract `Genome Coverage`.
             if "Genome Coverage" in (
                 seq_record.annotations["structured_comment"]
                                       ["Assembly-Data"]):
-                info['Gen_Coverage'] = (
+                info.gen_coverage = (
                     seq_record.annotations["structured_comment"]
                                           ["Assembly-Data"]
                                           ["Genome Coverage"])
-            else:
-                info['Gen_Coverage'] = "missing"
             # Extract `Sequencing Technology`.
             if "Sequencing Technology" in (
                 seq_record.annotations["structured_comment"]
                                       ["Assembly-Data"]):
-                info['Seq_Technol'] = (
+                info.seq_technol = (
                     seq_record.annotations["structured_comment"]
                                           ["Assembly-Data"]
                                           ["Sequencing Technology"])
-            else:
-                info['Seq_Technol'] = "missing"
-        # Otherwise, the info is missing.
-        else:
-            info['Assem_Method'] = "missing"
-            info['Gen_Coverage'] = "missing"
-            info['Seq_Technol'] = "missing"
-            info['Gen_Represent'] = "missing"
-            info['Exp_Final_Ver'] = "missing"
 
-        # Append info dictionary to records list.
-        records.append(info)
+        # Convert info class into a dictionary and append to records list.
+        records.append(vars(info))
 
         # ################################################
         # Get references and make an independent database.
         # ################################################
         if 'references' in seq_record.annotations:
             ref_records.extend(get_references(seq_record))
 
     return (records, ref_records)
 
 
+class References:
+    """Class to store references from a GenBank record."""
+
+    def __init__(
+        self, accession='missing', reference_num='missing', location='missing',
+        authors='missing', title='missing', journal='missing',
+        medline_id='missing', pubmed_id='missing', comment='missing'
+    ):
+        self.accession = accession
+        self.reference_num = reference_num
+        self.location = location
+        self.authors = authors
+        self.title = title
+        self.journal = journal
+        self.medline_id = medline_id
+        self.pubmed_id = pubmed_id
+        self.comment = comment
+
+
 def get_references(record: IO) -> list:
     """Get all references of accession number.
 
     Parameters
     ----------
     record : Biopython SeqIO.parser object
         TextIO object to parse a GenBank record.
@@ -571,30 +560,34 @@
     Returns
     -------
     references = list
         List of dictionaries with all the references of the GenBank record.
     """
     references = []
     for i, reference in enumerate(record.annotations['references']):
-        info = {}
-        info['accession'] = record.id
-        info['reference_num'] = str(i)
-        if len(reference.location) == 0:
-            info['location'] = "N/A"
-        else:
+        info = References()
+        info.accession = record.id
+        info.reference_num = str(i + 1)
+        if reference.location:
             start = reference.location[0].start
             end = reference.location[0].end
-            info['location'] = f"bases {start} to {end}"
-        info['authors'] = reference.authors
-        info['title'] = reference.title
-        info['journal'] = reference.journal
-        info['medline_id'] = reference.medline_id
-        info['pubmed_id'] = reference.pubmed_id
-        info['comment'] = reference.comment
-        references.append(info)
+            info.location = f"bases {start} to {end}"
+        if reference.authors:
+            info.authors = reference.authors
+        if reference.title:
+            info.title = reference.title
+        if reference.journal:
+            info.journal = reference.journal
+        if reference.medline_id:
+            info.medline_id = reference.medline_id
+        if reference.pubmed_id:
+            info.pubmed_id = reference.pubmed_id
+        if reference.comment:
+            info.comment = reference.comment
+        references.append(vars(info))
     return references
 
 
 def clean_references(updated_features: list, reference_records: list) -> list:
     """Remove references from outdated accession numbers.
 
     Parameters
@@ -670,35 +663,35 @@
                 country text,
                 lat_lon text,
                 collection_date text,
                 note text,
                 serovar text,
                 collected_by text,
                 genotype text,
-                BioProject text,
-                BioSample text,
-                Assem_Method text,
-                Gen_Coverage text,
-                Seq_Technol text,
-                Gen_Represent text,
-                Exp_Final_Ver
+                bioproject text,
+                biosample text,
+                assem_method text,
+                gen_coverage text,
+                seq_technol text,
+                gen_represent text,
+                exp_final_ver
                 )""")
     conn.commit()
 
     # Transfer results obtained from GenBank into the table features_raw
     # created in SQL.
     for _, raw_result in enumerate(raw_data):
         c.execute(
             """INSERT INTO features_raw VALUES(
                 :set_batch, :description, :accession, :size, :molecule,
                 :mod_date, :topology, :mol_type, :organism, :strain,
                 :isolation_source, :host, :plasmid, :country, :lat_lon,
                 :collection_date, :note, :serovar, :collected_by, :genotype,
-                :BioProject, :BioSample, :Assem_Method, :Gen_Coverage,
-                :Seq_Technol, :Gen_Represent, :Exp_Final_Ver
+                :bioproject, :biosample, :assem_method, :gen_coverage,
+                :seq_technol, :gen_represent, :exp_final_ver
             )""", {
                 'set_batch': int(raw_result['set_batch']),
                 'description': raw_result['description'],
                 'accession': raw_result['accession'],
                 'size': int(raw_result['size']),
                 'molecule': raw_result['molecule'],
                 'mod_date': raw_result['mod_date'],
@@ -712,21 +705,21 @@
                 'country': raw_result['country'],
                 'lat_lon': raw_result['lat_lon'],
                 'collection_date': raw_result['collection_date'],
                 'note': raw_result['note'],
                 'serovar': raw_result['serovar'],
                 'collected_by': raw_result['collected_by'],
                 'genotype': raw_result['genotype'],
-                'BioProject': raw_result['BioProject'],
-                'BioSample': raw_result['BioSample'],
-                'Assem_Method': raw_result['Assem_Method'],
-                'Gen_Coverage': raw_result['Gen_Coverage'],
-                'Seq_Technol': raw_result['Seq_Technol'],
-                'Gen_Represent': raw_result['Gen_Represent'],
-                'Exp_Final_Ver': raw_result['Exp_Final_Ver']
+                'bioproject': raw_result['bioproject'],
+                'biosample': raw_result['biosample'],
+                'assem_method': raw_result['assem_method'],
+                'gen_coverage': raw_result['gen_coverage'],
+                'seq_technol': raw_result['seq_technol'],
+                'gen_represent': raw_result['gen_represent'],
+                'exp_final_ver': raw_result['exp_final_ver']
             }
         )
     conn.commit()
 
     # Get the most updated files and order by size.
     c.execute(
         """
@@ -768,30 +761,30 @@
         info['country'] = updated_result[13]
         info['lat_lon'] = updated_result[14]
         info['collection_date'] = updated_result[15]
         info['note'] = updated_result[16]
         info['serovar'] = updated_result[17]
         info['collected_by'] = updated_result[18]
         info['genotype'] = updated_result[19]
-        info['BioProject'] = updated_result[20]
-        info['BioSample'] = updated_result[21]
-        info['Assem_Method'] = updated_result[22]
-        info['Gen_Coverage'] = updated_result[23]
-        info['Seq_Technol'] = updated_result[24]
-        info['Gen_Represent'] = updated_result[25]
-        info['Exp_Final_Ver'] = updated_result[26]
+        info['bioproject'] = updated_result[20]
+        info['biosample'] = updated_result[21]
+        info['assem_method'] = updated_result[22]
+        info['gen_coverage'] = updated_result[23]
+        info['seq_technol'] = updated_result[24]
+        info['gen_represent'] = updated_result[25]
+        info['exp_final_ver'] = updated_result[26]
         records.append(info.copy())
     conn.close()
 
     return records
 
 
 def save_results_as(
         results: Path, ref_results: Path, save_as: str = 'csv'
-        ) -> None:
+) -> None:
     """Save results in the requested format.
 
     The files are saved by default in csv before this function is called. This
     function helps to make excel files if user requested. Also, by defaults,
     all files are named `results.csv`, `ref_results.csv`, or the equivalent
     names with the .xlsx extention.
```

### Comparing `fetch_features-0.2.2/src/fetcher/gui.py` & `fetch_features-0.2.3/src/fetcher/gui.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.2/src/fetcher/user_input.py` & `fetch_features-0.2.3/src/fetcher/user_input.py`

 * *Files identical despite different names*

