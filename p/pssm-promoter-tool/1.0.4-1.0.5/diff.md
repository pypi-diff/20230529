# Comparing `tmp/pssm-promoter-tool-1.0.4.tar.gz` & `tmp/pssm-promoter-tool-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssm-promoter-tool-1.0.4.tar", last modified: Mon May 15 00:19:59 2023, max compression
+gzip compressed data, was "pssm-promoter-tool-1.0.5.tar", last modified: Mon May 29 01:39:10 2023, max compression
```

## Comparing `pssm-promoter-tool-1.0.4.tar` & `pssm-promoter-tool-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-15 00:19:59.655983 pssm-promoter-tool-1.0.4/
--rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.4/LICENSE.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.4/MANIFEST.in
--rw-r--r--   0 ellinium   (501) staff       (20)     5022 2023-05-15 00:19:59.655809 pssm-promoter-tool-1.0.4/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)     4565 2023-05-15 00:19:10.000000 pssm-promoter-tool-1.0.4/README.md
--rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.4/free_energy_coeffs.npy
--rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.4/model_intercept.npy
--rw-r--r--   0 ellinium   (501) staff       (20)    13075 2023-05-14 03:06:01.000000 pssm-promoter-tool-1.0.4/pssm_promoter_calculator.py
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-15 00:19:59.655454 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/
--rw-r--r--   0 ellinium   (501) staff       (20)     5022 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/not-zip-safe
--rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/requires.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/top_level.txt
--rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.4/pyproject.toml
--rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-05-15 00:19:59.656034 pssm-promoter-tool-1.0.4/setup.cfg
--rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-05-15 00:19:49.000000 pssm-promoter-tool-1.0.4/setup.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-29 01:39:10.371258 pssm-promoter-tool-1.0.5/
+-rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.5/LICENSE.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.5/MANIFEST.in
+-rw-r--r--   0 ellinium   (501) staff       (20)     5268 2023-05-29 01:39:10.371084 pssm-promoter-tool-1.0.5/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)     4811 2023-05-29 01:37:50.000000 pssm-promoter-tool-1.0.5/README.md
+-rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.5/free_energy_coeffs.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.5/model_intercept.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)    14908 2023-05-29 01:13:36.000000 pssm-promoter-tool-1.0.5/pssm_promoter_calculator.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-29 01:39:10.370842 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/
+-rw-r--r--   0 ellinium   (501) staff       (20)     5268 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/not-zip-safe
+-rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/requires.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/top_level.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.5/pyproject.toml
+-rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-05-29 01:39:10.371310 pssm-promoter-tool-1.0.5/setup.cfg
+-rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-05-29 01:38:59.000000 pssm-promoter-tool-1.0.5/setup.py
```

### Comparing `pssm-promoter-tool-1.0.4/LICENSE.txt` & `pssm-promoter-tool-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.4/PKG-INFO` & `pssm-promoter-tool-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssm-promoter-tool
-Version: 1.0.4
+Version: 1.0.5
 Summary: The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence
 Home-page: https://github.com/ellinium/PSSM_PromoterTool
 Author: Ellina Trofimova
 Author-email: ellina.trofimova@gmail.com
 License: GNU General Public License
 Keywords: promoter prediction transcription rate
 Description-Content-Type: text/markdown
@@ -28,15 +28,15 @@
 ```
 
 2. Download and unpack the archive with files using "Code"->"Download ZIP" buttons in the right corner at https://github.com/ellinium/pssm_promoter_tool. 
 Or use
 ```
 git clone https://github.com/ellinium/pssm-promoter-tool
 ```
-
+[! you need to have a Git account and be authorised in the system to run the command !]
 
 
 USAGE:
 
 The tool requires a text or fasta file with a nucleotide sequence of a gene to process.
 From the folder with the downloaded files run:
 ```
@@ -47,41 +47,42 @@
 Depending on the result, up to four output CSV files can be generated:
 1) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
 2) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
 3) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
 4) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
