# Comparing `tmp/Pras_Server-1.1.14.tar.gz` & `tmp/Pras_Server-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pras_Server-1.1.14.tar", last modified: Mon Apr 17 12:27:15 2023, max compression
+gzip compressed data, was "Pras_Server-1.2.0.tar", last modified: Mon May 29 06:02:25 2023, max compression
```

## Comparing `Pras_Server-1.1.14.tar` & `Pras_Server-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-04-17 12:27:15.801364 Pras_Server-1.1.14/
--rwxrwxrwx   0 osita     (1000) osita     (1000)     1061 2022-02-07 06:19:51.000000 Pras_Server-1.1.14/LICENSE.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)      130 2022-05-31 15:51:04.000000 Pras_Server-1.1.14/MANIFEST.in
--rwxrwxrwx   0 osita     (1000) osita     (1000)     6966 2023-04-17 12:27:15.800365 Pras_Server-1.1.14/PKG-INFO
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-04-17 12:27:15.731407 Pras_Server-1.1.14/Pras_Server/
--rwxrwxrwx   0 osita     (1000) osita     (1000)    27560 2023-04-16 14:31:54.000000 Pras_Server-1.1.14/Pras_Server/CheckPDBatoms.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     2191 2023-04-16 14:35:22.000000 Pras_Server-1.1.14/Pras_Server/DownloadPDB.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    13029 2023-04-16 14:32:36.000000 Pras_Server-1.1.14/Pras_Server/FixHeavyAtoms.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    10252 2023-04-16 14:35:22.000000 Pras_Server-1.1.14/Pras_Server/ForcefieldParam.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    12821 2023-04-16 14:35:22.000000 Pras_Server-1.1.14/Pras_Server/LinearAlgebra.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    49427 2023-04-16 14:35:22.000000 Pras_Server-1.1.14/Pras_Server/MissingHeavyAtoms.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    50624 2023-04-16 14:35:22.000000 Pras_Server-1.1.14/Pras_Server/MissingHydrogenAtoms.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     5580 2023-04-16 14:35:22.000000 Pras_Server-1.1.14/Pras_Server/PDBID.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    24594 2023-04-16 14:41:58.000000 Pras_Server-1.1.14/Pras_Server/PRAS.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     7565 2023-04-16 14:35:22.000000 Pras_Server-1.1.14/Pras_Server/PotentialEnergy.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     7156 2023-04-16 14:33:02.000000 Pras_Server-1.1.14/Pras_Server/RamaChandra.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    10844 2023-04-16 14:32:06.000000 Pras_Server-1.1.14/Pras_Server/ReadMaster.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    18051 2023-04-16 14:35:22.000000 Pras_Server-1.1.14/Pras_Server/ReadStructure.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    11886 2023-04-16 14:33:34.000000 Pras_Server-1.1.14/Pras_Server/ReadmmCIF.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     9419 2023-04-17 12:15:34.000000 Pras_Server-1.1.14/Pras_Server/RunType.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    12032 2023-04-16 14:32:00.000000 Pras_Server-1.1.14/Pras_Server/SecondaryStructure.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)        0 2022-07-24 19:07:18.000000 Pras_Server-1.1.14/Pras_Server/__init__.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)        6 2023-04-16 12:59:22.000000 Pras_Server-1.1.14/Pras_Server/_version.py
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-04-17 12:27:15.764386 Pras_Server-1.1.14/Pras_Server/data/
--rwxrwxrwx   0 osita     (1000) osita     (1000)    80000 2022-05-03 08:43:46.000000 Pras_Server-1.1.14/Pras_Server/data/KD.dat
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-04-17 12:27:15.795367 Pras_Server-1.1.14/Pras_Server/run_PRAS_with_FASPR/
--rwxrwxrwx   0 osita     (1000) osita     (1000)   109350 2022-05-09 13:30:38.000000 Pras_Server-1.1.14/Pras_Server/run_PRAS_with_FASPR/1aho.pdb
--rwxrwxrwx   0 osita     (1000) osita     (1000)   246708 2023-04-17 12:22:32.000000 Pras_Server-1.1.14/Pras_Server/run_PRAS_with_FASPR/PRAS_with_FASPR.pdf
--rwxrwxrwx   0 osita     (1000) osita     (1000)      827 2023-04-17 12:10:33.000000 Pras_Server-1.1.14/Pras_Server/run_PRAS_with_FASPR/linux_example.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     1146 2023-04-17 12:20:37.000000 Pras_Server-1.1.14/Pras_Server/run_PRAS_with_FASPR/syntax.txt
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-04-17 12:27:15.759389 Pras_Server-1.1.14/Pras_Server.egg-info/
--rwxrwxrwx   0 osita     (1000) osita     (1000)     6966 2023-04-17 12:27:15.000000 Pras_Server-1.1.14/Pras_Server.egg-info/PKG-INFO
--rwxrwxrwx   0 osita     (1000) osita     (1000)      923 2023-04-17 12:27:15.000000 Pras_Server-1.1.14/Pras_Server.egg-info/SOURCES.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)        1 2023-04-17 12:27:15.000000 Pras_Server-1.1.14/Pras_Server.egg-info/dependency_links.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)       28 2023-04-17 12:27:15.000000 Pras_Server-1.1.14/Pras_Server.egg-info/requires.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)       12 2023-04-17 12:27:15.000000 Pras_Server-1.1.14/Pras_Server.egg-info/top_level.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)     6516 2023-04-17 12:18:22.000000 Pras_Server-1.1.14/README.md
--rwxrwxrwx   0 osita     (1000) osita     (1000)       38 2023-04-17 12:27:15.802363 Pras_Server-1.1.14/setup.cfg
--rwxrwxrwx   0 osita     (1000) osita     (1000)      884 2023-04-17 11:22:31.000000 Pras_Server-1.1.14/setup.py
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.836248 Pras_Server-1.2.0/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     1061 2022-02-07 06:19:51.000000 Pras_Server-1.2.0/LICENSE.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)      130 2022-05-31 15:51:04.000000 Pras_Server-1.2.0/MANIFEST.in
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7693 2023-05-29 06:02:25.834250 Pras_Server-1.2.0/PKG-INFO
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.742308 Pras_Server-1.2.0/Pras_Server/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    27558 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/CheckPDBatoms.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     2191 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/DownloadPDB.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    13028 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/FixHeavyAtoms.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    10251 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/ForcefieldParam.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    12820 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/LinearAlgebra.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    49426 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/MissingHeavyAtoms.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    50569 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/MissingHydrogenAtoms.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     5579 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/PDBID.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    24667 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/PRAS.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7564 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/PotentialEnergy.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7155 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/RamaChandra.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    10843 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/ReadMaster.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    18050 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/ReadStructure.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    11885 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/ReadmmCIF.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    10006 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/RunType.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    12032 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/SecondaryStructure.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/__init__.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)        6 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/_version.py
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.800271 Pras_Server-1.2.0/Pras_Server/data/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    80000 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/data/KD.dat
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.829254 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)   109350 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/1aho.pdb
+-rwxrwxrwx   0 osita     (1000) osita     (1000)   246721 2023-05-29 05:44:59.000000 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/PRAS_with_FASPR.pdf
+-rwxrwxrwx   0 osita     (1000) osita     (1000)      834 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/linux_example.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     1177 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/syntax.txt
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.795275 Pras_Server-1.2.0/Pras_Server.egg-info/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7693 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/PKG-INFO
+-rwxrwxrwx   0 osita     (1000) osita     (1000)      923 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/SOURCES.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)        1 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/dependency_links.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)       28 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/requires.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)       12 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/top_level.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7244 2023-05-29 05:50:15.000000 Pras_Server-1.2.0/README.md
+-rwxrwxrwx   0 osita     (1000) osita     (1000)       38 2023-05-29 06:02:25.836248 Pras_Server-1.2.0/setup.cfg
+-rwxrwxrwx   0 osita     (1000) osita     (1000)      883 2023-05-29 06:02:05.000000 Pras_Server-1.2.0/setup.py
```

### Comparing `Pras_Server-1.1.14/LICENSE.txt` & `Pras_Server-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Pras_Server-1.1.14/PKG-INFO` & `Pras_Server-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: Pras_Server
-Version: 1.1.14
+Version: 1.2.0
 Summary: A webserver to repair PDB files
 Home-page: https://www.protein-science.com/
 Author: Osita S. Nnyigide
 Author-email: osita@protein-science.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Protein Repair and Analysis (PRAS) Server is a tool to repair PDB or mmCIF structures, add missing heavy atoms and hydrogen atoms and assign secondary structures by amide-amide interactions of the backbone
