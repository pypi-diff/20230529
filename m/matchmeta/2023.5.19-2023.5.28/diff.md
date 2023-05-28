# Comparing `tmp/matchmeta-2023.5.19.tar.gz` & `tmp/matchmeta-2023.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchmeta-2023.5.19.tar", last modified: Sat May 20 00:43:42 2023, max compression
+gzip compressed data, was "matchmeta-2023.5.28.tar", last modified: Sun May 28 22:18:42 2023, max compression
```

## Comparing `matchmeta-2023.5.19.tar` & `matchmeta-2023.5.28.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/matchmeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/mmi/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/mmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/mmi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/mmi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/matchmeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/mmi/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/mmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/mmi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/mmi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/setup.py
```

### Comparing `matchmeta-2023.5.19/LICENSE` & `matchmeta-2023.5.28/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmeta-2023.5.19/mmi/cli.py` & `matchmeta-2023.5.28/mmi/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,180 +1,218 @@
-import asyncio
-import datetime
+import argparse
+import concurrent.futures
 import hashlib
 import pathlib
 import pybloomfilter
-import sys
 import requests
+import sys
 from mmi import __emptyfile__
-from mmi import __gtfo__
 from mmi import __knownfile__
 from mmi import __knownmeta__
 from mmi import __largefile__
-from mmi import __mmi__
 from mmi import __nofilehash__
 from mmi import __partialmeta__
+from mmi import __gtfo__
+from mmi import __mmi__
 from mmi import __version__
 
-BLOCKSIZE = 65536
+def check(sha256, mmi, gtfo):
 
-now = int(datetime.datetime.now().timestamp())
-update = pathlib.Path('/tmp/mmi.lastupdate')
+    value = {}
+    if sha256 in mmi:
+        value['meta'] = 'YES'
+    else:
+        value['meta'] = 'NO'
+    if sha256 in gtfo:
+        value['gtfo'] = 'YES'
+    else:
+        value['gtfo'] = 'NO'
+    return value
+
+def calculate(location):
 
-async def calculate(item):
     BLOCKSIZE = 65536
     sha256_hasher = hashlib.sha256()
-    with open('/tmp/'+item+'.bloom', 'rb') as f:
+    with open(location, 'rb') as f:
         buf = f.read(BLOCKSIZE)
         while len(buf) > 0:
             sha256_hasher.update(buf)
             buf = f.read(BLOCKSIZE)
     f.close()
     sha256 = sha256_hasher.hexdigest().upper()
     return sha256
 
-async def check(sha256, mmi, gtfo):
-    value = {}
-    if sha256 in mmi:
-        value['meta'] = 'YES'
+def download():
+
+    if __gtfo__.is_file() == False:
+        print('UPDATING: '+str(__gtfo__))
+        gtfobloom()
+        sha256 = gtfoverify()
+        check = calculate(__gtfo__)
+        if check != sha256:
+            print('CORRUPTED: '+str(__gtfo__))
+            sys.exit(1)
+        else:
+            print('VERIFIED: '+str(__gtfo__))
     else:
-        value['meta'] = 'NO'
-    if sha256 in gtfo:
-        value['gtfo'] = 'YES'
+        sha256 = gtfoverify()
+        check = calculate(__gtfo__)
+        if check != sha256:
+            print('UPDATING: '+str(__gtfo__))
+            gtfobloom()
+            check = calculate(__gtfo__)
+            if check != sha256:
+                print('CORRUPTED: '+str(__gtfo__))
+                sys.exit(1)
+            else:
+                print('VERIFIED: '+str(__gtfo__))
+        else:
+            print('CURRENT: '+str(__gtfo__))
+
+    if __mmi__.is_file() == False:
+        print('UPDATING: '+str(__mmi__))
+        mmibloom()
+        sha256 = mmiverify()
+        check = calculate(__mmi__)
+        if check != sha256:
+            print('CORRUPTED: '+str(__mmi__))
+            sys.exit(1)
+        else:
+            print('VERIFIED: '+str(__mmi__))
     else:
-        value['gtfo'] = 'NO'
-    return value
+        sha256 = mmiverify()
+        check = calculate(__mmi__)
+        if check != sha256:
+            print('UPDATING: '+str(__mmi__))
+            mmibloom()
+            check = calculate(__mmi__)
+            if check != sha256:
+                print('CORRUPTED: '+str(__mmi__))
+                sys.exit(1)
+            else:
+                print('VERIFIED: '+str(__mmi__))
+        else:
+            print('CURRENT: '+str(__mmi__))
+
+def gtfobloom():
 
-async def download(item):
-    r = requests.get('https://static.matchmeta.info/'+item+'.bloom')
+    r = requests.get('https://static.matchmeta.info/gtfo.bloom')
     if r.status_code == 200:
-        with open('/tmp/'+item+'.bloom', 'wb') as f:
+        with open(__gtfo__, 'wb') as f:
+            print('SUCCESS: https://static.matchmeta.info/gtfo.bloom')
             f.write(r.content)
     else:
