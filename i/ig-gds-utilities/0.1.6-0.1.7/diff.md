# Comparing `tmp/ig_gds_utilities-0.1.6-py2.py3-none-any.whl.zip` & `tmp/ig_gds_utilities-0.1.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5645 bytes, number of entries: 8
+Zip file size: 5722 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx        0 b- defN 22-Feb-24 14:27 ig_gds_utilities/__init__.py
--rw-rw-r--  2.0 unx     8492 b- defN 23-Mar-14 14:48 ig_gds_utilities/ig_utilities.py
--rw-rw-r--  2.0 unx      648 b- defN 22-Mar-08 14:27 ig_gds_utilities-0.1.6.data/data/config_utilities_EXAMPLE.cfg
--rw-rw-r--  2.0 unx     1077 b- defN 23-Mar-14 14:59 ig_gds_utilities-0.1.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1112 b- defN 23-Mar-14 14:59 ig_gds_utilities-0.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Mar-14 14:59 ig_gds_utilities-0.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 23-Mar-14 14:59 ig_gds_utilities-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      720 b- defN 23-Mar-14 14:59 ig_gds_utilities-0.1.6.dist-info/RECORD
-8 files, 12176 bytes uncompressed, 4365 bytes compressed:  64.2%
+-rw-rw-r--  2.0 unx     9001 b- defN 23-May-29 21:10 ig_gds_utilities/ig_utilities.py
+-rw-rw-r--  2.0 unx      648 b- defN 22-Mar-08 14:27 ig_gds_utilities-0.1.7.data/data/config_utilities_EXAMPLE.cfg
+-rw-rw-r--  2.0 unx     1077 b- defN 23-May-29 21:16 ig_gds_utilities-0.1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1134 b- defN 23-May-29 21:16 ig_gds_utilities-0.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-29 21:16 ig_gds_utilities-0.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 23-May-29 21:16 ig_gds_utilities-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      720 b- defN 23-May-29 21:16 ig_gds_utilities-0.1.7.dist-info/RECORD
+8 files, 12707 bytes uncompressed, 4442 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ig_gds_utilities/__init__.py
 Comment: 
 
 Filename: ig_gds_utilities/ig_utilities.py
 Comment: 
 
-Filename: ig_gds_utilities-0.1.6.data/data/config_utilities_EXAMPLE.cfg
+Filename: ig_gds_utilities-0.1.7.data/data/config_utilities_EXAMPLE.cfg
 Comment: 
 
-Filename: ig_gds_utilities-0.1.6.dist-info/LICENSE
+Filename: ig_gds_utilities-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: ig_gds_utilities-0.1.6.dist-info/METADATA
+Filename: ig_gds_utilities-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: ig_gds_utilities-0.1.6.dist-info/WHEEL
+Filename: ig_gds_utilities-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: ig_gds_utilities-0.1.6.dist-info/top_level.txt
+Filename: ig_gds_utilities-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ig_gds_utilities-0.1.6.dist-info/RECORD
+Filename: ig_gds_utilities-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ig_gds_utilities/ig_utilities.py

```diff
@@ -176,57 +176,70 @@
         return country_text  
     
     except Exception as e: 
         msg_error = "##Error in get_country_twitter:%s" %str(e)
         logging.error(msg_error)
         return '---'
 
-def generate_google_map(latitud,longitud,event_info):
+def generate_google_map(latitud,longitud,event_info,*args):
 
     """
     This function generate a JPG of the epicenter of an earthquake
     If something goes wrong, returns a False so the caller can invoque another
     function to handle the map creation.  
     """
     cfg = read_parameters(config_path) 
     google_key =  cfg['ig_info']['google_key']
     google_url =  cfg['ig_info']['google_url']
     eqevent_path = cfg['ig_info']['eqevent_page_path']
 
     try:
-        image_path = os.path.join(eqevent_path,'%s/%s-map.jpg' %(event_info['event_id'],event_info['event_id']))
+        if args:
+            map_type = args[0]
+            logging.info(f"Args suplied {args[0]}")
+            image_path = os.path.join(eqevent_path,'%s/%s-%s-map.jpg' %(event_info['event_id'],event_info['event_id'],map_type))
+
+        else:
+            image_path = os.path.join(eqevent_path,'%s/%s-map.jpg' %(event_info['event_id'],event_info['event_id']))
         if os.path.isfile(image_path):
             os.remove(image_path)
         map_image_url = "%s|%s,%s&key=%s" %(google_url,latitud,longitud,google_key)
         buffer = BytesIO(urllib.request.urlopen(map_image_url).read())
         map_image = Image.open(buffer)
         map_image.convert('RGB').save(image_path)
         return True
     except Exception as e:
         logging.error("Error while creating a googlemap image:%s" %str(e))
         print(("Error while creating a googlemap image:%s" %str(e)))
         return False 
 
 
-def generate_gis_map(latitud,longitud,event_info):
+def generate_gis_map(latitud,longitud,event_info,*args):
 
 
     """
     This function generate a JPG of the epicenter of an earthquake
     If something goes wrong, returns a False so the caller can invoque another
     function to handle the map creation.  
     """
     margin_degree = 0.75
     image_size = 512
     cfg = read_parameters(config_path)
     gempa_gis_url =  cfg['ig_info']['gempa_gis_url']
     eqevent_path = cfg['ig_info']['eqevent_page_path']
 
     try:
-        image_path = os.path.join(eqevent_path,'%s/%s-map.jpg' %(event_info['event_id'],event_info['event_id']))
+
+        if args:
+            map_type = args[0]
+            logging.info(f"Args suplied {args[0]}")
+            image_path = os.path.join(eqevent_path,'%s/%s-%s-map.jpg' %(event_info['event_id'],event_info['event_id'],map_type))
+
+        else:
+            image_path = os.path.join(eqevent_path,'%s/%s-map.jpg' %(event_info['event_id'],event_info['event_id']))
         if os.path.isfile(image_path):
             os.remove(image_path)
 
         #map_image_url = "%s|%s,%s&key=%s" %(gempa_gis_url,latitud,longitud,google_key)
         
         map_image_url = "{0}/map?reg={1},{2},{3},{3}&ori={1},{2}&dim={4},{4}".format(
             gempa_gis_url,latitud,longitud,margin_degree,image_size)
```