+Protein Repair and Analysis (PRAS) Server is a tool to repair PDB or mmCIF structures, add missing heavy 
 
-You can use the server online at https://www.protein-science.com/ or on your local machine following the instructions given below
+atoms and hydrogen atoms and assign secondary structures by amide-amide interactions of the backbone
+
+You can use the server online at https://www.protein-science.com/ or on your local machine following the 
+
+instructions given below
 
 The program consists of:
 ```python
 Tools to automatically download PDB or mmCIF structures
 
 Tools to generate different rotamers if present in a PDB or mmCIF structure file
 
@@ -29,15 +33,19 @@
 Tools to assign secondary structure elements by amide-amide interactions of the backbone
 
 Tools to draw 4 Ramachandran types (i.e., general, glycine, proline and pre-proline)
 ```
 
 ## PRAS installation
 
-`pip install Pras-Server==1.0.11`
+On November 20, 2022, a C++ version of the server that is independent of the python counterpart was released. The C++ version is named Pras_Server_C++ and is part of this repository. Both versions produce the same result but the former is 9 to 12 times faster than the latter. To use the C++ version, download this ZIP and extract the Pras_Server_C++ folder and follow the instruction in the INSTALL file included with the distribution.
+
+To use the python distribution on your local machine, use pip as given below or copy Pras_Server folder to any of the directories that Python searches at run-time
+
+`pip install Pras-Server==1.1.0`
 
 ## PRAS usage
 
 A comprehensive test with 82 or 494 PDB or mmCIF structures may be performed to ensure the program works correctly.
 
 Since PRAS can download these structures automatically, 2 lists are provided which contain all the PDB IDs.
 
@@ -50,47 +58,42 @@
 #user's internet download speed
 import time
 from Pras_Server.RunType import InitRunType
 from Pras_Server.PDBID import  _82_pdbs, _494_pdbs
 
 startTime = time.time()
 
-fixing = InitRunType( rotamer="", 
-					mutation="", 
-					pdb_faspr="", 
-					keep_ligand="", 
-					chain_no="",
-					addh = False,
-					ss=False,
-					raman=False,
-					ofname=False,
-					pdbid=_82_pdbs
-					)
+fixing = InitRunType( rotamer="", mutation="", pdb_faspr="", keep_ligand="", chain_no="", 
+		      addh=False, ss=False, raman=False, ofname=False, pdbid=_82_pdbs, his_p=False)
 
 # fixed PDB is saved with name=PDB ID+_out.pdb
 # addh, use default or set to True to add hydrogen
 # pdbid, must be a list of PDB IDs or set to False
 # ss=secondary structure, set to True if you need it
 # raman=ramachandran plot, set to True if you need it
 # rotamer, use default or "yes" to use low occupancy conformers
 # mutation, use default or "yes" to use low occupancy conformers
 # keep_ligand, use default or "yes" to keep non-water ligands
 # chain_no, use default or string number (e.g., "1") to process a specific chain
 # ofname, output file name, use default. To use your own name read documentaion below
-# Execute print(InitRunType.ProcessOther().__doc__) or see RunType.py doc instructions
+# his_p, protonate 20% of HIS. A fraction of HIS may be charged at pH of 7. Use default
 # pdb_faspr, use default or enter a pdb output from faspr, reason is stated in pras paper
+# Execute print(InitRunType.ProcessOther().__doc__) or see RunType.py doc instructions
 
 fixing.ProcessWithoutDefaultUsingPDBID()
 #You can print(InitRunType.ProcessWithoutDefaultUsingPDBID.__doc__) 
 #to learn more about the member function
 print ('The program took {0} second !'.format(time.time() - startTime))
 ```
 
 The above will download and analyze 82 or 494 protein structures. One can modify the code to process either of the lists.
-If you set ss=True and rama=True, you may encounter failed to allocate bitmap error (depending on your computer's memory)
+
+If you set ss=True and rama=True, you may encounter failed to allocate bitmap error (depending on your computer's memory).
+
+Note that the above test will work in both windows and linux systems. For linux you just need to do python3 pras_test.py
 
 For users that do not want to do the above comprehensive test, instructions are given below to process a
 
 single protein structure in a windows or linux environment.
 
 For winddows, download a protein (e.g toxin II, 1aho.pdb, or let PRAS download it automatically)
 
@@ -103,82 +106,66 @@
 
 ```python
 import time
 from Pras_Server.RunType import InitRunType
 
 startTime = time.time()
 
-fixing = InitRunType(rotamer="", 
-					mutation="", 
-					pdb_faspr="", 
-					keep_ligand="", 
-					chain_no="",
-					addh = False,
-					ss=False,
-					raman=False,
-					ofname=False,
-					pdbid=False
-					)
+fixing = InitRunType(rotamer="", mutation="", pdb_faspr="", keep_ligand="", chain_no="", 
+		     addh=False, ss=False, raman=False, ofname=False,pdbid=False, his_p=False)
 
 fixing.fname = '1aho.pdb'
 
 fixing.ProcessWithDefault()
 #You can print(InitRunType.ProcessWithDefault.__doc__) 
 #to learn more about the member function
 print ('The program took {0} second !'.format(time.time() - startTime))
 ```
 
 For linux, do the same as above except for the example code where you should copy the code below (the annotation given above applies below):
 
 ```python
 import sys
 