-1) new_sequence - contains a gene sequence (nt) with substituted promoters. Empty for the original promoters.
-2) promoter_sequence - contains -35 motif, spacer and - 10 motif
-3) TSS -  transcriptional start site
-4) Tx_rate - transcription initiation rate
-5) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
-6) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
-7) hex35 -  an upstream 6-nucleotide site called the −35 motif 
-8) PSSM_hex35 - position-specific scoring matrix value for the -35 motif \
-9) AA_hex35 - an amino acid sequence for the -35 motif 
-10) spacer - a spacer region that separates the −10 and −35 motifs 
-11) hex10 - a downstream 6-nucleotide site called the −10 motif 
-12) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
-13) AA_hex10 - an amino acid sequence for the -10 motif 
-14) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
-15) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
-16) dG_total - total Gibbs free energy for the sequence 
-17) dG_10 - -10 motif Gibbs free energy 
-18) dG_35 - -35 motif Gibbs free energy 
-19) dG_disc - a discriminator Gibbs free energy 
-20) dG_ITR - an ITR Gibbs free energy 
-21) dG_ext10 −10 extended motif Gibbs free energy 
-22) dG_spacer - a spacer Gibbs free energy 
-23) dG_UP - an UP Gibbs free energy 
-24) dG_bind - binding Gibbs free energy 
-25) UP_position - a position of the UP element 
-26) hex35_position - a position of the -35 motif 
-27) spacer_position - a position of the spacer 
-28) hex10_position - a position of the -10 motif 
-29) disc_position - a position of the discriminator
+1) Type - 'Original Promoter' - for original sequence promoters; 'Modified Promoter' - for synonymous promoters. 
+2) TSS -  transcriptional start site 
+3) Tx_rate - transcription initiation rate 
+4) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers 
+5) hex35 -  an upstream 6-nucleotide site called the −35 motif 
+6) PSSM_hex35 - position-specific scoring matrix value for the -35 motif 
+7) AA_hex35 - an amino acid sequence for the -35 motif 
+8) hex10 - a downstream 6-nucleotide site called the −10 motif 
+9) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
+10) AA_hex10 - an amino acid sequence for the -10 motif 
+11) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
+12) spacer - a spacer region that separates the −10 and −35 motifs 
+13) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
+14) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
+15) new_gene_sequence - contains a gene sequence (nt) with substituted (Type = 'Modified Promoter') or  original promoters (Type = 'Original Promoter')
+16) promoter_sequence - contains -35 motif, spacer and - 10 motif 
+17) dG_total - total Gibbs free energy for the sequence 
+18) dG_10 - -10 motif Gibbs free energy 
+19) dG_35 - -35 motif Gibbs free energy 
+20) dG_disc - a discriminator Gibbs free energy 
+21) dG_ITR - an ITR Gibbs free energy 
+22) dG_ext10 −10 extended motif Gibbs free energy 
+23) dG_spacer - a spacer Gibbs free energy 
+24) dG_UP - an UP Gibbs free energy 
+25) dG_bind - binding Gibbs free energy 
+26) UP_position - a position of the UP element 
+27) hex35_position - a position of the -35 motif 
+28) spacer_position - a position of the spacer 
+29) hex10_position - a position of the -10 motif 
+30) disc_position - a position of the discriminator
 
 References:
 
 1. Logel DY, Trofimova E, Jaschke PR. Codon-Restrained Method for Both Eliminating and Creating Intragenic Bacterial Promoters. ACS Synth Biol. 2022 Jan 19;acssynbio.1c00359. Available from https://pubs.acs.org/doi/10.1021/acssynbio.1c00359. doi: 10.1021/acssynbio.1c00359
 2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
```

### Comparing `pssm-promoter-tool-1.0.4/README.md` & `pssm-promoter-tool-1.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ```
 
 2. Download and unpack the archive with files using "Code"->"Download ZIP" buttons in the right corner at https://github.com/ellinium/pssm_promoter_tool. 
 Or use
 ```
 git clone https://github.com/ellinium/pssm-promoter-tool
 ```
-
+[! you need to have a Git account and be authorised in the system to run the command !]
 
 
 USAGE:
 
 The tool requires a text or fasta file with a nucleotide sequence of a gene to process.
 From the folder with the downloaded files run:
 ```
@@ -35,41 +35,42 @@
 Depending on the result, up to four output CSV files can be generated:
 1) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
 2) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
 3) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
 4) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
