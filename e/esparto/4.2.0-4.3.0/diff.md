# Comparing `tmp/esparto-4.2.0.tar.gz` & `tmp/esparto-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esparto-4.2.0.tar", max compression
+gzip compressed data, was "esparto-4.3.0.tar", max compression
```

## Comparing `esparto-4.2.0.tar` & `esparto-4.3.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1071 2022-04-19 15:56:37.678436 esparto-4.2.0/LICENSE
--rw-r--r--   0        0        0     3792 2022-06-29 20:48:26.649962 esparto-4.2.0/README.md
--rw-r--r--   0        0        0     1120 2022-11-10 18:27:36.095751 esparto-4.2.0/esparto/__init__.py
--rw-r--r--   0        0        0       69 2022-04-20 07:43:09.473785 esparto-4.2.0/esparto/__main__.py
--rw-r--r--   0        0        0     3265 2022-04-20 07:43:09.473785 esparto-4.2.0/esparto/_cli.py
--rw-r--r--   0        0        0     7064 2022-06-29 20:40:25.602795 esparto-4.2.0/esparto/_options.py
--rw-r--r--   0        0        0        0 2022-04-20 07:43:09.473785 esparto-4.2.0/esparto/design/__init__.py
--rw-r--r--   0        0        0     3331 2022-04-20 07:43:09.473785 esparto-4.2.0/esparto/design/adaptors.py
--rw-r--r--   0        0        0     2506 2022-04-20 07:43:09.473785 esparto-4.2.0/esparto/design/base.py
--rw-r--r--   0        0        0    16989 2022-04-20 07:43:09.473785 esparto-4.2.0/esparto/design/content.py
--rw-r--r--   0        0        0    32166 2022-06-29 20:40:25.602795 esparto-4.2.0/esparto/design/layout.py
--rw-r--r--   0        0        0        0 2022-04-20 07:43:09.473785 esparto-4.2.0/esparto/publish/__init__.py
--rw-r--r--   0        0        0     2389 2022-04-20 07:43:09.473785 esparto-4.2.0/esparto/publish/contentdeps.py
--rw-r--r--   0        0        0     6343 2022-11-10 18:27:36.095751 esparto-4.2.0/esparto/publish/output.py
--rw-r--r--   0        0        0   163874 2022-06-29 14:45:25.039530 esparto-4.2.0/esparto/resources/css/bootstrap.min.css
--rw-r--r--   0        0        0     3041 2022-06-29 20:40:25.602795 esparto-4.2.0/esparto/resources/css/esparto.css
--rw-r--r--   0        0        0     3646 2022-11-10 18:27:36.095751 esparto-4.2.0/esparto/resources/jinja/base.html.jinja
--rw-r--r--   0        0        0      924 2022-06-29 20:40:25.602795 esparto-4.2.0/esparto/resources/js/esparto.js
--rw-r--r--   0        0        0     1810 2022-11-10 18:27:36.095751 esparto-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 esparto-4.2.0/setup.py
--rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 esparto-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-04-19 15:56:37.678436 esparto-4.3.0/LICENSE
+-rw-r--r--   0        0        0     3792 2022-06-29 20:48:26.649962 esparto-4.3.0/README.md
+-rw-r--r--   0        0        0     1317 2023-05-29 09:40:48.655809 esparto-4.3.0/esparto/__init__.py
+-rw-r--r--   0        0        0       69 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/__main__.py
+-rw-r--r--   0        0        0     3265 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/_cli.py
+-rw-r--r--   0        0        0     7127 2023-05-29 09:20:09.460818 esparto-4.3.0/esparto/_options.py
+-rw-r--r--   0        0        0        0 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/design/__init__.py
+-rw-r--r--   0        0        0     3326 2023-05-29 09:41:13.871626 esparto-4.3.0/esparto/design/adaptors.py
+-rw-r--r--   0        0        0     2506 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/design/base.py
+-rw-r--r--   0        0        0    16968 2023-05-29 09:48:22.504510 esparto-4.3.0/esparto/design/content.py
+-rw-r--r--   0        0        0    32166 2022-06-29 20:40:25.602795 esparto-4.3.0/esparto/design/layout.py
+-rw-r--r--   0        0        0        0 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/publish/__init__.py
+-rw-r--r--   0        0        0     2388 2023-05-29 09:39:11.168518 esparto-4.3.0/esparto/publish/contentdeps.py
+-rw-r--r--   0        0        0     6344 2023-05-29 09:39:25.736412 esparto-4.3.0/esparto/publish/output.py
+-rw-r--r--   0        0        0   163874 2022-06-29 14:45:25.039530 esparto-4.3.0/esparto/resources/css/bootstrap.min.css
+-rw-r--r--   0        0        0     3041 2022-06-29 20:40:25.602795 esparto-4.3.0/esparto/resources/css/esparto.css
+-rw-r--r--   0        0        0     3646 2022-11-10 18:27:36.095751 esparto-4.3.0/esparto/resources/jinja/base.html.jinja
+-rw-r--r--   0        0        0      924 2022-06-29 20:40:25.602795 esparto-4.3.0/esparto/resources/js/esparto.js
+-rw-r--r--   0        0        0     1856 2023-05-29 09:35:32.734106 esparto-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 esparto-4.3.0/PKG-INFO
```

### Comparing `esparto-4.2.0/LICENSE` & `esparto-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esparto-4.2.0/README.md` & `esparto-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `esparto-4.2.0/esparto/__init__.py` & `esparto-4.3.0/esparto/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 
 Data driven report builder for the PyData ecosystem.
 
 Please visit https://domvwt.github.io/esparto/ for documentation and examples.
 
 """
 
+import dataclasses as _dc
 from importlib.util import find_spec as _find_spec
 from pathlib import Path as _Path
-from typing import Set as _Set
 
 __author__ = """Dominic Thorn"""
 __email__ = "dominic.thorn@gmail.com"
-__version__ = "4.2.0"
+__version__ = "4.3.0"
 
 _MODULE_PATH: _Path = _Path(__file__).parent.absolute()
 
 
-_OPTIONAL_DEPENDENCIES: _Set[str] = {
-    "PIL",  # Only used for type checking and conversion
-    "IPython",
-    "matplotlib",
-    "pandas",
-    "bokeh",
-    "plotly",
-    "weasyprint",
-}
-
-_INSTALLED_MODULES: _Set[str] = {
-    x.name for x in [_find_spec(dep) for dep in _OPTIONAL_DEPENDENCIES] if x
-}
+@_dc.dataclass(frozen=True)
+class _OptionalDependencies:
+    PIL: bool = _find_spec("PIL") is not None
+    IPython: bool = _find_spec("IPython") is not None
+    matplotlib: bool = _find_spec("matplotlib") is not None
+    pandas: bool = _find_spec("pandas") is not None
+    bokeh: bool = _find_spec("bokeh") is not None
+    plotly: bool = _find_spec("plotly") is not None
+    weasyprint: bool = _find_spec("weasyprint") is not None
+
+    def all_extras(self) -> bool:
+        return all(_dc.astuple(self))
+
 
 from esparto._options import OutputOptions, options
 from esparto.design.content import (
     DataFramePd,
     FigureBokeh,
     FigureMpl,
     FigurePlotly,
```