-if len(sys.argv) == 8:
+if len(sys.argv) == 9:
 	import time
 	from Pras_Server.RunType import InitRunType
 	startTime = time.time()
 
 	rotamer=sys.argv[2] 
 	mutation=sys.argv[3]
 	pdb_faspr=sys.argv[4]
 	keep_ligand=sys.argv[5]
 	chain_no=sys.argv[6] 
 	ofname=sys.argv[7]
-	fixing=InitRunType(
-					rotamer, 
-					mutation, 
-					pdb_faspr, 
-					keep_ligand, 
-					chain_no,
-					addh=False,
-					ss=False,
-					raman=False,
-					ofname=False,
-					pdbid=False
-					)
+	his_p=sys.argv[8]
+	fixing=InitRunType(rotamer, mutation, pdb_faspr, keep_ligand, chain_no, 
+			   addh=False, ss=False, raman=False, ofname=False, pdbid=False, his_p=False)
 	fixing.fname=sys.argv[1]
 	fixing.ProcessWithDefault()
 	print ('The program took {0} second !'.format(time.time() - startTime))
 
 else:
-	print("PRAS takes 8 compulsory arguments." 
+	print("PRAS takes 9 compulsory arguments." 
 		  " Execute the code below on your shell prompt to learn more\n")
 	print("printf \"from Pras_Server.PRAS import" 
 		  " repairPDB\\nprint(repairPDB.__doc__)\\n\\n()\" | python3\n")
 ```
 
 Then, cd to the directory where example.py is located and enter the following argument on your shell prompt:
 
-`python3 example.py 1aho.pdb "" "" "" "" "" ""`
+`python3 example.py 1aho.pdb "" "" "" "" "" "" ""`
 
 
 ## WINDOWS SUBSYSTEM FOR LINUX (WSL)
 
 In order to run Linux GUI applications e.g., the plots for
+
 secondary structure assignment and 4 Ramachandran types
+
 using Windows Subsystem for Linux (WSL), you must install X server for Windows.
 
 Thus, you need to:
 
 Install X server for Windows
 
 Configure bash to tell GUIs to use the local X server
```

### Comparing `Pras_Server-1.1.14/Pras_Server/CheckPDBatoms.py` & `Pras_Server-1.2.0/Pras_Server/CheckPDBatoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
 
@@ -285,15 +285,15 @@
                 ' S.G. Lee, K. Hyun. Protein Repair and Analysis Server: A Web' +'\n'+
                 'Server to Repair PDB Structures, Add Missing Heavy'
                 ' Atoms and Hydrogen Atoms, and Assign Secondary Structures by'
                 ' Amide Interactions. J. Chem. Inf. Model., 2022, 62, 4232–4246.'+'\n')
 
         log.write('#'*183+'\n')
 