-1) new_sequence - contains a gene sequence (nt) with substituted promoters. Empty for the original promoters.
-2) promoter_sequence - contains -35 motif, spacer and - 10 motif
-3) TSS -  transcriptional start site
-4) Tx_rate - transcription initiation rate
-5) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
-6) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
-7) hex35 -  an upstream 6-nucleotide site called the −35 motif 
-8) PSSM_hex35 - position-specific scoring matrix value for the -35 motif \
-9) AA_hex35 - an amino acid sequence for the -35 motif 
-10) spacer - a spacer region that separates the −10 and −35 motifs 
-11) hex10 - a downstream 6-nucleotide site called the −10 motif 
-12) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
-13) AA_hex10 - an amino acid sequence for the -10 motif 
-14) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
-15) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
-16) dG_total - total Gibbs free energy for the sequence 
-17) dG_10 - -10 motif Gibbs free energy 
-18) dG_35 - -35 motif Gibbs free energy 
-19) dG_disc - a discriminator Gibbs free energy 
-20) dG_ITR - an ITR Gibbs free energy 
-21) dG_ext10 −10 extended motif Gibbs free energy 
-22) dG_spacer - a spacer Gibbs free energy 
-23) dG_UP - an UP Gibbs free energy 
-24) dG_bind - binding Gibbs free energy 
-25) UP_position - a position of the UP element 
-26) hex35_position - a position of the -35 motif 
-27) spacer_position - a position of the spacer 
-28) hex10_position - a position of the -10 motif 
-29) disc_position - a position of the discriminator
+1) Type - 'Original Promoter' - for original sequence promoters; 'Modified Promoter' - for synonymous promoters. 
+2) TSS -  transcriptional start site 
+3) Tx_rate - transcription initiation rate 
+4) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers 
+5) hex35 -  an upstream 6-nucleotide site called the −35 motif 
+6) PSSM_hex35 - position-specific scoring matrix value for the -35 motif 
+7) AA_hex35 - an amino acid sequence for the -35 motif 
+8) hex10 - a downstream 6-nucleotide site called the −10 motif 
+9) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
+10) AA_hex10 - an amino acid sequence for the -10 motif 
+11) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
+12) spacer - a spacer region that separates the −10 and −35 motifs 
+13) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
+14) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
+15) new_gene_sequence - contains a gene sequence (nt) with substituted (Type = 'Modified Promoter') or  original promoters (Type = 'Original Promoter')
+16) promoter_sequence - contains -35 motif, spacer and - 10 motif 
+17) dG_total - total Gibbs free energy for the sequence 
+18) dG_10 - -10 motif Gibbs free energy 
+19) dG_35 - -35 motif Gibbs free energy 
+20) dG_disc - a discriminator Gibbs free energy 
+21) dG_ITR - an ITR Gibbs free energy 
+22) dG_ext10 −10 extended motif Gibbs free energy 
+23) dG_spacer - a spacer Gibbs free energy 
+24) dG_UP - an UP Gibbs free energy 
+25) dG_bind - binding Gibbs free energy 
+26) UP_position - a position of the UP element 
+27) hex35_position - a position of the -35 motif 
+28) spacer_position - a position of the spacer 
+29) hex10_position - a position of the -10 motif 
+30) disc_position - a position of the discriminator
 
 References:
 
 1. Logel DY, Trofimova E, Jaschke PR. Codon-Restrained Method for Both Eliminating and Creating Intragenic Bacterial Promoters. ACS Synth Biol. 2022 Jan 19;acssynbio.1c00359. Available from https://pubs.acs.org/doi/10.1021/acssynbio.1c00359. doi: 10.1021/acssynbio.1c00359
 2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
