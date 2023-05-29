# Comparing `tmp/ajm1102pandemic2d-0.3-py3-none-any.whl.zip` & `tmp/ajm1102pandemic2d-0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 5105 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-29 19:00 ajm1102pandemic2d/__init__.py
+Zip file size: 7283 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       47 b- defN 23-May-29 19:26 ajm1102pandemic2d/__init__.py
 -rw-rw-rw-  2.0 fat       41 b- defN 23-May-29 19:00 ajm1102pandemic2d/boundary_class.py
 -rw-rw-rw-  2.0 fat     2471 b- defN 23-May-29 18:57 ajm1102pandemic2d/person_class.py
 -rw-rw-rw-  2.0 fat     7453 b- defN 23-May-29 18:59 ajm1102pandemic2d/simulation.py
+-rw-rw-rw-  2.0 fat     7453 b- defN 23-May-29 18:59 ajm1102pandemic2d/simulation_class.py
 -rw-rw-rw-  2.0 fat       89 b- defN 23-May-29 18:59 ajm1102pandemic2d/virus_class.py
--rw-rw-rw-  2.0 fat      288 b- defN 23-May-29 19:18 ajm1102pandemic2d-0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 19:18 ajm1102pandemic2d-0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-29 19:18 ajm1102pandemic2d-0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      768 b- defN 23-May-29 19:18 ajm1102pandemic2d-0.3.dist-info/RECORD
-9 files, 11261 bytes uncompressed, 3759 bytes compressed:  66.6%
+-rw-rw-rw-  2.0 fat      288 b- defN 23-May-29 19:29 ajm1102pandemic2d-0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 19:29 ajm1102pandemic2d-0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-29 19:29 ajm1102pandemic2d-0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      862 b- defN 23-May-29 19:29 ajm1102pandemic2d-0.4.dist-info/RECORD
+10 files, 18814 bytes uncompressed, 5787 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: ajm1102pandemic2d/person_class.py
 Comment: 
 
 Filename: ajm1102pandemic2d/simulation.py
 Comment: 
 
+Filename: ajm1102pandemic2d/simulation_class.py
+Comment: 
+
 Filename: ajm1102pandemic2d/virus_class.py
 Comment: 
 
-Filename: ajm1102pandemic2d-0.3.dist-info/METADATA
+Filename: ajm1102pandemic2d-0.4.dist-info/METADATA
 Comment: 
 
-Filename: ajm1102pandemic2d-0.3.dist-info/WHEEL
+Filename: ajm1102pandemic2d-0.4.dist-info/WHEEL
 Comment: 
 
-Filename: ajm1102pandemic2d-0.3.dist-info/top_level.txt
+Filename: ajm1102pandemic2d-0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ajm1102pandemic2d-0.3.dist-info/RECORD
+Filename: ajm1102pandemic2d-0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ajm1102pandemic2d/__init__.py

```diff
@@ -1,4 +1,4 @@
 
-from simulation import simulation
+from simulation_class import simulation
```

## Comparing `ajm1102pandemic2d-0.3.dist-info/RECORD` & `ajm1102pandemic2d-0.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-ajm1102pandemic2d/__init__.py,sha256=jg9gFx65M-VLLil2jNbzIRf9kLuwLSFqJQ3Y2iSJf9w,41
+ajm1102pandemic2d/__init__.py,sha256=URoPq8QgbGhPdRtFKYKCZP9ybfpLYmDSQ-loZEQosMA,47
 ajm1102pandemic2d/boundary_class.py,sha256=l80HX2L6N6JV9Md8TfBMh3Za67IuzOJd0LrmcbfLCn4,41
 ajm1102pandemic2d/person_class.py,sha256=HIKX3OMHk0nxV3ffqsT1_-lSycZbVCu-CgEm-aRUQ4g,2471
 ajm1102pandemic2d/simulation.py,sha256=YXrnErWjo6OcJsuANdVqExtH1XVN8sgLZEVGZPfj9Qo,7453
+ajm1102pandemic2d/simulation_class.py,sha256=YXrnErWjo6OcJsuANdVqExtH1XVN8sgLZEVGZPfj9Qo,7453
 ajm1102pandemic2d/virus_class.py,sha256=As7sO_UmR3Qmxem_iN2KfDNoRfPzmLd48-jI3XIilvY,89
-ajm1102pandemic2d-0.3.dist-info/METADATA,sha256=M7VZiBql7yOcrKlwx9KgtRrpjMYLPEye0CGwZbyN_0E,288
-ajm1102pandemic2d-0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ajm1102pandemic2d-0.3.dist-info/top_level.txt,sha256=dbfceC_sctK0vAYrIzSWVbe0sDDJvnEH6I6n4F6tCrc,18
-ajm1102pandemic2d-0.3.dist-info/RECORD,,
+ajm1102pandemic2d-0.4.dist-info/METADATA,sha256=DOaLJ5DnK-NHhyra6_f9ozT80HCXAKhXsin1pXrgvy0,288
+ajm1102pandemic2d-0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ajm1102pandemic2d-0.4.dist-info/top_level.txt,sha256=dbfceC_sctK0vAYrIzSWVbe0sDDJvnEH6I6n4F6tCrc,18
+ajm1102pandemic2d-0.4.dist-info/RECORD,,
```

