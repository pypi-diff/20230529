# Comparing `tmp/MyDataSort001-0.0.3-py3-none-any.whl.zip` & `tmp/MyDataSort001-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3458 bytes, number of entries: 6
+Zip file size: 3473 bytes, number of entries: 6
 -rw-r--r--  2.0 unx     3488 b- defN 23-May-29 05:03 mySort/Sort.py
--rw-r--r--  2.0 unx     1062 b- defN 23-May-29 05:51 MyDataSort001-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      732 b- defN 23-May-29 05:51 MyDataSort001-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 05:51 MyDataSort001-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-29 05:51 MyDataSort001-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      485 b- defN 23-May-29 05:51 MyDataSort001-0.0.3.dist-info/RECORD
-6 files, 5866 bytes uncompressed, 2574 bytes compressed:  56.1%
+-rw-r--r--  2.0 unx     1062 b- defN 23-May-29 05:58 MyDataSort001-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      749 b- defN 23-May-29 05:58 MyDataSort001-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 05:58 MyDataSort001-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-29 05:58 MyDataSort001-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      485 b- defN 23-May-29 05:58 MyDataSort001-0.0.4.dist-info/RECORD
+6 files, 5883 bytes uncompressed, 2589 bytes compressed:  56.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: mySort/Sort.py
 Comment: 
 
-Filename: MyDataSort001-0.0.3.dist-info/LICENSE
+Filename: MyDataSort001-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: MyDataSort001-0.0.3.dist-info/METADATA
+Filename: MyDataSort001-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: MyDataSort001-0.0.3.dist-info/WHEEL
+Filename: MyDataSort001-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: MyDataSort001-0.0.3.dist-info/top_level.txt
+Filename: MyDataSort001-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: MyDataSort001-0.0.3.dist-info/RECORD
+Filename: MyDataSort001-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `MyDataSort001-0.0.3.dist-info/LICENSE` & `MyDataSort001-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MyDataSort001-0.0.3.dist-info/METADATA` & `MyDataSort001-0.0.4.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: MyDataSort001
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is pip, which is a collection of functions used for data structures.
 Home-page: https://github.com/YGC20
 Download-URL: https://github.com/YGC20
 Author: YGC20
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # MyDataSort001
 ## 이 PIP 파일은 데이터 구조의 정렬부분을 구현했습니다.
-데이터 구조 정렬의 Bubble sort, Insertion sort, Selection sort, Merge sort, Quick sort, Shell sort, Heap sort를 구현했습니다.
-사용 방법 :
-'''python
+데이터 구조 정렬의 Bubble sort, Insertion sort, Selection sort, Merge sort, Quick sort, Shell sort, Heap sort를 구현했습니다.   사용 방법 :   
+<pre><code>
 from mySort import Sort
 
 B = [4,24,8,2,34,2,1,9,2]
 A=Sort.Quick(B)
 print(A)
-'''
+</code></pre>
```