### Comparing `esparto-4.2.0/esparto/_cli.py` & `esparto-4.3.0/esparto/_cli.py`

 * *Files identical despite different names*

### Comparing `esparto-4.2.0/esparto/_options.py` & `esparto-4.3.0/esparto/_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,17 +130,17 @@
         "crossorigin='anonymous' referrerpolicy='no-referrer'>"
     )
     bootstrap_css: str = str(_MODULE_PATH / "resources/css/bootstrap.min.css")
     esparto_css: str = str(_MODULE_PATH / "resources/css/esparto.css")
     esparto_js: str = str(_MODULE_PATH / "resources/js/esparto.js")
     jinja_template: str = str(_MODULE_PATH / "resources/jinja/base.html.jinja")
 
-    matplotlib: MatplotlibOptions = MatplotlibOptions()
-    bokeh: BokehOptions = BokehOptions()
-    plotly: PlotlyOptions = PlotlyOptions()
+    matplotlib: MatplotlibOptions = field(default_factory=MatplotlibOptions)
+    bokeh: BokehOptions = field(default_factory=BokehOptions)
+    plotly: PlotlyOptions = field(default_factory=PlotlyOptions)
 
     _pdf_temp_dir: str = TemporaryDirectory().name
 
     _options_source: str = ""
 
     def save(self, path: Union[str, Path] = "./esparto-config.yaml") -> None:
         """Save config to yaml file at `path`."""