-        print('FAILED: https://static.matchmeta.info/'+item+'.bloom')
+        print('FAILED: https://static.matchmeta.info/gtfo.bloom')
+        sys.exit(1)
+
+def gtfoverify():
+
+    r = requests.get('https://static.matchmeta.info/gtfo.sha256')
+    if r.status_code == 200:
+        print('SUCCESS: https://static.matchmeta.info/gtfo.sha256')
+        return r.text
+    else:
+        print('FAILED: https://static.matchmeta.info/gtfo.sha256')
         sys.exit(1)
 
-async def hasher(fullpath, mmi, gtfo):
+def hasher(fullpath, mmi, gtfo):
+
     try:
+        BLOCKSIZE = 65536
         sha256_hasher = hashlib.sha256()
         with open(fullpath,'rb') as afile:
             buf = afile.read(BLOCKSIZE)
             while len(buf) > 0:
                 sha256_hasher.update(buf)
                 buf = afile.read(BLOCKSIZE)
         sha256_file = sha256_hasher.hexdigest().upper()
     except:
         sha256_file = __nofilehash__.format('** N/A **                                                       ')
         pass
     if sha256_file == 'E3B0C44298FC1C149AFBF4C8996FB92427AE41E4649B934CA495991B7852B855':
         sha256_file = __emptyfile__.format('** EMPTY **                                                     ')
-    status = await check(sha256_file, mmi, gtfo)
+    status = check(sha256_file, mmi, gtfo)
     if status['meta'] == 'YES':
         sha256_file = __knownfile__.format(sha256_file)
     if status['gtfo'] == 'YES':
         gtfo_hash = __largefile__.format('H')
     else:
         gtfo_hash = ' '
     value = {}
     value['sha256'] = sha256_file
     value['gtfo'] = gtfo_hash
     return value
 
-async def metahash(fullpath, mmi, gtfo):
+def metahash(fullpath, mmi, gtfo):
+
     sha256_meta = hashlib.sha256()
     sha256_meta.update(fullpath.encode())
     sha256_hash = sha256_meta.hexdigest().upper()
-    status = await check(sha256_hash, mmi, gtfo)
+    status = check(sha256_hash, mmi, gtfo)
     return status
 
-async def normalize(path):
+def mmibloom():
+
+    r = requests.get('https://static.matchmeta.info/mmi.bloom')
+    if r.status_code == 200:
+        with open(__mmi__, 'wb') as f:
+            print('SUCCESS: https://static.matchmeta.info/mmi.bloom')
+            f.write(r.content)
+    else:
+        print('FAILED: https://static.matchmeta.info/mmi.bloom')
+        sys.exit(1)
+
+def mmiverify():
+
+    r = requests.get('https://static.matchmeta.info/mmi.sha256')
+    if r.status_code == 200:
+        print('SUCCESS: https://static.matchmeta.info/mmi.sha256')
+        return r.text
+    else:
+        print('FAILED: https://static.matchmeta.info/mmi.sha256')
+        sys.exit(1)
+
+def normalize(path):
+
     if path[:1] == '/':
         out = path.split('/')
         try:
-            if out[1] == 'home':
+            if out[1] == 'home':            ### LINUX
                 out[2] = 'user'
                 path = '/'.join(out)
+            elif out[1] == 'Users':         ### APPLE
+                if out[2] != 'Shared':
+                    out[2] = 'user'
+                    path = '/'.join(out)
         except:
             pass
     return path
 
-async def parsefilename(filename, mmi, gtfo):
+def parsefilename(filename, mmi, gtfo):
+
     if filename[:1] == '/':
         out = filename.split('/')
         count = len(out) - 1
-        status = await metahash(out[count], mmi, gtfo)
+        status = metahash(out[count], mmi, gtfo)
     return status
 
-async def parseonlypath(onlypath, mmi, gtfo):
+def parseonlypath(onlypath, mmi, gtfo):
+
     if onlypath[:1] == '/':
         out = onlypath.split('/')
         del out[-1]
         onlypath = '/'.join(out)
-        status = await metahash(onlypath, mmi, gtfo)
+        status = metahash(onlypath, mmi, gtfo)
     return status
 
