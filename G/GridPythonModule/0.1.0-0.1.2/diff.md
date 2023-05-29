# Comparing `tmp/GridPythonModule-0.1.0.tar.gz` & `tmp/GridPythonModule-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridPythonModule-0.1.0.tar", last modified: Sun Apr 16 04:15:50 2023, max compression
+gzip compressed data, was "GridPythonModule-0.1.2.tar", last modified: Mon May 29 08:27:51 2023, max compression
```

## Comparing `GridPythonModule-0.1.0.tar` & `GridPythonModule-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 agnesebarbensi   (501) staff       (20)        0 2023-04-16 04:15:50.593622 GridPythonModule-0.1.0/
-drwxr-xr-x   0 agnesebarbensi   (501) staff       (20)        0 2023-04-16 04:15:50.592470 GridPythonModule-0.1.0/GridPythonModule/
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)    82061 2023-04-16 03:59:08.000000 GridPythonModule-0.1.0/GridPythonModule/GridPyM.py
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)       22 2023-04-16 03:40:12.000000 GridPythonModule-0.1.0/GridPythonModule/__init__.py
-drwxr-xr-x   0 agnesebarbensi   (501) staff       (20)        0 2023-04-16 04:15:50.593338 GridPythonModule-0.1.0/GridPythonModule.egg-info/
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)      482 2023-04-16 04:15:50.000000 GridPythonModule-0.1.0/GridPythonModule.egg-info/PKG-INFO
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)      282 2023-04-16 04:15:50.000000 GridPythonModule-0.1.0/GridPythonModule.egg-info/SOURCES.txt
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)        1 2023-04-16 04:15:50.000000 GridPythonModule-0.1.0/GridPythonModule.egg-info/dependency_links.txt
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)       25 2023-04-16 04:15:50.000000 GridPythonModule-0.1.0/GridPythonModule.egg-info/requires.txt
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)       17 2023-04-16 04:15:50.000000 GridPythonModule-0.1.0/GridPythonModule.egg-info/top_level.txt
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)    35149 2023-04-16 03:04:20.000000 GridPythonModule-0.1.0/LICENSE
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)      482 2023-04-16 04:15:50.593502 GridPythonModule-0.1.0/PKG-INFO
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)      394 2023-04-16 04:08:44.000000 GridPythonModule-0.1.0/README.md
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)       38 2023-04-16 04:15:50.593666 GridPythonModule-0.1.0/setup.cfg
--rw-r--r--   0 agnesebarbensi   (501) staff       (20)      704 2023-04-16 03:28:35.000000 GridPythonModule-0.1.0/setup.py
+drwxrwxr-x   0 springfield  (1000) springfield  (1000)        0 2023-05-29 08:27:51.239790 GridPythonModule-0.1.2/
+drwxrwxr-x   0 springfield  (1000) springfield  (1000)        0 2023-05-29 08:27:51.239790 GridPythonModule-0.1.2/GridPythonModule/
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)    81937 2023-05-29 08:18:08.000000 GridPythonModule-0.1.2/GridPythonModule/GridPyM.py
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)       22 2023-05-29 08:18:08.000000 GridPythonModule-0.1.2/GridPythonModule/__init__.py
+drwxrwxr-x   0 springfield  (1000) springfield  (1000)        0 2023-05-29 08:27:51.239790 GridPythonModule-0.1.2/GridPythonModule.egg-info/
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)      482 2023-05-29 08:27:51.000000 GridPythonModule-0.1.2/GridPythonModule.egg-info/PKG-INFO
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)      282 2023-05-29 08:27:51.000000 GridPythonModule-0.1.2/GridPythonModule.egg-info/SOURCES.txt
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)        1 2023-05-29 08:27:51.000000 GridPythonModule-0.1.2/GridPythonModule.egg-info/dependency_links.txt
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)       25 2023-05-29 08:27:51.000000 GridPythonModule-0.1.2/GridPythonModule.egg-info/requires.txt
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)       17 2023-05-29 08:27:51.000000 GridPythonModule-0.1.2/GridPythonModule.egg-info/top_level.txt
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)    35149 2023-05-29 08:18:08.000000 GridPythonModule-0.1.2/LICENSE
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)      482 2023-05-29 08:27:51.239790 GridPythonModule-0.1.2/PKG-INFO
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)     1480 2023-05-29 08:18:08.000000 GridPythonModule-0.1.2/README.md
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)       38 2023-05-29 08:27:51.239790 GridPythonModule-0.1.2/setup.cfg
+-rw-rw-r--   0 springfield  (1000) springfield  (1000)      704 2023-05-29 08:26:22.000000 GridPythonModule-0.1.2/setup.py
```

### Comparing `GridPythonModule-0.1.0/GridPythonModule/GridPyM.py` & `GridPythonModule-0.1.2/GridPythonModule/GridPyM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #########################################################################
-#          V1.1  20-09-22
+#          V1.2  29-05-23
 
 
 #          For any question, contact us at agnese.barbensi or 
 #          daniele.celoria  followed by @unimelb.edu.au
 
 
 #########################################################################