-        log.write('PRAS 1.0.11. This is a PRAS-generated log file.'
+        log.write('PRAS 1.2.0. This is a PRAS-generated log file.'
                 ' For your information, all missing or fixed atoms'
                 ' and other relevant information concerning the repair'
                 ' are appended below '+'\n')
 
         log.write('#'*183+'\n\n')
         log.write('This is the log for {}'.format(pdb_pras)+'\n\n')
```

### Comparing `Pras_Server-1.1.14/Pras_Server/DownloadPDB.py` & `Pras_Server-1.2.0/Pras_Server/DownloadPDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
 
@@ -88,8 +88,8 @@
 
     else:
         with gzip.open(f_in, "rb") as gz:
             with open(f_out, "wb") as out:
                 out.writelines(gz)
         os.remove(f_in)
 
-    return
+    return
```

### Comparing `Pras_Server-1.1.14/Pras_Server/FixHeavyAtoms.py` & `Pras_Server-1.2.0/Pras_Server/FixHeavyAtoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/ForcefieldParam.py` & `Pras_Server-1.2.0/Pras_Server/ForcefieldParam.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/LinearAlgebra.py` & `Pras_Server-1.2.0/Pras_Server/LinearAlgebra.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/MissingHeavyAtoms.py` & `Pras_Server-1.2.0/Pras_Server/MissingHeavyAtoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/MissingHydrogenAtoms.py` & `Pras_Server-1.2.0/Pras_Server/MissingHydrogenAtoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
 
@@ -1133,15 +1133,14 @@
     None:   writes to a log.txt file
 
     """
     if resNo[-1].isalpha():
         resNo = resNo[:-1]
     with open('log.txt', 'a') as f:
         f.write('HIS {} in chain {} is protonated (+1 charge)'\
-        '. Comment line 471 in PRAS.py to turn it off'
         ' (ref @ www.protein-science.com)'
         .format(resNo,chainNo)+'\n\n')
 
 def get_hd1(ires):
     """
     This function adds hydrogen atom to ND1 of
     histidine making it to have +1 charge.
@@ -1184,8 +1183,8 @@
         prot = len(his)//5
 
         for i in range(prot):
             res_pos[res_pos.index(num[i])].extend(get_hd1(his[i]))
             atom_name[atom_name.index(name[i])].extend(['HD1'])
             his_note(his[i][0][3:],chainNo+1)
 
-    return [res_pos, atom_name]
+    return [res_pos, atom_name]
```

### Comparing `Pras_Server-1.1.14/Pras_Server/PDBID.py` & `Pras_Server-1.2.0/Pras_Server/PDBID.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/PRAS.py` & `Pras_Server-1.2.0/Pras_Server/PRAS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 __doc__ = """
 
 This program requires python 3.6 or higher.
 
 This module, PRAS.py is the main module that
 
@@ -16,15 +16,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
 
@@ -190,15 +190,15 @@
     else:
         if res[-1].isalpha():
             return res[-1]
         else:
             return "?"
 
 
-def repairPDB(pdb_pras,rotamer,mutation,pdb_faspr,keep_ligand,chain_no, ofname=False):
+def repairPDB(pdb_pras,rotamer,mutation,pdb_faspr,keep_ligand,chain_no, ofname=False,his_p=False):
     """
     This function steps over each residue of a chain and obtains from
     MissingHydrogenAtoms.py all atoms of the residue to be wrttien to a new PDB file.
 
     If the residue is not the last and the next residue is not PRO the returned list
     will contain a backbone H otherwise it will have no backbone H.
 
@@ -251,14 +251,16 @@
                  use a specific chain, user should provide an integer or a string number as the argument.
                  PRAS will map the integer to alphabets. Chain can start with any letter. Thus,
                  1 = the first chain, 2 = the second chain, etc. If user supplies a string number PRAS
                  will convert it to integer but if alphabet error will be generated.
 
     ofname     : the output file name, default name is out.pdb or out.cif
 
+    his_p     : If True, 20% of histidines will be protonated (+1 charge). It only matters if there are more than 4 HIS
+
     Returns
     -------
     None:        repaired and hydrogenated PDB structure will be written.
                  Ensure you have write permission in the directory where you
                  run the program
     """
 
@@ -465,18 +467,17 @@
                     else:
                         apos,name=notDisulfide(x[i],i,resNo[i],atom,atmpos,resNo,resseq)
                         res_pos.extend([apos])
                         atom_name.extend([name])
 
         """
         Next code line randomly protonates 20% of all HIS residues
-        comment next code line if you want all HIS side-chain neutral
         See explanation online at www.protein-science.com
         """
-        res_pos, atom_name = prot_his(x,res_pos,atom_name,n)
+        if his_p: res_pos, atom_name = prot_his(x,res_pos,atom_name,n)
 
         # Add backbone hydrogen.
         # It belongs to resi i+1
         for i,j in enumerate(h_pos):
             res_pos[h_pos[i][1]+1].extend([h_pos[i][0]])
             atom_name[h_pos[i][1]+1].extend('H')
```

### Comparing `Pras_Server-1.1.14/Pras_Server/PotentialEnergy.py` & `Pras_Server-1.2.0/Pras_Server/PotentialEnergy.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/RamaChandra.py` & `Pras_Server-1.2.0/Pras_Server/RamaChandra.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/ReadMaster.py` & `Pras_Server-1.2.0/Pras_Server/ReadMaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/ReadStructure.py` & `Pras_Server-1.2.0/Pras_Server/ReadStructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/ReadmmCIF.py` & `Pras_Server-1.2.0/Pras_Server/ReadmmCIF.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.1.14/Pras_Server/RunType.py` & `Pras_Server-1.2.0/Pras_Server/RunType.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
 
@@ -36,31 +36,32 @@
 from Pras_Server.SecondaryStructure import assignStructure
 
 class InitRunType:
 	"""
 
 	"""
 	fname=None
-	def __init__(self, rotamer="", mutation="", pdb_faspr="", keep_ligand="", chain_no="",addh=False, ss=False, raman=False, ofname=False, pdbid=False):
+	def __init__(self, rotamer="", mutation="", pdb_faspr="", keep_ligand="", chain_no="",addh=False, ss=False, raman=False, ofname=False, pdbid=False, his_p=False):
 		self.ss=ss
 		self.addh=addh 
 		self.raman=raman         
 		self.rotamer=rotamer
 		self.mutation=mutation
 		self.chain_no=chain_no
 		self.pdb_faspr=pdb_faspr
 		self.keep_ligand=keep_ligand
 		self.ofname=ofname
 		self.pdbid=pdbid
+		self.his_p=his_p
 
 	def ProcessWithoutDefault(self):
 		"""
 		Use this member function if you want to process all the PDBs in the directory where you called this program.
 		Here, the name of the output file will be the name of your input file minus ending .pdb plus _out.
-		In the case of a rurun PRAS will remove previous output files because PRAS writes in append mode
+		In the case of a rerun PRAS will remove previous output files because PRAS writes in append mode
 
 		The log file has the name of each PDB repaired so that you will know which PDB structure has missing atoms
 		In the case of a rerun the log file will be removed for the reasons stated above.
 
 		As an example, copy and run the below code in a python document in your directory with a PDB file.
 
 		import time
@@ -71,47 +72,48 @@
 		fixing = InitRunType(rotamer="", 
 							mutation="", 
 							pdb_faspr="", 
 							keep_ligand="", 
 							chain_no="",
 							addh = False,
 							ss=False,
-							raman=True,
+							raman=False,
 							ofname=False,
-							pdbid=False
+							pdbid=False,
+							his_p=False
 							)
 
 		fixing.ProcessWithoutDefault()
 
 		print ('The program took {0} second !'.format(time.time() - startTime))
 
 		"""
 		for i in os.listdir(os.getcwd()):
 			if i[-8:-4] == '_out' or i == 'log.txt': os.remove(i)
 
 		for i in os.listdir(os.getcwd()):
 			if i.endswith(".pdb") or i.endswith(".ent"):
-				if self.addh:repairPDB( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i[:-4]+'_out.pdb')
+				if self.addh:repairPDB( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i[:-4]+'_out.pdb', self.his_p)
 				else:fixheavyAtoms( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i[:-4]+'_out.pdb')
 				if self.ss:assignStructure(i[:-4]+'_out.pdb')
 				if self.raman:ramachandranTypes(i[:-4]+'_out.pdb')
 				print("fixed {}".format(i))
 
 			elif  i.endswith(".cif"):
-				if self.addh:repairPDB( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i[:-4]+'_out.cif')
+				if self.addh:repairPDB( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i[:-4]+'_out.cif', self.his_p)
 				else:fixheavyAtoms( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i[:-4]+'_out.cif')
 				if self.ss:assignStructure(i[:-4]+'_out.cif')
 				if self.raman:ramachandranTypes(i[:-4]+'_out.cif')
 				print("fixed {}".format(i))
 
 	def ProcessWithoutDefaultUsingPDBID(self):
 		"""
-		Use this member function if you want to process all the PDBs in a pdbid list supplied to PRAS.
-		Here, the name of the output file will be the name of your input PDB id plus _out.
-		In the case of a rurun PRAS will remove previous output files because PRAS writes in append mode
+		Use this member function if you want to process all the PDBs in a PDB ID list supplied to PRAS.
+		Here, the name of the output file will be the name of your input PDB ID plus _out.
+		In the case of a rerun PRAS will remove previous output files because PRAS writes in append mode
 
 		The log file has the name of each PDB repaired so that you will know which PDB structure has missing atoms
 		In the case of a rerun the log file will be removed for the reasons stated above.
 
 		As an example, copy and run the below code in a python document in your current working directory.
 
 		import time
@@ -124,48 +126,49 @@
 							pdb_faspr="", 
 							keep_ligand="", 
 							chain_no="",
 							addh = False,
 							ss=False,
 							raman=False,
 							ofname=False,
-							pdbid=['1crn','1hen']
+							pdbid=['1crn','1hen'],
+							his_p=False
 							)
 
 		fixing.ProcessWithoutDefaultUsingPDBID()
 
 		print ('The program took {0} second !'.format(time.time() - startTime))
 
 		"""
 		if not isinstance(self.pdbid, list):
 			print("You need to supply a list of PDB IDs. PRAS has terminated abnormally")
-			sys.exit()
+			sys.exit(1)
 		for i in os.listdir(os.getcwd()):
 			if i[-8:-4] == '_out' or i == 'log.txt': os.remove(i)
 
 		for i in self.pdbid:
 			if not i.endswith(".cif"):
-				if self.addh:repairPDB( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i+'_out.pdb')
+				if self.addh:repairPDB( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i+'_out.pdb', self.his_p)
 				else:fixheavyAtoms( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i+'_out.pdb')
 				if self.ss:assignStructure(i+'_out.pdb')
 				if self.raman:ramachandranTypes(i+'_out.pdb')
 				print("fixed {}".format(i+'.pdb'))
 
 			elif  i.endswith(".cif"):
 				if not self.ofname:self.ofname=i[:-4]+'_out.cif'
-				if self.addh:repairPDB( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i[:-4]+'_out.cif')
+				if self.addh:repairPDB( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i[:-4]+'_out.cif', self.his_p)
 				else:fixheavyAtoms( i, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, i[:-4]+'_out.cif')
 				if self.ss:assignStructure(i[:-4]+'_out.cif')
 				if self.raman:ramachandranTypes(i[:-4]+'_out.cif')
 				print("fixed {}".format(i))
 
 	def ProcessWithDefault(self):
 		"""
 		Use this member function if you want to process a single PDB file using PRAS default output name.