```

### Comparing `esparto-4.2.0/esparto/design/adaptors.py` & `esparto-4.3.0/esparto/design/adaptors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools as ft
 import mimetypes as mt
 from pathlib import Path
 from typing import Any, Dict, Union
 
-from esparto import _INSTALLED_MODULES
+from esparto import _OptionalDependencies
 from esparto.design.content import (
     Content,
     DataFramePd,
     FigureBokeh,
     FigureMpl,
     FigurePlotly,
     Image,
@@ -61,44 +61,44 @@
     """Pass through dict of `{"title": content}`."""
     if not (len(content) == 1 and isinstance(list(content.keys())[0], str)):
         raise ValueError("Content dict must be passed as {'title': content}")
     return content
 
 
 # Function only available if Pandas is installed.
-if "pandas" in _INSTALLED_MODULES:
+if _OptionalDependencies.pandas:
     from pandas.core.frame import DataFrame  # type: ignore
 
     @content_adaptor.register(DataFrame)
     def content_adaptor_df(content: DataFrame) -> DataFramePd:
         """Convert Pandas DataFrame to DataFramePD content."""
         return DataFramePd(content)
 
 
 # Function only available if Matplotlib is installed.
-if "matplotlib" in _INSTALLED_MODULES:
+if _OptionalDependencies.matplotlib:
     from matplotlib.figure import Figure  # type: ignore
 
     @content_adaptor.register(Figure)
     def content_adaptor_mpl(content: Figure) -> FigureMpl:
         """Convert Matplotlib Figure to FigureMpl content."""
         return FigureMpl(content)
 
 
 # Function only available if Bokeh is installed.
-if "bokeh" in _INSTALLED_MODULES:
+if _OptionalDependencies.bokeh:
     from bokeh.layouts import LayoutDOM as BokehObject  # type: ignore
 
     @content_adaptor.register(BokehObject)
     def content_adaptor_bokeh(content: BokehObject) -> FigureBokeh:
         """Convert Bokeh Layout to FigureBokeh content."""
         return FigureBokeh(content)
 
 
 # Function only available if Plotly is installed.
-if "plotly" in _INSTALLED_MODULES:
+if _OptionalDependencies.plotly:
     from plotly.graph_objs._figure import Figure as PlotlyFigure  # type: ignore
 
     @content_adaptor.register(PlotlyFigure)
     def content_adaptor_plotly(content: PlotlyFigure) -> FigurePlotly:
         """Convert Plotly Figure to FigurePlotly content."""
         return FigurePlotly(content)
```

### Comparing `esparto-4.2.0/esparto/design/base.py` & `esparto-4.3.0/esparto/design/base.py`

 * *Files identical despite different names*

### Comparing `esparto-4.2.0/esparto/design/content.py` & `esparto-4.3.0/esparto/design/content.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 from io import BytesIO, StringIO
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, TypeVar, Union
 from uuid import uuid4
 
 import markdown as md
 
-from esparto import _INSTALLED_MODULES
+from esparto import _OptionalDependencies
 from esparto._options import options
 from esparto.design.base import AbstractContent, AbstractLayout, Child
 from esparto.design.layout import Row
 from esparto.publish.output import nb_display
 
-if "PIL" in _INSTALLED_MODULES:
+if _OptionalDependencies.PIL:
     from PIL.Image import Image as PILImage  # type: ignore
 
-if "pandas" in _INSTALLED_MODULES:
+if _OptionalDependencies.pandas:
     from pandas import DataFrame  # type: ignore
 
-if "matplotlib" in _INSTALLED_MODULES:
+if _OptionalDependencies.matplotlib:
     from matplotlib.figure import Figure as MplFigure  # type: ignore
 
-if "bokeh" in _INSTALLED_MODULES:
+if _OptionalDependencies.bokeh:
     from bokeh.embed import components  # type: ignore
     from bokeh.models.layouts import LayoutDOM as BokehObject  # type: ignore
 
-if "plotly" in _INSTALLED_MODULES:
+if _OptionalDependencies.plotly:
     from plotly.graph_objs._figure import Figure as PlotlyFigure  # type: ignore
     from plotly.io import to_html as plotly_to_html  # type: ignore
 
 
 T = TypeVar("T", bound="Content")
 
 
@@ -99,15 +99,14 @@
 
     """
 
     _dependencies: Set[Any] = set("")
     content: str
 
     def __init__(self, html: str) -> None:
-
         if not isinstance(html, str):
             raise TypeError(r"HTML must be str")
 
         self.content = html
 
     def to_html(self, **kwargs: bool) -> str:
         return self.content
@@ -120,15 +119,14 @@
         text (str): Markdown text to be added to document.
 
     """
 
     _dependencies = {"bootstrap"}
 
     def __init__(self, text: str) -> None:
-
         if not isinstance(text, str):
             raise TypeError(r"text must be str")
 
         self.content: str = text
 
     def to_html(self, **kwargs: bool) -> str:
         html = md.markdown(self.content, extensions=["extra", "smarty"])
@@ -159,18 +157,17 @@
         image: Union[str, Path, "PILImage", BytesIO],
         caption: Optional[str] = "",
         alt_text: Optional[str] = "Image",
         scale: Optional[float] = None,
         set_width: Optional[int] = None,
         set_height: Optional[int] = None,
     ):