-async def verify(item):
-    r = requests.get('https://static.matchmeta.info/'+item+'.sha256')
-    if r.status_code == 200:
-        return r.text
-    else:
-        print('FAILED: https://static.matchmeta.info/'+item+'.sha256')
-        sys.exit(1)
-
-async def start():
-
-    if __gtfo__.is_file() == False:
-        pathlib.Path(update).write_text(str(now + 3600))
-        await download('gtfo')
-        sha256 = await verify('gtfo')
-        check = await calculate('gtfo')
-        if check != sha256:
-            print('CORRUPTED: /tmp/gtfo.bloom')
-            sys.exit(1)
-    else:
-        checked = int(pathlib.Path(update).read_text())
-        if now > checked:
-            sha256 = await verify('gtfo')
-            check = await calculate('gtfo')
-            if check != sha256:
-                await download('gtfo')
-                check = await calculate('gtfo')
-                if check != sha256:
-                    print('CORRUPTED: /tmp/gtfo.bloom')
-                    sys.exit(1)
-            pathlib.Path(update).write_text(str(now + 3600))
-
-    if __mmi__.is_file() == False:
-        pathlib.Path(update).write_text(str(now + 3600))
-        await download('mmi')
-        sha256 = await verify('mmi')
-        check = await calculate('mmi')
-        if check != sha256:
-            print('CORRUPTED: /tmp/mmi.bloom')
-            sys.exit(1)
-    else:
-        checked = int(pathlib.Path(update).read_text())
-        if now > checked:
-            sha256 = await verify('mmi')
-            check = await calculate('mmi')
-            if check != sha256:
-                await download('mmi')
-                check = await calculate('mmi')
-                if check != sha256:
-                    print('CORRUPTED: /tmp/mmi.bloom')
-                    sys.exit(1)
-            pathlib.Path(update).write_text(str(now + 3600))
+def start(skip):
 
     mmi = pybloomfilter.BloomFilter.open(str(__mmi__))      ### MMI ###
     gtfo = pybloomfilter.BloomFilter.open(str(__gtfo__))    ### GTFO ###
 
-    print('|---------------------------------------')
-    print('| MatchMeta.Info v'+__version__+' (mmi) ')
-    print('|---------------------------------------')
-
     for p in pathlib.Path.cwd().iterdir():
         try:
             gtfo_file = ' '
             gtfo_hash = ' '
             gtfo_path = ' '
             isFile = p.is_file()
             isDir = p.is_dir()
@@ -185,34 +223,38 @@
                     size = 0
                     pass
                 if size == 0:
                     sha256 = __emptyfile__.format('** EMPTY **                                                     ')
                 elif size > 104857599:
                     sha256 = __largefile__.format('** LARGE **                                                     ')
                 else:
-                    value = await hasher(p, mmi, gtfo)
-                    gtfo_hash = value['gtfo']
-                    sha256 = value['sha256']
+                    if skip == False:
+                        value = hasher(p, mmi, gtfo)
+                        gtfo_hash = value['gtfo']
+                        sha256 = value['sha256']
+                    else:
+                        gtfo_hash = ' '
+                        sha256 = '                                                                '
             elif isDir == True:
                 sha256 = ' -- DIR --                                                      '
-            normalized = await normalize(str(p))
-            fullpath = await metahash(normalized, mmi, gtfo)
+            normalized = normalize(str(p))
+            fullpath = metahash(normalized, mmi, gtfo)
             if fullpath['gtfo'] == 'YES':
                 gtfo_path = __largefile__.format('P')
             if fullpath['meta'] == 'YES':
                 dir = __knownmeta__.format(str(p.parent))
                 file = __knownmeta__.format(str(p.name))
                 slash = __knownmeta__.format('/')
             elif fullpath['meta'] == 'NO':
-                directory = await parseonlypath(normalized, mmi, gtfo)
+                directory = parseonlypath(normalized, mmi, gtfo)
                 if directory['meta'] == 'YES':
                     dir = __partialmeta__.format(str(p.parent))
                 else:
                     dir = str(p.parent)
-                filename = await parsefilename(normalized, mmi, gtfo)
+                filename = parsefilename(normalized, mmi, gtfo)
                 if filename['gtfo'] == 'YES' and isFile == True:
                     gtfo_file = __largefile__.format('F')
                 if filename['meta'] == 'YES':
                     file = __partialmeta__.format(str(p.name))
                 else:
                     file = str(p.name)
                 slash = '/'
@@ -236,8 +278,19 @@
 
             if str(p.parent) == '/':
                 print(denied+' '+sha256+' '+dir+file)
             else:
                 print(denied+' '+sha256+' '+dir+slash+file)
 
 def main():
-    asyncio.run(start())
+
+    parser = argparse.ArgumentParser(description='MMI - OS Triage for Anyone and Everyone')
+    parser.add_argument('-d', '--download', help='Download Bloom Filters', action='store_true')
+    parser.add_argument('-s', '--skip', help='Skip File Hashing', action='store_true')
+    parser.add_argument('-v', '--version', action='version', version=__version__)
+    args = parser.parse_args()
+
+    if args.download:
+        download()
+    else:
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            executor.submit(start, args.skip)
```

### Comparing `matchmeta-2023.5.19/setup.py` & `matchmeta-2023.5.28/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "matchmeta",
     version = __version__,
-    description = "Amazon Linux Triage for Anyone and Everyone",
+    description = "OS Triage for Anyone and Everyone",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/jblukach/mmi",
     author = "John Lukach",
     author_email = "hello@lukach.io",
     license = "Apache-2.0",
     packages = ["mmi"],
```

