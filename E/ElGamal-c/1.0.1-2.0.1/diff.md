# Comparing `tmp/ElGamal_c-1.0.1.tar.gz` & `tmp/ElGamal_c-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElGamal_c-1.0.1.tar", last modified: Sat May 27 23:53:26 2023, max compression
+gzip compressed data, was "ElGamal_c-2.0.1.tar", last modified: Mon May 29 16:22:27 2023, max compression
```

## Comparing `ElGamal_c-1.0.1.tar` & `ElGamal_c-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 23:53:26.528083 ElGamal_c-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-27 23:53:26.528083 ElGamal_c-1.0.1/ElGamal_c.egg-info/
--rw-rw-rw-   0        0        0      863 2023-05-27 23:53:26.000000 ElGamal_c-1.0.1/ElGamal_c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-05-27 23:53:26.000000 ElGamal_c-1.0.1/ElGamal_c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 23:53:26.000000 ElGamal_c-1.0.1/ElGamal_c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 23:53:26.000000 ElGamal_c-1.0.1/ElGamal_c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      863 2023-05-27 23:53:26.528083 ElGamal_c-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9714 2023-05-27 23:26:46.000000 ElGamal_c-1.0.1/encryptmodule.c
--rw-rw-rw-   0        0        0       42 2023-05-27 23:53:26.528083 ElGamal_c-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1261 2023-05-27 23:51:25.000000 ElGamal_c-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:22:27.491795 ElGamal_c-2.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-29 16:22:27.489398 ElGamal_c-2.0.1/ElGamal_c.egg-info/
+-rw-rw-rw-   0        0        0      863 2023-05-29 16:22:27.000000 ElGamal_c-2.0.1/ElGamal_c.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-05-29 16:22:27.000000 ElGamal_c-2.0.1/ElGamal_c.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 16:22:27.000000 ElGamal_c-2.0.1/ElGamal_c.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 16:22:27.000000 ElGamal_c-2.0.1/ElGamal_c.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      863 2023-05-29 16:22:27.491795 ElGamal_c-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9615 2023-05-29 16:15:19.000000 ElGamal_c-2.0.1/encryptmodule.c
+-rw-rw-rw-   0        0        0       42 2023-05-29 16:22:27.491795 ElGamal_c-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1261 2023-05-29 16:18:29.000000 ElGamal_c-2.0.1/setup.py
```

### Comparing `ElGamal_c-1.0.1/ElGamal_c.egg-info/PKG-INFO` & `ElGamal_c-2.0.1/ElGamal_c.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElGamal-c
-Version: 1.0.1
+Version: 2.0.1
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ElGamal_c-1.0.1/PKG-INFO` & `ElGamal_c-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElGamal_c
-Version: 1.0.1
+Version: 2.0.1
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ElGamal_c-1.0.1/encryptmodule.c` & `ElGamal_c-2.0.1/encryptmodule.c`

 * *Files 1% similar despite different names*

```diff
@@ -68,33 +68,29 @@
             count++;
             if (count==2) return i;
         }
     }
     return 2;
 } 
 
-long long cget_second_primitive_root_loop(long long p){
+long long cget_first_primitive_root_loop(long long p){
 
     long long o = 1;
     long long k;
-    long long z = 0;
     
     for (long long r = 2; r < p; r++) {
         k = cpow_mod(r, o, p);
 
         while (k > 1) {
             o++;
             k *= r;
             k %= p;
         }
         if (o == (p - 1)) {
-            // roots[z] = r;
-            z++;
-            if (z==2)
-                return r;
+            return r;
         }
         o = 1;
     }
 
 } 
 
 
@@ -111,15 +107,15 @@
     return cpow_mod(g, secret, p);
 }
 
 void gen_g(int*g, int p){
     *g = cget_second_primitive_root(p);
 }
 void gen_g_FAST(int *g, int p){
-    *g = cget_second_primitive_root_loop(p);
+    *g = cget_first_primitive_root_loop(p);
 }
 
 void gen_e(int*e, int g, int x_secret, int p){
     *e = cpow_mod(g, x_secret, p);
 }
 
 void gen_keys(int* g, int x_secret, int* e, int p){
```

### Comparing `ElGamal_c-1.0.1/setup.py` & `ElGamal_c-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 This module have been made for the project of discret math CSC281 at ksu university.
 The project supervisor is Aqil Alazimi. LinkedIn: https://www.linkedin.com/in/aqil-azmi-20903960/
 The project repo is: https://github.com/Wouze/csc281-project
 """
 
 setup(name="ElGamal_c",
-      version="1.0.1",
+      version="2.0.1",
       author="Wouze (Mohammad)",
       author_email="m7mdwats1@hotmail.com",
       description="This module is for csc281 encryption project ",
       long_description_content_type="text/markdown",
       long_description=long_description,
       url='https://github.com/Wouze/csc281-project',
       keywords=['python', 'c', 'primitive root', 'encryption', 'algamal', 'prime'],
```