-
         valid_types: Tuple[Any, ...]
 
-        if "PIL" in _INSTALLED_MODULES:
+        if _OptionalDependencies.PIL:
             valid_types = (str, Path, PILImage, BytesIO)
         else:
             valid_types = (str, Path, BytesIO)
 
         if not isinstance(image, (valid_types)):
             raise TypeError(r"`image` must be one of {}".format(valid_types))
 
@@ -246,15 +243,14 @@
     """
 
     _dependencies = {"bootstrap"}
 
     def __init__(
         self, df: "DataFrame", index: bool = True, col_space: Union[int, str] = 0
     ):
-
         if not isinstance(df, DataFrame):
             raise TypeError(r"df must be Pandas DataFrame")
 
         self.content: "DataFrame" = df
         self.index = index
         self.col_space = col_space
         self.css_classes = [
@@ -288,40 +284,37 @@
 
     def __init__(
         self,
         figure: "MplFigure",
         output_format: Optional[str] = None,
         pdf_figsize: Optional[Union[Tuple[int, int], float]] = None,
     ) -> None:
-
         if not isinstance(figure, MplFigure):
             raise TypeError(r"figure must be a Matplotlib Figure")
 
         self.content: MplFigure = figure
         self.output_format = output_format or options.matplotlib.html_output_format
         self.pdf_figsize = pdf_figsize or options.matplotlib.pdf_figsize
 
         self._original_figsize = figure.get_size_inches()
 
     def to_html(self, **kwargs: bool) -> str:
-
         if kwargs.get("notebook_mode"):
             output_format = options.matplotlib.notebook_format
         else:
             output_format = self.output_format
 
         if kwargs.get("pdf_mode") and self.pdf_figsize:
             if isinstance(self.pdf_figsize, float):
                 figsize = self.pdf_figsize * self._original_figsize
             else:
                 figsize = self.pdf_figsize
             self.content.set_size_inches(*figsize)
 
         if output_format == "svg":
-
             string_buffer = StringIO()
             self.content.savefig(string_buffer, format="svg")
             string_buffer.seek(0)
             xml = string_buffer.read()
 
             dpi = 96
             fig_width, fig_height = (
@@ -378,15 +371,14 @@
         if not issubclass(type(figure), BokehObject):
             raise TypeError(r"figure must be a Bokeh object")
 
         self.content: BokehObject = figure
         self.layout_attributes = layout_attributes or options.bokeh.layout_attributes
 
     def to_html(self, **kwargs: bool) -> str:
-
         if self.layout_attributes:
             for key, value in self.layout_attributes.items():
                 setattr(self.content, key, value)
 
         # Bokeh to PDF is experimental and untested
         if kwargs.get("pdf_mode"):  # pragma: no cover
             from bokeh.io import export_svg  # type: ignore
@@ -422,25 +414,23 @@
     _dependencies = {"plotly"}
 
     def __init__(
         self,
         figure: "PlotlyFigure",
         layout_args: Optional[Dict[Any, Any]] = None,
     ):
-
         if not isinstance(figure, PlotlyFigure):
             raise TypeError(r"figure must be a Plotly Figure")
 
         self.layout_args = layout_args or options.plotly.layout_args
 
         self.content: PlotlyFigure = figure
         self._original_layout = figure.layout
 
     def to_html(self, **kwargs: bool) -> str:
-
         if self.layout_args:
             self.content.update_layout(**self.layout_args)
 
         # Default width is 700, default height is 450
         fig_width: int = getattr(self.content, "width", 700)
 
         if kwargs.get("pdf_mode"):
@@ -481,15 +471,15 @@
 
     Returns:
         BytesIO: image as bytes object.
 
     """
     if isinstance(image, BytesIO):
         return image
