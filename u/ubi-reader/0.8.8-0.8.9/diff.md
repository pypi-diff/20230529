# Comparing `tmp/ubi_reader-0.8.8.tar.gz` & `tmp/ubi_reader-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubi_reader-0.8.8.tar", max compression
+gzip compressed data, was "ubi_reader-0.8.9.tar", max compression
```

## Comparing `ubi_reader-0.8.8.tar` & `ubi_reader-0.8.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35117 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/LICENSE
--rwxr-xr-x   0        0        0     5551 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/README.md
--rw-r--r--   0        0        0     1179 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/__init__.py
--rwxr-xr-x   0        0        0     1892 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/debug.py
--rw-r--r--   0        0        0        1 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/scripts/__init__.py
--rwxr-xr-x   0        0        0     7425 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/scripts/ubireader_display_blocks.py
--rwxr-xr-x   0        0        0     7275 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/scripts/ubireader_display_info.py
--rwxr-xr-x   0        0        0     7554 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/scripts/ubireader_extract_files.py
--rwxr-xr-x   0        0        0     6572 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/scripts/ubireader_extract_images.py
--rwxr-xr-x   0        0        0     6714 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/scripts/ubireader_list_files.py
--rwxr-xr-x   0        0        0    13792 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/scripts/ubireader_utils_info.py
--rwxr-xr-x   0        0        0     1575 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/settings.py
--rwxr-xr-x   0        0        0     6725 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi/__init__.py
--rwxr-xr-x   0        0        0     8700 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi/block/__init__.py
--rwxr-xr-x   0        0        0     2181 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi/block/layout.py
--rw-r--r--   0        0        0     4043 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi/block/sort.py
--rw-r--r--   0        0        0     4867 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi/defines.py
--rwxr-xr-x   0        0        0     5443 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi/display.py
--rwxr-xr-x   0        0        0     3683 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi/headers.py
--rwxr-xr-x   0        0        0     2132 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi/image.py
--rwxr-xr-x   0        0        0     3923 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi/volume.py
--rwxr-xr-x   0        0        0     7684 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubi_io.py
--rwxr-xr-x   0        0        0     5161 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubifs/__init__.py
--rw-r--r--   0        0        0    19399 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubifs/defines.py
--rw-r--r--   0        0        0     5071 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubifs/display.py
--rwxr-xr-x   0        0        0     5672 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubifs/list.py
--rwxr-xr-x   0        0        0     2465 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubifs/misc.py
--rwxr-xr-x   0        0        0     7982 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubifs/nodes.py
--rwxr-xr-x   0        0        0     7759 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubifs/output.py
--rwxr-xr-x   0        0        0     5990 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/ubifs/walk.py
--rwxr-xr-x   0        0        0     5342 2023-05-22 19:22:25.000054 ubi_reader-0.8.8/ubireader/utils.py
--rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 ubi_reader-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0    35117 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/LICENSE
+-rwxr-xr-x   0        0        0     5551 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/README.md
+-rw-r--r--   0        0        0     1179 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/__init__.py
+-rwxr-xr-x   0        0        0     1892 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/debug.py
+-rw-r--r--   0        0        0        1 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/scripts/__init__.py
+-rwxr-xr-x   0        0        0     7425 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/scripts/ubireader_display_blocks.py
+-rwxr-xr-x   0        0        0     7275 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/scripts/ubireader_display_info.py
+-rwxr-xr-x   0        0        0     7554 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/scripts/ubireader_extract_files.py
+-rwxr-xr-x   0        0        0     6572 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/scripts/ubireader_extract_images.py
+-rwxr-xr-x   0        0        0     6714 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/scripts/ubireader_list_files.py
+-rwxr-xr-x   0        0        0    13792 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/scripts/ubireader_utils_info.py
+-rwxr-xr-x   0        0        0     1575 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/settings.py
+-rwxr-xr-x   0        0        0     6725 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi/__init__.py
+-rwxr-xr-x   0        0        0     8700 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi/block/__init__.py
+-rwxr-xr-x   0        0        0     2181 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi/block/layout.py
+-rw-r--r--   0        0        0     4043 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi/block/sort.py
+-rw-r--r--   0        0        0     4867 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi/defines.py
+-rwxr-xr-x   0        0        0     5443 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi/display.py
+-rwxr-xr-x   0        0        0     3683 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi/headers.py
+-rwxr-xr-x   0        0        0     2132 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi/image.py
+-rwxr-xr-x   0        0        0     3923 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi/volume.py
+-rwxr-xr-x   0        0        0     7684 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubi_io.py
+-rwxr-xr-x   0        0        0     5161 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubifs/__init__.py
+-rw-r--r--   0        0        0    19399 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubifs/defines.py
+-rw-r--r--   0        0        0     5071 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubifs/display.py
+-rwxr-xr-x   0        0        0     5672 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubifs/list.py
+-rwxr-xr-x   0        0        0     2444 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubifs/misc.py
+-rwxr-xr-x   0        0        0     7982 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubifs/nodes.py
+-rwxr-xr-x   0        0        0     7759 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubifs/output.py
+-rwxr-xr-x   0        0        0     5990 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/ubifs/walk.py
+-rwxr-xr-x   0        0        0     5342 2023-05-29 18:38:43.715312 ubi_reader-0.8.9/ubireader/utils.py
+-rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 ubi_reader-0.8.9/PKG-INFO
```

### Comparing `ubi_reader-0.8.8/LICENSE` & `ubi_reader-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/README.md` & `ubi_reader-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/pyproject.toml` & `ubi_reader-0.8.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ubi-reader"
-version = "0.8.8"
+version = "0.8.9"
 description = "Extract files from UBI and UBIFS images."
 authors = ["ONEKEY <support@onekey.com>", "Jason Pruitt <jrspruitt@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [{include = "ubireader"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ubi_reader-0.8.8/ubireader/debug.py` & `ubi_reader-0.8.9/ubireader/debug.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/scripts/ubireader_display_blocks.py` & `ubi_reader-0.8.9/ubireader/scripts/ubireader_display_blocks.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/scripts/ubireader_display_info.py` & `ubi_reader-0.8.9/ubireader/scripts/ubireader_display_info.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/scripts/ubireader_extract_files.py` & `ubi_reader-0.8.9/ubireader/scripts/ubireader_extract_files.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/scripts/ubireader_extract_images.py` & `ubi_reader-0.8.9/ubireader/scripts/ubireader_extract_images.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/scripts/ubireader_list_files.py` & `ubi_reader-0.8.9/ubireader/scripts/ubireader_list_files.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/scripts/ubireader_utils_info.py` & `ubi_reader-0.8.9/ubireader/scripts/ubireader_utils_info.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/settings.py` & `ubi_reader-0.8.9/ubireader/settings.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi/__init__.py` & `ubi_reader-0.8.9/ubireader/ubi/__init__.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi/block/__init__.py` & `ubi_reader-0.8.9/ubireader/ubi/block/__init__.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi/block/layout.py` & `ubi_reader-0.8.9/ubireader/ubi/block/layout.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi/block/sort.py` & `ubi_reader-0.8.9/ubireader/ubi/block/sort.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi/defines.py` & `ubi_reader-0.8.9/ubireader/ubi/defines.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi/display.py` & `ubi_reader-0.8.9/ubireader/ubi/display.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi/headers.py` & `ubi_reader-0.8.9/ubireader/ubi/headers.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi/image.py` & `ubi_reader-0.8.9/ubireader/ubi/image.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi/volume.py` & `ubi_reader-0.8.9/ubireader/ubi/volume.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubi_io.py` & `ubi_reader-0.8.9/ubireader/ubi_io.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubifs/__init__.py` & `ubi_reader-0.8.9/ubireader/ubifs/__init__.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubifs/defines.py` & `ubi_reader-0.8.9/ubireader/ubifs/defines.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubifs/display.py` & `ubi_reader-0.8.9/ubireader/ubifs/display.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubifs/list.py` & `ubi_reader-0.8.9/ubireader/ubifs/list.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubifs/misc.py` & `ubi_reader-0.8.9/ubireader/ubifs/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #############################################################
 
-from lzallright.lzallright import LZOCompressor as lzo
+from lzallright import LZOCompressor, LZOError
 import struct
 import zlib
 from ubireader.ubifs.defines import *
 from ubireader.debug import error
 
 # For happy printing
 ino_types = ['file', 'dir','lnk','blk','chr','fifo','sock']
@@ -58,15 +58,15 @@
     Str:data     -- Data to be uncompessed.
 
     Returns:
     Uncompressed Data.
     """
     if ctype == UBIFS_COMPR_LZO:
         try:
-            return lzo.decompress(b''.join((b'\xf0', struct.pack('>I', unc_len), data)))
+            return LZOCompressor.decompress(data, output_size_hint=unc_len)
         except Exception as e:
             error(decompress, 'Warn', 'LZO Error: %s' % e)
     elif ctype == UBIFS_COMPR_ZLIB:
         try:
             return zlib.decompress(data, -11)
         except Exception as e:
             error(decompress, 'Warn', 'ZLib Error: %s' % e)
```

### Comparing `ubi_reader-0.8.8/ubireader/ubifs/nodes.py` & `ubi_reader-0.8.9/ubireader/ubifs/nodes.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubifs/output.py` & `ubi_reader-0.8.9/ubireader/ubifs/output.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/ubifs/walk.py` & `ubi_reader-0.8.9/ubireader/ubifs/walk.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/ubireader/utils.py` & `ubi_reader-0.8.9/ubireader/utils.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.8/PKG-INFO` & `ubi_reader-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubi-reader
-Version: 0.8.8
+Version: 0.8.9
 Summary: Extract files from UBI and UBIFS images.
 License: GNU GPL
 Author: ONEKEY
 Author-email: support@onekey.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