```

### Comparing `pssm-promoter-tool-1.0.4/free_energy_coeffs.npy` & `pssm-promoter-tool-1.0.5/free_energy_coeffs.npy`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.4/pssm_promoter_calculator.py` & `pssm-promoter-tool-1.0.5/pssm_promoter_calculator.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 #For colab
 #from google.colab import files
 ##sys.path.append(os.path.abspath('PSSM_PromoterTool/'))
 import pssm_util
 
 OUTPUT_FILE_NAME = "PSSMPromoterCalculator"
-
+USE_PROMOTERS_OUTPUT = "using the synonymous promoters "
 def get_gene_sequence():
     gene_sequence = ""
     if len(sys.argv) < 2:
         raise Exception('Please provide a file name with a gene sequence.')
 
     gene_file_name = sys.argv[1]
 
@@ -55,16 +55,18 @@
     fwd_TSS_df, rev_TSS_df = calc.output()
     end_time = datetime.now()
     ##print('Duration of 1 salis calc run: {}'.format(end_time - start_time))
 
     #fwd_TSS_df = TSS_results_to_df(output['Forward_Predictions_per_TSS'])
     #rev_TSS_df = TSS_results_to_df(output['Reverse_Predictions_per_TSS'])
 
-    fwd_TSS_df = fwd_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer', 'ITR'], keep='last')
-    rev_TSS_df = rev_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer', 'ITR'], keep='last')
+    ##fwd_TSS_df = fwd_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer', 'ITR'], keep='last')
+    fwd_TSS_df = fwd_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer'], keep='last')
+    ##rev_TSS_df = rev_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer', 'ITR'], keep='last')
+    rev_TSS_df = rev_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer'], keep='last')
 
     fwd_TSS_df = fwd_TSS_df.sort_values(by = 'Tx_rate', ascending = False)
     rev_TSS_df = rev_TSS_df.sort_values(by = 'Tx_rate', ascending = False)
 
     fwd_TSS_df['AA_Promoter_35'] = fwd_TSS_df['hex35'].apply(lambda x: str(Seq(x).translate()))
     fwd_TSS_df = fwd_TSS_df[fwd_TSS_df['AA_Promoter_35'].str.contains('*', regex = False) == False]
 
@@ -73,29 +75,31 @@
 
     rev_TSS_df['AA_Promoter_35'] = rev_TSS_df['hex35'].apply(lambda x: str(Seq(x).translate()))
     rev_TSS_df = rev_TSS_df[rev_TSS_df['AA_Promoter_35'].str.contains('*', regex = False) == False]
 
     rev_TSS_df['AA_Promoter_10'] = rev_TSS_df['hex10'].apply(lambda x: str(Seq(x).translate()))
     rev_TSS_df = rev_TSS_df[rev_TSS_df['AA_Promoter_10'].str.contains('*', regex = False) == False]
 
-    #TOP 5 Tx_rate revords
-    max_fwd_TSS_df = fwd_TSS_df.head(1)
-    def_fwd_max_tx_rate = max_fwd_TSS_df['Tx_rate'].values[0]
-
-    min_fwd_TSS_df = fwd_TSS_df.tail(1)
+    #TOP 5 Tx_rate records / Top1
+    #minimise max values
+    #maximise min values
+    min_fwd_TSS_df = fwd_TSS_df.head(1)
     def_fwd_min_tx_rate = min_fwd_TSS_df['Tx_rate'].values[0]
 
+    max_fwd_TSS_df = fwd_TSS_df.tail(1)
+    def_fwd_max_tx_rate = max_fwd_TSS_df['Tx_rate'].values[0]
 
-    max_rev_TSS_df = rev_TSS_df.head(1)
-    def_rev_max_tx_rate = max_rev_TSS_df['Tx_rate'].values[0]
 
-    min_rev_TSS_df = rev_TSS_df.tail(1)
+    min_rev_TSS_df = rev_TSS_df.head(1)
     def_rev_min_tx_rate = min_rev_TSS_df['Tx_rate'].values[0]
 
-    max_min_tx_rate_df = {"sequence": sequence, "max_fwd": def_fwd_max_tx_rate, "max_rev": def_rev_max_tx_rate, "min_fwd": def_fwd_min_tx_rate, "min_rev": def_rev_min_tx_rate}
+    max_rev_TSS_df = rev_TSS_df.tail(1)
+    def_rev_max_tx_rate = max_rev_TSS_df['Tx_rate'].values[0]
+
+    max_min_tx_rate_df = {"sequence": sequence, "sequence_compl": str(Seq(sequence).reverse_complement()), "max_fwd": def_fwd_max_tx_rate, "max_rev": def_rev_max_tx_rate, "min_fwd": def_fwd_min_tx_rate, "min_rev": def_rev_min_tx_rate}
 
     # for (TSS, result) in output['Forward_Predictions_per_TSS'].items():
     #     print("Fwd TSS: %s. TX Rate: %s. Calcs: %s" % (TSS, result['Tx_rate'], str(result) ))
     #     process_TSS_results(TSS, result)
     #
     # for (TSS, result) in output['Reverse_Predictions_per_TSS'].items():
     #     print("Rev TSS: %s. TX Rate: %s. Calcs: %s" % (TSS, result['Tx_rate'], str(result) ))
@@ -103,141 +107,161 @@
     # print("Elapsed Time: ", time.time() - begin, " seconds.")
 
 
     #prm_df = process_promoters_nt(promoters_35, promoters_10, spacers)
 
 
 
+    #processes 10 records to maximise and 10 to minimise
+    #IF PRIMERS ARE DUPLICATED TAKE ONLY with higher/lower tx rate
 
-    fwd_res_df_max = pssm_util.process_df_promoters(fwd_TSS_df.head(10), 'fwd', 'max', max_min_tx_rate_df)
+    fwd_res_df_max = pssm_util.process_df_promoters(fwd_TSS_df.tail(10), 'fwd', 'max', max_min_tx_rate_df)
     #fwd_res_df_max = pssm_util.process_df_promoters(fwd_TSS_df, 'fwd', 'max', max_min_tx_rate_df)
-    rev_res_df_max = pssm_util.process_df_promoters(rev_TSS_df.head(10), 'rev', 'max', max_min_tx_rate_df)
+    rev_res_df_max = pssm_util.process_df_promoters(rev_TSS_df.tail(12), 'rev', 'max', max_min_tx_rate_df)
     #rev_res_df_max = pssm_util.process_df_promoters(rev_TSS_df, 'rev', 'max', max_min_tx_rate_df)
 
-    fwd_res_df_min = pssm_util.process_df_promoters(fwd_TSS_df.tail(10), 'fwd', 'min', max_min_tx_rate_df)
+    fwd_res_df_min = pssm_util.process_df_promoters(fwd_TSS_df.head(10), 'fwd', 'min', max_min_tx_rate_df)
     #fwd_res_df_min = pssm_util.process_df_promoters(fwd_TSS_df, 'fwd', 'min', max_min_tx_rate_df)
-    rev_res_df_min = pssm_util.process_df_promoters(rev_TSS_df.tail(10), 'rev', 'min', max_min_tx_rate_df)
+    rev_res_df_min = pssm_util.process_df_promoters(rev_TSS_df.head(10), 'rev', 'min', max_min_tx_rate_df)
     #rev_res_df_min = pssm_util.process_df_promoters(rev_TSS_df, 'rev', 'min', max_min_tx_rate_df)
 
 
     #TODO:  keep original_TSS
-    max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float) >= float(def_fwd_max_tx_rate)]
-    max_rev_TSS_df = rev_res_df_max.loc[rev_res_df_max['Tx_rate'].astype(float) >= float(def_rev_max_tx_rate)]
+    #max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float) >= float(def_fwd_max_tx_rate)]
+##    max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float) >= float(def_fwd_max_tx_rate)]
+    #max_rev_TSS_df = rev_res_df_max.loc[rev_res_df_max['Tx_rate'].astype(float) >= float(def_rev_max_tx_rate)]
+##    max_rev_TSS_df = rev_res_df_max.loc[rev_res_df_max['Tx_rate'].astype(float) >= float(def_rev_max_tx_rate)]
+
+    #min_fwd_TSS_df = fwd_res_df_min.loc[fwd_res_df_min['Tx_rate'].astype(float) <= float(def_fwd_min_tx_rate)]
+##    min_fwd_TSS_df = fwd_res_df_min.loc[fwd_res_df_min['Tx_rate'].astype(float) <= float(def_fwd_min_tx_rate)]
+    #min_rev_TSS_df = rev_res_df_min.loc[rev_res_df_min['Tx_rate'].astype(float) <= float(def_rev_min_tx_rate)]
+##    min_rev_TSS_df = rev_res_df_min.loc[rev_res_df_min['Tx_rate'].astype(float) <= float(def_rev_min_tx_rate)]
+
+    #res_final_df_max = pd.concat([max_fwd_TSS_df, max_rev_TSS_df], ignore_index=True, sort=False)
+    res_final_df_max = pd.concat([fwd_res_df_max, rev_res_df_max], ignore_index=True, sort=False)
 
-    min_fwd_TSS_df = fwd_res_df_min.loc[fwd_res_df_min['Tx_rate'].astype(float) <= float(def_fwd_min_tx_rate)]
-    min_rev_TSS_df = rev_res_df_min.loc[rev_res_df_min['Tx_rate'].astype(float) <= float(def_rev_min_tx_rate)]
+    #res_final_df_min = pd.concat([min_fwd_TSS_df, min_rev_TSS_df], ignore_index=True, sort=False)
+    res_final_df_min = pd.concat([fwd_res_df_min, rev_res_df_min], ignore_index=True, sort=False)
 
-    res_final_df_max = pd.concat([max_fwd_TSS_df, max_rev_TSS_df], ignore_index=True, sort=False)
-    res_final_df_min = pd.concat([min_fwd_TSS_df, min_rev_TSS_df], ignore_index=True, sort=False)
     #res_final_df = res_final_df.drop_duplicates()
     res_final_df_max = res_final_df_max.drop_duplicates(
-        subset=['hex35', 'hex10', 'Tx_rate', 'ITR', 'original_record', 'direction'],
+        subset=['hex35', 'hex10', 'Tx_rate', 'ITR', 'Type', 'direction'],
         keep='last').reset_index(drop=True)
 
 
     res_final_df_min = res_final_df_min.drop_duplicates(
-        subset=['hex35', 'hex10', 'Tx_rate', 'ITR', 'original_record', 'direction'],
+        subset=['hex35', 'hex10', 'Tx_rate', 'ITR', 'Type', 'direction'],
         keep='last').reset_index(drop=True)
 
     res_final_df_max['AA_hex35'] = res_final_df_max['hex35'].apply(lambda x: str(Seq(x).translate()))
     res_final_df_min['AA_hex35'] = res_final_df_min['hex35'].apply(lambda x: str(Seq(x).translate()))
     res_final_df_max['AA_hex10'] = res_final_df_max['hex10'].apply(lambda x: str(Seq(x).translate()))
     res_final_df_min['AA_hex10'] = res_final_df_min['hex10'].apply(lambda x: str(Seq(x).translate()))
 
     #+PSSM values
     res_final_df_max['PSSM_hex35'] = res_final_df_max['hex35'].apply(lambda x: pssm_util.calc_PSSM(x, '35'))
-    res_final_df_max['PSSM_hex10'] = res_final_df_max['hex35'].apply(lambda x: pssm_util.calc_PSSM(x, '10'))
-    res_final_df_min['PSSM_hex35'] = res_final_df_max['hex10'].apply(lambda x: pssm_util.calc_PSSM(x, '35'))
+    res_final_df_max['PSSM_hex10'] = res_final_df_max['hex10'].apply(lambda x: pssm_util.calc_PSSM(x, '10'))
+    res_final_df_min['PSSM_hex35'] = res_final_df_max['hex35'].apply(lambda x: pssm_util.calc_PSSM(x, '35'))
     res_final_df_min['PSSM_hex10'] = res_final_df_max['hex10'].apply(lambda x: pssm_util.calc_PSSM(x, '10'))
 
     #perm_prom_pssm_df['PSSM_Promoters_perm'] = perm_prom_pssm_df['Promoters_perm_nt'].apply(lambda x: calc_PSSM(x, type))
 
     #res_final_df_max.to_csv('SalisLogelPromoterCalculator_MAX_results.csv')
     #res_final_df_min.to_csv('SalisLogelPromoterCalculator_MIN_results.csv')
 
     print(sequence)
 
     res_final_df_max_fwd_df = res_final_df_max.loc[res_final_df_max["direction"] == 'fwd']
     new_max_fwd_Tx_rate_df = res_final_df_max_fwd_df.sort_values(by='Tx_rate', ascending=False)
-    new_max_fwd_Tx_rate = new_max_fwd_Tx_rate_df['Tx_rate'].head(1).values[0]
+    new_min_max_fwd_Tx_rate = new_max_fwd_Tx_rate_df['Tx_rate'].tail(1).values[0]
+    new_max_max_fwd_Tx_rate = new_max_fwd_Tx_rate_df['Tx_rate'].head(1).values[0]
 
 
     res_final_df_min_fwd_df = res_final_df_min.loc[res_final_df_min["direction"] == 'fwd']
     new_min_fwd_Tx_rate_df = res_final_df_min_fwd_df.sort_values(by='Tx_rate', ascending=False)
-    new_min_fwd_Tx_rate = new_min_fwd_Tx_rate_df['Tx_rate'].tail(1).values[0]
+    new_max_min_fwd_Tx_rate = new_min_fwd_Tx_rate_df['Tx_rate'].head(1).values[0]
+    new_min_min_fwd_Tx_rate = new_min_fwd_Tx_rate_df['Tx_rate'].tail(1).values[0]
+    #new_min_fwd_Tx_rate = new_min_fwd_Tx_rate_df['Tx_rate'].head(1).values[0]
 
 
     res_final_df_max_rev_df = res_final_df_max.loc[res_final_df_max["direction"] == 'rev']
     new_max_rev_Tx_rate_df = res_final_df_max_rev_df.sort_values(by='Tx_rate', ascending=False)
-    new_max_rev_Tx_rate = new_max_rev_Tx_rate_df['Tx_rate'].head(1).values[0]
+    new_max_max_rev_Tx_rate = new_max_rev_Tx_rate_df['Tx_rate'].head(1).values[0]
+    new_min_max_rev_Tx_rate = new_max_rev_Tx_rate_df['Tx_rate'].tail(1).values[0]
 
     res_final_df_min_rev_df = res_final_df_min.loc[res_final_df_min["direction"] == 'rev']
     new_min_rev_Tx_rate_df = res_final_df_min_rev_df.sort_values(by='Tx_rate', ascending=False)
-    new_min_rev_Tx_rate = new_min_rev_Tx_rate_df['Tx_rate'].tail(1).values[0]
+    new_max_min_rev_Tx_rate = new_min_rev_Tx_rate_df['Tx_rate'].head(1).values[0]
+    new_min_min_rev_Tx_rate = new_min_rev_Tx_rate_df['Tx_rate'].tail(1).values[0]
 
-    column_list = ["new_gene_sequence", "promoter_sequence", "TSS", "Tx_rate", "Tx_rate_FoldChange", "UP", "hex35", "PSSM_hex35", "AA_hex35", "spacer", "hex10", "PSSM_hex10", "AA_hex10", "disc", "ITR", "dG_total", "dG_10", "dG_35", "dG_disc", "dG_ITR", "dG_ext10", "dG_spacer", "dG_UP", "dG_bind",  "UP_position", "hex35_position", "spacer_position", "hex10_position", "disc_position"]
+    column_list =  ["Type", "TSS", "Tx_rate", "Tx_rate_FoldChange", "hex35", "PSSM_hex35", "AA_hex35", "hex10", "PSSM_hex10", "AA_hex10", "UP", "spacer", "disc", "ITR", "new_gene_sequence", "promoter_sequence", "dG_total", "dG_10", "dG_35", "dG_disc", "dG_ITR", "dG_ext10", "dG_spacer", "dG_UP", "dG_bind",  "UP_position", "hex35_position", "spacer_position", "hex10_position", "disc_position"]
 
     ##max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float)
     ##max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float) >= float(def_fwd_max_tx_rate)]
 
-    print("\n")
-    print("The minimum transcription rate for the sequence (forward) is " + str(def_fwd_min_tx_rate))
+    print("\nThe maximum transcription rate for the sequence (forward) is " + str(new_max_min_fwd_Tx_rate))
     if len(res_final_df_min_fwd_df) > 1:
         min_fwd_output_file = OUTPUT_FILE_NAME + "_MIN_FWD_results.csv"
-        if float(new_min_fwd_Tx_rate) < float(def_fwd_min_tx_rate):
-            print ("can be decreased up to " + str(new_min_fwd_Tx_rate))
-            print("using the promoters in the " + min_fwd_output_file)
+        #if float(new_min_fwd_Tx_rate) < float(def_fwd_min_tx_rate):
+        if float(new_min_min_fwd_Tx_rate) < float(new_max_min_fwd_Tx_rate):
+            print ("can be decreased up to " + str(new_min_min_fwd_Tx_rate))
+            print(USE_PROMOTERS_OUTPUT + "(" + min_fwd_output_file + ")")
             #res_final_df_min_fwd_df['Tx_rate_FoldChange'] = res_final_df_min_fwd_df['Tx_rate'].copy()/def_fwd_min_tx_rate.astype(float)
-            res_final_df_min_fwd_df = pssm_util.add_txrate_foldchange_col(res_final_df_min_fwd_df,def_fwd_min_tx_rate)
+            res_final_df_min_fwd_df = pssm_util.add_txrate_foldchange_col(res_final_df_min_fwd_df, 'min')
             res_final_df_min_fwd_df.to_csv(min_fwd_output_file, columns = column_list, float_format='%.2f')
 
             ##files.download(min_fwd_output_file)
 
     else:
         print(" cannot be further decreased")
 
-    print("\n")
-    print("The minimum transcription rate for the sequence (reverse) is " + str(def_rev_min_tx_rate))
+    print("\nThe maximum transcription rate for the sequence (reverse) is " + str(new_max_min_rev_Tx_rate))
     if len(res_final_df_min_rev_df) > 1:
         min_rev_output_file = OUTPUT_FILE_NAME + "_MIN_REV_results.csv"
-        if float(new_min_rev_Tx_rate) < float(def_rev_min_tx_rate):
-            print ("can be decreased up to " + str(new_min_rev_Tx_rate))
-            print("using the promoters in the " + min_rev_output_file)
-            res_final_df_min_rev_df = pssm_util.add_txrate_foldchange_col(res_final_df_min_rev_df,def_rev_min_tx_rate)
+        #if float(new_min_rev_Tx_rate) < float(def_rev_min_tx_rate):
+        if float(new_min_min_rev_Tx_rate) < float(new_max_min_rev_Tx_rate):
+            print ("can be decreased up to " + str(new_min_min_rev_Tx_rate))
+            print(USE_PROMOTERS_OUTPUT + "(" + min_rev_output_file + ")")
+            res_final_df_min_rev_df = pssm_util.add_txrate_foldchange_col(res_final_df_min_rev_df, 'min')
             res_final_df_min_rev_df.to_csv(min_rev_output_file, columns = column_list, float_format='%.2f')
 
             ##files.download(min_rev_output_file)
 
     else:
         print(" cannot be further decreased")
 
-    print("\n")
-    print("The maximum transcription rate for the sequence (forward) is " + str(def_fwd_max_tx_rate))
+    print("\nThe minimum transcription rate for the sequence (forward) is " + str(new_min_max_fwd_Tx_rate))
     if len(res_final_df_max_fwd_df) > 1:
         max_fwd_output_file = OUTPUT_FILE_NAME + "_MAX_FWD_results.csv"
-        if float(new_max_fwd_Tx_rate) > float(def_fwd_max_tx_rate):
-            print ("can be increased up to " + str(new_max_fwd_Tx_rate))
-            print("using the promoters in the " + max_fwd_output_file)
-            res_final_df_max_fwd_df = pssm_util.add_txrate_foldchange_col(res_final_df_max_fwd_df,def_fwd_max_tx_rate)
+        #if float(new_max_fwd_Tx_rate) > float(def_fwd_max_tx_rate):
+        if float(new_max_max_fwd_Tx_rate) > float(new_min_max_fwd_Tx_rate):
+            print ("can be increased up to " + str(new_max_max_fwd_Tx_rate))
+            print(USE_PROMOTERS_OUTPUT + "(" + max_fwd_output_file + ")")
+            res_final_df_max_fwd_df = pssm_util.add_txrate_foldchange_col(res_final_df_max_fwd_df, 'max')
 
             res_final_df_max_fwd_df.to_csv(max_fwd_output_file, columns = column_list, float_format='%.2f')
             ##files.download(max_fwd_output_file)
-
     else:
         print(" cannot be further increased")
-    print("\n")
-    print("The maximum transcription rate for the sequence (reverse) is " + str(def_rev_max_tx_rate))
+
+    print("\nThe minimum transcription rate for the sequence (reverse) is " + str(new_min_max_rev_Tx_rate))
     if len(res_final_df_max_rev_df) > 1:
         max_rev_output_file = OUTPUT_FILE_NAME + "_MAX_REV_results.csv"
-        if float(new_max_rev_Tx_rate) > float(def_rev_max_tx_rate):
-            print ("can be increased up to " + str(new_max_rev_Tx_rate))
-            print("using the promoters in the " + max_rev_output_file)
-            res_final_df_max_rev_df = pssm_util.add_txrate_foldchange_col(res_final_df_max_rev_df,def_rev_max_tx_rate)
+        #if float(new_max_rev_Tx_rate) > float(def_rev_max_tx_rate):
+        if float(new_max_max_rev_Tx_rate) > float(new_min_max_rev_Tx_rate):
+            print ("can be increased up to " + str(new_max_max_rev_Tx_rate))
+            print(USE_PROMOTERS_OUTPUT + "(" + max_rev_output_file + ")")
+            res_final_df_max_rev_df = pssm_util.add_txrate_foldchange_col(res_final_df_max_rev_df, 'max')
 
             res_final_df_max_rev_df.to_csv(max_rev_output_file, columns = column_list, float_format='%.2f')
             ##files.download(max_rev_output_file)
 
     else:
         print(" cannot be further increased")
 
+    print("\n")
+
+    print("\n")
+
+
     end_time = datetime.now()
     print('Duration: {}'.format(end_time - start_time))
```