-		In the case of a rurun PRAS will remove previous output files because PRAS writes in append mode
+		In the case of a rerun PRAS will remove previous output files because PRAS writes in append mode
 
 		As an example, copy and run the below code in a python document in your directory with a PDB file 
 
 		import time
 		from Pras_Server.RunType import InitRunType
 
 		startTime = time.time()
@@ -175,36 +178,40 @@
 							pdb_faspr="", 
 							keep_ligand="", 
 							chain_no="",
 							addh = False,
 							ss=False,
 							raman=False,
 							ofname=False,
-							pdbid=False
+							pdbid=False,
+							his_p=False
 							)
 
 		fixing.fname = '1crn.pdb' # change this to whatever your file is named
 
 		fixing.ProcessWithDefault()
 
 		print ('The program took {0} second !'.format(time.time() - startTime))
 
 		"""
 		if not self.fname:
 			print("You need to supply a file name. PRAS has terminated abnormally")
-			sys.exit()
+			sys.exit(1)
+		if self.ofname:
+			print("Output file name must be set to False. PRAS has terminated abnormally")
+			sys.exit(1)
 		if self.fname.endswith(".pdb") or self.fname.endswith(".ent"):
-			if self.addh:repairPDB(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no)
+			if self.addh:repairPDB(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, self.ofname, self.his_p)
 			else:fixheavyAtoms(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no)
 			if self.ss:assignStructure('out.pdb')
 			if self.raman:ramachandranTypes('out.pdb')
 			print("fixed {}".format(self.fname))
 
 		if self.fname.endswith(".cif"):
-			if self.addh:repairPDB(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no)
+			if self.addh:repairPDB(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, self.ofname, self.his_p)
 			else:fixheavyAtoms(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no)
 			if self.ss:assignStructure('out.cif')
 			if self.raman:ramachandranTypes('out.cif')
 			print("fixed {}".format(self.fname))
 
 	def ProcessOther(self):
 		"""
@@ -214,47 +221,55 @@
 		you instantiate InitRunType class and supply the ofname, say xxxx.pdb.
 
 		Warning: PRAS writes in append mode and you're responsibe for deleting the output files in case of a rerun!!
 
 		As an example, copy and run the below code in a python document in your directory with many PDBs
 
 		import os
+		import sys
 		import time
 		from Pras_Server.RunType import InitRunType
 
 		startTime = time.time()
-		out = ['xxx.pdb','zzz.pdb','sss.pdb'] # size of this list MUST be equal to the total number of PDBs
+		out = ['xxxx.pdb','zzzz.pdb','ssss.pdb'] # size of this list MUST be equal to the total number of PDB structures in your working directory
 		k=0
 		for i in os.listdir(os.getcwd()):
-			if i.endswith(".pdb"):
+			if i.endswith(".pdb") or i.endswith(".ent"):
+				try:
+					out[k]
+				except:
+					print('Index error. Size of the name list is small')
+					sys.exit()
 				fixing = InitRunType(rotamer="", 
 									mutation="", 
 									pdb_faspr="", 
 									keep_ligand="", 
 									chain_no="",
 									addh = False,
-									ss=True,
-									raman=True,
+									ss=False,
+									raman=False,
 									ofname=out[k],
-									pdbid=False
+									pdbid=False,
+									his_p=False
 									)
