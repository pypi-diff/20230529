# Comparing `tmp/relativedate-1.3.1.tar.gz` & `tmp/relativedate-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relativedate-1.3.1.tar", last modified: Thu May 25 11:49:55 2023, max compression
+gzip compressed data, was "relativedate-1.3.2.tar", last modified: Mon May 29 20:15:27 2023, max compression
```

## Comparing `relativedate-1.3.1.tar` & `relativedate-1.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 11:49:55.800966 relativedate-1.3.1/
--rw-rw-rw-   0        0        0     2414 2023-05-25 11:49:55.799969 relativedate-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2254 2023-05-24 11:24:35.000000 relativedate-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 11:49:55.759082 relativedate-1.3.1/relativedate/
--rw-rw-rw-   0        0        0     2004 2023-05-25 11:32:43.000000 relativedate-1.3.1/relativedate/__init__.py
--rw-rw-rw-   0        0        0      945 2023-05-24 12:43:06.000000 relativedate-1.3.1/relativedate/dtget.py
--rw-rw-rw-   0        0        0     1243 2023-05-25 11:28:49.000000 relativedate-1.3.1/relativedate/dtmath.py
-drwxrwxrwx   0        0        0        0 2023-05-25 11:49:55.796976 relativedate-1.3.1/relativedate.egg-info/
--rw-rw-rw-   0        0        0     2414 2023-05-25 11:49:55.000000 relativedate-1.3.1/relativedate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-25 11:49:55.000000 relativedate-1.3.1/relativedate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 11:49:55.000000 relativedate-1.3.1/relativedate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 11:49:55.000000 relativedate-1.3.1/relativedate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 11:49:55.801963 relativedate-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      455 2023-05-25 11:49:17.000000 relativedate-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:15:27.054959 relativedate-1.3.2/
+-rw-rw-rw-   0        0        0     2414 2023-05-29 20:15:27.053961 relativedate-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2254 2023-05-24 11:24:35.000000 relativedate-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 20:15:27.043987 relativedate-1.3.2/relativedate/
+-rw-rw-rw-   0        0        0     2030 2023-05-29 20:11:29.000000 relativedate-1.3.2/relativedate/__init__.py
+-rw-rw-rw-   0        0        0     1095 2023-05-29 20:12:04.000000 relativedate-1.3.2/relativedate/dtget.py
+-rw-rw-rw-   0        0        0     1243 2023-05-25 11:28:49.000000 relativedate-1.3.2/relativedate/dtmath.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:15:27.052965 relativedate-1.3.2/relativedate.egg-info/
+-rw-rw-rw-   0        0        0     2414 2023-05-29 20:15:26.000000 relativedate-1.3.2/relativedate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-29 20:15:26.000000 relativedate-1.3.2/relativedate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 20:15:26.000000 relativedate-1.3.2/relativedate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 20:15:26.000000 relativedate-1.3.2/relativedate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 20:15:27.054959 relativedate-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      455 2023-05-29 20:15:24.000000 relativedate-1.3.2/setup.py
```

### Comparing `relativedate-1.3.1/PKG-INFO` & `relativedate-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relativedate
-Version: 1.3.1
+Version: 1.3.2
 Summary: Pacote Python para tabalhar com Datas Relativas
 Description-Content-Type: text/markdown
 
 <h1>Python Package: relativedate</h1>
 
 <b>Descrição:</b>
 <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: relativedate Version: 1.3.1 Summary: Pacote Python
+Metadata-Version: 2.1 Name: relativedate Version: 1.3.2 Summary: Pacote Python
 para tabalhar com Datas Relativas Description-Content-Type: text/markdown
 ****** Python Package: relativedate ******
 DescriÃ§Ã£o:
 Biblioteca Python relacionada a datas, onde Ã© criado um objeto "RelativeDate"
 que possui o atributo datetime, onde Ã© retornado um objeto datetime.
 O objetivo desta biblioteca Ã© facilitar a manipulaÃ§Ã£o de datas relativas e
 calculos com datas, em sua primeira versÃ£o estamos trabalhando apenas com a
```

### Comparing `relativedate-1.3.1/README.md` & `relativedate-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `relativedate-1.3.1/relativedate/__init__.py` & `relativedate-1.3.2/relativedate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,12 +54,12 @@
     ### DATE GET ###
     def lastDay(self):
         return dtget.lastDay(self.datetime)
     
     def lastDate(self):
         return dtget.lastDate(self.datetime)
     
-    def getUtilDay(self, util_day, disregard=[]):
-        return dtget.getUtilDay(self.datetime, util_day, disregard)
+    def getUtilDay(self, util_day, disregard=[], last_day=False):
+        return dtget.getUtilDay(self.datetime, util_day, disregard, last_day)
 
     def utilDays(self, disregard=[]):
         return dtget.utilDays(self.datetime, disregard)
```

### Comparing `relativedate-1.3.1/relativedate/dtget.py` & `relativedate-1.3.2/relativedate/dtget.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,25 @@
     dt = addMonth(dt, 1) # Calcula para o Próximo Mês
     dt = addDay(dt.replace(day=1), -1) # Altera a data para o dia 1 e remove 1 dia
     return dt.day
 
 def lastDate(dt):    
     return dt.replace(day=lastDay(dt), hour=0, minute=0, second=0, microsecond=0)
 
-def getUtilDay(dt, util_day, disregard=[]):
+def getUtilDay(dt, util_day, disregard=[], last_day=False):
     util_day = util_day
     util = 0
+    retorno = None
     for day in [datetime(dt.year, dt.month, d) for d in range(1, lastDay(dt)+1)]:
         if day.weekday() not in (5,6) and day.day not in disregard:
             util += 1
             if util == util_day:
-                return day
+                retorno = day                   
+    return retorno if retorno is not None or last_day is False else lastDate(dt)
+        
             
 def utilDays(dt, disregard=[]):
     util = 0
     for day in [datetime(dt.year, dt.month, d) for d in range(1, lastDay(dt)+1)]:
         if day.weekday() not in (5,6) and day.day not in disregard:
             util += 1
     return util
```

### Comparing `relativedate-1.3.1/relativedate/dtmath.py` & `relativedate-1.3.2/relativedate/dtmath.py`

 * *Files identical despite different names*

### Comparing `relativedate-1.3.1/relativedate.egg-info/PKG-INFO` & `relativedate-1.3.2/relativedate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relativedate
-Version: 1.3.1
+Version: 1.3.2
 Summary: Pacote Python para tabalhar com Datas Relativas
 Description-Content-Type: text/markdown
 
 <h1>Python Package: relativedate</h1>
 
 <b>Descrição:</b>
 <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: relativedate Version: 1.3.1 Summary: Pacote Python
+Metadata-Version: 2.1 Name: relativedate Version: 1.3.2 Summary: Pacote Python
 para tabalhar com Datas Relativas Description-Content-Type: text/markdown
 ****** Python Package: relativedate ******
 DescriÃ§Ã£o:
 Biblioteca Python relacionada a datas, onde Ã© criado um objeto "RelativeDate"
 que possui o atributo datetime, onde Ã© retornado um objeto datetime.
 O objetivo desta biblioteca Ã© facilitar a manipulaÃ§Ã£o de datas relativas e
 calculos com datas, em sua primeira versÃ£o estamos trabalhando apenas com a
```