-    elif "PIL" in _INSTALLED_MODULES and isinstance(image, PILImage):
+    elif _OptionalDependencies.PIL and isinstance(image, PILImage):
         return BytesIO(image.tobytes())
     elif isinstance(image, (str, Path)):
         return BytesIO(Path(image).read_bytes())
     else:
         raise TypeError(type(image))
```

### Comparing `esparto-4.2.0/esparto/design/layout.py` & `esparto-4.3.0/esparto/design/layout.py`

 * *Files identical despite different names*

### Comparing `esparto-4.2.0/esparto/publish/contentdeps.py` & `esparto-4.3.0/esparto/publish/contentdeps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Content dependency management."""
 
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import List, Optional, Set
 
-from esparto import _INSTALLED_MODULES
+from esparto import _OptionalDependencies
 from esparto._options import options
 
 
 @dataclass
 class ContentDependency:
     name: str
     cdn: str
@@ -36,25 +36,25 @@
     bootstrap_inline = f"<style>\n{bootstrap_inline}\n</style>"
 
     content_dependency_dict = ContentDependencyDict()
     content_dependency_dict += ContentDependency(
         "bootstrap", options.bootstrap_cdn, bootstrap_inline, "head"
     )
 
-    if "bokeh" in _INSTALLED_MODULES:
+    if _OptionalDependencies.bokeh:
         import bokeh.resources as bk_resources  # type: ignore
 
         bokeh_cdn = bk_resources.CDN.render_js()
         bokeh_inline = bk_resources.INLINE.render_js()
 
         content_dependency_dict += ContentDependency(
             "bokeh", bokeh_cdn, bokeh_inline, "tail"
         )
 
-    if "plotly" in _INSTALLED_MODULES:
+    if _OptionalDependencies.plotly:
         from plotly import offline as plotly_offline  # type: ignore
 
         plotly_version = "latest"
         plotly_cdn = f"<script src='https://cdn.plot.ly/plotly-{plotly_version}.min.js'></script>"
         plotly_inline = plotly_offline.get_plotlyjs()
         plotly_inline = f"<script>\n{plotly_inline}\n</script>"
```

### Comparing `esparto-4.2.0/esparto/publish/output.py` & `esparto-4.3.0/esparto/publish/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Union
 
 from bs4 import BeautifulSoup, Tag  # type: ignore
 from jinja2 import Template
 
-from esparto import _INSTALLED_MODULES
+from esparto import _OptionalDependencies
 from esparto._options import options, resolve_config_option
 from esparto.design.base import AbstractContent, AbstractLayout
 from esparto.publish.contentdeps import resolve_deps
 
 if TYPE_CHECKING:
     from esparto.design.layout import Page
 
@@ -84,15 +84,15 @@
       filepath (str): Filepath to write to.
       return_html (bool): Returns HTML string if True.
 
     Returns:
       str: HTML string if return_html is True.
 
     """
