# Comparing `tmp/pytamaro-0.4.1.tar.gz` & `tmp/pytamaro-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytamaro-0.4.1.tar", max compression
+gzip compressed data, was "pytamaro-0.5.0.tar", max compression
```

## Comparing `pytamaro-0.4.1.tar` & `pytamaro-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     1103 2022-03-04 16:39:39.043278 pytamaro-0.4.1/LICENSE
--rw-r--r--   0        0        0      817 2023-04-06 12:18:49.527231 pytamaro-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      472 2023-04-06 12:19:23.593798 pytamaro-0.4.1/pytamaro/__init__.py
--rw-r--r--   0        0        0     3659 2023-02-27 12:54:43.437950 pytamaro-0.4.1/pytamaro/checks.py
--rw-r--r--   0        0        0      962 2023-02-27 12:54:43.438236 pytamaro-0.4.1/pytamaro/color.py
--rw-r--r--   0        0        0     4641 2023-02-27 12:54:43.438488 pytamaro-0.4.1/pytamaro/color_functions.py
--rw-r--r--   0        0        0      799 2023-02-27 12:54:43.438694 pytamaro-0.4.1/pytamaro/color_names.py
--rw-r--r--   0        0        0      456 2023-02-27 12:54:43.439015 pytamaro-0.4.1/pytamaro/de/__init__.py
--rw-r--r--   0        0        0     3948 2023-02-27 12:54:43.439329 pytamaro-0.4.1/pytamaro/de/color.py
--rw-r--r--   0        0        0     1093 2022-03-04 16:39:39.049297 pytamaro-0.4.1/pytamaro/de/color_names.py
--rw-r--r--   0        0        0      445 2023-02-27 12:54:43.439701 pytamaro-0.4.1/pytamaro/de/graphic.py
--rw-r--r--   0        0        0     2574 2023-02-27 12:54:43.440104 pytamaro-0.4.1/pytamaro/de/io.py
--rw-r--r--   0        0        0     4206 2023-02-27 12:54:43.440314 pytamaro-0.4.1/pytamaro/de/operations.py
--rw-r--r--   0        0        0      119 2023-02-27 12:54:43.440547 pytamaro-0.4.1/pytamaro/de/point.py
--rw-r--r--   0        0        0     1364 2023-02-27 12:54:43.440806 pytamaro-0.4.1/pytamaro/de/point_names.py
--rw-r--r--   0        0        0     4626 2023-02-27 12:54:43.441003 pytamaro-0.4.1/pytamaro/de/primitives.py
--rw-r--r--   0        0        0     2643 2023-02-27 12:54:43.441184 pytamaro-0.4.1/pytamaro/debug.py
--rw-r--r--   0        0        0     8147 2023-02-27 12:54:43.441456 pytamaro-0.4.1/pytamaro/graphic.py
--rw-r--r--   0        0        0     6386 2023-02-27 12:54:43.441700 pytamaro-0.4.1/pytamaro/io.py
--rw-r--r--   0        0        0      457 2023-02-27 12:54:43.441979 pytamaro-0.4.1/pytamaro/it/__init__.py
--rw-r--r--   0        0        0     3370 2023-02-27 12:54:43.442282 pytamaro-0.4.1/pytamaro/it/color.py
--rw-r--r--   0        0        0      923 2022-11-30 08:45:09.899740 pytamaro-0.4.1/pytamaro/it/color_names.py
--rw-r--r--   0        0        0      459 2023-02-27 12:54:43.442558 pytamaro-0.4.1/pytamaro/it/graphic.py
--rw-r--r--   0        0        0     2320 2023-02-27 12:54:43.442718 pytamaro-0.4.1/pytamaro/it/io.py
--rw-r--r--   0        0        0     4512 2023-02-27 12:54:43.442887 pytamaro-0.4.1/pytamaro/it/operations.py
--rw-r--r--   0        0        0      111 2023-02-27 12:54:43.443014 pytamaro-0.4.1/pytamaro/it/point.py
--rw-r--r--   0        0        0     1626 2023-02-27 12:54:43.443240 pytamaro-0.4.1/pytamaro/it/point_names.py
--rw-r--r--   0        0        0     4636 2023-02-27 12:54:43.443425 pytamaro-0.4.1/pytamaro/it/primitives.py
--rw-r--r--   0        0        0     5786 2023-02-27 12:54:43.443621 pytamaro-0.4.1/pytamaro/localization.py
--rw-r--r--   0        0        0     5834 2023-02-27 12:54:43.443786 pytamaro-0.4.1/pytamaro/operations.py
--rw-r--r--   0        0        0     1900 2023-02-27 12:54:43.443994 pytamaro-0.4.1/pytamaro/point.py
--rw-r--r--   0        0        0     1233 2023-02-27 12:54:43.444184 pytamaro-0.4.1/pytamaro/point_names.py
--rw-r--r--   0        0        0     4997 2023-02-27 12:54:43.444392 pytamaro-0.4.1/pytamaro/primitives.py
--rw-r--r--   0        0        0        0 2022-10-31 08:45:16.764275 pytamaro-0.4.1/pytamaro/py.typed
--rw-r--r--   0        0        0     1032 2023-04-06 12:16:34.179637 pytamaro-0.4.1/pytamaro/utils.py
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 pytamaro-0.4.1/setup.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 pytamaro-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1103 2022-03-04 16:39:39.043278 pytamaro-0.5.0/LICENSE
+-rw-r--r--   0        0        0      818 2023-05-29 07:51:55.773691 pytamaro-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      472 2023-05-29 07:51:55.777560 pytamaro-0.5.0/pytamaro/__init__.py
+-rw-r--r--   0        0        0     3659 2023-02-27 12:54:43.437950 pytamaro-0.5.0/pytamaro/checks.py
+-rw-r--r--   0        0        0      962 2023-02-27 12:54:43.438236 pytamaro-0.5.0/pytamaro/color.py
+-rw-r--r--   0        0        0     4641 2023-02-27 12:54:43.438488 pytamaro-0.5.0/pytamaro/color_functions.py
+-rw-r--r--   0        0        0      799 2023-02-27 12:54:43.438694 pytamaro-0.5.0/pytamaro/color_names.py
+-rw-r--r--   0        0        0      456 2023-02-27 12:54:43.439015 pytamaro-0.5.0/pytamaro/de/__init__.py
+-rw-r--r--   0        0        0     3948 2023-02-27 12:54:43.439329 pytamaro-0.5.0/pytamaro/de/color.py
+-rw-r--r--   0        0        0     1093 2022-03-04 16:39:39.049297 pytamaro-0.5.0/pytamaro/de/color_names.py
+-rw-r--r--   0        0        0      445 2023-02-27 12:54:43.439701 pytamaro-0.5.0/pytamaro/de/graphic.py
+-rw-r--r--   0        0        0     3211 2023-05-29 07:53:52.456525 pytamaro-0.5.0/pytamaro/de/io.py
+-rw-r--r--   0        0        0     4206 2023-02-27 12:54:43.440314 pytamaro-0.5.0/pytamaro/de/operations.py
+-rw-r--r--   0        0        0      119 2023-02-27 12:54:43.440547 pytamaro-0.5.0/pytamaro/de/point.py
+-rw-r--r--   0        0        0     1364 2023-02-27 12:54:43.440806 pytamaro-0.5.0/pytamaro/de/point_names.py
+-rw-r--r--   0        0        0     4626 2023-02-27 12:54:43.441003 pytamaro-0.5.0/pytamaro/de/primitives.py
+-rw-r--r--   0        0        0     2643 2023-02-27 12:54:43.441184 pytamaro-0.5.0/pytamaro/debug.py
+-rw-r--r--   0        0        0     8147 2023-02-27 12:54:43.441456 pytamaro-0.5.0/pytamaro/graphic.py
+-rw-r--r--   0        0        0     8534 2023-05-24 07:48:53.130050 pytamaro-0.5.0/pytamaro/io.py
+-rw-r--r--   0        0        0      457 2023-02-27 12:54:43.441979 pytamaro-0.5.0/pytamaro/it/__init__.py
+-rw-r--r--   0        0        0     3370 2023-02-27 12:54:43.442282 pytamaro-0.5.0/pytamaro/it/color.py
+-rw-r--r--   0        0        0      923 2022-11-30 08:45:09.899740 pytamaro-0.5.0/pytamaro/it/color_names.py
+-rw-r--r--   0        0        0      459 2023-02-27 12:54:43.442558 pytamaro-0.5.0/pytamaro/it/graphic.py
+-rw-r--r--   0        0        0     2949 2023-05-24 07:12:31.769928 pytamaro-0.5.0/pytamaro/it/io.py
+-rw-r--r--   0        0        0     4512 2023-02-27 12:54:43.442887 pytamaro-0.5.0/pytamaro/it/operations.py
+-rw-r--r--   0        0        0      111 2023-02-27 12:54:43.443014 pytamaro-0.5.0/pytamaro/it/point.py
+-rw-r--r--   0        0        0     1626 2023-02-27 12:54:43.443240 pytamaro-0.5.0/pytamaro/it/point_names.py
+-rw-r--r--   0        0        0     4636 2023-02-27 12:54:43.443425 pytamaro-0.5.0/pytamaro/it/primitives.py
+-rw-r--r--   0        0        0     5786 2023-02-27 12:54:43.443621 pytamaro-0.5.0/pytamaro/localization.py
+-rw-r--r--   0        0        0     5834 2023-02-27 12:54:43.443786 pytamaro-0.5.0/pytamaro/operations.py
+-rw-r--r--   0        0        0     1900 2023-02-27 12:54:43.443994 pytamaro-0.5.0/pytamaro/point.py
+-rw-r--r--   0        0        0     1233 2023-02-27 12:54:43.444184 pytamaro-0.5.0/pytamaro/point_names.py
+-rw-r--r--   0        0        0     4997 2023-02-27 12:54:43.444392 pytamaro-0.5.0/pytamaro/primitives.py
+-rw-r--r--   0        0        0        0 2022-10-31 08:45:16.764275 pytamaro-0.5.0/pytamaro/py.typed
+-rw-r--r--   0        0        0     1032 2023-04-06 12:16:34.179637 pytamaro-0.5.0/pytamaro/utils.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pytamaro-0.5.0/PKG-INFO
```

### Comparing `pytamaro-0.4.1/LICENSE` & `pytamaro-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pyproject.toml` & `pytamaro-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "pytamaro"
-version = "0.4.1"
+version = "0.5.0"
 description = "Educational library for teaching problem decompositon using graphics"
 authors = ["Luca Chiodini <luca@chiodini.org>"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.8"
 Pillow = "^9.0.0"
 skia-python = "^87.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-watch = "^4.2.0"
 pytest-cov = "^3.0.0"
```

### Comparing `pytamaro-0.4.1/pytamaro/checks.py` & `pytamaro-0.5.0/pytamaro/checks.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/color.py` & `pytamaro-0.5.0/pytamaro/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/color_functions.py` & `pytamaro-0.5.0/pytamaro/color_functions.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/color_names.py` & `pytamaro-0.5.0/pytamaro/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/de/color.py` & `pytamaro-0.5.0/pytamaro/de/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/de/color_names.py` & `pytamaro-0.5.0/pytamaro/de/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/de/io.py` & `pytamaro-0.5.0/pytamaro/de/io.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Funktionen zur Ausgabe (Anzeigen oder Speichern) von Grafiken.
 """
 
 from __future__ import annotations
 
-from pytamaro.io import save_gif, save_graphic, show_graphic
+from pytamaro.io import save_animation, save_graphic, show_animation, show_graphic
 from pytamaro.de.graphic import Grafik
 
 
 def zeige_grafik(grafik: Grafik, debug: bool = False):
     """
-    Zeige die gegebene Grafik in einem neuen Fenster an.
+    Zeige die gegebene Grafik an.
 
     Eine Grafik ohne Fläche kann nicht angezeigt werden.
 
     Falls `debug` `True` ist werden auf der Grafik zusätzliche Informationen
     dargestellt, welche für das Debugging nützlich sein können.
     Ein roter Rahmen markiert den Begrenzungsrahmen der Grafik,
     und ein gelbliches Kreuz gibt die Fixierposition an.
@@ -44,24 +44,40 @@
     :param grafik: zu speichernde Grafik
     :param debug: kann optional auf `True` gesetzt werden, um über der Grafik
                   Debug-Informationen darzustellen
     """
     save_graphic(datei_name, grafik, debug)
 
 
-def speichere_gif(
+def speichere_animation(
     datei_name: str, grafiken: list[Grafik], dauer: int = 40, loop: bool = True
 ):
     """
-    Speichere die gegebene Sequenz von Grafiken als animierte GIF-Datei.
+    Speichere eine Sequenz von Grafiken als Animation (GIF).
 
     Beim Anzeigen des GIFs werden die Grafiken in einer unendlichen Schleife
     animiert (normalerweise mit 25 Grafiken pro Sekunde).
 
     :param datei_name: Name der zu kreierenden Datei (mit Erweiterung '.gif')
     :param grafiken: Liste der zu speichernden Grafiken
     :param dauer: Dauer jeder Grafik, in Millisekunden (Default: 40
            Millisekunden, enspricht 25 Grafiken pro Sekunde)
     :param loop: bestimmt ob das GIF in einer unendlichen Schleife abgespielt
            werden soll (Default: true)
     """
-    save_gif(datei_name, grafiken, dauer, loop)
+    save_animation(datei_name, grafiken, dauer, loop)
+
+
+def zeige_animation(grafiken: list[Grafik], dauer: int = 40, loop: bool = True):
+    """
+    Zeige eine Sequenz von Grafiken als Animation (GIF) an.
+
+    Beim Anzeigen des GIFs werden die Grafiken in einer unendlichen Schleife
+    animiert (normalerweise mit 25 Grafiken pro Sekunde).
+
+    :param grafiken: Liste der anzuzeigenden Grafiken
+    :param dauer: Dauer jeder Grafik, in Millisekunden (Default: 40
+           Millisekunden, enspricht 25 Grafiken pro Sekunde)
+    :param loop: bestimmt ob das GIF in einer unendlichen Schleife abgespielt
+           werden soll (Default: true)
+    """
+    show_animation(grafiken, dauer, loop)
```

### Comparing `pytamaro-0.4.1/pytamaro/de/operations.py` & `pytamaro-0.5.0/pytamaro/de/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/de/point_names.py` & `pytamaro-0.5.0/pytamaro/de/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/de/primitives.py` & `pytamaro-0.5.0/pytamaro/de/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/debug.py` & `pytamaro-0.5.0/pytamaro/debug.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/graphic.py` & `pytamaro-0.5.0/pytamaro/graphic.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/io.py` & `pytamaro-0.5.0/pytamaro/io.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
-Functions to do I/O with graphics, such as showing or saving them.
+Functions for output (show or save) of graphics.
 """
 
 import base64
 import io
 import os
+import re
 from pathlib import Path
+import subprocess
+import sys
+from tempfile import NamedTemporaryFile
 from typing import List
 
 from PIL import Image as PILImageMod
 from PIL.Image import Image as PILImage
 from skia import Canvas, FILEWStream, Image, Rect, Surface, SVGCanvas, kPNG
 
 from pytamaro.checks import check_graphic, check_type
@@ -53,14 +57,23 @@
     """
     size = graphic.size()
     stream = FILEWStream(filename)
     canvas = SVGCanvas.Make(Rect.MakeSize(size), stream)
     _draw_to_canvas(canvas, graphic)
     del canvas
     stream.flush()
+    # Manually add shape-rendering="crispEdges" to the SVG file.
+    # We don't use the XML parser from the standard library because,
+    # among other aspects, it does not properly maintain the doctype.
+    with open(filename, "r", encoding="utf-8") as file:
+        content = file.read()
+    # `svg` tag may be self-closing
+    new_content = re.sub("<svg(.*?)(/?)>", r'<svg\1 shape-rendering="crispEdges"\2>', content)
+    with open(filename, "w", encoding="utf-8") as file:
+        file.write(new_content)
 
 
 def graphic_to_image(graphic: Graphic) -> Image:
     """
     Renders a graphic into a Skia image.
 
     :param graphic: graphic to be rendered
@@ -95,15 +108,15 @@
     """
     graphic_to_image(graphic).save(filename, kPNG)
 
 
 @export
 def show_graphic(graphic: Graphic, debug: bool = False):
     """
-    Show a graphic in a window. Graphics with no area cannot be shown.
+    Show a graphic. Graphics with no area cannot be shown.
 
     When `debug` is `True`, adorns the visualization with useful information
     for debugging: a red border around the bounding box and a yellowish cross
     around the pinning position.
 
     :param graphic: graphic to be shown
     :param debug: can be optionally set to `True` to overlay debugging
@@ -112,15 +125,15 @@
     check_graphic(graphic)
     if graphic.empty_area():
         _warning_no_area(graphic)
     else:
         to_show = add_debug_info(graphic) if debug else graphic
         pil_image = graphic_to_pillow_image(to_show)
         if is_notebook():
-            # pylint: disable=undefined-variable
+            # pylint: disable-next=undefined-variable
             display(pil_image)  # type: ignore[name-defined]
         elif "PYTAMARO_OUTPUT_DATA_URI" in os.environ:
             buffer = io.BytesIO()
             pil_image.save(buffer, format="PNG")
             b64_str = base64.b64encode(buffer.getvalue()).decode("utf-8")
             print(f"data:image/png;base64,{b64_str}", end="")
         else:
@@ -157,23 +170,23 @@
     elif extension == ".svg":
         _save_as_SVG(filename, to_show)
     else:
         raise ValueError(translate("INVALID_FILENAME_EXTENSION"))
 
 
 @export
-def save_gif(filename: str, graphics: List[Graphic], duration: int = 40, loop: bool = True):
+def save_animation(filename: str, graphics: List[Graphic], duration: int = 40, loop: bool = True):
     """
-    Save a sequence of graphics as an animated GIF.
+    Save a sequence of graphics as an animation (GIF).
 
     Graphics are sequentially reproduced (normally at 25 frames per second) in
     a loop (unless specificied otherwise).
 
     :param filename: name of the file to create, including the extension '.gif'
-    :param graphics: list of graphics to be saved as a GIF
+    :param graphics: list of graphics to be saved as an animation
     :param duration: duration in milliseconds for each frame
            (defaults to 40 milliseconds, which leads to 25 frames per second)
     :param loop: whether the GIF should loop indefinitely (defaults to true)
     """
     check_type(filename, str, "filename")
     if Path(filename).suffix != ".gif":
         raise ValueError(translate("INVALID_FILENAME_GIF"))
@@ -184,7 +197,40 @@
     pil_images[0].save(
         filename,
         save_all=True,
         append_images=pil_images[1:],
         duration=duration,
         loop=0 if loop else 1,  # loop 0 means "indefinitely", 1 means "once"
     )
+
+
+@export
+def show_animation(graphics: List[Graphic], duration: int = 40, loop: bool = True):
+    """
+    Show a sequence of graphics as an animation (GIF).
+
+    Graphics are sequentially reproduced (normally at 25 frames per second) in
+    a loop (unless specificied otherwise).
+
+    :param graphics: list of graphics to be shown as an animation
+    :param duration: duration in milliseconds for each frame
+           (defaults to 40 milliseconds, which leads to 25 frames per second)
+    :param loop: whether the animation should loop indefinitely (defaults to true)
+    """
+    with NamedTemporaryFile(suffix=".gif", delete=False) as file:
+        save_animation(file.name, graphics, duration, loop)
+        if is_notebook():
+            # pylint: disable-next=import-outside-toplevel, import-error
+            from IPython.display import Image as IPythonImage  # type: ignore[import]
+            with open(file.name, "rb") as stream:
+                # pylint: disable-next=undefined-variable
+                display(IPythonImage(stream.read()))  # type: ignore[name-defined]
+        elif "PYTAMARO_OUTPUT_DATA_URI" in os.environ:
+            with open(file.name, "rb") as stream:
+                b64_str = base64.b64encode(stream.read()).decode("utf-8")
+                print(f"data:image/gif;base64,{b64_str}", end="")
+        elif sys.platform == "win32":
+            os.startfile(file.name)
+        elif sys.platform == "darwin":
+            subprocess.call(["open", "-a", "Safari", file.name])
+        else:
+            subprocess.call(["xdg-open", file.name])
```

### Comparing `pytamaro-0.4.1/pytamaro/it/color.py` & `pytamaro-0.5.0/pytamaro/it/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/it/color_names.py` & `pytamaro-0.5.0/pytamaro/it/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/it/io.py` & `pytamaro-0.5.0/pytamaro/it/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-Funzioni per I/O con grafiche, come visualizzarle oppure salvarle.
+Funzioni per output di grafiche (visualizzare o salvare).
 """
 
 from __future__ import annotations
 
-from pytamaro.io import save_gif, save_graphic, show_graphic
+from pytamaro.io import save_animation, save_graphic, show_animation, show_graphic
 from pytamaro.it.graphic import Grafica
 
 
 def visualizza_grafica(grafica: Grafica, debug: bool = False):
     """
-    Visualizza una grafica in una nuova finestra.
-    Grafiche prive di area non possono essere visualizzate.
+    Visualizza una grafica. Grafiche prive di area non possono essere
+    visualizzate.
 
     Quando `debug` è `True`, adorna la visualizzazione con informazioni utili
     per debugging: un bordo rosso attorno alla bounding box e una croce
     giallastra attorno al punto di fissaggio.
 
     :param grafica: grafica da visualizzare
     :param debug: può facoltativamente essere impostato a `True` per
@@ -41,23 +41,38 @@
     :param grafica: grafica da visualizzare
     :param debug: può facoltativamente essere impostato a `True` per
            sovrapporre informazioni di debug
     """
     save_graphic(nome_file, grafica, debug)
 
 
-def salva_gif(
+def salva_animazione(
     nome_file: str, grafiche: list[Grafica], durata: int = 40, loop: bool = True
 ):
     """
-    Salva una sequenza di grafiche come una GIF animata.
+    Salva una sequenza di grafiche come un'animazione (GIF).
 
     Le grafiche vengono riprodotte sequenzialmente (normalmente a 25 frame al
     secondo) a ciclo continuo.
 
     :param nome_file: nome del file da creare (inclusa l'estensione '.gif')
-    :param grafiche: lista di grafiche da salvare come GIF
+    :param grafiche: lista di grafiche da salvare come animazione
     :param durata: durata in millisecondi di ciascun frame (default a 40
            millisecondi, ovvero 25 frame al secondo)
     :param loop: determina se la GIF debba riprodursi in loop indefinitamente (default a True)
     """
-    save_gif(nome_file, grafiche, durata, loop)
+    save_animation(nome_file, grafiche, durata, loop)
+
+
+def visualizza_animazione(grafiche: list[Grafica], durata: int = 40, loop: bool = True):
+    """
+    Visualizza una sequenza di grafiche come un'animazione (GIF).
+
+    Le grafiche vengono riprodotte sequenzialmente (normalmente a 25 frame al
+    secondo) a ciclo continuo.
+
+    :param grafiche: lista di grafiche da salvare come animazione
+    :param durata: durata in millisecondi di ciascun frame (default a 40
+           millisecondi, ovvero 25 frame al secondo)
+    :param loop: determina se la GIF debba riprodursi in loop indefinitamente (default a True)
+    """
+    show_animation(grafiche, durata, loop)
```

### Comparing `pytamaro-0.4.1/pytamaro/it/operations.py` & `pytamaro-0.5.0/pytamaro/it/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/it/point_names.py` & `pytamaro-0.5.0/pytamaro/it/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/it/primitives.py` & `pytamaro-0.5.0/pytamaro/it/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/localization.py` & `pytamaro-0.5.0/pytamaro/localization.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/operations.py` & `pytamaro-0.5.0/pytamaro/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/point.py` & `pytamaro-0.5.0/pytamaro/point.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/point_names.py` & `pytamaro-0.5.0/pytamaro/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/primitives.py` & `pytamaro-0.5.0/pytamaro/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/pytamaro/utils.py` & `pytamaro-0.5.0/pytamaro/utils.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.4.1/PKG-INFO` & `pytamaro-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: pytamaro
-Version: 0.4.1
+Version: 0.5.0
 Summary: Educational library for teaching problem decompositon using graphics
 Author: Luca Chiodini
 Author-email: luca@chiodini.org
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.0.0,<10.0.0)
 Requires-Dist: skia-python (>=87.4,<88.0)
```

