# Comparing `tmp/HaversineAPI-1.8.tar.gz` & `tmp/HaversineAPI-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HaversineAPI-1.8.tar", last modified: Sun Mar 20 23:03:11 2022, max compression
+gzip compressed data, was "HaversineAPI-1.9.tar", last modified: Mon Mar 21 23:21:20 2022, max compression
```

## Comparing `HaversineAPI-1.8.tar` & `HaversineAPI-1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-03-20 23:03:11.829513 HaversineAPI-1.8/
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-03-20 23:03:11.824979 HaversineAPI-1.8/Haversine/
--rw-r--r--   0 dave       (501) staff       (20)        0 2022-03-16 07:49:30.000000 HaversineAPI-1.8/Haversine/__init__.py
--rwxr-xr-x   0 dave       (501) staff       (20)    12831 2022-03-20 01:05:06.000000 HaversineAPI-1.8/Haversine/haversine.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-03-20 23:03:11.829150 HaversineAPI-1.8/HaversineAPI.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)     9938 2022-03-20 23:03:10.000000 HaversineAPI-1.8/HaversineAPI.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      252 2022-03-20 23:03:10.000000 HaversineAPI-1.8/HaversineAPI.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2022-03-20 23:03:10.000000 HaversineAPI-1.8/HaversineAPI.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       56 2022-03-20 23:03:10.000000 HaversineAPI-1.8/HaversineAPI.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       10 2022-03-20 23:03:10.000000 HaversineAPI-1.8/HaversineAPI.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)     9938 2022-03-20 23:03:11.829680 HaversineAPI-1.8/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)     9616 2022-03-20 23:02:18.000000 HaversineAPI-1.8/README.md
--rw-r--r--   0 dave       (501) staff       (20)       79 2022-03-20 23:03:11.832351 HaversineAPI-1.8/setup.cfg
--rwxr-xr-x   0 dave       (501) staff       (20)      792 2022-03-20 22:59:49.000000 HaversineAPI-1.8/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-03-21 23:21:20.565192 HaversineAPI-1.9/
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-03-21 23:21:20.557264 HaversineAPI-1.9/Haversine/
+-rw-r--r--   0 dave       (501) staff       (20)        0 2022-03-16 07:49:30.000000 HaversineAPI-1.9/Haversine/__init__.py
+-rwxr-xr-x   0 dave       (501) staff       (20)    12845 2022-03-21 22:56:33.000000 HaversineAPI-1.9/Haversine/haversine.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-03-21 23:21:20.564191 HaversineAPI-1.9/HaversineAPI.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)     9942 2022-03-21 23:21:18.000000 HaversineAPI-1.9/HaversineAPI.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      252 2022-03-21 23:21:19.000000 HaversineAPI-1.9/HaversineAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2022-03-21 23:21:18.000000 HaversineAPI-1.9/HaversineAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       56 2022-03-21 23:21:19.000000 HaversineAPI-1.9/HaversineAPI.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       10 2022-03-21 23:21:19.000000 HaversineAPI-1.9/HaversineAPI.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)     9942 2022-03-21 23:21:20.565343 HaversineAPI-1.9/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)     9620 2022-03-21 00:09:39.000000 HaversineAPI-1.9/README.md
+-rw-r--r--   0 dave       (501) staff       (20)       79 2022-03-21 23:21:20.568382 HaversineAPI-1.9/setup.cfg
+-rwxr-xr-x   0 dave       (501) staff       (20)      793 2022-03-21 23:20:02.000000 HaversineAPI-1.9/setup.py
```

### Comparing `HaversineAPI-1.8/Haversine/haversine.py` & `HaversineAPI-1.9/Haversine/haversine.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from Spanners.Squirrel import Squirrel  # uses credstash, use your favourite password safe instead if you like
 from Argumental.Argue import Argue # decorator for command line calling using argparse and argcomplete, cf $ ./haversine.py -h
 
 squirrel = Squirrel()
 args = Argue() 
 
-
 #________________________________________________________________________________________________
 @args.command()
 class Haversine(object):
 	'''
 	wrapper around the most excellent REST API for waypoints by joao @ haversine
 	https://haversine.com/webapi
 	'''
@@ -37,14 +36,15 @@
 	def verbose(self): return
 	
 	@args.property(flag=True, short='i', help='use insecure mode for old clients with old cert trees, will remove later, developing on Pythonista')
 	def insecure(self): return
 	
 	
 #________________________________________________________________________________________________
+
 @args.command(name='waypoints')
 class Waypoints(Haversine):
 	'''
 	wrapper around the most excellent REST API for waypoints by joao @ haversine
 	https://haversine.com/webapi	
 	'''
 