### Comparing `pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/PKG-INFO` & `pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssm-promoter-tool
-Version: 1.0.4
+Version: 1.0.5
 Summary: The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence
 Home-page: https://github.com/ellinium/PSSM_PromoterTool
 Author: Ellina Trofimova
 Author-email: ellina.trofimova@gmail.com
 License: GNU General Public License
 Keywords: promoter prediction transcription rate
 Description-Content-Type: text/markdown
@@ -28,15 +28,15 @@
 ```
 
 2. Download and unpack the archive with files using "Code"->"Download ZIP" buttons in the right corner at https://github.com/ellinium/pssm_promoter_tool. 
 Or use
 ```
 git clone https://github.com/ellinium/pssm-promoter-tool
 ```
-
+[! you need to have a Git account and be authorised in the system to run the command !]
 
 
 USAGE:
 
 The tool requires a text or fasta file with a nucleotide sequence of a gene to process.
 From the folder with the downloaded files run:
 ```
@@ -47,41 +47,42 @@
 Depending on the result, up to four output CSV files can be generated:
 1) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
 2) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
 3) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
 4) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
-1) new_sequence - contains a gene sequence (nt) with substituted promoters. Empty for the original promoters.
-2) promoter_sequence - contains -35 motif, spacer and - 10 motif
-3) TSS -  transcriptional start site
-4) Tx_rate - transcription initiation rate
-5) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
-6) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
-7) hex35 -  an upstream 6-nucleotide site called the −35 motif 
-8) PSSM_hex35 - position-specific scoring matrix value for the -35 motif \
-9) AA_hex35 - an amino acid sequence for the -35 motif 
-10) spacer - a spacer region that separates the −10 and −35 motifs 
-11) hex10 - a downstream 6-nucleotide site called the −10 motif 
-12) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
-13) AA_hex10 - an amino acid sequence for the -10 motif 
-14) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
-15) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
-16) dG_total - total Gibbs free energy for the sequence 
-17) dG_10 - -10 motif Gibbs free energy 
-18) dG_35 - -35 motif Gibbs free energy 
-19) dG_disc - a discriminator Gibbs free energy 
-20) dG_ITR - an ITR Gibbs free energy 
-21) dG_ext10 −10 extended motif Gibbs free energy 
-22) dG_spacer - a spacer Gibbs free energy 
-23) dG_UP - an UP Gibbs free energy 
-24) dG_bind - binding Gibbs free energy 
-25) UP_position - a position of the UP element 
-26) hex35_position - a position of the -35 motif 
-27) spacer_position - a position of the spacer 
-28) hex10_position - a position of the -10 motif 
-29) disc_position - a position of the discriminator
+1) Type - 'Original Promoter' - for original sequence promoters; 'Modified Promoter' - for synonymous promoters. 
+2) TSS -  transcriptional start site 
+3) Tx_rate - transcription initiation rate 
+4) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers 
+5) hex35 -  an upstream 6-nucleotide site called the −35 motif 
+6) PSSM_hex35 - position-specific scoring matrix value for the -35 motif 
+7) AA_hex35 - an amino acid sequence for the -35 motif 
+8) hex10 - a downstream 6-nucleotide site called the −10 motif 
+9) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
+10) AA_hex10 - an amino acid sequence for the -10 motif 
+11) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
+12) spacer - a spacer region that separates the −10 and −35 motifs 
+13) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
+14) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
+15) new_gene_sequence - contains a gene sequence (nt) with substituted (Type = 'Modified Promoter') or  original promoters (Type = 'Original Promoter')
+16) promoter_sequence - contains -35 motif, spacer and - 10 motif 
+17) dG_total - total Gibbs free energy for the sequence 
+18) dG_10 - -10 motif Gibbs free energy 
+19) dG_35 - -35 motif Gibbs free energy 
+20) dG_disc - a discriminator Gibbs free energy 
+21) dG_ITR - an ITR Gibbs free energy 
+22) dG_ext10 −10 extended motif Gibbs free energy 
+23) dG_spacer - a spacer Gibbs free energy 
+24) dG_UP - an UP Gibbs free energy 
+25) dG_bind - binding Gibbs free energy 
+26) UP_position - a position of the UP element 
+27) hex35_position - a position of the -35 motif 
+28) spacer_position - a position of the spacer 
+29) hex10_position - a position of the -10 motif 
+30) disc_position - a position of the discriminator
 
 References:
 
 1. Logel DY, Trofimova E, Jaschke PR. Codon-Restrained Method for Both Eliminating and Creating Intragenic Bacterial Promoters. ACS Synth Biol. 2022 Jan 19;acssynbio.1c00359. Available from https://pubs.acs.org/doi/10.1021/acssynbio.1c00359. doi: 10.1021/acssynbio.1c00359
 2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
```

### Comparing `pssm-promoter-tool-1.0.4/setup.py` & `pssm-promoter-tool-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='pssm-promoter-tool',
-      version='1.0.4',
+      version='1.0.5',
       description='The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ellinium/PSSM_PromoterTool',
       author='Ellina Trofimova',
       author_email='ellina.trofimova@gmail.com',
       license='GNU General Public License',
```

