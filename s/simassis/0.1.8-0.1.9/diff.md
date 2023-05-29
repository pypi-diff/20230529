# Comparing `tmp/simassis-0.1.8.tar.gz` & `tmp/simassis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simassis-0.1.8.tar", last modified: Tue Feb  7 11:25:52 2023, max compression
+gzip compressed data, was "simassis-0.1.9.tar", last modified: Tue Feb  7 11:46:20 2023, max compression
```

## Comparing `simassis-0.1.8.tar` & `simassis-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-02-07 11:25:52.250226 simassis-0.1.8/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      618 2023-02-07 11:25:52.250226 simassis-0.1.8/PKG-INFO
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       38 2023-02-07 11:25:52.250226 simassis-0.1.8/setup.cfg
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      808 2023-02-07 11:25:45.000000 simassis-0.1.8/setup.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-02-07 11:25:52.246226 simassis-0.1.8/simassis/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      165 2023-02-07 11:24:35.000000 simassis-0.1.8/simassis/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    22691 2023-02-07 11:23:58.000000 simassis-0.1.8/simassis/files.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     5579 2023-01-11 18:30:24.000000 simassis-0.1.8/simassis/general.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-02-07 11:25:52.246226 simassis-0.1.8/simassis.egg-info/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      618 2023-02-07 11:25:51.000000 simassis-0.1.8/simassis.egg-info/PKG-INFO
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      226 2023-02-07 11:25:52.000000 simassis-0.1.8/simassis.egg-info/SOURCES.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)        1 2023-02-07 11:25:51.000000 simassis-0.1.8/simassis.egg-info/dependency_links.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       12 2023-02-07 11:25:52.000000 simassis-0.1.8/simassis.egg-info/requires.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)        9 2023-02-07 11:25:52.000000 simassis-0.1.8/simassis.egg-info/top_level.txt
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-02-07 11:46:20.842040 simassis-0.1.9/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      618 2023-02-07 11:46:20.842040 simassis-0.1.9/PKG-INFO
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       38 2023-02-07 11:46:20.842040 simassis-0.1.9/setup.cfg
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      808 2023-02-07 11:45:50.000000 simassis-0.1.9/setup.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-02-07 11:46:20.842040 simassis-0.1.9/simassis/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      165 2023-02-07 11:24:35.000000 simassis-0.1.9/simassis/__init__.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    22404 2023-02-07 11:45:40.000000 simassis-0.1.9/simassis/files.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     5579 2023-01-11 18:30:24.000000 simassis-0.1.9/simassis/general.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-02-07 11:46:20.842040 simassis-0.1.9/simassis.egg-info/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      618 2023-02-07 11:46:20.000000 simassis-0.1.9/simassis.egg-info/PKG-INFO
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      226 2023-02-07 11:46:20.000000 simassis-0.1.9/simassis.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)        1 2023-02-07 11:46:20.000000 simassis-0.1.9/simassis.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       12 2023-02-07 11:46:20.000000 simassis-0.1.9/simassis.egg-info/requires.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)        9 2023-02-07 11:46:20.000000 simassis-0.1.9/simassis.egg-info/top_level.txt
```

### Comparing `simassis-0.1.8/PKG-INFO` & `simassis-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simassis
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python Package for MD calculations in solids
 Home-page: https://github.com/marcinkrynskipw/simassis
 Author: Marcin Krynski
 Author-email: marcin.krynski@pw.edu.pl
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `simassis-0.1.8/setup.py` & `simassis-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='simassis',
-    version='0.1.8',
+    version='0.1.9',
     description='A python Package for MD calculations in solids',
     author='Marcin Krynski',
     author_email='marcin.krynski@pw.edu.pl',
     url='https://github.com/marcinkrynskipw/simassis',
     license='BSD 2-clause',
     packages=['simassis'],
     install_requires=[
```

### Comparing `simassis-0.1.8/simassis/files.py` & `simassis-0.1.9/simassis/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,76 +539,75 @@
     lines = lines[brak[0]+1:brak[1]]
     return np.array([l.split()[4] for l in lines], dtype=float)
 
 def vasp_to_runner_data_train(finput, charges_default):
     samples = list_of_directories(finput)
     text = ''
     for sample in samples:
-        try:
-            #charges and positions
-            file = open(finput + sample + '/ACF.dat')
-            lines = file.readlines()
-            file.close()
-            total_electrones = float(lines[-1].split()[-1])
-            lines = lines[2:-4]
-            positions = np.array([l.split()[1:4] for l in lines], dtype=float)*Angstrom_2_Bohr
-            positions = np.array(positions, dtype='str')
-            charges_ = np.array([l.split()[4] for l in lines], dtype=float)
-
-            file = open(finput + sample + '/POSCAR')
-            lines = file.readlines()
-            atoms = lines[6].split()
-            atoms_names = lines[5].split()
-            file.close()
-            atoms = [int(a) for a in atoms]
-            charges_default_vec = []
-            atoms_names_vec = []
-            for a, cd, an in zip(atoms, charges_default, atoms_names):
-                charges_default_vec = charges_default_vec + [cd]*a
-                atoms_names_vec = atoms_names_vec + [an]*a
-            charges_default_vec = np.array(charges_default_vec)
-            charges = (-charges_+charges_default_vec).tolist()
-            charges = [str(c) for c in charges]
-            basis = lines[2:5]
-
-            #forces
-            file = open(finput + sample + '/OUTCAR')
-            lines = file.readlines()[2:-4]
-            file.close()
-            energy = [l for l in lines if 'energy  without entropy' in l]
-            energy = str(float(energy[-1].split('=')[1].split()[0])*ev2H)
-
-            start = [i for i in range(len(lines)) if 'TOTAL-FORCE' in lines[i]]
-            lines = lines[start[-1]+2:]
-            stop = [i for i in range(len(lines)) if 'total drift:' in lines[i]]
-            lines = lines[:stop[-1]-1]
-            forces = np.array([l.split()[3:] for l in lines], dtype=float)
-            forces = np.array(forces*eV_per_Angstrom_2_Ha_per_Bohr, dtype='str')
-
-            text = text + 'begin\n'
-            text = text + 'lattice         '+'   '.join((np.array(np.array(basis[0].split(), dtype=float)*Angstrom_2_Bohr, dtype=str)).tolist()) + '\n'
-            text = text + 'lattice         '+'   '.join((np.array(np.array(basis[1].split(), dtype=float)*Angstrom_2_Bohr, dtype=str)).tolist()) + '\n'
-            text = text + 'lattice         '+'   '.join((np.array(np.array(basis[2].split(), dtype=float)*Angstrom_2_Bohr, dtype=str)).tolist()) + '\n'
-            lines = ''
-            for i in range(len(atoms_names_vec)):
-                line = [
-                        'atom',
-                        ("%.10f" % float(positions[i][0])),
-                        ("%.10f" % float(positions[i][1])),
-                        ("%.10f" % float(positions[i][2])),
-                        atoms_names_vec[i],
-                        ("%.10f" % float(charges[i])),
-                        '0',
-                        ("%.10f" % float(forces[i][0])),
-                        ("%.10f" % float(forces[i][1])),
-                        ("%.10f" % float(forces[i][2])),
-                        ]
-                lines = lines + ''.join(word.ljust(15) for word in line)+'\n'
-            text = text + lines
-            text = text + 'energy    ' + energy + '\n'
-            text = text + 'charge    '+str(-np.sum(charges_default_vec)+total_electrones)+ '\n'
-            text = text + 'end\n'
-        except()
-            print('problems with '+sample)
+        print(sample)
+        #charges and positions
+        file = open(finput + sample + '/ACF.dat')
+        lines = file.readlines()
+        file.close()
+        total_electrones = float(lines[-1].split()[-1])
+        lines = lines[2:-4]
+        positions = np.array([l.split()[1:4] for l in lines], dtype=float)*Angstrom_2_Bohr
+        positions = np.array(positions, dtype='str')
+        charges_ = np.array([l.split()[4] for l in lines], dtype=float)
+
+        file = open(finput + sample + '/POSCAR')
+        lines = file.readlines()
+        atoms = lines[6].split()
+        atoms_names = lines[5].split()
+        file.close()
+        atoms = [int(a) for a in atoms]
+        charges_default_vec = []
+        atoms_names_vec = []
+        for a, cd, an in zip(atoms, charges_default, atoms_names):
+            charges_default_vec = charges_default_vec + [cd]*a
+            atoms_names_vec = atoms_names_vec + [an]*a
+        charges_default_vec = np.array(charges_default_vec)
+        charges = (-charges_+charges_default_vec).tolist()
+        charges = [str(c) for c in charges]
+        basis = lines[2:5]
+
+        #forces
+        file = open(finput + sample + '/OUTCAR')
+        lines = file.readlines()[2:-4]
+        file.close()
+        energy = [l for l in lines if 'energy  without entropy' in l]
+        energy = str(float(energy[-1].split('=')[1].split()[0])*ev2H)
+
+        start = [i for i in range(len(lines)) if 'TOTAL-FORCE' in lines[i]]
+        lines = lines[start[-1]+2:]
+        stop = [i for i in range(len(lines)) if 'total drift:' in lines[i]]
+        lines = lines[:stop[-1]-1]
+        forces = np.array([l.split()[3:] for l in lines], dtype=float)
+        forces = np.array(forces*eV_per_Angstrom_2_Ha_per_Bohr, dtype='str')
+
+        text = text + 'begin\n'
+        text = text + 'lattice         '+'   '.join((np.array(np.array(basis[0].split(), dtype=float)*Angstrom_2_Bohr, dtype=str)).tolist()) + '\n'
+        text = text + 'lattice         '+'   '.join((np.array(np.array(basis[1].split(), dtype=float)*Angstrom_2_Bohr, dtype=str)).tolist()) + '\n'
+        text = text + 'lattice         '+'   '.join((np.array(np.array(basis[2].split(), dtype=float)*Angstrom_2_Bohr, dtype=str)).tolist()) + '\n'
+        lines = ''
+        for i in range(len(atoms_names_vec)):
+            line = [
+                    'atom',
+                    ("%.10f" % float(positions[i][0])),
+                    ("%.10f" % float(positions[i][1])),
+                    ("%.10f" % float(positions[i][2])),
+                    atoms_names_vec[i],
+                    ("%.10f" % float(charges[i])),
+                    '0',
+                    ("%.10f" % float(forces[i][0])),
+                    ("%.10f" % float(forces[i][1])),
+                    ("%.10f" % float(forces[i][2])),
+                    ]
+            lines = lines + ''.join(word.ljust(15) for word in line)+'\n'
+        text = text + lines
+        text = text + 'energy    ' + energy + '\n'
+        text = text + 'charge    '+str(-np.sum(charges_default_vec)+total_electrones)+ '\n'
+        text = text + 'end\n'
+
     file = open(finput + '/input.data', 'w')
     file.writelines(text)
     file.close()
```

### Comparing `simassis-0.1.8/simassis/general.py` & `simassis-0.1.9/simassis/general.py`

 * *Files identical despite different names*

### Comparing `simassis-0.1.8/simassis.egg-info/PKG-INFO` & `simassis-0.1.9/simassis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simassis
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python Package for MD calculations in solids
 Home-page: https://github.com/marcinkrynskipw/simassis
 Author: Marcin Krynski
 Author-email: marcin.krynski@pw.edu.pl
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