-    if "weasyprint" not in _INSTALLED_MODULES:
+    if not _OptionalDependencies.weasyprint:
         raise ModuleNotFoundError("Install weasyprint for PDF support")
     import weasyprint as wp  # type: ignore
 
     temp_dir = Path(options._pdf_temp_dir)
     temp_dir.mkdir(parents=True, exist_ok=True)
 
     html_rendered = publish_html(
```

### Comparing `esparto-4.2.0/esparto/resources/css/bootstrap.min.css` & `esparto-4.3.0/esparto/resources/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `esparto-4.2.0/esparto/resources/css/esparto.css` & `esparto-4.3.0/esparto/resources/css/esparto.css`

 * *Files identical despite different names*

### Comparing `esparto-4.2.0/esparto/resources/jinja/base.html.jinja` & `esparto-4.3.0/esparto/resources/jinja/base.html.jinja`

 * *Files identical despite different names*

### Comparing `esparto-4.2.0/esparto/resources/js/esparto.js` & `esparto-4.3.0/esparto/resources/js/esparto.js`

 * *Files identical despite different names*

### Comparing `esparto-4.2.0/pyproject.toml` & `esparto-4.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "esparto"
-version = "4.2.0"
+version = "4.3.0"
 description = "Data driven report builder for the PyData ecosystem."
 authors = ["Dominic Thorn <dominic.thorn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://domvwt.github.io/esparto"
 repository = "https://github.com/domvwt/esparto"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.6.1"
 jinja2 = ">=2.10.1"
 markdown = ">=3.1"
```

### Comparing `esparto-4.2.0/PKG-INFO` & `esparto-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: esparto
-Version: 4.2.0
+Version: 4.3.0
 Summary: Data driven report builder for the PyData ecosystem.
 Home-page: https://domvwt.github.io/esparto
 License: MIT
 Author: Dominic Thorn
 Author-email: dominic.thorn@gmail.com
 Requires-Python: >=3.6.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: extras
 Requires-Dist: beautifulsoup4 (>=4.7)
-Requires-Dist: dataclasses; python_version < "3.7"
+Requires-Dist: dataclasses ; python_version < "3.7"
 Requires-Dist: jinja2 (>=2.10.1)
 Requires-Dist: markdown (>=3.1)
 Requires-Dist: pyyaml (>=5.1)
-Requires-Dist: weasyprint (>=51); extra == "extras"
+Requires-Dist: weasyprint (>=51) ; extra == "extras"
 Project-URL: Repository, https://github.com/domvwt/esparto
 Description-Content-Type: text/markdown
 
 #
 
 <br>
 <div align="center">
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: esparto Version: 4.2.0 Summary: Data driven report
+Metadata-Version: 2.1 Name: esparto Version: 4.3.0 Summary: Data driven report
 builder for the PyData ecosystem. Home-page: https://domvwt.github.io/esparto
 License: MIT Author: Dominic Thorn Author-email: dominic.thorn@gmail.com
 Requires-Python: >=3.6.1 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: extras Requires-Dist: beautifulsoup4 (>=4.7) Requires-Dist:
-dataclasses; python_version < "3.7" Requires-Dist: jinja2 (>=2.10.1) Requires-
-Dist: markdown (>=3.1) Requires-Dist: pyyaml (>=5.1) Requires-Dist: weasyprint
-(>=51); extra == "extras" Project-URL: Repository, https://github.com/domvwt/
-esparto Description-Content-Type: text/markdown #
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Provides-Extra: extras Requires-Dist: beautifulsoup4
+(>=4.7) Requires-Dist: dataclasses ; python_version < "3.7" Requires-Dist:
+jinja2 (>=2.10.1) Requires-Dist: markdown (>=3.1) Requires-Dist: pyyaml (>=5.1)
+Requires-Dist: weasyprint (>=51) ; extra == "extras" Project-URL: Repository,
+https://github.com/domvwt/esparto Description-Content-Type: text/markdown #
      [https://github.com/domvwt/esparto/blob/main/logo/logo.svg?raw=true]
 
    [https://img.shields.io/pypi/pyversions/esparto.svg] [https://github.com/
     domvwt/esparto/actions/workflows/lint-and-test.yml/badge.svg] [https://
   codecov.io/gh/domvwt/esparto/branch/main/graph/badge.svg?token=35J8NZCUYC]
                   [https://sonarcloud.io/api/project_badges/
               measure?project=domvwt_esparto&metric=alert_status]
```