## Comparing `ig_gds_utilities-0.1.6.data/data/config_utilities_EXAMPLE.cfg` & `ig_gds_utilities-0.1.7.data/data/config_utilities_EXAMPLE.cfg`

 * *Files identical despite different names*

## Comparing `ig_gds_utilities-0.1.6.dist-info/LICENSE` & `ig_gds_utilities-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ig_gds_utilities-0.1.6.dist-info/METADATA` & `ig_gds_utilities-0.1.7.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ig-gds-utilities
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python library to be used by differente GDS services
 Home-page: https://github.com/awacero/ig_gds_utilities
 Author: Wilson Acero
 Author-email: acerowilson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests (>=2.22.0)
 
 # ig_gds_utilities
 This is the repository for a library with some functions used by GDS services like igtwitter or igtelegram. 
 The ig_gds_utilities shoul be installed using pip as a local user or as system 
 
 ``` bash
```

## Comparing `ig_gds_utilities-0.1.6.dist-info/RECORD` & `ig_gds_utilities-0.1.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 ig_gds_utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ig_gds_utilities/ig_utilities.py,sha256=exb-VxsyZ_I7HPKN7q_gVkQokd1607cJe5pLjR9tlgc,8492
-ig_gds_utilities-0.1.6.data/data/config_utilities_EXAMPLE.cfg,sha256=LJ7W4FIhYd0WAgvMC2SSusRuAiWJsBnw-s7FskId0p4,648
-ig_gds_utilities-0.1.6.dist-info/LICENSE,sha256=1jMj6pADhHYZrmThADvN3zWBl-Sv3hdSHpK0IhJq5Xc,1077
-ig_gds_utilities-0.1.6.dist-info/METADATA,sha256=CsGQlhVGA8NTaPrysXPuDSHtJyB936b5RWnoonwfoNQ,1112
-ig_gds_utilities-0.1.6.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
-ig_gds_utilities-0.1.6.dist-info/top_level.txt,sha256=mJQtlM2fLegNkuAKIEWdTbwRP8pvuHAliSEA2h_oKCM,17
-ig_gds_utilities-0.1.6.dist-info/RECORD,,
+ig_gds_utilities/ig_utilities.py,sha256=2CZUyOex3K3590ODwk-k-xmjvgekGo6i6UxmJSNcJM4,9001
+ig_gds_utilities-0.1.7.data/data/config_utilities_EXAMPLE.cfg,sha256=LJ7W4FIhYd0WAgvMC2SSusRuAiWJsBnw-s7FskId0p4,648
+ig_gds_utilities-0.1.7.dist-info/LICENSE,sha256=1jMj6pADhHYZrmThADvN3zWBl-Sv3hdSHpK0IhJq5Xc,1077
+ig_gds_utilities-0.1.7.dist-info/METADATA,sha256=27q5PfT41XjtzDqdIUjRxkihd8jpevz6Yx8iRTXgRbE,1134
+ig_gds_utilities-0.1.7.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+ig_gds_utilities-0.1.7.dist-info/top_level.txt,sha256=mJQtlM2fLegNkuAKIEWdTbwRP8pvuHAliSEA2h_oKCM,17
+ig_gds_utilities-0.1.7.dist-info/RECORD,,
```