+				fixing.fname = i
 				fixing.ProcessOther()
 				k+=1
 		print ('The program took {0} second !'.format(time.time() - startTime))
 
 		"""
 		if not self.fname:
-			print("You need to supply a file name. PRAS has terminated abnormally")
+			print("No PDB structure file found in your working direcotry. PRAS has terminated abnormally")
 			sys.exit()
 		if self.fname.endswith(".pdb") or self.fname.endswith(".ent"):
-			if self.addh:repairPDB(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no,self.ofname)
+			if self.addh:repairPDB(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, self.ofname, self.his_p)
 			else:fixheavyAtoms(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no,self.ofname)
 			if self.ss:assignStructure(self.ofname)
 			if self.raman:ramachandranTypes(self.ofname)
-			print("fixed {}".format(self.fname))
+			print("fixed {}".format(self.ofname))
 
 		if self.fname.endswith(".cif"):
-			if self.addh:repairPDB(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no,self.ofname)
-			else:fixheavyAtoms(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no,self.ofname)
+			if self.addh:repairPDB(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, self.ofname, self.his_p)
+			else:fixheavyAtoms(self.fname, self.rotamer, self.mutation, self.pdb_faspr, self.keep_ligand, self.chain_no, self.ofname)
 			if self.ss:assignStructure(self.ofname)
 			if self.raman:ramachandranTypes(self.ofname)
-			print("fixed {}".format(self.fname))
+			print("fixed {}".format(self.ofname))
```

### Comparing `Pras_Server-1.1.14/Pras_Server/SecondaryStructure.py` & `Pras_Server-1.2.0/Pras_Server/SecondaryStructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.0.11"
+__version__    = "1.2.0"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
 
@@ -293,8 +293,8 @@
 			plt.savefig('sec_strc_plot_'+'chain'+str(n+1)+'_'+filename[:-4]+'.tif')
 			plt.close(fig)
 
 			if _format == '.pdb':
 				if n == 0:
 					count+= chains[n]+1
 				else:
-					count+= (chains[n]-chains[n-1])
+					count+= (chains[n]-chains[n-1])
```

### Comparing `Pras_Server-1.1.14/Pras_Server/data/KD.dat` & `Pras_Server-1.2.0/Pras_Server/data/KD.dat`

 * *Files identical despite different names*

### Comparing `Pras_Server-1.1.14/Pras_Server/run_PRAS_with_FASPR/1aho.pdb` & `Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/1aho.pdb`

 * *Files identical despite different names*

### Comparing `Pras_Server-1.1.14/Pras_Server/run_PRAS_with_FASPR/PRAS_with_FASPR.pdf` & `Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/PRAS_with_FASPR.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 3% similar despite different names*

#### pdftotext {} -

```diff
@@ -2,32 +2,33 @@
 i
 Download FASPR from https://github.com/tommyhuangthu/FASPR
 and extract to any folder as below. Then enter/open the folder
 
 iii
 After successful compilation you will see FASPR as pointed towards
 
-In line 72, change string pdbin=(string)"example/1mol.pdb" to string pdbin=(string)“.“
+In FASPR.cpp, line 72, change string pdbin=(string)"example/1mol.pdb" to string pdbin=(string)“.“
 In line 73, change string pdbout=(string)"example/1mol_FASPR.pdb" to string pdbout=(string)“.“
 Without these changes, your input PDB and its path must correspond to example/1mol.pdb
 
 iv
 
 ii
 Type “bash” in the search window and hit enter to open lunix terminal as shown.
 Then, execute the code below to compile FASPR (it takes ≈ 1 min. to compile):
 
 Now install PRAS server (if not installed) using the command below
 
 g++ -ffast-math -O3 -o FASPR src/*.cpp
 
 Install PRAS server which is added to path automatically with:
-pip install Pras-Server==1.0.11
+pip install Pras-Server==1.1.0
 
 Now download 1aho.pdb and copy to the current folder and run the code in
 syntax.txt that invokes linux_examply.py in the folder containing this
 document to repair several missing atoms using chi from FASPR PDB output.
 It is a good practice to type commands in Linux than copy and paste as
 Linux is extremely sensitive.
+
 This is not a substitute for FASPR installation instructions. Always refer to the software documentation
```

### Comparing `Pras_Server-1.1.14/Pras_Server/run_PRAS_with_FASPR/syntax.txt` & `Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/syntax.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Compile FASPR
-`g++ -ffast-math -O3 -o FASPR src/*.cpp`
-
-Install PRAS server
-`pip install Pras-Server==1.0.11`
-
-Execute to run PRAS with FASPR output PDB
-`./FASPR –i 1aho.pdb -o output.pdb;python3 linux_example.py 1aho.pdb "" "" output.pdb "" ""`
-
-You will see that both 	secondary structure assignemnt(ss) and ramachandran plot (rama) 
-are set to False and the reason is because you must install X server for Windows
-in order to run Linux GUI applications using Windows Subsystem for Linux (WSL).
-
-Thus, you need to:
-
-Install X server for Windows
-
-Configure bash to tell GUIs to use the local X server
-
-So, install VcXsrv which is open source by downloading from https://sourceforge.net/projects/vcxsrv/
-
-Configure bash to use the local X server (VcXsrv is an X server). In bash run:
-
-`echo "export DISPLAY=localhost:0.0" >> ~/.bashrc`
-
-To have the configuration changes take effect, restart bash, or run:
-
-`. ~/.bashrc`
-
-Then open VcXsrv from your taskbar (you should send the icon to taskbar for easy access).
-Note that VcXsrv must be open/running each time you use plotting tools in the linux terminal
-Now you can set ss True and raman True
+Compile FASPR
+`g++ -ffast-math -O3 -o FASPR src/*.cpp`
+
+Install PRAS server
+`pip install Pras-Server==1.1.0`
+
+Execute to run PRAS with FASPR output PDB
+`./FASPR –i 1aho.pdb -o output.pdb;python3 linux_example.py 1aho.pdb "" "" output.pdb "" ""`
+
+You will see that both 	secondary structure assignemnt(ss) and ramachandran plot (rama) 
+are set to False and the reason is because you must install X server for Windows
+in order to run Linux GUI applications using Windows Subsystem for Linux (WSL).
+
+Thus, you need to:
+
+Install X server for Windows
+
+Configure bash to tell GUIs to use the local X server
+
+So, install VcXsrv which is open source by downloading from https://sourceforge.net/projects/vcxsrv/
+
+Configure bash to use the local X server (VcXsrv is an X server). In bash run:
+
+`echo "export DISPLAY=localhost:0.0" >> ~/.bashrc`
+
+To have the configuration changes take effect, restart bash, or run:
+
+`. ~/.bashrc`
+
+Then open VcXsrv from your taskbar (you should send the icon to taskbar for easy access).
+Note that VcXsrv must be open/running each time you use plotting tools in the linux terminal
+Now you can set ss True and raman True
```

### Comparing `Pras_Server-1.1.14/Pras_Server.egg-info/PKG-INFO` & `Pras_Server-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,14 @@
-Metadata-Version: 2.1
-Name: Pras-Server
-Version: 1.1.14
-Summary: A webserver to repair PDB files
-Home-page: https://www.protein-science.com/
-Author: Osita S. Nnyigide
-Author-email: osita@protein-science.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+Protein Repair and Analysis (PRAS) Server is a tool to repair PDB or mmCIF structures, add missing heavy 
 
-Protein Repair and Analysis (PRAS) Server is a tool to repair PDB or mmCIF structures, add missing heavy atoms and hydrogen atoms and assign secondary structures by amide-amide interactions of the backbone
+atoms and hydrogen atoms and assign secondary structures by amide-amide interactions of the backbone
 
-You can use the server online at https://www.protein-science.com/ or on your local machine following the instructions given below
+You can use the server online at https://www.protein-science.com/ or on your local machine following the 
+
+instructions given below
 
 The program consists of:
 ```python
 Tools to automatically download PDB or mmCIF structures
 
 Tools to generate different rotamers if present in a PDB or mmCIF structure file
 
@@ -29,15 +19,19 @@
 Tools to assign secondary structure elements by amide-amide interactions of the backbone
 
 Tools to draw 4 Ramachandran types (i.e., general, glycine, proline and pre-proline)
 ```
 
 ## PRAS installation
 
-`pip install Pras-Server==1.0.11`
+On November 20, 2022, a C++ version of the server that is independent of the python counterpart was released. The C++ version is named Pras_Server_C++ and is part of this repository. Both versions produce the same result but the former is 9 to 12 times faster than the latter. To use the C++ version, download this ZIP and extract the Pras_Server_C++ folder and follow the instruction in the INSTALL file included with the distribution.
+
+To use the python distribution on your local machine, use pip as given below or copy Pras_Server folder to any of the directories that Python searches at run-time
+
+`pip install Pras-Server==1.1.0`
 
 ## PRAS usage
 
 A comprehensive test with 82 or 494 PDB or mmCIF structures may be performed to ensure the program works correctly.
 
 Since PRAS can download these structures automatically, 2 lists are provided which contain all the PDB IDs.
 
@@ -50,47 +44,42 @@
 #user's internet download speed
 import time
 from Pras_Server.RunType import InitRunType
 from Pras_Server.PDBID import  _82_pdbs, _494_pdbs
 
 startTime = time.time()
 
-fixing = InitRunType( rotamer="", 
-					mutation="", 
-					pdb_faspr="", 
-					keep_ligand="", 
-					chain_no="",
-					addh = False,
-					ss=False,
-					raman=False,
-					ofname=False,
-					pdbid=_82_pdbs
-					)
+fixing = InitRunType( rotamer="", mutation="", pdb_faspr="", keep_ligand="", chain_no="", 
+		      addh=False, ss=False, raman=False, ofname=False, pdbid=_82_pdbs, his_p=False)
 
 # fixed PDB is saved with name=PDB ID+_out.pdb
 # addh, use default or set to True to add hydrogen
 # pdbid, must be a list of PDB IDs or set to False
 # ss=secondary structure, set to True if you need it
 # raman=ramachandran plot, set to True if you need it
 # rotamer, use default or "yes" to use low occupancy conformers
 # mutation, use default or "yes" to use low occupancy conformers
 # keep_ligand, use default or "yes" to keep non-water ligands
 # chain_no, use default or string number (e.g., "1") to process a specific chain
 # ofname, output file name, use default. To use your own name read documentaion below
-# Execute print(InitRunType.ProcessOther().__doc__) or see RunType.py doc instructions
+# his_p, protonate 20% of HIS. A fraction of HIS may be charged at pH of 7. Use default
 # pdb_faspr, use default or enter a pdb output from faspr, reason is stated in pras paper
+# Execute print(InitRunType.ProcessOther().__doc__) or see RunType.py doc instructions
 
 fixing.ProcessWithoutDefaultUsingPDBID()
 #You can print(InitRunType.ProcessWithoutDefaultUsingPDBID.__doc__) 
 #to learn more about the member function
 print ('The program took {0} second !'.format(time.time() - startTime))
 ```
 
 The above will download and analyze 82 or 494 protein structures. One can modify the code to process either of the lists.
-If you set ss=True and rama=True, you may encounter failed to allocate bitmap error (depending on your computer's memory)
+
+If you set ss=True and rama=True, you may encounter failed to allocate bitmap error (depending on your computer's memory).
+
+Note that the above test will work in both windows and linux systems. For linux you just need to do python3 pras_test.py
 
 For users that do not want to do the above comprehensive test, instructions are given below to process a
 
 single protein structure in a windows or linux environment.
 
 For winddows, download a protein (e.g toxin II, 1aho.pdb, or let PRAS download it automatically)
 
@@ -103,82 +92,66 @@
 
 ```python
 import time
 from Pras_Server.RunType import InitRunType
 
 startTime = time.time()
 
-fixing = InitRunType(rotamer="", 
-					mutation="", 
-					pdb_faspr="", 
-					keep_ligand="", 
-					chain_no="",
-					addh = False,
-					ss=False,
-					raman=False,
-					ofname=False,
-					pdbid=False
-					)
+fixing = InitRunType(rotamer="", mutation="", pdb_faspr="", keep_ligand="", chain_no="", 
+		     addh=False, ss=False, raman=False, ofname=False,pdbid=False, his_p=False)
 
 fixing.fname = '1aho.pdb'
 
 fixing.ProcessWithDefault()
 #You can print(InitRunType.ProcessWithDefault.__doc__) 
 #to learn more about the member function
 print ('The program took {0} second !'.format(time.time() - startTime))
 ```
 
 For linux, do the same as above except for the example code where you should copy the code below (the annotation given above applies below):
 
 ```python
 import sys
 
-if len(sys.argv) == 8:
+if len(sys.argv) == 9:
 	import time
 	from Pras_Server.RunType import InitRunType
 	startTime = time.time()
 
 	rotamer=sys.argv[2] 
 	mutation=sys.argv[3]
 	pdb_faspr=sys.argv[4]
 	keep_ligand=sys.argv[5]
 	chain_no=sys.argv[6] 
 	ofname=sys.argv[7]
-	fixing=InitRunType(
-					rotamer, 
-					mutation, 
-					pdb_faspr, 
-					keep_ligand, 
-					chain_no,
-					addh=False,
-					ss=False,
-					raman=False,
-					ofname=False,
-					pdbid=False
-					)
+	his_p=sys.argv[8]
+	fixing=InitRunType(rotamer, mutation, pdb_faspr, keep_ligand, chain_no, 
+			   addh=False, ss=False, raman=False, ofname=False, pdbid=False, his_p=False)
 	fixing.fname=sys.argv[1]
 	fixing.ProcessWithDefault()
 	print ('The program took {0} second !'.format(time.time() - startTime))
 
 else:
-	print("PRAS takes 8 compulsory arguments." 
+	print("PRAS takes 9 compulsory arguments." 
 		  " Execute the code below on your shell prompt to learn more\n")
 	print("printf \"from Pras_Server.PRAS import" 
 		  " repairPDB\\nprint(repairPDB.__doc__)\\n\\n()\" | python3\n")
 ```
 
 Then, cd to the directory where example.py is located and enter the following argument on your shell prompt:
 
-`python3 example.py 1aho.pdb "" "" "" "" "" ""`
+`python3 example.py 1aho.pdb "" "" "" "" "" "" ""`
 
 
 ## WINDOWS SUBSYSTEM FOR LINUX (WSL)
 
 In order to run Linux GUI applications e.g., the plots for
+
 secondary structure assignment and 4 Ramachandran types
+
 using Windows Subsystem for Linux (WSL), you must install X server for Windows.
 
 Thus, you need to:
 
 Install X server for Windows
 
 Configure bash to tell GUIs to use the local X server
```

### Comparing `Pras_Server-1.1.14/Pras_Server.egg-info/SOURCES.txt` & `Pras_Server-1.2.0/Pras_Server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pras_Server-1.1.14/README.md` & `Pras_Server-1.2.0/Pras_Server.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,28 @@
-Protein Repair and Analysis (PRAS) Server is a tool to repair PDB or mmCIF structures, add missing heavy atoms and hydrogen atoms and assign secondary structures by amide-amide interactions of the backbone
+Metadata-Version: 2.1
+Name: Pras-Server
+Version: 1.2.0
+Summary: A webserver to repair PDB files
+Home-page: https://www.protein-science.com/
+Author: Osita S. Nnyigide
+Author-email: osita@protein-science.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.6, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-You can use the server online at https://www.protein-science.com/ or on your local machine following the instructions given below
+Protein Repair and Analysis (PRAS) Server is a tool to repair PDB or mmCIF structures, add missing heavy 
+
+atoms and hydrogen atoms and assign secondary structures by amide-amide interactions of the backbone
+
+You can use the server online at https://www.protein-science.com/ or on your local machine following the 
+
+instructions given below
 
 The program consists of:
 ```python
 Tools to automatically download PDB or mmCIF structures
 
 Tools to generate different rotamers if present in a PDB or mmCIF structure file
 
@@ -15,15 +33,19 @@
 Tools to assign secondary structure elements by amide-amide interactions of the backbone
 
 Tools to draw 4 Ramachandran types (i.e., general, glycine, proline and pre-proline)
 ```
 
 ## PRAS installation
 
-`pip install Pras-Server==1.0.11`
+On November 20, 2022, a C++ version of the server that is independent of the python counterpart was released. The C++ version is named Pras_Server_C++ and is part of this repository. Both versions produce the same result but the former is 9 to 12 times faster than the latter. To use the C++ version, download this ZIP and extract the Pras_Server_C++ folder and follow the instruction in the INSTALL file included with the distribution.
+
+To use the python distribution on your local machine, use pip as given below or copy Pras_Server folder to any of the directories that Python searches at run-time
+
+`pip install Pras-Server==1.1.0`
 
 ## PRAS usage
 
 A comprehensive test with 82 or 494 PDB or mmCIF structures may be performed to ensure the program works correctly.
 
 Since PRAS can download these structures automatically, 2 lists are provided which contain all the PDB IDs.
 
@@ -36,47 +58,42 @@
 #user's internet download speed
 import time
 from Pras_Server.RunType import InitRunType
 from Pras_Server.PDBID import  _82_pdbs, _494_pdbs
 
 startTime = time.time()
 
-fixing = InitRunType( rotamer="", 
-					mutation="", 
-					pdb_faspr="", 
-					keep_ligand="", 
-					chain_no="",
-					addh = False,
-					ss=False,
-					raman=False,
-					ofname=False,
-					pdbid=_82_pdbs
-					)
+fixing = InitRunType( rotamer="", mutation="", pdb_faspr="", keep_ligand="", chain_no="", 
+		      addh=False, ss=False, raman=False, ofname=False, pdbid=_82_pdbs, his_p=False)
 
 # fixed PDB is saved with name=PDB ID+_out.pdb
 # addh, use default or set to True to add hydrogen
 # pdbid, must be a list of PDB IDs or set to False
 # ss=secondary structure, set to True if you need it
 # raman=ramachandran plot, set to True if you need it
 # rotamer, use default or "yes" to use low occupancy conformers
 # mutation, use default or "yes" to use low occupancy conformers
 # keep_ligand, use default or "yes" to keep non-water ligands
 # chain_no, use default or string number (e.g., "1") to process a specific chain
 # ofname, output file name, use default. To use your own name read documentaion below
-# Execute print(InitRunType.ProcessOther().__doc__) or see RunType.py doc instructions
+# his_p, protonate 20% of HIS. A fraction of HIS may be charged at pH of 7. Use default
 # pdb_faspr, use default or enter a pdb output from faspr, reason is stated in pras paper
+# Execute print(InitRunType.ProcessOther().__doc__) or see RunType.py doc instructions
 
 fixing.ProcessWithoutDefaultUsingPDBID()
 #You can print(InitRunType.ProcessWithoutDefaultUsingPDBID.__doc__) 
 #to learn more about the member function
 print ('The program took {0} second !'.format(time.time() - startTime))
 ```
 
 The above will download and analyze 82 or 494 protein structures. One can modify the code to process either of the lists.
-If you set ss=True and rama=True, you may encounter failed to allocate bitmap error (depending on your computer's memory)
+
+If you set ss=True and rama=True, you may encounter failed to allocate bitmap error (depending on your computer's memory).
+
+Note that the above test will work in both windows and linux systems. For linux you just need to do python3 pras_test.py
 
 For users that do not want to do the above comprehensive test, instructions are given below to process a
 
 single protein structure in a windows or linux environment.
 
 For winddows, download a protein (e.g toxin II, 1aho.pdb, or let PRAS download it automatically)
 
@@ -89,82 +106,66 @@
 
 ```python
 import time
 from Pras_Server.RunType import InitRunType
 
 startTime = time.time()
 
-fixing = InitRunType(rotamer="", 
-					mutation="", 
-					pdb_faspr="", 
-					keep_ligand="", 
-					chain_no="",
-					addh = False,
-					ss=False,
-					raman=False,
-					ofname=False,
-					pdbid=False
-					)
+fixing = InitRunType(rotamer="", mutation="", pdb_faspr="", keep_ligand="", chain_no="", 
+		     addh=False, ss=False, raman=False, ofname=False,pdbid=False, his_p=False)
 
 fixing.fname = '1aho.pdb'
 
 fixing.ProcessWithDefault()
 #You can print(InitRunType.ProcessWithDefault.__doc__) 
 #to learn more about the member function
 print ('The program took {0} second !'.format(time.time() - startTime))
 ```
 
 For linux, do the same as above except for the example code where you should copy the code below (the annotation given above applies below):
 
 ```python
 import sys
 
-if len(sys.argv) == 8:
+if len(sys.argv) == 9:
 	import time
 	from Pras_Server.RunType import InitRunType
 	startTime = time.time()
 
 	rotamer=sys.argv[2] 
 	mutation=sys.argv[3]
 	pdb_faspr=sys.argv[4]
 	keep_ligand=sys.argv[5]
 	chain_no=sys.argv[6] 
 	ofname=sys.argv[7]
-	fixing=InitRunType(
-					rotamer, 
-					mutation, 
-					pdb_faspr, 
-					keep_ligand, 
-					chain_no,
-					addh=False,
-					ss=False,
-					raman=False,
-					ofname=False,
-					pdbid=False
-					)
+	his_p=sys.argv[8]
+	fixing=InitRunType(rotamer, mutation, pdb_faspr, keep_ligand, chain_no, 
+			   addh=False, ss=False, raman=False, ofname=False, pdbid=False, his_p=False)
 	fixing.fname=sys.argv[1]
 	fixing.ProcessWithDefault()
 	print ('The program took {0} second !'.format(time.time() - startTime))
 
 else:
-	print("PRAS takes 8 compulsory arguments." 
+	print("PRAS takes 9 compulsory arguments." 
 		  " Execute the code below on your shell prompt to learn more\n")
 	print("printf \"from Pras_Server.PRAS import" 
 		  " repairPDB\\nprint(repairPDB.__doc__)\\n\\n()\" | python3\n")
 ```
 
 Then, cd to the directory where example.py is located and enter the following argument on your shell prompt:
 
-`python3 example.py 1aho.pdb "" "" "" "" "" ""`
+`python3 example.py 1aho.pdb "" "" "" "" "" "" ""`
 
 
 ## WINDOWS SUBSYSTEM FOR LINUX (WSL)
 
 In order to run Linux GUI applications e.g., the plots for
+
 secondary structure assignment and 4 Ramachandran types
+
 using Windows Subsystem for Linux (WSL), you must install X server for Windows.
 
 Thus, you need to:
 
 Install X server for Windows
 
 Configure bash to tell GUIs to use the local X server
```

### Comparing `Pras_Server-1.1.14/setup.py` & `Pras_Server-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 current_dir = pathlib.Path(__file__).parent.resolve()
 
 long_description = (current_dir / 'README.md').read_text(encoding='utf-8')
 
 setup(
 
     name = 'Pras_Server',
-    version = '1.1.14',
+    version = '1.2.0',
     description='A webserver to repair PDB files',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.protein-science.com/',
     author='Osita S. Nnyigide',
     author_email='osita@protein-science.com',
     classifiers=[
```

