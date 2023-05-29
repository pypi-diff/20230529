# Comparing `tmp/digikuery-20230529.tar.gz` & `tmp/digikuery-20230529.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digikuery-20230529.tar", last modified: Mon May 29 18:29:18 2023, max compression
+gzip compressed data, was "digikuery-20230529.post2.tar", last modified: Mon May 29 19:21:38 2023, max compression
```

## Comparing `digikuery-20230529.tar` & `digikuery-20230529.post2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 18:29:18.139195 digikuery-20230529/
--rw-rw-r--   0 l         (1000) l         (1000)     3073 2023-05-29 18:29:18.139195 digikuery-20230529/PKG-INFO
--rw-r--r--   0 l         (1000) l         (1000)     2750 2023-05-29 18:26:58.000000 digikuery-20230529/README.md
--rw-rw-r--   0 l         (1000) l         (1000)      593 2023-05-29 18:24:36.000000 digikuery-20230529/pyproject.toml
--rw-rw-r--   0 l         (1000) l         (1000)       38 2023-05-29 18:29:18.139195 digikuery-20230529/setup.cfg
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 18:29:18.138195 digikuery-20230529/src/
--rw-rw-r--   0 l         (1000) l         (1000)        0 2023-05-29 18:19:46.000000 digikuery-20230529/src/__init__.py
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 18:29:18.139195 digikuery-20230529/src/digikuery.egg-info/
--rw-rw-r--   0 l         (1000) l         (1000)     3073 2023-05-29 18:29:18.000000 digikuery-20230529/src/digikuery.egg-info/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)      281 2023-05-29 18:29:18.000000 digikuery-20230529/src/digikuery.egg-info/SOURCES.txt
--rw-rw-r--   0 l         (1000) l         (1000)        1 2023-05-29 18:29:18.000000 digikuery-20230529/src/digikuery.egg-info/dependency_links.txt
--rw-rw-r--   0 l         (1000) l         (1000)       45 2023-05-29 18:29:18.000000 digikuery-20230529/src/digikuery.egg-info/entry_points.txt
--rw-rw-r--   0 l         (1000) l         (1000)       11 2023-05-29 18:29:18.000000 digikuery-20230529/src/digikuery.egg-info/requires.txt
--rw-rw-r--   0 l         (1000) l         (1000)       19 2023-05-29 18:29:18.000000 digikuery-20230529/src/digikuery.egg-info/top_level.txt
--rwxr-xr-x   0 l         (1000) l         (1000)    12238 2023-05-29 18:22:50.000000 digikuery-20230529/src/digikuery.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 19:21:38.441291 digikuery-20230529.post2/
+-rw-rw-r--   0 l         (1000) l         (1000)     3753 2023-05-29 19:21:38.441291 digikuery-20230529.post2/PKG-INFO
+-rw-r--r--   0 l         (1000) l         (1000)     3424 2023-05-29 19:20:05.000000 digikuery-20230529.post2/README.md
+-rw-rw-r--   0 l         (1000) l         (1000)      593 2023-05-29 18:24:36.000000 digikuery-20230529.post2/pyproject.toml
+-rw-rw-r--   0 l         (1000) l         (1000)       38 2023-05-29 19:21:38.441291 digikuery-20230529.post2/setup.cfg
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 19:21:38.441291 digikuery-20230529.post2/src/
+-rw-rw-r--   0 l         (1000) l         (1000)        0 2023-05-29 18:19:46.000000 digikuery-20230529.post2/src/__init__.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 19:21:38.441291 digikuery-20230529.post2/src/digikuery.egg-info/
+-rw-rw-r--   0 l         (1000) l         (1000)     3753 2023-05-29 19:21:38.000000 digikuery-20230529.post2/src/digikuery.egg-info/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)      281 2023-05-29 19:21:38.000000 digikuery-20230529.post2/src/digikuery.egg-info/SOURCES.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        1 2023-05-29 19:21:38.000000 digikuery-20230529.post2/src/digikuery.egg-info/dependency_links.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       45 2023-05-29 19:21:38.000000 digikuery-20230529.post2/src/digikuery.egg-info/entry_points.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       11 2023-05-29 19:21:38.000000 digikuery-20230529.post2/src/digikuery.egg-info/requires.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       19 2023-05-29 19:21:38.000000 digikuery-20230529.post2/src/digikuery.egg-info/top_level.txt
+-rwxr-xr-x   0 l         (1000) l         (1000)    12579 2023-05-29 19:20:54.000000 digikuery-20230529.post2/src/digikuery.py
```

### Comparing `digikuery-20230529/PKG-INFO` & `digikuery-20230529.post2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: digikuery
-Version: 20230529
-Summary: Digikam database query tool
-Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
-License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/looran/digikuery
-Keywords: digikam,database,query
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-
 digikuery is a script to perform queries in [digikam](https://www.digikam.org/) (photo manager) database.
 
 It can
 * Query albums which contains tags matching a given regex
 * Query most used tags and corresponding albums
 * Print other tags present in matching albums
 * List digikam database structure
@@ -94,10 +83,37 @@
         TagAccess/Walking (9), TagAccess/Train(1)
       album_grece
 		TagAccess/Car(6), TagAccess/Walking (3)
       album_albanie
 		TagAccess/Walking (5)
 ```
 
+## Interactive shell in database
+
+```
+$ digikuery shell
+Interactive mode help:
+   available objects
+      dk.session
+         dk.session.query(Album).count()
+         dk.session.query(AlbumRoot).all()
+         dk.session.query(Image).filter(Image.name == 'example.png').all()
+         dk.session.query(Album, Tag, sqlalchemy.func.count(Tag.name)).join(imagetag).join(Image).join(Album)
+      dk.engine
+         access sqlalchemy engine
+      dk.metadata
+         access sqlalchemy metadata
+   available functions
+      help()
+         print this message
+      dk.query_album(album)
+      dk.query_tag(tag)
+      dk.schema()
+      dk.stats()
+running ipython...
+
+In [1]:
+```
+
 ## Internals
 
 digikuery uses sqlalchemy to map digikam database to python objects.
```

### Comparing `digikuery-20230529/README.md` & `digikuery-20230529.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: digikuery
+Version: 20230529.post2
+Summary: Digikam database query tool
+Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/looran/digikuery
+Keywords: digikam,database,query
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+
 digikuery is a script to perform queries in [digikam](https://www.digikam.org/) (photo manager) database.
 
 It can
 * Query albums which contains tags matching a given regex
 * Query most used tags and corresponding albums
 * Print other tags present in matching albums
 * List digikam database structure
@@ -83,10 +94,37 @@
         TagAccess/Walking (9), TagAccess/Train(1)
       album_grece
 		TagAccess/Car(6), TagAccess/Walking (3)
       album_albanie
 		TagAccess/Walking (5)
 ```
 
+## Interactive shell in database
+
+```
+$ digikuery shell
+Interactive mode help:
+   available objects
+      dk.session
+         dk.session.query(Album).count()
+         dk.session.query(AlbumRoot).all()
+         dk.session.query(Image).filter(Image.name == 'example.png').all()
+         dk.session.query(Album, Tag, sqlalchemy.func.count(Tag.name)).join(imagetag).join(Image).join(Album)
+      dk.engine
+         access sqlalchemy engine
+      dk.metadata
+         access sqlalchemy metadata
+   available functions
+      help()
+         print this message
+      dk.query_album(album)
+      dk.query_tag(tag)
+      dk.schema()
+      dk.stats()
+running ipython...
+
+In [1]:
+```
+
 ## Internals
 
 digikuery uses sqlalchemy to map digikam database to python objects.
```

### Comparing `digikuery-20230529/pyproject.toml` & `digikuery-20230529.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `digikuery-20230529/src/digikuery.egg-info/PKG-INFO` & `digikuery-20230529.post2/src/digikuery.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digikuery
-Version: 20230529
+Version: 20230529.post2
 Summary: Digikam database query tool
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/digikuery
 Keywords: digikam,database,query
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
@@ -94,10 +94,37 @@
         TagAccess/Walking (9), TagAccess/Train(1)
       album_grece
 		TagAccess/Car(6), TagAccess/Walking (3)
       album_albanie
 		TagAccess/Walking (5)
 ```
 
+## Interactive shell in database
+
+```
+$ digikuery shell
+Interactive mode help:
+   available objects
+      dk.session
+         dk.session.query(Album).count()
+         dk.session.query(AlbumRoot).all()
+         dk.session.query(Image).filter(Image.name == 'example.png').all()
+         dk.session.query(Album, Tag, sqlalchemy.func.count(Tag.name)).join(imagetag).join(Image).join(Album)
+      dk.engine
+         access sqlalchemy engine
+      dk.metadata
+         access sqlalchemy metadata
+   available functions
+      help()
+         print this message
+      dk.query_album(album)
+      dk.query_tag(tag)
+      dk.schema()
+      dk.stats()
+running ipython...
+
+In [1]:
+```
+
 ## Internals
 
 digikuery uses sqlalchemy to map digikam database to python objects.
```

### Comparing `digikuery-20230529/src/digikuery.py` & `digikuery-20230529.post2/src/digikuery.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # external ressources for digikam sqlite or sqlalchemy
 # * 2020 digikam+sqlite https://github.com/clutterstack/digikam-to-tiddlywiki/blob/master/Digikam%20to%20TiddlyWiki.ipynb
 # * 2019 digikam+sqlite https://github.com/ksmathers/digikam-migrate/blob/master/migrate_thumbnails.py
 # * 2018 digikam+sqlite https://github.com/lsaffre/picsel/blob/master/digikam2blog.py
 # * 2008 digikam+sqlalchemy http://blog.mekk.waw.pl/archives/12-Moving-images-from-F-Spot-to-digiKam.html
 
-VERSION = "20230529"
+VERSION = "20230529-2"
 DESCRIPTION = 'Digikam database query tool'
 EXAMPLES = """examples:
 List albums when tag 'Paquerette' is present, together with other tags of this album
 $ digikuery tag Paquerette
 """
 
 import re
@@ -32,17 +32,23 @@
         Column('imageid', ForeignKey('Images.id'), primary_key=True),
         Column('tagid', ForeignKey('Tags.id'), primary_key=True)
 )
 
 def help():
     print("""Interactive mode help:
    available objects
-      dk.engine
       dk.session
+         dk.session.query(Album).count()
+         dk.session.query(AlbumRoot).all()
+         dk.session.query(Image).filter(Image.name == 'example.png').all()
+         dk.session.query(Album, Tag, sqlalchemy.func.count(Tag.name)).join(imagetag).join(Image).join(Album)
+      dk.engine
+         access sqlalchemy engine
       dk.metadata
+         access sqlalchemy metadata
    available functions
       help()
          print this message
       dk.query_album(album)
       dk.query_tag(tag)
       dk.schema()
       dk.stats()""")
```