@@ -72,14 +72,15 @@
 			return response.json()['waypoints']
 		
 		sys.stderr.write(f'{response}\n{response.text}\n')
 		return
 		
 
 	#____________________________________________________________________________________________
+
 	@args.operation
 	@args.parameter(name='id', help='The point ID, max 7 chars')
 	def get(self, id):
 		'''
 		get a single waypoint by id
 		'''
 		
@@ -88,14 +89,15 @@
 		if id in waypoints.keys():
 			return waypoints[id]
 			
 		return
 		
 
 	#____________________________________________________________________________________________
+	
 	@args.operation
 	@args.parameter(name='id', help='The point ID, max 7 chars')
 	@args.parameter(name='description', help='The point description, max 63 chars')
 	@args.parameter(name='latitude', type=float, help='y=DDD.DDDDDDD')
 	@args.parameter(name='longitude', type=float, help='x=DDD.DDDDDDD')
 	@args.parameter(name='elevation', short='e', type=float, help='EEEE.EEEE in feet', default=0.0)
 	def create(self, id, description, latitude, longitude, elevation=0.0):
@@ -129,14 +131,15 @@
 			return response.json()['waypoint']
 		
 		sys.stderr.write(f'{response}\n{response.text}\n')
 		return False
 
 
 	#____________________________________________________________________________________________
+	
 	@args.operation
 	@args.parameter(name='id', help='The point ID, max 7 chars')
 	@args.parameter(name='description', help='The point description, max 63 chars')
 	@args.parameter(name='latitude', type=float, help='y=DDD.DDDDDDD')
 	@args.parameter(name='longitude', type=float, help='x=DDD.DDDDDDD')
 	@args.parameter(name='elevation', short='e', type=float, help='EEEE.EEEE in feet', default=0.0)
 	def update(self, id, description, latitude, longitude, elevation=0.0):
@@ -171,14 +174,15 @@
 		
 		sys.stderr.write(f'{response}\n{response.text}\n')
 		return False
 
 
 
 	#____________________________________________________________________________________________
+	
 	@args.operation
 	@args.parameter(name='id', help='The point ID, max 7 chars')		
 	def delete(self, id):
 		''' 
 		delete a single waypoint by id
 		'''
 		
@@ -200,14 +204,15 @@
 			return response.json()
 		
 		sys.stderr.write(f'{response}\n{response.text}\n')
 		return
 
 	
 #________________________________________________________________________________________________
+
 @args.command(name='routes')
 class Routes(Haversine):
 	'''
 	wrapper around the most excellent REST API for routes by joao @ haversine
 	https://haversine.com/webapi
 	'''
 	
@@ -235,14 +240,15 @@
 			return response.json()['routes']
 		
 		sys.stderr.write(f'{response}\n{response.text}\n')
 		return		
 
 
 	#____________________________________________________________________________________________
+
 	@args.operation
 	@args.parameter(name='name', help='The route name to recover')
 	def get(self, name):
 		'''
 		get a single route by name, reads whole list and filters
 		'''
 		routes = dict(map(lambda x: (x['name'], x), self.list()))
@@ -250,14 +256,15 @@
 		if name in routes.keys():
 			return routes[name]
 		
 		return
 		
 
 	#____________________________________________________________________________________________