@@ -76,15 +76,15 @@
     5 crossings:
 
     5_1  5_2  
     
     """
     if  cr_number < 0 or cr_number > 8:
         raise Exception("We only have links up to 8 crossings!")
-    if cr_number not in [True, 3,4,5,6,7,8]:
+    elif cr_number not in [True, 3,4,5,6,7,8]:
         raise Exception("Invalid crossing number input")
     list_of_knots = ['3_1', '4_1', '5_1', '5_2', '6_1', '6_2', '6_3', '7_1', '7_2', '7_3', '7_4', '7_5', '7_6', '7_7', '8_1', '8_2', '8_3', '8_4', '8_5', '8_6', '8_7', '8_8', '8_9', '8_10', '8_11', '8_12', '8_13', '8_14', '8_15', '8_16', '8_17', '8_18', '8_19', '8_20', '8_21']
     if cr_number == True or cr_number == 3:
         print('3 crossings:\n',list_of_knots[0],'\n')
     if cr_number == True or cr_number == 4:
         print('4 crossings:\n',list_of_knots[1],'\n')
     if cr_number == True or cr_number == 5:
@@ -125,15 +125,15 @@
     >> available_legendrian_knots(5)
     5 crossings:
 
     5_1  m(5_1)  5_2  m(5_2)
     
     """
     if  cr_number <= 0 or cr_number > 7:
-        raise Exception("We only have nontrivial knots up to 8 crossings!")
+        raise Exception("We only have nontrivial knots up to 7 crossings!")
     if cr_number not in [True, 3,4,5,6,7]:
         raise Exception("Invalid input")
     list_of_knots = ['3_1', 'm(3_1)', '4_1', '5_1', 'm(5_1)', '5_2', 'm(5_2)', '6_1', 'm(6_1)', '6_2', 'm(6_2)', '6_3', '7_1', 'm(7_1)', '7_2', 'm(7_2)', '7_3', 'm(7_3)', '7_4', 'm(7_4)', '7_5', 'm(7_5)', '7_6', 'm(7_6)', '7_7', 'm(7_7)']
     if cr_number == True or cr_number == 3:
         print('3 crossings:\n')
         for el in list_of_knots[:2]:
             print(el,' ', end="")
@@ -214,16 +214,16 @@
         raise Exception("Invalid input, the only options are 'rows', 'r', 'columns', 'c'.")
     if check_grid(input_grid) == 1:
         raise Exception("Invalid Input grid")
     if (which == 'r' or which == 'rows') and _check_rows_for_bands(input_grid,where)[0] != 0: 
         raise Exception("The selected rows/columns are not a band attachment site")   
     if (which == 'c' or which == 'columns') and _check_rows_for_bands(rotate(input_grid,1),where)[0] != 0:
         raise Exception("The selected rows/columns are not a band attachment site")
-    A = input_grid[0]
-    B = input_grid[1]
+    A = input_grid[0].copy()
+    B = input_grid[1].copy()
     if which == 'rows' or which == 'r':    
         remember = [A[where], A[where+1]]
         A[where] = remember[1]
         A[where+1] = remember[0]
         return(A,B)
     if which == 'columns' or which == 'c':
         AA,BB = rotate([A,B],1)
@@ -245,25 +245,19 @@
     is always performed (unless the adjacent markings at the same height).
 
     OUTPUT:
 
     A grid where the two selected rows are commuted, according to the interleaving
     parameter.
 
-    EXAMPLES::
-    
-    >> A = [[2, 3, 0, 1, 4], [3, 4, 1, 0, 2]]
-    >> B = commute_columns(A,1)
-    >> B
-    [[1, 3, 0, 2, 4], [3, 4, 2, 0, 1]]
     
     """
     if check_grid(input_grid) == 1:
         raise Exception("Invalid Input grid")
-    if where > len(input_grid[0]) or where < 0 or interleaving not in ['A','Y','N']:
+    if where > len(input_grid[0]) -1 or where < 0 or interleaving not in ['A','Y','N']:
         raise Exception("Invalid parameters")
     A = input_grid[0]
     B = input_grid[1]
     if _check_rows(input_grid, where) == 5:
         return 0
     if interleaving == 'A':
         return([A[:where] + [A[where+1]] + [A[where]] + A[where+2:],B[:where] + [B[where+1]] + [B[where]] + B[where+2:]])
@@ -1649,15 +1643,15 @@
     [[0, 1, 2, 3, 4, 5, 6], [4, 5, 6, 0, 1, 2, 3]]
     >> stabilisation(G, 2, kind = 'XNW')
     [[0, 1, 2, 3, 4, 5, 6, 7], [5, 6, 3, 7, 0, 1, 2, 4]]
     
     """
     if check_grid(input_grid) == 1:
         raise Exception("Invalid Input")
-    if kind not in ['XNE','XNW','XSE','XSW','ONE','ONW','OSE','OSW'] or 0 > row  or  row > len(input_grid[0]) :
+    if kind not in ['XNE','XNW','XSE','XSW','ONE','ONW','OSE','OSW'] or 0 > row  or  row > len(input_grid[0]) -1 :
         raise Exception("Invalid kind of stabilisation!")
     n = len(input_grid[0])
     if kind[0] == 'X':
         Oflag = False
         A,B = input_grid
     else:
         Oflag = True
```

### Comparing `GridPythonModule-0.1.0/LICENSE` & `GridPythonModule-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GridPythonModule-0.1.0/setup.py` & `GridPythonModule-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='GridPythonModule',
-    version='0.1.0',    
+    version='0.1.2',    
     description='A Sage compatible Python module to manipulate and simplify grid diagrams.',
     url='https://github.com/agnesedaniele/GridPythonModule',
     author='Agnese Barbensi and Daniele Celoria',
     author_email='dceloria.maths@gmail.com',
     license='GNU general public',
     packages=['GridPythonModule'],
     install_requires=['simpy',
```

