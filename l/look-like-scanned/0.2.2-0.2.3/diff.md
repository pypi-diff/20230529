# Comparing `tmp/look_like_scanned-0.2.2.tar.gz` & `tmp/look_like_scanned-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "look_like_scanned-0.2.2.tar", max compression
+gzip compressed data, was "look_like_scanned-0.2.3.tar", max compression
```

## Comparing `look_like_scanned-0.2.2.tar` & `look_like_scanned-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/LICENSE
--rw-r--r--   0        0        0    10207 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/README.md
--rw-r--r--   0        0        0     1758 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/scanner/__init__.py
--rw-r--r--   0        0        0    12157 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/scanner/scanner.py
--rw-r--r--   0        0        0    11684 1970-01-01 00:00:00.000000 look_like_scanned-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/LICENSE
+-rw-r--r--   0        0        0    10207 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/README.md
+-rw-r--r--   0        0        0     1778 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/scanner/__init__.py
+-rw-r--r--   0        0        0    13210 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/scanner/scanner.py
+-rw-r--r--   0        0        0    11725 1970-01-01 00:00:00.000000 look_like_scanned-0.2.3/PKG-INFO
```

### Comparing `look_like_scanned-0.2.2/LICENSE` & `look_like_scanned-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `look_like_scanned-0.2.2/README.md` & `look_like_scanned-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `look_like_scanned-0.2.2/pyproject.toml` & `look_like_scanned-0.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "look-like-scanned"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python script to make documents look like they were scanned."
 authors = ["navchandar <12165092+navchandar@users.noreply.github.com>"]
 repository    = "https://github.com/navchandar/look-like-scanned"
 homepage = "https://github.com/navchandar/look-like-scanned"
 readme = "README.md"
 keywords = ["pdf", "scan", "scanner", "image-to-pdf", "pdf-to-scan"]
 packages = [
@@ -28,14 +28,15 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pillow = "^9.5.0"
 pypdfium2 = "^4.11.0"
+colorama = "^0.4.6"
 
 
 [tool.poetry.scripts]
 scanner = "scanner:main"
 
 
 [tool.poetry.urls]
```

### Comparing `look_like_scanned-0.2.2/scanner/scanner.py` & `look_like_scanned-0.2.3/scanner/scanner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,46 @@
 #!/usr/bin/env python
 """Module to convert PDF/Images to look like they were scanned"""
 
 import os
 import io
 import random
 import argparse
+import colorama
+from colorama import Fore, Style
 from pprint import pprint
 import pypdfium2 as pdfium
 from PIL import Image, ImageEnhance
 
 SUPPORTED_IMAGES = [".jpg", ".png", ".jpeg", ".webp"]
 SUPPORTED_DOCS = [".pdf", ".PDF"]
-CHOICES = ["y", "yes", "n", "no"]
+CHOICES = ["y", "yes", "n", "no", "true", "false"]
+
+
+def print_color_text(text, color):
+    """
+    Print the specified text in the given color.
+    Available colors: 'black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white'.
+    """
+    color_map = {
+        "black": Fore.BLACK,
+        "red": Fore.RED,
+        "green": Fore.GREEN,
+        "yellow": Fore.YELLOW,
+        "blue": Fore.BLUE,
+        "magenta": Fore.MAGENTA,
+        "cyan": Fore.CYAN,
+        "white": Fore.WHITE,
+    }
+    color_code = color_map.get(color.lower(), Fore.RESET)
+    print(color_code + text + Style.RESET_ALL)
+
+
+# Initialize colorama
+colorama.init()
 
 
 def parse_args():
     """Parse input command-line arguments for the script"""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-i",
@@ -53,59 +78,58 @@
         default="no",
         help="Recurse in all sub folders to find matching files and convert them (default: no)",
     )
 
     return parser.parse_args()
 
 
-def get_argument(argument_name):
+def get_input_folder(args):
     """
     Gets the input folder from the command-line argument.
-    If no input folder provided, returns the current working directory.
+    If argument not provided, returns current working directory as input folder
     """