+	
 	@args.operation
 	@args.parameter(name='origin', help='ICAO of origin')
 	@args.parameter(name='destination', help='ICAO of destination')
 	@args.parameter(name='first', short='f', flag=True, help='take first suggestion and convert to importable route')
 	@args.parameter(name='output', short='o', help='output to file name, null for stdout')
 	def suggest(self, origin, destination, first=None, output=None):
 		'''
@@ -307,15 +314,14 @@
 					json.dump(result, _output, indent='\t')
 													
 			return result
 
 		sys.stderr.write(f'{response}\n{response.text}\n')
 		return
 
-	
 	@args.operation
 	def sample(self):
 		'''
 		provide a sample route to be populated and used to create/update a route
 		'''
 		return {
 			#Field					Type			Description	
@@ -352,14 +358,15 @@
 				'longitude'			:'DOUBLE		Latitude',
 				'elevation'			:'DOUBLE		Elevation in feet MSL at which to cross or NULL (if unspecified)',
 			}]
 		}	
 
 
 	#____________________________________________________________________________________________
+
 	@args.operation
 	@args.parameter(name='route', short='r', help='file with json route, or None for stdin')
 	def create(self, route=None):
 		'''
 		create a new route, format as follows;
 		'''
 
@@ -388,23 +395,25 @@
 				json.dump(response.json(), sys.stdout,  indent='\t')
 			return response.json()
 			
 		sys.stderr.write(f'{response}\n{response.text}\n')
 		return
 				
 	#____________________________________________________________________________________________
+	
 	@args.operation
 	def update(self, name, origin, destination, points=[]):
 		'''
 		update an existing route, I'm doing it now Sybil
 		'''
 		pass #todo
 			
 	
 	#____________________________________________________________________________________________
+
 	@args.operation
 	@args.parameter(name='origin', help='ICAO of origin')
 	def delete(self, name):
 		'''
 		delete an existing route
 		'''
 		
@@ -424,9 +433,10 @@
 			return response.json()
 		
 		sys.stderr.write(f'{response}\n{response.text}\n')
 		return		
 		
 
 #________________________________________________________________________________________________
+
 if __name__ == '__main__': 
 	json.dump(args.execute(), sys.stdout, indent='\t')
```

### Comparing `HaversineAPI-1.8/HaversineAPI.egg-info/PKG-INFO` & `HaversineAPI-1.9/HaversineAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: HaversineAPI
-Version: 1.8
+Version: 1.9
 Summary: UNKNOWN
 Home-page: https://github.com/eddo888/HaversineAPI
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/HaversineAPI/archive/1.8.tar.gz
+Download-URL: https://github.com/eddo888/HaversineAPI/archive/1.9.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # haversine API python command line wrapper and client
 
 This is a simple python wrapper around the excellent new haversine waypoint REST API
 can be used from within python or from the unix command line (cygwin as well)
@@ -47,18 +47,20 @@
 ___
 
 # jupyter
 
 [Jupyter Notebook](https://jupyter.org/)
 
 if you like jupyter notebook, you can see some python examples of how to get routes and waypoints
+
 [HaversineAPI.ipynb](HaversineAPI.ipynb)
 
 there is also a Flight Plan converter that will read an x-plane FMS file and upload it to navigraph, great for batch uploads.
-[Flight Plans.ipynb](Flight Plans.ipynb)
+
+[Flight Plans.ipynb](Flight%20Plans.ipynb)
 
 ___
 
 # waypoints
 
 ```
 $ haversine.py waypoints -h
```

### Comparing `HaversineAPI-1.8/PKG-INFO` & `HaversineAPI-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: HaversineAPI
-Version: 1.8
+Version: 1.9
 Summary: UNKNOWN
 Home-page: https://github.com/eddo888/HaversineAPI
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/HaversineAPI/archive/1.8.tar.gz
+Download-URL: https://github.com/eddo888/HaversineAPI/archive/1.9.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # haversine API python command line wrapper and client
 
 This is a simple python wrapper around the excellent new haversine waypoint REST API
 can be used from within python or from the unix command line (cygwin as well)
@@ -47,18 +47,20 @@
 ___
 
 # jupyter
 
 [Jupyter Notebook](https://jupyter.org/)
 
 if you like jupyter notebook, you can see some python examples of how to get routes and waypoints
+
 [HaversineAPI.ipynb](HaversineAPI.ipynb)
 
 there is also a Flight Plan converter that will read an x-plane FMS file and upload it to navigraph, great for batch uploads.
-[Flight Plans.ipynb](Flight Plans.ipynb)
+
+[Flight Plans.ipynb](Flight%20Plans.ipynb)
 
 ___
 
 # waypoints
 
 ```
 $ haversine.py waypoints -h
```

### Comparing `HaversineAPI-1.8/README.md` & `HaversineAPI-1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,20 @@
 ___
 
 # jupyter
 
 [Jupyter Notebook](https://jupyter.org/)
 
 if you like jupyter notebook, you can see some python examples of how to get routes and waypoints
+
 [HaversineAPI.ipynb](HaversineAPI.ipynb)
 
 there is also a Flight Plan converter that will read an x-plane FMS file and upload it to navigraph, great for batch uploads.
-[Flight Plans.ipynb](Flight Plans.ipynb)
+
+[Flight Plans.ipynb](Flight%20Plans.ipynb)
 
 ___
 
 # waypoints
 
 ```
 $ haversine.py waypoints -h
```

### Comparing `HaversineAPI-1.8/setup.py` & `HaversineAPI-1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 import codecs
 from os import path
 from setuptools import setup
 
 pwd = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(pwd, 'README.md'), 'r', encoding='utf8') as input:
     long_description = input.read()
 
-version='1.8'
+version='1.9'
 	
 setup(
 	name='HaversineAPI',
 	version=version,
 	license='MIT',
     long_description=long_description,
 	long_description_content_type="text/markdown",
```