-    args = parse_args()
-    if argument_name == "folder":
-        input_folder = os.getcwd()
-        if args.input_folder:
-            input_folder = args.input_folder
-        else:
-            print("Defaulting to current directory")
-        input_folder = os.path.abspath(input_folder)
-
-        # check if folder path exists
-        if os.path.exists(input_folder):
-            print(f"Processing files from {input_folder=}")
-        else:
-            print(f"Error: Input folder path not found: {input_folder}")
-        return input_folder
-
-    if argument_name == "quality":
-        return int(args.file_quality) if args.file_quality else 95
-
-    if argument_name == "askew":
-        return args.askew.lower().startswith("y") if args.askew else True
-
-    if argument_name == "recurse":
-        return args.recurse.lower().startswith("y") if args.recurse else True
-
-    if argument_name == "file_type":
-        match = (None, None)
-        if args.file_type_or_name:
-            file = args.file_type_or_name.lower()
-            if file == "image":
-                match = ("image", SUPPORTED_IMAGES)
-            elif any(f.endswith(file) or file.endswith(f) for f in SUPPORTED_IMAGES):
-                match = ("image", [args.file_type_or_name])
-            elif any(f.endswith(file) or file.endswith(f) for f in SUPPORTED_DOCS):
-                match = ("pdf", [args.file_type_or_name])
-            else:
-                print("Defaulting to find pdf files")
-        else:
-            match = ("pdf", SUPPORTED_DOCS)
-        return match
+    input_folder = (
+        os.path.abspath(args.input_folder) if args.input_folder else os.getcwd()
+    )
+    if os.path.exists(input_folder):
+        print(f"Processing files from {input_folder=}")
+    else:
+        print(f"Error: Input folder path not found: {input_folder}")
+    return input_folder
+
+
+def get_quality(args):
+    return args.file_quality
+
+
+def get_askew(args):
+    return args.askew.lower().startswith(("y", "t"))
+
+
+def get_recurse(args):
+    return args.recurse.lower().startswith(("y", "t"))
+
+
+def get_file_type(args):
+    """Get file type and supported documents based on input arguments"""
+    if args.file_type_or_name:
+        file_type = args.file_type_or_name.lower()
+        if file_type == "image":
+            return "image", SUPPORTED_IMAGES
+        elif any(
+            f.endswith(file_type) or file_type.endswith(f) for f in SUPPORTED_IMAGES
+        ):
+            return "image", [args.file_type_or_name]
+        elif any(
+            f.endswith(file_type) or file_type.endswith(f) for f in SUPPORTED_DOCS
+        ):
+            return "pdf", [args.file_type_or_name]
+    else:
+        print("Defaulting to find pdf files")
+        return "pdf", SUPPORTED_DOCS
 
 
 def human_size(num, suffix="B"):
     """Return file size in a human readable format"""
     for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
         if abs(num) < 1024.0:
             return f"{num:3.1f}{unit}{suffix}"
@@ -114,14 +138,23 @@
 
 
 def get_file_size(file_path):
     """Get file size for a given file path"""
     return human_size(os.stat(file_path).st_size)
 
 
+def files_exists(file_path):
+    """Check if given file path exists in the file system"""
+    if os.path.exists(file_path):
+        return True
+    else:
+        print_color_text(f"File doesn't exist or incorrect path: {file_path}", "Red")
+        return False
+
+
 def reduce_image_quality(image, quality=100, compression="JPEG"):
     """Reduce quality of a given image object"""
     img_byte_array = io.BytesIO()
     # Save the image to the in-memory file object
     image.save(img_byte_array, quality=quality, format=compression)
 
     # Rewind the file object to the beginning
@@ -181,37 +214,38 @@
 
 
 def _save_image_obj_to_pdf(images_list, output_pdf_path, pdf_version=17):
     """
     Save image objects into output pdf
     """
     pages_scanned = 0
-    output_pdf = pdfium.PdfDocument.new()
-    for image_file in images_list:
-        pdf_image = pdfium.PdfImage.new(output_pdf)
-        pdf_image.load_jpeg(image_file)
-        width, height = pdf_image.get_size()
-        # since render size increased by 2, decrease by same amount
-        width = width / 2
-        height = height / 2
-
-        matrix = pdfium.PdfMatrix().scale(width, height)
-        pdf_image.set_matrix(matrix)
-
-        page = output_pdf.new_page(width, height)
-        page.insert_obj(pdf_image)
-        page.gen_content()
-        page.close()
-        pdf_image.close()
-        pages_scanned += 1
-
-    output_pdf.save(output_pdf_path, version=pdf_version)
-    output_pdf.close()
-    file_size = get_file_size(output_pdf_path)
-    print(f"{output_pdf_path=} {file_size=}")
+    if images_list:
+        output_pdf = pdfium.PdfDocument.new()
+        for image_file in images_list:
+            pdf_image = pdfium.PdfImage.new(output_pdf)
+            pdf_image.load_jpeg(image_file)
+            width, height = pdf_image.get_size()
+            # since render size increased by 2, decrease by same amount
+            width = width / 2
+            height = height / 2
+
+            matrix = pdfium.PdfMatrix().scale(width, height)
+            pdf_image.set_matrix(matrix)
+
+            page = output_pdf.new_page(width, height)
+            page.insert_obj(pdf_image)
+            page.gen_content()
+            page.close()
+            pdf_image.close()
+            pages_scanned += 1
+
+        output_pdf.save(output_pdf_path, version=pdf_version)
+        output_pdf.close()
+        file_size = get_file_size(output_pdf_path)
+        print(f"{output_pdf_path=} {file_size=}")
     return pages_scanned
 
 
 def _add_suffix(filename):
     """Adds output suffix to given file name"""
     extension = "pdf"
     suffix = "_output"
@@ -246,59 +280,62 @@
     elif energy_saved < 1000000:
         energy_saved = energy_saved / 1000
         energy_saved = f"{energy_saved:.2f} kilo Watt hours"
     else:
         energy_saved = energy_saved / 1000000
         energy_saved = f"{energy_saved:.2f} Mega Watt hours"
 
-    savings = f"You just saved {energy_saved} energy by avoiding printing {pages_scanned} pages of paper!"
-    print(savings)
+    if pages_scanned > 0:
+        savings = f"\nYou just saved {energy_saved} energy by avoiding printing {pages_scanned} pages of paper!\n"
+        print_color_text(savings, "Green")
 
 
 def convert_images_to_pdf(input_image_list, image_quality, askew):
     """Converts all image files in a folder to PDF"""
     images_list = []
 
     # Output pdf name will be the fetched from first Image's name
     output_pdf_path = os.path.splitext(input_image_list[0])[0] + "_output.pdf"
     for image_path in input_image_list:
-        try:
-            image = Image.open(image_path)
-            # reduce image quality a little bit
-            image = reduce_image_quality(image, image_quality)
-            image = image.convert("RGB")
-
-            # Rotate every image by a small random angle
-            if askew:
-                image = rotate_image(image, random.uniform(-0.75, 0.75))
-
-            image = _change_image_to_byte_buffer(image)
-            images_list.append(image)
-        except Exception as e:
-            print(f"Error converting file {image_path} :-", e)
+        if files_exists(image_path):
+            try:
+                image = Image.open(image_path)
+                # reduce image quality a little bit
+                image = reduce_image_quality(image, image_quality)
+                image = image.convert("RGB")
+
+                # Rotate every image by a small random angle
+                if askew:
+                    image = rotate_image(image, random.uniform(-0.75, 0.75))
+
+                image = _change_image_to_byte_buffer(image)
+                images_list.append(image)
+            except Exception as e:
+                print_color_text(f"Error converting file {image_path} :- {e}", "Red")
 
     pages_scanned = _save_image_obj_to_pdf(images_list, output_pdf_path, pdf_version=17)
     _calc_energy_savings(pages_scanned)
     return output_pdf_path
 
 
 def convert_pdf_to_scanned(pdf_list, image_quality, askew):
     """
     Converts PDF files into scanned PDF files
     """
     output_file_list = []
     pages_scanned = 0
     for pdf_path in pdf_list:
-        try:
-            output_path = _add_suffix(pdf_path)
-            images = _convert_pdf_pages_to_jpg_list(pdf_path, image_quality, askew)
-            pages_scanned += _save_image_obj_to_pdf(images, output_path)
-            output_file_list.append(output_path)
-        except Exception as e:
-            print(f"Error converting file {pdf_path} :-", e)
+        if files_exists(pdf_path):
+            try:
+                output_path = _add_suffix(pdf_path)
+                images = _convert_pdf_pages_to_jpg_list(pdf_path, image_quality, askew)
+                pages_scanned += _save_image_obj_to_pdf(images, output_path)
+                output_file_list.append(output_path)
+            except Exception as e:
+                print_color_text(f"Error converting file {pdf_path} :- {e}", "Red")
 
     _calc_energy_savings(pages_scanned)
     return output_file_list
 
 
 def find_matching_files(input_folder, file_type_list, recurse=False):
     """
@@ -312,53 +349,60 @@
             if os.path.isfile(path) and any(
                 file.endswith(ext) for ext in file_type_list
             ):
                 files_list.append(path)
             if recurse and os.path.isdir(path):
                 files_list.extend(find_matching_files(path, file_type_list, recurse))
     except Exception as e:
-        print("Error when searching for files :-", e)
+        print_color_text(f"Error when searching for files :- {e}", "Red")
     return files_list
 
 
 def sort_by_top_level_directory(path):
     """Method to help sort file paths based on level"""
     directories = path.split(os.path.sep)
     return len(directories)
 
 
 def main():
     """Get input arguments and run the script"""
+    args = parse_args()
 
     # Gather input arguments from command-line
-    input_folder = get_argument("folder")
-    quality = get_argument("quality")
-    askew = get_argument("askew")
-    recurse = get_argument("recurse")
-    doc_type, file_type_list = get_argument("file_type")
-    print(f"{quality=} {recurse=} {askew=} {doc_type=} {file_type_list=}")
+    input_folder = get_input_folder(args)
+    quality = get_quality(args)
+    askew = get_askew(args)
+    recurse = get_recurse(args)
+    doc_type, file_type_list = get_file_type(args)
+
+    print_color_text(
+        f"{quality=} {recurse=} {askew=} {doc_type=} {file_type_list=}", "Cyan"
+    )
 
     # Gather the input files based on the arguments
     files_list = find_matching_files(input_folder, file_type_list, recurse)
     # Sort file paths so output gets saved in top level directory
     files_list = sorted(files_list, key=sort_by_top_level_directory)
 
-    print(f"Matching Files Found: {len(files_list)}")
+    print_color_text(f"\nMatching Files Found: {len(files_list)}", "Blue")
     pprint(files_list)
 
     # Convert the files found into output files
     pdf_path = None
     if doc_type == "image":
         pdf_path = convert_images_to_pdf(files_list, quality, askew)
     elif doc_type == "pdf":
         pdf_path = convert_pdf_to_scanned(files_list, quality, askew)
     else:
         print("Error: Unsupported file format!")
 
     if pdf_path:
-        pprint(f"The Output PDF files saved at {pdf_path}")
+        print(f"The Output PDF files saved at:")
+        pprint(pdf_path)
     else:
-        print("No valid file type found. No output documents generated")
+        print_color_text(
+            "No matching files found. No output documents generated!", "Red"
+        )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `look_like_scanned-0.2.2/PKG-INFO` & `look_like_scanned-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: look-like-scanned
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python script to make documents look like they were scanned.
 Home-page: https://github.com/navchandar/look-like-scanned
 Keywords: pdf,scan,scanner,image-to-pdf,pdf-to-scan
 Author: navchandar
 Author-email: 12165092+navchandar@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pypdfium2 (>=4.11.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/navchandar/look-like-scanned/issues
 Project-URL: Funding, https://www.buymeacoffee.com/navchandar/
 Project-URL: Repository, https://github.com/navchandar/look-like-scanned
 Description-Content-Type: text/markdown
```

